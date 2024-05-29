# Comparing `tmp/jy_lib-0.7.9.tar.gz` & `tmp/jy_lib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.7.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.7.9.tar` & `jy_lib-0.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.7.9/.gitignore
--rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.7.9/.pypirc
--rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.7.9/LICENSE
--rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.7.9/Pipfile
--rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.7.9/Pipfile.lock
--rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.7.9/README.md
--rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.7.9/README_Project.md
--rw-r--r--   0        0        0      518 2024-05-24 06:16:16.193638 jy_lib-0.7.9/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.7.9/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.7.9/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.7.9/jy_lib/base.py
--rw-r--r--   0        0        0    14336 2024-05-14 04:58:53.299881 jy_lib-0.7.9/jy_lib/cache.py
--rw-r--r--   0        0        0    12013 2024-05-16 00:51:10.062483 jy_lib-0.7.9/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.7.9/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.7.9/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.7.9/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.7.9/jy_lib/date.py
--rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.7.9/jy_lib/decorator.py
--rw-r--r--   0        0        0     5916 2024-04-24 02:27:16.042289 jy_lib-0.7.9/jy_lib/exchange.py
--rw-r--r--   0        0        0      983 2024-05-21 07:30:55.744007 jy_lib-0.7.9/jy_lib/forex.py
--rw-r--r--   0        0        0      859 2024-05-24 06:16:00.834319 jy_lib-0.7.9/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.7.9/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.7.9/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.7.9/jy_lib/nav.py
--rw-r--r--   0        0        0     2194 2024-05-06 01:34:15.372232 jy_lib-0.7.9/jy_lib/reader.py
--rw-r--r--   0        0        0    18478 2024-04-17 00:51:09.235795 jy_lib-0.7.9/jy_lib/smb_client.py
--rw-r--r--   0        0        0    22189 2024-05-09 07:54:46.613755 jy_lib-0.7.9/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.7.9/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.7.9/jy_lib/time.py
--rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.7.9/publish-jypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.7.9/publish-pypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.7.9/publish-test.sh
--rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.7.9/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-15 07:06:48.431549 jy_lib-0.7.9/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.8.0/.gitignore
+-rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.8.0/.pypirc
+-rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.8.0/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.8.0/Pipfile
+-rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.8.0/Pipfile.lock
+-rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.8.0/README.md
+-rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.8.0/README_Project.md
+-rw-r--r--   0        0        0      518 2024-05-29 07:44:22.393270 jy_lib-0.8.0/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.8.0/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.8.0/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.8.0/jy_lib/base.py
+-rw-r--r--   0        0        0    14349 2024-05-29 07:43:16.778923 jy_lib-0.8.0/jy_lib/cache.py
+-rw-r--r--   0        0        0    12013 2024-05-16 00:51:10.062483 jy_lib-0.8.0/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.8.0/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.8.0/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.8.0/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.8.0/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.8.0/jy_lib/decorator.py
+-rw-r--r--   0        0        0     5960 2024-05-29 07:43:16.779460 jy_lib-0.8.0/jy_lib/exchange.py
+-rw-r--r--   0        0        0      983 2024-05-21 07:30:55.744007 jy_lib-0.8.0/jy_lib/forex.py
+-rw-r--r--   0        0        0      859 2024-05-24 06:16:00.834319 jy_lib-0.8.0/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2394 2024-05-29 07:43:16.779917 jy_lib-0.8.0/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.8.0/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.8.0/jy_lib/nav.py
+-rw-r--r--   0        0        0     2194 2024-05-06 01:34:15.372232 jy_lib-0.8.0/jy_lib/reader.py
+-rw-r--r--   0        0        0    18478 2024-04-17 00:51:09.235795 jy_lib-0.8.0/jy_lib/smb_client.py
+-rw-r--r--   0        0        0    22189 2024-05-09 07:54:46.613755 jy_lib-0.8.0/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.8.0/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.8.0/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.8.0/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.8.0/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.8.0/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-15 07:06:48.431549 jy_lib-0.8.0/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.8.0/PKG-INFO
```

### Comparing `jy_lib-0.7.9/.gitignore` & `jy_lib-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/LICENSE` & `jy_lib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/Pipfile` & `jy_lib-0.8.0/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/Pipfile.lock` & `jy_lib-0.8.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/__init__.py` & `jy_lib-0.8.0/jy_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     SymbolFlag,
     SymbolSubType,
     SymbolType,
     WarrantsType,
 )
 from .symbol_em import EMParser, KLineRecord, TrendRecord
 
