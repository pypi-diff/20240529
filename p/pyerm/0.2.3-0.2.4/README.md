# Comparing `tmp/pyerm-0.2.3.tar.gz` & `tmp/pyerm-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerm-0.2.3.tar", last modified: Fri Mar 15 07:17:45 2024, max compression
+gzip compressed data, was "pyerm-0.2.4.tar", last modified: Wed May 29 12:55:54 2024, max compression
```

## Comparing `pyerm-0.2.3.tar` & `pyerm-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:17:45.715413 pyerm-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 07:17:37.000000 pyerm-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-03-15 07:17:45.715413 pyerm-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-03-15 07:17:37.000000 pyerm-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:17:45.711413 pyerm-0.2.3/pyerm/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/dbbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:17:45.711413 pyerm-0.2.3/pyerm/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/scripts/db_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/scripts/erm_webui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/scripts/export_xls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:17:45.711413 pyerm-0.2.3/pyerm/webUI/
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/webUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/webUI/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/webUI/home.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-03-15 07:17:37.000000 pyerm-0.2.3/pyerm/webUI/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:17:45.715413 pyerm-0.2.3/pyerm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-03-15 07:17:45.000000 pyerm-0.2.3/pyerm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-15 07:17:45.000000 pyerm-0.2.3/pyerm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 07:17:45.000000 pyerm-0.2.3/pyerm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-15 07:17:45.000000 pyerm-0.2.3/pyerm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-15 07:17:45.000000 pyerm-0.2.3/pyerm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 07:17:45.000000 pyerm-0.2.3/pyerm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 07:17:45.715413 pyerm-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-15 07:17:37.000000 pyerm-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:55:54.955794 pyerm-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:55:42.000000 pyerm-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-29 12:55:54.951794 pyerm-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-29 12:55:42.000000 pyerm-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:55:54.951794 pyerm-0.2.4/pyerm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:55:54.951794 pyerm-0.2.4/pyerm/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/database/dbbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14342 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/database/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:55:54.951794 pyerm-0.2.4/pyerm/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/scripts/db_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/scripts/erm_webui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/scripts/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/scripts/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:55:54.951794 pyerm-0.2.4/pyerm/webUI/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/webUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/webUI/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/webUI/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-29 12:55:42.000000 pyerm-0.2.4/pyerm/webUI/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:55:54.951794 pyerm-0.2.4/pyerm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-29 12:55:54.000000 pyerm-0.2.4/pyerm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-29 12:55:54.000000 pyerm-0.2.4/pyerm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:55:54.000000 pyerm-0.2.4/pyerm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 12:55:54.000000 pyerm-0.2.4/pyerm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 12:55:54.000000 pyerm-0.2.4/pyerm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 12:55:54.000000 pyerm-0.2.4/pyerm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:55:54.955794 pyerm-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-29 12:55:42.000000 pyerm-0.2.4/setup.py
```

### Comparing `pyerm-0.2.3/PKG-INFO` & `pyerm-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,64 @@
-Metadata-Version: 2.1
-Name: pyerm
-Version: 0.2.3
-Summary: This project is an local experiment record manager for python based on SQLite DMS, suitable for recording experiment and analysing experiment data with a web UI, which can help you efficiently save your experiment settings and results for later analysis.
-Home-page: https://github.com/Mr-SGXXX/pyerm
-Author: Yuxuan Shao
-Author-email: yx_shao@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: pillow
-Requires-Dist: xlsxwriter
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: streamlit>=1.31.1
-
 # PyERM (Python Experiment Record Manager)
-This project is an experiment record manager for python based on SQLite DMS, which can help you efficiently save your experiment settings and results for later analysis. 
+This project is a general experiment record manager for python based on SQLite DMS, which can help you efficiently save your experiment settings and results for later analysis. 
 
 *In the current version, all operations will be performed locally.*
 
 # Introduction
-This project is used to save the settings and results of any experiment consists of three parts: method, data, task. 
+This project is used to save the settings and results of any experiment which consists of three parts: method, data, task. 
 
