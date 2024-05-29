# Comparing `tmp/kassorm-1.1.4.tar.gz` & `tmp/kassorm-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kassorm-1.1.4.tar", max compression
+gzip compressed data, was "kassorm-1.1.5.tar", max compression
```

## Comparing `kassorm-1.1.4.tar` & `kassorm-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      214 2024-02-19 20:45:30.559425 kassorm-1.1.4/KassOrm/__init__.py
--rw-r--r--   0        0        0     5898 2024-02-19 22:48:38.810079 kassorm-1.1.4/KassOrm/Conn.py
--rw-r--r--   0        0        0     3560 2024-02-20 19:26:41.325508 kassorm-1.1.4/KassOrm/Creator.py
--rw-r--r--   0        0        0       81 2024-02-15 23:50:41.137924 kassorm-1.1.4/KassOrm/Factory.py
--rw-r--r--   0        0        0    19808 2024-03-29 14:33:34.815317 kassorm-1.1.4/KassOrm/Migration.py
--rw-r--r--   0        0        0     8812 2024-03-29 22:53:54.662614 kassorm-1.1.4/KassOrm/Modelr.py
--rw-r--r--   0        0        0    19462 2024-03-29 22:54:20.927276 kassorm-1.1.4/KassOrm/Querier.py
--rw-r--r--   0        0        0       64 2024-02-15 23:53:54.584552 kassorm-1.1.4/KassOrm/Seeder.py
--rw-r--r--   0        0        0        0 2024-01-02 19:34:05.905914 kassorm-1.1.4/KassOrm/stubs/__init__.py
--rw-r--r--   0        0        0      232 2024-02-15 18:08:52.972775 kassorm-1.1.4/KassOrm/stubs/migration_alter.stub
--rw-r--r--   0        0        0      320 2024-02-20 14:02:58.145096 kassorm-1.1.4/KassOrm/stubs/migration_create.stub
--rw-r--r--   0        0        0       91 2024-02-20 20:17:08.691388 kassorm-1.1.4/KassOrm/stubs/model.stub
--rw-r--r--   0        0        0     1089 2024-02-06 08:30:09.055236 kassorm-1.1.4/LICENSE
--rw-r--r--   0        0        0     1062 2024-03-30 11:49:38.529584 kassorm-1.1.4/pyproject.toml
--rw-r--r--   0        0        0    19446 2024-03-26 12:23:32.184978 kassorm-1.1.4/README.md
--rw-r--r--   0        0        0    20219 1970-01-01 00:00:00.000000 kassorm-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      214 2024-02-19 20:45:30.559425 kassorm-1.1.5/KassOrm/__init__.py
+-rw-r--r--   0        0        0     5930 2024-05-29 16:25:30.510063 kassorm-1.1.5/KassOrm/Conn.py
+-rw-r--r--   0        0        0     3560 2024-02-20 19:26:41.325508 kassorm-1.1.5/KassOrm/Creator.py
+-rw-r--r--   0        0        0       81 2024-02-15 23:50:41.137924 kassorm-1.1.5/KassOrm/Factory.py
+-rw-r--r--   0        0        0    20521 2024-03-30 18:34:59.565415 kassorm-1.1.5/KassOrm/Migration.py
+-rw-r--r--   0        0        0     8836 2024-05-29 16:26:13.417578 kassorm-1.1.5/KassOrm/Modelr.py
+-rw-r--r--   0        0        0    19462 2024-03-29 22:54:20.927276 kassorm-1.1.5/KassOrm/Querier.py
+-rw-r--r--   0        0        0       64 2024-02-15 23:53:54.584552 kassorm-1.1.5/KassOrm/Seeder.py
+-rw-r--r--   0        0        0        0 2024-01-02 19:34:05.905914 kassorm-1.1.5/KassOrm/stubs/__init__.py
+-rw-r--r--   0        0        0      232 2024-02-15 18:08:52.972775 kassorm-1.1.5/KassOrm/stubs/migration_alter.stub
+-rw-r--r--   0        0        0      320 2024-02-20 14:02:58.145096 kassorm-1.1.5/KassOrm/stubs/migration_create.stub
+-rw-r--r--   0        0        0       91 2024-02-20 20:17:08.691388 kassorm-1.1.5/KassOrm/stubs/model.stub
+-rw-r--r--   0        0        0     1089 2024-02-06 08:30:09.055236 kassorm-1.1.5/LICENSE
+-rw-r--r--   0        0        0     1062 2024-05-29 16:26:20.318627 kassorm-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    19446 2024-03-26 12:23:32.184978 kassorm-1.1.5/README.md
+-rw-r--r--   0        0        0    20219 1970-01-01 00:00:00.000000 kassorm-1.1.5/PKG-INFO
```

### Comparing `kassorm-1.1.4/KassOrm/Conn.py` & `kassorm-1.1.5/KassOrm/Conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import mysql.connector
 import logging
 from mysql.connector import errorcode