-__version__ = "0.7.9"
+__version__ = "0.8.0"
```

### Comparing `jy_lib-0.7.9/jy_lib/auth_client.py` & `jy_lib-0.8.0/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/bank.py` & `jy_lib-0.8.0/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/base.py` & `jy_lib-0.8.0/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/cache.py` & `jy_lib-0.8.0/jy_lib/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import pickle
 import re
 import sqlite3
 import threading
 import time
 from typing import Any, Set, List, Tuple, Dict
+from .lock import SyncRWLock
 
 
 class Cache:
     """持久化TTL缓存"""
 
     def __init__(self, path: str = None):
         current_frame = inspect.currentframe()
@@ -22,53 +23,59 @@
         caller_file = caller_frame.f_code.co_filename
         if not path:
             path: str = f'_{os.path.splitext(os.path.basename(caller_file))[0]}.db3'
         self.path: str = os.path.join(os.path.dirname(caller_file), path)
         self.default_dataset: str = 'DEFAULT'
         self.compress_min_size: int = max(64, len(lz4.frame.compress(b'\x00')))
         self.conn = sqlite3.connect(self.path, check_same_thread=False)
-        self.lock = threading.RLock()
+        self.lock = SyncRWLock(reentrant=True)
         # self.conn.execute('PRAGMA auto_vacuum = FULL')
         self.datasets: Set[str] = self.get_tables()
         self.upgrade_tables()
 
     def get_tables(self) -> Set[str]:
         """获取所有数据集"""
         with self.lock:
             cursor = self.conn.cursor()
             r = cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
             return {row[0] for row in r.fetchall()}
 
     def upgrade_tables(self):
         """升级表到最新版本"""
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             updated: bool = False
             for dataset in self.datasets:
                 cursor = self.conn.cursor()
                 r = cursor.execute(f"PRAGMA table_info({dataset});")
                 cols: List[str] = [x[1] for x in r.fetchall()]
                 if 'encoding' not in cols:
                     self.conn.execute(f'ALTER TABLE `{dataset}` ADD COLUMN `encoding` INTEGER;')
                     self.conn.execute(f'UPDATE `{dataset}` SET `encoding` = 5;')
                     updated |= True
             if updated:
                 self.conn.commit()
+        finally:
+            self.lock.write_release()
 
     def create_table(self, dataset: str) -> None:
         """创建数据集"""
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             assert not re.findall(r'\s', dataset)
             self.conn.execute(f"""CREATE TABLE IF NOT EXISTS `{dataset}` (
                 `key` TEXT PRIMARY KEY NOT NULL,
                 `value` BLOB,
                 `encoding` INTEGER NOT NULL,
                 `expired_at` REAL NOT NULL
             )""")
             self.conn.execute(f"""CREATE INDEX IF NOT EXISTS expired_at ON `{dataset}` (`expired_at`)""")
             self.conn.commit()
+        finally:
+            self.lock.write_release()
 
     def encode_value(self, value: Any) -> Tuple[Any, int]:
         """数据编码"""
         if value is None:
             return value, 0     # 原始数据
         elif isinstance(value, bool):
             return value, 64
@@ -130,33 +137,37 @@
             case 68:
                 return int(value)
             case _:
                 raise ValueError(encoding)
 
     def set(self, dataset: str = None, key: str = '', value: Any = None, expire: float = math.inf) -> None:
         """设置键值"""
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             if not dataset:
                 dataset = self.default_dataset
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             assert isinstance(key, str), 'key必须是字符串'
             assert key, 'key不能为空'
             if dataset not in self.datasets:
                 self.create_table(dataset=dataset)
                 self.datasets.clear()
                 self.datasets.update(self.get_tables())
             payload, encoding = self.encode_value(value=value)
             sql: str = f"""REPLACE INTO `{dataset}` (`key`, `value`, `encoding`, `expired_at`) VALUES(?,?,?,?)"""
             self.conn.execute(sql, (key, payload, encoding, time.time() + expire))
             self.conn.commit()