-Besides, the basic information and detail information of the experiment will also be recorded.
+Besides, the basic information and detail information of the experiment can also be recorded.
 
-All data you want can be efficiently saved by API provided without knowing the detail implement, but I suggest reading the table introduction for further dealing with the records. 
+All data you want can be efficiently saved by API provided without knowing the project detail implement, but I suggest reading the table introduction for further dealing with the records. 
 
 ## Install Introduction
 All you need to do for using the python package is using the following command:
 
 ```pip install pyerm```
 
 ## Workflow Introduction
 ### Table Define & Init
 Before starting the experiment, you need to init the tables you need for the experiment by three init function: `data_init()`, `method_init()`, `task_init()`.
 
- You need to input the name and experiment parameter for the first two. The function can automatically detect the data type, and they will create the table if not exist. If you want to define the DMS type yourself, you can input a `param_def_dict` to these function, whose key means column name, and value means column SQL type define, like `{"people", "TEXT DEFAULT NULL"}`. 
+ You need to input the name and experiment parameter for the first two. The function can automatically detect the data type from input dict, like `{"name: "Alice", "age": 20}`, and they will create the table if not exist. If you want to define the DMS type yourself, you can input a `param_def_dict` to these function, whose key means column name, and value means column SQL type define, like `{"name", "TEXT DEFAULT NULL", "age": "INTEGER DEFAULT 20"}`. 
 
 ### Experiment 
 
 The experiment recorder mainly consists of four parts, `experiment_start()`, `experiment_over()`, `experiment_failed()`, `detail_update()`. From the name of these function, you can easily know where and how to use them.
 
 `experiment_start()` saves the basic experiment information before experiment formally starts and will set the experiment status to running.
 
 `experiment_over()` saves the experiment results after experiment ends and will set the experiment status to over.
 
 `experiment_failed()` saves the reason why experiment failed and will set the experiment status to failed.
 
 `detail_update()` saves the intermediate results. It's optional, and if you never use it and don't manually set the define dict, the detail table may not be created.
 