+import mysql.connector.pooling
 
 
 class Conn:
 
     def __init__(self, conn=None) -> None:
         logging.basicConfig(
             filename="logs/KassOrm.log",
```

### Comparing `kassorm-1.1.4/KassOrm/Creator.py` & `kassorm-1.1.5/KassOrm/Creator.py`

 * *Files identical despite different names*

### Comparing `kassorm-1.1.4/KassOrm/Migration.py` & `kassorm-1.1.5/KassOrm/Migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,39 @@
         Args:
             name (str): nome da coluna
         """
         col = "{} DATETIME NOT NULL".format(name)
         self.columns.append(col)
         return self
 
+    def date(self, name: str):
+        col = "{} DATE NOT NULL ".format(name)
+        self.columns.append(col)
+        return self
+
+    def longtext(self, name: str):
+        col = "{} LONGTEXT NOT NULL ".format(name)
+        self.columns.append(col)
+        return self
+
+    def mediumtext(self, name: str):
+        col = "{} MEDIUMTEXT NOT NULL ".format(name)
+        self.columns.append(col)
+        return self
+
+    def decimal(self, name: str):
+        col = "{} DECIMAL NOT NULL ".format(name)
+        self.columns.append(col)
+        return self
+
+    def float(self, name: str):
+        col = "{} FLOAT NOT NULL ".format(name)
+        self.columns.append(col)
+        return self
+
     def default(self, value: str):
         """Propriedade 'DEFAULT' da coluna definindo qual o valor padrão
 
         Args:
             value (str): valor padrão da coluna
         """
         if self.columns:
```

### Comparing `kassorm-1.1.4/KassOrm/Modelr.py` & `kassorm-1.1.5/KassOrm/Modelr.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,16 @@
                     for chave, valor in dicionario.items()
                     if chave in self.columns
                 }
                 new_rows.append(new_dict)
             rows = new_rows[0]
 
         rows = json.dumps(rows, default=self.json_date_serializer)
-        return json.loads(rows)
+        rows = json.loads(rows)
+        return rows[0]
 
     def toSql(self, formmated: bool = True):
         return self.querier.toSql(formmated)
 
     def delete(self):
         if self.__with_trash():
             return self.querier.update({self.__softdelete__: dt.now()})
```

### Comparing `kassorm-1.1.4/KassOrm/Querier.py` & `kassorm-1.1.5/KassOrm/Querier.py`

 * *Files identical despite different names*

### Comparing `kassorm-1.1.4/LICENSE` & `kassorm-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kassorm-1.1.4/pyproject.toml` & `kassorm-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "KassOrm"
-version = "1.1.4"
+version = "1.1.5"
 description = "Gerenciador de banco de dados relacional"
 authors = ["kassiodouglas <kass.doug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "KassOrm"}]
 classifiers = [
     "Natural Language :: Portuguese (Brazilian)",
```

### Comparing `kassorm-1.1.4/README.md` & `kassorm-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kassorm-1.1.4/PKG-INFO` & `kassorm-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KassOrm
-Version: 1.1.4
+Version: 1.1.5
 Summary: Gerenciador de banco de dados relacional
 License: MIT
 Author: kassiodouglas
 Author-email: kass.doug@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