+        finally:
+            self.lock.write_release()
 
     def rename(self, dataset: str = None, key: str = '', new_key: str = '') -> None:
         """重命名键值"""
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             if not dataset:
                 dataset = self.default_dataset
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             assert isinstance(key, str), 'key必须是字符串'
             assert key, 'key不能为空'
             assert isinstance(new_key, str), 'new_key必须是字符串'
@@ -166,18 +177,21 @@
             if dataset not in self.datasets:
                 self.create_table(dataset=dataset)
                 self.datasets.clear()
                 self.datasets.update(self.get_tables())
             sql: str = f"""UPDATE `{dataset}` SET `key` = ? WHERE `key` = ?"""
             self.conn.execute(sql, (new_key, key))
             self.conn.commit()
+        finally:
+            self.lock.write_release()
 
     def update(self, dataset: str = None, items: Dict[str, Any] = None, expire: float = math.inf) -> None:
         """批量设置键值"""
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             if not dataset:
                 dataset = self.default_dataset
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             assert isinstance(items, dict), 'items必须是字典'
             if not items:
                 return
@@ -192,35 +206,41 @@
             now = time.time()
             for key, value in items.items():
                 payload, encoding = self.encode_value(value=value)
                 ps.append((key, payload, encoding, now + expire))
             sql: str = f"""REPLACE INTO `{dataset}` (`key`, `value`, `encoding`, `expired_at`) VALUES(?,?,?,?)"""
             self.conn.executemany(sql, ps)
             self.conn.commit()
+        finally:
+            self.lock.write_release()
 
     def add(self, dataset: str = None, key: str = '', value: Any = None, expire: float = math.inf) -> None:
         """添加值到集合中"""
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             if not dataset:
                 dataset = self.default_dataset
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             assert isinstance(key, str), 'key必须是字符串'
             assert key, 'key不能为空'
             rs: Set = self.get(dataset=dataset, key=key) or set()
             try:
                 hash(value)
                 rs.add(value)
             except TypeError:
                 rs.update(value)
             self.set(dataset=dataset, key=key, value=rs, expire=expire)
+        finally:
+            self.lock.write_release()
 
     def delete(self, dataset: str = None, key: str | List[str] = None) -> None:
         """删除键值对"""
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             if not dataset:
                 dataset = self.default_dataset
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             assert key, 'key不能为空'
             if isinstance(key, str):
                 key: List[str] = [key]
@@ -231,106 +251,101 @@
             else:
                 raise ValueError('key必须是字符串或字符串列表')
             if dataset in self.datasets:
                 placeholders: str = ', '.join(['?'] * len(key))
                 sql: str = f"""DELETE FROM `{dataset}` WHERE `key` IN ({placeholders})"""
                 self.conn.execute(sql, key)
                 self.conn.commit()
+        finally:
+            self.lock.write_release()
 
     def get(self, dataset: str = None, key: str = '') -> Any | None:
         """获取键值"""
+        r = None
         with self.lock:
             if not dataset:
                 dataset = self.default_dataset
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             assert isinstance(key, str), 'key必须是字符串'
             assert key, 'key不能为空'
             if dataset in self.datasets:
                 cursor = self.conn.cursor()
-                sql: str = f"""SELECT `value`, `encoding`, `expired_at` FROM `{dataset}` WHERE `key`=?"""
-                r = cursor.execute(sql, (key, ))
+                sql: str = f"""SELECT `value`, `encoding` FROM `{dataset}` WHERE `key` = ? AND `expired_at` > ?"""
+                r = cursor.execute(sql, (key, time.time()))
                 r = r.fetchone()