+you can see a specific example in the [github repositories of this project](https://github.com/Mr-SGXXX/pyerm/tree/master/examples) 
+
 
 ## Scripts Introduction
-### export_xls 
-Export the content of a SQLite database to an Excel file
+### export_zip 
+Export the content of a SQLite database to an Excel file and the result images (if exists) in a zip
 ```shell
-export_xls db_path(default ~/experiment.db) output_path(default ./experiment_record.xls)
+export_zip db_path(default ~/experiment.db) output_dir(default ./)
 ```
 ### db_merge 
-Merge two SQLite databases.
+Merge two SQLite databases. The two database must have the same structure for current version.
 ```shell
 db_merge db_path_destination db_path_source
 ```
 
+### pyerm_webui
+Open the WebUI of pyerm, and other devices in the network can also access it for remote check. 
+In the WebUI, you can see all the table of the database including the images of result table or use SQL to get what you want to see. 
+Besides, the WebUI also offers a way to download the zip the same as `export_zip` or the raw db file. 
+```shell
+pyerm_webui
+```
 
 ## Table Introduction
 
 ### Experiment Table
 All experiments' basic information will be recorded in the experiment_list table. It contains the description of the method, the method (with its setting id) & data (with its setting id) & task, the start & end time of the experiment, useful & total time cost, tags, experimenters, failure reason and the experiment status, each experiment is identified by the experiment id.
 
 ### Method Table
@@ -79,25 +70,26 @@
 Each Data is identified by its corresponding data name, and any different data will be assigned a different table for saving its different parameter setting, such as data-specific preprocess parameters, etc. The table is used to save different parameter for every data.
 
 The only necessary column for method table is the data setting id, which will be set automatically, other specific column is set by users.
 
 ### Result Table
 Each Result Table is identified by its corresponding task name, and different tasks will be assigned with different tables for saving its different experiment results, such as accuracy for classification, normalized mutual information for clustering. 
 
-Besides, this table offers several columns for saving image in order for latter visualization. 
+Besides, this table can save the result images without amount limit in the code. 
 
 The only necessary column for result table is the experiment id, other specific column is set by users.
 
 ### Detail Table
-Each Detail Table is identified by its corresponding method name, different methods are related to different detail table. During an experiment, you may need to record some intermediate results, which can be saved in this table.
+Each Detail Table is identified by its corresponding method name, different methods are related to different detail table. During an experiment, you may need to record some intermediate results, such as epoch&loss for deep learning, which can be saved in this table.
 
 The only necessary column for detail table is the detail id (which can be set automatically) and the experiment id, other specific column is set by users.
 
 
 # Future Plan
 
-- [ ] Some Scripts For Better Usage  
+- [x] Web UI Visualization 
 - [ ] Experiment Summary Report Generate
-- [ ] Web UI Visualize & Commonly Used Analyze Fuctions
+- [ ] Commonly Used Analyze Fuctions
+- [ ] Bug fix & performence improving
 
 # Contact
 My email is yx_shao@qq.com. If you have any question or advice, please contact me.
```

### Comparing `pyerm-0.2.3/pyerm/__init__.py` & `pyerm-0.2.4/pyerm/database/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,12 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# Version: 0.2.2
+# Version: 0.2.4
 
-import os
 from .experiment import Experiment
 
-PACKAGE_PATH = os.path.dirname(os.path.abspath(__file__))
-
 __all__ = ["Experiment"]
```

### Comparing `pyerm-0.2.3/pyerm/dbbase.py` & `pyerm-0.2.4/pyerm/database/dbbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# Version: 0.2.1
+# Version: 0.2.4
 
 import sqlite3
 import re
 
 class Database:
     def __init__(self, db_path:str, output_info=True) -> None:
         self.db_path = db_path
@@ -66,62 +66,74 @@
     def __del__(self):
         self.cursor.close()
         self.conn.close()
     
     def get_table(self, table_name:str):
         return self[table_name]
 
+    def get_db_version(self):
+        self.cursor.execute("PRAGMA data_version;")
+        version = self.cursor.fetchone()[0]
+        return version
+
+
 class Table:
     def __init__(self, db:Database, table_name:str, columns:dict=None) -> None:
         self.db = db
+        table_name = table_name.strip().replace(' ', '_')
         self.table_name = table_name
         self._column = None
         if not table_exists(db, table_name):
             assert columns, 'Columns must be provided when creating a new table'
-            columns_str = ', '.join([f'{key} {value}' for key, value in columns.items()])
+            columns_str = ', '.join([f"{key.strip().replace(' ', '_')} {value}" for key, value in columns.items()])
             self.db.cursor.execute(f'CREATE TABLE IF NOT EXISTS {table_name} ({columns_str})')
             self.db.conn.commit()
             self.db.table_names.append(table_name)
             if self.db.info:
                 print(f'Table {table_name} created')
         else:
             if columns is not None:
                 for column, definition in list(columns.items()):
                     if 'VIRTUAL' in definition:
-                        del columns[column]
+                        del columns[column.replace(' ', '_')]
             assert columns is None or list(columns.keys()) == list([column[1] for column in self.db.cursor.execute(f'PRAGMA table_info({table_name})').fetchall()]), f'Columns do not match for table {table_name}, consider to check or change table name'
             if self.db.info:
                 print(f'Table {table_name} already exists')
         self.primary_key = [column[1] for column in self.db.cursor.execute(f'PRAGMA table_info({table_name})').fetchall() if column[5] == 1]
     
     def insert(self, **kwargs) -> int:
         assert len(kwargs) <= len(self.columns), 'Parameter inputted too much'
-        columns = ', '.join(kwargs.keys())
+        columns = ', '.join([key.replace(' ', '_') for key in kwargs.keys()])
         values = ', '.join(['?' for _ in kwargs])
         query = f'INSERT INTO {self.table_name} ({columns}) VALUES ({values})'
         self.db.cursor.execute(query, tuple(kwargs.values()))
         self.db.conn.commit()
         return self.db.cursor.lastrowid
 
     def delete(self, where:str) -> None:
         query = f'DELETE FROM {self.table_name} WHERE {where}'
         self.db.cursor.execute(query)
         self.db.conn.commit()
 
     def update(self, where:str, **kwargs) -> None:
-        set_values = ', '.join([f'{key}=?' for key in kwargs])
+        set_values = ', '.join([f'{key.replace(" ", "_")}=?' for key in kwargs])
         query = f'UPDATE {self.table_name} SET {set_values} WHERE {where}'
         self.db.cursor.execute(query, tuple(kwargs.values()))
         self.db.conn.commit()
 
     def select(self, *columns:str, where:str=None) -> list:
-        columns_str = ', '.join(columns) if columns else '*'
+        columns_str = ', '.join([col.replace(' ', '_') for col in columns]) if columns else '*'
         where_clause = f'WHERE {where}' if where else ''
         query = f'SELECT {columns_str} FROM {self.table_name} {where_clause}'
         return self.db.cursor.execute(query).fetchall()
+    
+    def add_column(self, column_name:str, column_definition:str) -> None:
+        column_name = column_name.replace(' ', '_')
+        self.db.cursor.execute(f'ALTER TABLE {self.table_name} ADD COLUMN {column_name} {column_definition}')
+        self.db.conn.commit()
 
     @property
     def columns(self):
         if self._column is None:
             self._column = [column[1] for column in self.db.cursor.execute(f'PRAGMA table_info({self.table_name})').fetchall()]
         return self._column
 
@@ -138,14 +150,15 @@
         return str([column[1] for column in self.db.cursor.execute(f'PRAGMA table_info({self.table_name})').fetchall()]) + '\n' + \
                 str([column[2] for column in self.db.cursor.execute(f'PRAGMA table_info({self.table_name})').fetchall()]) + '\n' + \
                 str(self.select())
 
 class View:
     def __init__(self, db:Database, view_name:str, query:str=None) -> None:
         self.db = db
+        view_name = view_name.replace(' ', '_')
         self.view_name = view_name
         if not view_exists(db, view_name):
             assert query, 'Query must be provided when creating a new view'
             self.db.cursor.execute(f'CREATE VIEW IF NOT EXISTS {view_name} AS {query}')
             self.query = query
             self.db.conn.commit()
             self.db.view_names.append(view_name)
@@ -154,15 +167,15 @@
         else:
             self.db.cursor.execute(f"SELECT sql FROM sqlite_master WHERE type='view' AND name='{self.view_name}'")
             self.query = self.db.cursor.fetchone()[0]
             if self.db.info:
                 print(f'View {view_name} already exists')
     
     def select(self, *columns:str, where:str=None) -> list:
-        columns = ', '.join(columns) if columns else '*'
+        columns = ', '.join([col.replace(' ', '_') for col in columns]) if columns else '*'
         where = f'WHERE {where}' if where else ''
         return self.db.cursor.execute(f'SELECT {columns} FROM {self.view_name} {where}').fetchall()
     
     @property
     def columns(self):
         columns = self.query.split('SELECT ')[1].split(' FROM')[0].split(',')
         column_names = [col.strip() for col in columns]
```

### Comparing `pyerm-0.2.3/pyerm/scripts/__init__.py` & `pyerm-0.2.4/pyerm/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyerm-0.2.3/pyerm/scripts/db_merge.py` & `pyerm-0.2.4/pyerm/scripts/db_merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 # Version: 0.1.9
 import sqlite3
 import argparse
 import os
 
-from ..dbbase import Table, Database
+from pyerm.database.dbbase import Table, Database
 
 def copy_table(db1:Database, db2:Database, table_name:str):
     table = Table(db2, table_name)
     columns = [info[1] for info in db2.cursor.execute(f"PRAGMA table_info({table_name})").fetchall() if info[1] not in table.primary_key]
     columns_list_str = ', '.join(columns)  
     placeholders = ', '.join(['?'] * len(columns))  
     insert_stmt = f"INSERT INTO {table_name} ({columns_list_str}) VALUES ({placeholders})"
@@ -44,15 +44,15 @@
 def merge_db(db_path1:str, db_path2:str):
     db1 = Database(db_path1)
     db2 = Database(db_path2)
     for table_name in db2.table_names:
         copy_table(db1, db2, table_name)
 
 def main():
-    parser = argparse.ArgumentParser(description='Merge two SQLite databases.')
+    parser = argparse.ArgumentParser(description='Merge two SQLite databases. For now, the merged two databases must have the same schema.')
     parser.add_argument('db_path_destination', type=str, help='Destination database file path.')
     parser.add_argument('db_path_source', type=str, help='Source database file path.')
     args = parser.parse_args()
     if not os.path.exists(args.db_path_destination):
         raise FileNotFoundError(f"The database file {args.db_path_destination} does not exist")
     if not os.path.exists(args.db_path_source):
         raise FileNotFoundError(f"The database file {args.db_path_source} does not exist")
```

### Comparing `pyerm-0.2.3/pyerm/scripts/erm_webui.py` & `pyerm-0.2.4/pyerm/scripts/erm_webui.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 import argparse
 import subprocess
 
 from pyerm import PACKAGE_PATH
 
 def open_webui(port:int=8501):
-    print(PACKAGE_PATH)
     subprocess.run(["streamlit", "run", f"{PACKAGE_PATH}/webUI/app.py", f"server.port={port}"])
 
 def main():
     parser = argparse.ArgumentParser(description='Open the web user interface of the experiment record manager')
     parser.add_argument('port', type=int, nargs='?', default=8501, help='The port number of the web server')
     args = parser.parse_args()
     open_webui(args.port)
```

### Comparing `pyerm-0.2.3/pyerm/scripts/export_xls.py` & `pyerm-0.2.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,46 +16,46 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# Version: 0.2.2
+# Version: 0.2.4
+from setuptools import setup, find_packages
 
-import PIL.Image as Image
-import io
-import pandas as pd
-import sqlite3
-import argparse
-import os
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
 
-USER_HOME = os.path.expanduser('~')
-
-def export_xls(db_path:str, output_path:str):
-    if not os.path.exists(os.path.dirname(output_path)):
-        os.makedirs(os.path.dirname(output_path))
-    conn = sqlite3.connect(db_path)
-    table_names = pd.read_sql_query("SELECT name FROM sqlite_master WHERE type IN ('table', 'view')", conn)
-    writer = pd.ExcelWriter(output_path, engine='xlsxwriter')
-
-    for table_name in table_names['name']:
-        df = pd.read_sql_query(f"SELECT * FROM {table_name}", conn)
-        columns_nonimg = [col for col in df.columns if not col.startswith("image_")]
-        df[columns_nonimg].to_excel(writer, sheet_name=table_name, index=False)
-    writer.close()
-    conn.close()
-
-def main():
-    parser = argparse.ArgumentParser(description="Export the content of a SQLite database to an Excel file")
-    parser.add_argument('db_path', type=str, nargs='?', default=None, help='The path of the database file')
-    parser.add_argument('output_path', type=str, nargs='?', default="./experiment_record.xls", help='The path of the output excel file')
-    args = parser.parse_args()
-    if args.db_path is None:
-        args.db_path = os.path.join(USER_HOME, 'experiment.db')
-    if not os.path.exists(args.db_path):
-        print(f"Error: The database file {args.db_path} does not exist, please run any experiment first or check the database path.")
-        return
-    export_xls(args.db_path, args.output_path)
-
-if __name__ == "__main__":
-    main()
+setup(
+    name='pyerm',
+    version='0.2.4',
+    author='Yuxuan Shao',
+    author_email='yx_shao@qq.com',
+    description='This project is an local experiment record manager for python based on SQLite DMS, suitable for recording experiment and analysing experiment data with a web UI, which can help you efficiently save your experiment settings and results for later analysis.',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Mr-SGXXX/pyerm",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    packages=find_packages(),
+    include_package_data=True,
+    entry_points={
+        'console_scripts': [
+            'export_zip=pyerm.scripts.export_data:main',
+            'db_merge=pyerm.scripts.db_merge:main',
+            'pyerm_webui=pyerm.scripts.erm_webui:main',
+        ],
+    },
+    install_requires=[
+        "pandas",
+        "pillow",
+        "xlsxwriter",
+        "numpy",
+        "matplotlib",
+        "streamlit>=1.31.1"
+    ],
+    python_requires='>=3.9',
+)
```

### Comparing `pyerm-0.2.3/pyerm/webUI/__init__.py` & `pyerm-0.2.4/pyerm/webUI/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# Version: 0.2.1
-from ..dbbase import Database
+# Version: 0.2.4
```

### Comparing `pyerm-0.2.3/pyerm/webUI/app.py` & `pyerm-0.2.4/pyerm/webUI/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# Version: 0.2.2
+# Version: 0.2.4
 
 import streamlit as st
 import os
 
 from home import home
 from tables import tables
 
@@ -33,16 +33,18 @@
 def init():
     if 'db_path' not in st.session_state:
         st.session_state.db_path = os.path.join(USER_HOME, 'experiment.db')
     if 'table_name' not in st.session_state:
         st.session_state.table_name = None
     if 'sql' not in st.session_state:
         st.session_state.sql = None
-    if 'xls' not in st.session_state:
-        st.session_state.xls = None
+    if 'zip' not in st.session_state:
+        st.session_state.zip = None
+    if 'last_version' not in st.session_state:
+        st.session_state.last_version = None
 
 
 def main():
     init()
     st.set_page_config(page_title="PyERM WebUI", page_icon="📊", layout="wide", initial_sidebar_state="auto")
     st.sidebar.title("PyERM WebUI")
     st.sidebar.markdown("## Please select a page")
```

### Comparing `pyerm-0.2.3/pyerm.egg-info/PKG-INFO` & `pyerm-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 Metadata-Version: 2.1
 Name: pyerm
-Version: 0.2.3
+Version: 0.2.4
 Summary: This project is an local experiment record manager for python based on SQLite DMS, suitable for recording experiment and analysing experiment data with a web UI, which can help you efficiently save your experiment settings and results for later analysis.
 Home-page: https://github.com/Mr-SGXXX/pyerm
 Author: Yuxuan Shao
 Author-email: yx_shao@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: pillow
 Requires-Dist: xlsxwriter
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: streamlit>=1.31.1
 
 # PyERM (Python Experiment Record Manager)
-This project is an experiment record manager for python based on SQLite DMS, which can help you efficiently save your experiment settings and results for later analysis. 
+This project is a general experiment record manager for python based on SQLite DMS, which can help you efficiently save your experiment settings and results for later analysis. 
 
 *In the current version, all operations will be performed locally.*
 
 # Introduction
-This project is used to save the settings and results of any experiment consists of three parts: method, data, task. 
+This project is used to save the settings and results of any experiment which consists of three parts: method, data, task. 
 
-Besides, the basic information and detail information of the experiment will also be recorded.
+Besides, the basic information and detail information of the experiment can also be recorded.
 
-All data you want can be efficiently saved by API provided without knowing the detail implement, but I suggest reading the table introduction for further dealing with the records. 
+All data you want can be efficiently saved by API provided without knowing the project detail implement, but I suggest reading the table introduction for further dealing with the records. 
 
 ## Install Introduction
 All you need to do for using the python package is using the following command:
 
 ```pip install pyerm```
 
 ## Workflow Introduction
 ### Table Define & Init
 Before starting the experiment, you need to init the tables you need for the experiment by three init function: `data_init()`, `method_init()`, `task_init()`.
 
- You need to input the name and experiment parameter for the first two. The function can automatically detect the data type, and they will create the table if not exist. If you want to define the DMS type yourself, you can input a `param_def_dict` to these function, whose key means column name, and value means column SQL type define, like `{"people", "TEXT DEFAULT NULL"}`. 
+ You need to input the name and experiment parameter for the first two. The function can automatically detect the data type from input dict, like `{"name: "Alice", "age": 20}`, and they will create the table if not exist. If you want to define the DMS type yourself, you can input a `param_def_dict` to these function, whose key means column name, and value means column SQL type define, like `{"name", "TEXT DEFAULT NULL", "age": "INTEGER DEFAULT 20"}`. 
 
 ### Experiment 
 
 The experiment recorder mainly consists of four parts, `experiment_start()`, `experiment_over()`, `experiment_failed()`, `detail_update()`. From the name of these function, you can easily know where and how to use them.
 
 `experiment_start()` saves the basic experiment information before experiment formally starts and will set the experiment status to running.
 
 `experiment_over()` saves the experiment results after experiment ends and will set the experiment status to over.
 
 `experiment_failed()` saves the reason why experiment failed and will set the experiment status to failed.
 
 `detail_update()` saves the intermediate results. It's optional, and if you never use it and don't manually set the define dict, the detail table may not be created.
 
+you can see a specific example in the [github repositories of this project](https://github.com/Mr-SGXXX/pyerm/tree/master/examples) 
+
 
 ## Scripts Introduction
-### export_xls 
-Export the content of a SQLite database to an Excel file
+### export_zip 
+Export the content of a SQLite database to an Excel file and the result images (if exists) in a zip
 ```shell
-export_xls db_path(default ~/experiment.db) output_path(default ./experiment_record.xls)
+export_zip db_path(default ~/experiment.db) output_dir(default ./)
 ```
 ### db_merge 
-Merge two SQLite databases.
+Merge two SQLite databases. The two database must have the same structure for current version.
 ```shell
 db_merge db_path_destination db_path_source
 ```
 
+### pyerm_webui
+Open the WebUI of pyerm, and other devices in the network can also access it for remote check. 
+In the WebUI, you can see all the table of the database including the images of result table or use SQL to get what you want to see. 
+Besides, the WebUI also offers a way to download the zip the same as `export_zip` or the raw db file. 
+```shell
+pyerm_webui
+```
 
 ## Table Introduction
 
 ### Experiment Table
 All experiments' basic information will be recorded in the experiment_list table. It contains the description of the method, the method (with its setting id) & data (with its setting id) & task, the start & end time of the experiment, useful & total time cost, tags, experimenters, failure reason and the experiment status, each experiment is identified by the experiment id.
 
 ### Method Table
@@ -79,25 +89,26 @@
 Each Data is identified by its corresponding data name, and any different data will be assigned a different table for saving its different parameter setting, such as data-specific preprocess parameters, etc. The table is used to save different parameter for every data.
 
 The only necessary column for method table is the data setting id, which will be set automatically, other specific column is set by users.
 
 ### Result Table
 Each Result Table is identified by its corresponding task name, and different tasks will be assigned with different tables for saving its different experiment results, such as accuracy for classification, normalized mutual information for clustering. 
 
-Besides, this table offers several columns for saving image in order for latter visualization. 
+Besides, this table can save the result images without amount limit in the code. 
 
 The only necessary column for result table is the experiment id, other specific column is set by users.
 
 ### Detail Table
-Each Detail Table is identified by its corresponding method name, different methods are related to different detail table. During an experiment, you may need to record some intermediate results, which can be saved in this table.
+Each Detail Table is identified by its corresponding method name, different methods are related to different detail table. During an experiment, you may need to record some intermediate results, such as epoch&loss for deep learning, which can be saved in this table.
 
 The only necessary column for detail table is the detail id (which can be set automatically) and the experiment id, other specific column is set by users.
 
 
 # Future Plan
 
-- [ ] Some Scripts For Better Usage  
+- [x] Web UI Visualization 
 - [ ] Experiment Summary Report Generate
-- [ ] Web UI Visualize & Commonly Used Analyze Fuctions
+- [ ] Commonly Used Analyze Fuctions
+- [ ] Bug fix & performence improving
 
 # Contact
 My email is yx_shao@qq.com. If you have any question or advice, please contact me.
```