-                if r is None:
-                    return r
-                else:
-                    value, encoding, expired_at = r
-                    if expired_at > time.time():
-                        return self.decode_value(value=value, encoding=encoding)
-                    else:
-                        self.delete(dataset=dataset, key=key)
-                        return None
+        if r is None:
+            return r
+        else:
+            value, encoding = r
+            return self.decode_value(value=value, encoding=encoding)
 
     def keys(self, dataset: str = None) -> List[str] | None:
         """列出所有键名"""
         with self.lock:
             if not dataset:
                 dataset = self.default_dataset
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             if dataset in self.datasets:
                 cursor = self.conn.cursor()
-                now: float = time.time()
-                sql: str = f"""SELECT `key`, `expired_at` FROM `{dataset}`"""
-                r = cursor.execute(sql)
+                sql: str = f"""SELECT `key` FROM `{dataset}` WHERE `expired_at` > ?"""
+                r = cursor.execute(sql, (time.time(), ))
                 result: List[str] = []
-                delete_keys: List[str] = []
-                for key, expired_at in r.fetchall():
-                    if expired_at > now:
-                        result.append(key)
-                    else:
-                        delete_keys.append(key)
-                if delete_keys:
-                    self.delete(dataset=dataset, key=delete_keys)
+                for (key, ) in r.fetchall():
+                    result.append(key)
                 return result
 
     def items(self, dataset: str = None) -> Dict:
         """列出所有键值对"""
+        rs: List[Tuple] = []
+        result: Dict[str, Any] = {}
         with self.lock:
             if not dataset:
                 dataset = self.default_dataset
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             if dataset in self.datasets:
                 cursor = self.conn.cursor()
-                now: float = time.time()
-                sql: str = f"""SELECT `key`, `value`, `encoding`, `expired_at` FROM `{dataset}`"""
-                r = cursor.execute(sql)
-                result: Dict[str, Any] = {}
-                delete_keys: List[str] = []
-                for key, value, encoding, expired_at in r.fetchall():
-                    print([key, value, encoding, expired_at])
-                    if expired_at > now:
-                        result[key] = self.decode_value(value=value, encoding=encoding)
-                    else:
-                        delete_keys.append(key)
-                if delete_keys:
-                    self.delete(dataset=dataset, key=delete_keys)
-                return result
+                sql: str = f"""SELECT `key`, `value`, `encoding` FROM `{dataset}` WHERE `expired_at` > ?"""
+                r = cursor.execute(sql, (time.time(), ))
+                rs = r.fetchall()
+        for key, value, encoding in rs:
+            result[key] = self.decode_value(value=value, encoding=encoding)
+        return result
 
     def drop_table(self, dataset: str):
         """删除数据集"""
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             assert isinstance(dataset, str), 'dataset必须是字符串'
             assert dataset, 'dataset不能为空'
             if dataset in self.datasets:
                 sql: str = f"""DROP TABLE IF EXISTS `{dataset}`"""
                 self.conn.execute(sql)
                 self.conn.commit()
                 self.datasets.discard(dataset)
+        finally:
+            self.lock.write_release()
 
     def vacuum(self, force: bool = True):
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             key_vacuum_at: str = '__VACUUM__'
             vacuum_at: int | None = self.get(key=key_vacuum_at)
             if force or not vacuum_at or time.time() - vacuum_at >= 86400:
                 self.conn.execute('VACUUM')
                 self.set(key=key_vacuum_at, value=int(time.time()))
+        finally:
+            self.lock.write_release()
 
     def close(self):
-        with self.lock:
+        self.lock.write_acquire()
+        try:
             self.conn.commit()
             for dataset in self.datasets:
                 sql: str = f"DELETE FROM `{dataset}` WHERE `expired_at` <= ?"
                 self.conn.execute(sql, (int(time.time()), ))
             self.vacuum(force=False)
             self.conn.close()
+        finally:
+            self.lock.write_release()
```

### Comparing `jy_lib-0.7.9/jy_lib/clickhouse.py` & `jy_lib-0.8.0/jy_lib/clickhouse.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/compressor.py` & `jy_lib-0.8.0/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/country.py` & `jy_lib-0.8.0/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/currency.py` & `jy_lib-0.8.0/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/date.py` & `jy_lib-0.8.0/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/decorator.py` & `jy_lib-0.8.0/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/exchange.py` & `jy_lib-0.8.0/jy_lib/exchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,26 +23,26 @@
             extra_ids.add(self.mic)
         return extra_ids
 
 
 class Exchange(Enum):
     """交易所简称枚举"""
     BSE = ExchangeDetail(acronym='BSE', mic='BJSE', extra_ids=['BJ', 'BJE', 'BJEX'], en_name='BEIJING STOCK EXCHANGE', cn_name='北京证券交易所', website='www.bse.cn')
-    CFFEX = ExchangeDetail(acronym='CFFEX', mic='CCFX', extra_ids=['IF'], en_name='CHINA FINANCIAL FUTURES EXCHANGE', cn_name='中国金融期货交易所', website='www.cffex.com.cn')
+    CFFEX = ExchangeDetail(acronym='CFFEX', mic='CCFX', extra_ids=['IF', 'CFX'], en_name='CHINA FINANCIAL FUTURES EXCHANGE', cn_name='中国金融期货交易所', website='www.cffex.com.cn')
     NEEQ = ExchangeDetail(acronym='NEEQ', mic='NEEQ', en_name='NATIONAL EQUITIES EXCHANGE AND QUOTATIONS', cn_name='全国中小企业股份转让系统', website='www.neeq.com.cn')
     SGE = ExchangeDetail(acronym='SGE', mic='SGEX', en_name='SHANGHAI GOLD EXCHANGE', cn_name='上海黄金交易所', website='www.sge.sh')
     CFETS = ExchangeDetail(acronym='CFETS', mic='XCFE', en_name='CHINA FOREIGN EXCHANGE TRADE SYSTEM', cn_name='中国外汇交易系统', website='www.chinamoney.com.cn')
-    SSE = ExchangeDetail(acronym='SSE', mic='XSHG', extra_ids=['SH', 'SHO'], en_name='SHANGHAI STOCK EXCHANGE', cn_name='上海证券交易所', website='www.szse.cn')
-    SZSE = ExchangeDetail(acronym='SZSE', mic='XSHE', extra_ids=['SZ', 'SZO'], en_name='SHENZHEN STOCK EXCHANGE', cn_name='深圳证券交易所', website='www.szse.cn')
+    SSE = ExchangeDetail(acronym='SSE', mic='XSHG', extra_ids=['SH', 'SHO', 'SHOP'], en_name='SHANGHAI STOCK EXCHANGE', cn_name='上海证券交易所', website='www.szse.cn')
+    SZSE = ExchangeDetail(acronym='SZSE', mic='XSHE', extra_ids=['SZ', 'SZO', 'SZOP'], en_name='SHENZHEN STOCK EXCHANGE', cn_name='深圳证券交易所', website='www.szse.cn')
     CSI = ExchangeDetail(acronym='CSI', mic='', en_name='CHINA SECURITIES INDEX', cn_name='中证指数', website='www.csindex.com.cn')
-    SHFE = ExchangeDetail(acronym='SHFE', mic='XSGE', extra_ids=['SF'], en_name='SHANGHAI FUTURES EXCHANGE', cn_name='上海期货交易所', website='www.shfe.com.cn')
+    SHFE = ExchangeDetail(acronym='SHFE', mic='XSGE', extra_ids=['SF', 'SHF'], en_name='SHANGHAI FUTURES EXCHANGE', cn_name='上海期货交易所', website='www.shfe.com.cn')
     INE = ExchangeDetail(acronym='INE', mic='XINE', en_name='SHANGHAI INTERNATIONAL ENERGY EXCHANGE', cn_name='上海国际能源交易中心', website='www.ine.cn')
     DCE = ExchangeDetail(acronym='DCE', mic='XDCE', extra_ids=['DF'], en_name='DALIAN COMMODITY EXCHANGE', cn_name='大连商品交易所', website='www.dce.com.cn')
-    CZCE = ExchangeDetail(acronym='CZCE', mic='XZCE', extra_ids=['ZF'], en_name='ZHENGZHOU COMMODITY EXCHANGE', cn_name='郑州商品交易所', website='www.czce.com.cn')
-    GFEX = ExchangeDetail(acronym='GFEX', mic='', extra_ids=['GF'], en_name='GUANGZHOU COMMODITY EXCHANGE', cn_name='广州商品交易所', website='www.gfex.com.cn')
+    CZCE = ExchangeDetail(acronym='CZCE', mic='XZCE', extra_ids=['ZF', 'ZCE'], en_name='ZHENGZHOU COMMODITY EXCHANGE', cn_name='郑州商品交易所', website='www.czce.com.cn')
+    GFEX = ExchangeDetail(acronym='GFEX', mic='', extra_ids=['GF', 'GFE'], en_name='GUANGZHOU COMMODITY EXCHANGE', cn_name='广州商品交易所', website='www.gfex.com.cn')
     CBOT = ExchangeDetail(acronym='CBOT', mic='CBTS', en_name='CME SWAPS MARKETS (CBOT)', cn_name='芝加哥期货交易所', website='www.cmegroup.com')
     COMEX = ExchangeDetail(acronym='COMEX', mic='CECS', en_name='CME SWAPS MARKETS (COMEX)', cn_name='纽约商品交易所', website='www.cmegroup.com')
     CME = ExchangeDetail(acronym='CME', mic='CMES', en_name='CME SWAPS MARKETS (CME)', cn_name='芝加哥商业交易所', website='www.cmegroup.com')
     NYMEX = ExchangeDetail(acronym='NYMEX', mic='NYMS', en_name='CME SWAPS MARKETS (NYMEX)', cn_name='纽约商品交易所', website='www.cmegroup.com')
     NYBOT = ExchangeDetail(acronym='NYBOT', mic='', en_name='THE NEW YORK BOARD OF TRADE', cn_name='纽约期货交易所', website='www.nybot.com')
     LME = ExchangeDetail(acronym='LME', mic='XLME', en_name='LONDON METAL EXCHANGE', cn_name='伦敦金属交易所', website='www.lme.co.uk')
     TOCOM = ExchangeDetail(acronym='TOCOM', mic='XTKT', en_name='TOKYO COMMODITY EXCHANGE', cn_name='东京商品交易所', website='www.tocom.or.jp')
```

### Comparing `jy_lib-0.7.9/jy_lib/forex.py` & `jy_lib-0.8.0/jy_lib/forex.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/interrupt_protect.py` & `jy_lib-0.8.0/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/lock.py` & `jy_lib-0.8.0/jy_lib/lock.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import threading
+import time
 
 
 class SyncRWLock:
     """同步读写锁,单写多读"""
-    def __init__(self):
+    def __init__(self, reentrant: bool = True):
         self.readers: int = 0  # 读取者数量
-        self.r_lock: threading.Lock = threading.Lock()
-        self.w_lock: threading.Lock = threading.Lock()
+        self.reentrant: bool = reentrant
+        if reentrant:
+            self.r_lock: threading.RLock = threading.RLock()
+            self.w_lock: threading.RLock = threading.RLock()
+        else:
+            self.r_lock: threading.Lock = threading.Lock()
+            self.w_lock: threading.Lock = threading.Lock()
 
     def read_acquire(self):
         """获取读锁"""
         with self.r_lock:
             self.readers += 1
             if self.readers == 1:
                 self.w_lock.acquire()
```

### Comparing `jy_lib-0.7.9/jy_lib/math.py` & `jy_lib-0.8.0/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/nav.py` & `jy_lib-0.8.0/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/reader.py` & `jy_lib-0.8.0/jy_lib/reader.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/smb_client.py` & `jy_lib-0.8.0/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/symbol.py` & `jy_lib-0.8.0/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/symbol_em.py` & `jy_lib-0.8.0/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/jy_lib/time.py` & `jy_lib-0.8.0/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.9/pyproject.toml` & `jy_lib-0.8.0/pyproject.toml`

 * *Files identical despite different names*

