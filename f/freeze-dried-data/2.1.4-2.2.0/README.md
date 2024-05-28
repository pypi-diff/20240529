# Comparing `tmp/freeze_dried_data-2.1.4.tar.gz` & `tmp/freeze_dried_data-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-2.1.4.tar", last modified: Tue May  7 22:29:24 2024, max compression
+gzip compressed data, was "freeze_dried_data-2.2.0.tar", last modified: Tue May 28 23:04:22 2024, max compression
```

## Comparing `freeze_dried_data-2.1.4.tar` & `freeze_dried_data-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 22:29:24.563307 freeze_dried_data-2.1.4/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2024-05-07 22:28:14.000000 freeze_dried_data-2.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11553 2024-05-07 22:29:24.559307 freeze_dried_data-2.1.4/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    10686 2024-05-07 22:28:14.000000 freeze_dried_data-2.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 22:29:24.559307 freeze_dried_data-2.1.4/freeze_dried_data/
--rwxr-xr-x   0 root         (0) root         (0)       33 2024-05-07 22:28:14.000000 freeze_dried_data-2.1.4/freeze_dried_data/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    30815 2024-05-07 22:28:14.000000 freeze_dried_data-2.1.4/freeze_dried_data/freeze_dried_data.py
--rwxr-xr-x   0 root         (0) root         (0)    11613 2024-05-07 22:28:14.000000 freeze_dried_data-2.1.4/freeze_dried_data/freeze_dried_data_old.py
--rwxr-xr-x   0 root         (0) root         (0)    40245 2024-05-07 22:28:14.000000 freeze_dried_data-2.1.4/freeze_dried_data/test_freeze_dried_data.py
--rwxr-xr-x   0 root         (0) root         (0)     7982 2024-05-07 22:28:14.000000 freeze_dried_data-2.1.4/freeze_dried_data/test_freeze_dried_data_old.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 22:29:24.559307 freeze_dried_data-2.1.4/freeze_dried_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11553 2024-05-07 22:29:24.000000 freeze_dried_data-2.1.4/freeze_dried_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-07 22:29:24.000000 freeze_dried_data-2.1.4/freeze_dried_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 22:29:24.000000 freeze_dried_data-2.1.4/freeze_dried_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-07 22:29:24.000000 freeze_dried_data-2.1.4/freeze_dried_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 22:29:24.563307 freeze_dried_data-2.1.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1125 2024-05-07 22:28:14.000000 freeze_dried_data-2.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1072 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11553 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    10686 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/freeze_dried_data/
+-rwxr-xr-x   0 root         (0) root         (0)       33 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5125 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/efficient_index.py
+-rwxr-xr-x   0 root         (0) root         (0)    34904 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/freeze_dried_data.py
+-rwxr-xr-x   0 root         (0) root         (0)    11613 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/freeze_dried_data_old.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/test_efficient_index.py
+-rwxr-xr-x   0 root         (0) root         (0)    40000 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/test_freeze_dried_data.py
+-rwxr-xr-x   0 root         (0) root         (0)     7982 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/test_freeze_dried_data_old.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11553 2024-05-28 23:04:22.000000 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-28 23:04:22.000000 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 23:04:22.000000 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-28 23:04:22.000000 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1125 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/setup.py
```

### Comparing `freeze_dried_data-2.1.4/LICENSE` & `freeze_dried_data-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.4/PKG-INFO` & `freeze_dried_data-2.2.0/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: freeze_dried_data
-Version: 2.1.4
+Name: freeze-dried-data
+Version: 2.2.0
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.1.4/README.md` & `freeze_dried_data-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.4/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-2.2.0/freeze_dried_data/freeze_dried_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,57 @@
 import pickle as pkl
 import os
 from typing import Any, Dict, Iterator, Tuple, Optional, Union, List
 import sys
 import warnings
+import zlib
+import torch
+from efficient_index import FDDIndexKeyless, FDDIndexComparableKey, FDDIntList, FDDIndexGeneral
 
 # data is stored in the following format:
 # [record, record, ..., record], [custom_property, custom_property, ..., custom_property], [split, split, ..., split], [columns], index_index, 8 bytes for index_index length
 
+
+
+
+type_to_serializer = {
+    'any': pkl.dumps,
+    'str': lambda x: x.encode('utf-8'),
+    'str_compressed': lambda x: zlib.compress(x.encode('utf-8')),
+    'bytes': lambda x: x,
+    'int128': lambda x: x.to_bytes(16, 'little'),
+    'int64': lambda x: x.to_bytes(8, 'little'),
+    'int': lambda x: x.to_bytes(8, 'little'),
+    'int32': lambda x: x.to_bytes(4, 'little'),
+    'int16': lambda x: x.to_bytes(2, 'little'),
+    'int8': lambda x: x.to_bytes(1, 'little'),
+    'numpy': pkl.dumps,
+    'torch': lambda x: pkl.dumps(x.cpu().numpy()),
+    'float': pkl.dumps
+}
+
+type_to_deserializer = {
+    'any': pkl.loads,
+    'str': lambda x: x.decode('utf-8'),
+    'str_compressed': lambda x: zlib.decompress(x).decode('utf-8'),
+    'bytes': lambda x: x,
+    'int128': lambda x: int.from_bytes(x, 'little'),
+    'int64': lambda x: int.from_bytes(x, 'little'),
+    'int': lambda x: int.from_bytes(x, 'little'),
+    'int32': lambda x: int.from_bytes(x, 'little'),
+    'int16': lambda x: int.from_bytes(x, 'little'),
+    'int8': lambda x: int.from_bytes(x, 'little'),
+    'numpy': pkl.loads,
+    'torch': lambda x: torch.from_numpy(pkl.loads(x)),
+    'float': pkl.loads
+}
+
+
+
+
 class BaseFDD:
     """
     Base class for freeze-dried data. Should not be instantiated directly.
     There are two subclasses: RFDD (for reading) and WFDD (for writing).
 
     :param filename: The name of the file.
     """
@@ -80,37 +121,32 @@
 class RFDD(BaseFDD):
     """
     RFDD (Freeze Dried Data Reader) class for reading freeze-dried data files.
 
     :param filename: The path to the freeze-dried data file.
     :param split: The split name to load, defaults to the all rows split.
     :param system_deserialize: The function to use for deserializing the index, splits, and columns.
-    :param no_columns_deserialize: The function to use for deserializing rows when there are no columns.
     :param column_to_deserialize: A tuple of functions to use for deserializing columns. There must be
         one function for each column.
     """
     def __init__(self,
                  filename: str,
                  split: str = 'all_rows',
-                 system_deserialize: callable = pkl.loads,
-                 no_columns_deserialize: callable = pkl.loads,
-                 column_to_deserialize: tuple[callable] = None) -> None:
+                 system_deserialize: callable = pkl.loads) -> None:
         super().__init__(filename)
         self.file = open(filename, 'rb')
         self.system_deserialize = system_deserialize
-        self.no_columns_deserialize = no_columns_deserialize
+        self.no_columns_deserialize = pkl.loads
         
         
         self.load_indices(split)
 
         if self.columns is not None:
-            if column_to_deserialize is None:
+            if self.column_to_deserialize is None:
                 self.column_to_deserialize = tuple(self.system_deserialize for i in range(len(self.columns)))
-            else:
-                self.column_to_deserialize = column_to_deserialize
         
         self.custom_properties_cache = {}
         self.read_row_cache = None
         self.cashed_read_row_key = None
 
         os.register_at_fork(after_in_child=self._after_fork)
 
@@ -152,19 +188,20 @@
             if isinstance(key, tuple):
                 if key in self.index:
                     return self[key]
                 else:
                     if key[0] in self.index:
                         indices = self.index[key[0]]
                         col_index = self.columns[key[1]]
-                        start, end = indices[col_index:col_index+2]
+                        start = indices[col_index]
+                        end = indices[col_index+1]
                         data = self.read_chunk(start, end)
                         return self.column_to_deserialize[col_index](data)
             else:
-                raise KeyError("Key not found.", key)
+                raise KeyError("Key not found.", key, self.index.keys())
         
         if self.columns is None:
             
             start, end = self.index[key]
             data = self.read_chunk(start, end)
 
             return self.no_columns_deserialize(data)
@@ -237,14 +274,26 @@
         else:
             columns_start, columns_end = index_index['_columns_']
             index_index.pop('_columns_')
 
             self.columns = self.system_deserialize(self.read_chunk(columns_start, columns_end))
             if self.columns is not None:
                 self.columns = {n: i for i, n in enumerate(self.columns)}
+        
+        if '_column_def_' in index_index:
+            column_def_start, column_def_end = index_index['_column_def_']
+            index_index.pop('_column_def_')
+            try:
+                self.column_def = self.system_deserialize(self.read_chunk(column_def_start, column_def_end))
+            except Exception as e:
+                import dill
+                self.column_def = dill.loads(self.read_chunk(column_def_start, column_def_end))
+
+            self.column_to_deserialize = {v: type_to_deserializer[t] if isinstance(t, str) else t[1] for v, t in self.column_def.items()}   
+            self.column_to_deserialize = tuple(self.column_to_deserialize.values())
                 
 
         self.custom_properties = {k[6:]:v for k,v in index_index.items() if k.startswith('_prop_')}
 
 
     def __getattr__(self, name: str) -> Any:
         """
@@ -291,15 +340,16 @@
 
         :param key: The index of the column, or the name of the column.
         :return: The value of the column.
         """
         if isinstance(key, str):
             key = self._fdd_row_parent.columns[key]
         if self._fdd_row_cache[key] is None:
-            start, end = self._fdd_row_index[key:key+2]
+            start = self._fdd_row_index[key]
+            end = self._fdd_row_index[key+1]
             if start == end:
                 self._fdd_row_cache[key] = None
                 # alternatively, we could raise an error here
             else:
                 deserialize = self._fdd_row_parent.column_to_deserialize[key]
                 self._fdd_row_cache[key] = deserialize(self._fdd_row_parent.read_chunk(start, end))
             
@@ -363,14 +413,16 @@
         """
         rep = ""
         for i, key in enumerate(self._fdd_row_parent.columns):
             value = self[i]
             rep += f"{key}: {value}\n"
         return rep
 
+
+
 class WFDD(BaseFDD):
     """
     WFDD (Freeze Dried Data Writer) class for writing freeze-dried data files.
 
     :param filename: The path to the freeze-dried data file.
     :param columns: The column names for the data. If None, columns won't be used to store the data.
     :param overwrite: Whether to overwrite an existing file, default is False.
@@ -381,58 +433,64 @@
     :param column_to_deserialize: A tuple of functions to use for deserializing columns. There must be
         one function for each column. If None, the system deserializer is used. This is only necessary
         when reading back data that was written with a custom serializer.
 
     """
     def __init__(self,
                  filename: str,
-                 columns: Tuple[str] = None,
+                 columns: dict[str, str | tuple[callable, callable]] = None,
                  overwrite: bool = False,
                  reopen: bool = False,
                  system_serialize: callable = pkl.dumps,
                  system_deserialize: callable = pkl.loads,
-                 no_columns_serialize: callable = pkl.dumps,
-                 column_to_serialize: tuple[callable] = None,
-                 no_columns_deserialize: callable = pkl.loads,
-                 column_to_deserialize: tuple[callable] = None) -> None:
+                 preserve_order=True,
+                 ) -> None:
         self.__dict__['_initializing'] = True # Use self.__dict__ to bypass __setattr__
         super().__init__(filename)
         
         if not overwrite and not reopen and os.path.exists(filename):
             raise FileExistsError("File already exists.", filename)
         
         if reopen and not os.path.exists(filename):
             raise FileNotFoundError("File not found.", filename)
         
-
+        column_to_serialize = {v: type_to_serializer[t] if isinstance(t, str) else t[0] for v, t in columns.items()} if columns is not None else None
         
+        column_to_deserialize = {v: type_to_deserializer[t] if isinstance(t, str) else t[1] for v, t in columns.items()} if columns is not None else None
+        
+        self.column_def = columns
 
         if columns is not None:
             if column_to_deserialize is None:
                 self.column_to_deserialize = tuple(pkl.loads for i in range(len(columns)))
             else:
-                self.column_to_deserialize = column_to_deserialize
+                self.column_to_deserialize = tuple(column_to_deserialize.values())
             if column_to_serialize is None:
                 self.column_to_serialize = tuple(system_serialize for i in range(len(columns)))
             else:
-                self.column_to_serialize = column_to_serialize
+                self.column_to_serialize = tuple(column_to_serialize.values())
+        else:
+            self.column_to_deserialize = None
+            self.column_to_serialize = None
         
         
         self.system_serialize = system_serialize
         self.system_deserialize = system_deserialize
-        self.no_columns_serialize = no_columns_serialize
-        self.no_columns_deserialize = no_columns_deserialize
+        self.no_columns_serialize = pkl.dumps
+        self.no_columns_deserialize = pkl.loads
+        self.preserve_order = preserve_order
 
         if reopen:
             self.reopen()
         else:
             self.file = open(filename, 'wb+')
             self.unfinished_setters = {}
-            self.index = {}
-            self.columns = columns
+            
+            self.columns = tuple(columns.keys()) if columns is not None else None
+            self.index = FDDIndexGeneral(len(columns)+1 if columns is not None else 2)
             self.custom_properties = {}
             self.split_to_index = {}
         
         self._initializing = False
 
     def __setattr__(self, name: str, value: Any) -> None:
         """
@@ -547,26 +605,45 @@
                     serialize = self.no_columns_serialize
                 data = serialize(v)
                 self.file.write(data)
             positions.append(self.file.tell())
             
         self.index[key] = tuple(positions)    
 
-    def make_split(self, split: str, rows: list | tuple | set | frozenset, overwrite=False) -> None:
+    def make_split(self, split: str, rows: list | tuple | set | frozenset, overwrite=False, keyless=False) -> None:
         """
         Create a split in the WFDD.
 
         :param split: The name of the split.
         :param rows: The iterable of keys for the split.
         """
         if split in self.split_to_index and not overwrite:
             raise ValueError("Split already exists.", split, 'Use overwrite=True to overwrite it.')
         
         if isinstance(rows, (list, tuple, set, frozenset)):
-            self.split_to_index[split] = {key: self.index[key] for key in rows}
+            
+            if keyless:
+                split_index = FDDIndexKeyless(num_vals=len(self.columns)+1 if self.columns is not None else 2)
+                for i, key in enumerate(rows):
+                    split_index[i] = self.index[key]
+            else:
+                split_index_dict = {key: self.index[key] for key in rows}
+                try:
+                    if not self.preserve_order:
+                        split_index = FDDIndexComparableKey(split_index_dict)
+                    else:
+                        raise ValueError("dummy error go to except block")
+                except:
+                    split_index = FDDIndexGeneral(len(self.columns)+1 if self.columns is not None else 2)
+                    for k,v in split_index_dict.items():
+                        split_index[k] = v
+            if split == 'all_rows':
+                self.index = split_index
+            else:
+                self.split_to_index[split] = split_index
         else:
             raise ValueError("Rows must be an iterable of keys.")
         
     def add_to_split(self, split: str, rows: list | tuple | set | frozenset) -> None:
         """
         Add rows to a split in the WFDD.
 
@@ -658,22 +735,55 @@
             
             Writing {} unfinished setters to disk now.
             """.format(len(cpy)), UserWarning)
 
         for k in cpy:
             self.unfinished_setters[k].finalize()
 
+        
+        
         index_index = {}
+        has_lambda = False
+        if self.column_def is not None:
+            for k,v in self.column_def.items():
+                if isinstance(v, tuple):
+                    has_lambda = True
+                    break
+        
+        if self.column_def is not None:
+            column_def_start = self.file.tell()
+            if not has_lambda:
+                column_def_data = self.system_serialize(self.column_def)
+            else:
+                # use dill
+                import dill
+                column_def_data = dill.dumps(self.column_def)
+
+            self.file.write(column_def_data)
+            column_def_end = self.file.tell()
+            index_index['_column_def_'] = (column_def_start, column_def_end)
+
+
+
         for k,v in self.custom_properties.items():
             property_start = self.file.tell()
             property_data = self.system_serialize(v)
             self.file.write(property_data)
             property_end = self.file.tell()
             index_index["_prop_"+k] = (property_start, property_end)
 
+        if not isinstance(self.index, FDDIndexKeyless):
+            try:
+                if not self.preserve_order:
+                    self.index = FDDIndexComparableKey(self.index)
+            except:
+                pass
+        
+        
+
         self.split_to_index['all_rows'] = self.index
         for k,v in self.split_to_index.items():
             split_start = self.file.tell()
             split_data = self.system_serialize(v)
             self.file.write(split_data)
             split_end = self.file.tell()
             index_index["_split_"+k] = (split_start, split_end)
```

### Comparing `freeze_dried_data-2.1.4/freeze_dried_data/freeze_dried_data_old.py` & `freeze_dried_data-2.2.0/freeze_dried_data/freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.4/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-2.2.0/freeze_dried_data/test_freeze_dried_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import unittest
 import random
 from freeze_dried_data import RFDD, WFDD, add_column
+from efficient_index import FDDIndexBase
 
 class TestFDD(unittest.TestCase):
     test_file = '/tmp/test_fdd.fdd'
     test_file2 = '/tmp/test_fdd2.fdd'
     test_file3 = '/tmp/test_fdd3.fdd'
     test_file4 = '/tmp/test_fdd4.fdd'
 
@@ -39,15 +40,15 @@
         # Read operations
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['hello'], 'world')
             self.assertEqual(rfdd['number'], 123)
 
     def test_basic_operations_with_columns(self):
         # Write operations
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
 
         # Read operations
         with RFDD(self.test_file) as rfdd:
             self.assertTrue('house1' in rfdd)
@@ -116,20 +117,20 @@
 
     def test_file_does_not_exist(self):
         with self.assertRaises(FileNotFoundError):
             with RFDD(self.test_file) as rfdd:
                 pass
 
     def test_modify_and_write(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
 
-        with WFDD(self.test_file2, columns=('name','area', 'price'), overwrite=True) as wfdd,\
+        with WFDD(self.test_file2, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd,\
              RFDD(self.test_file) as rfdd:
              for k,v in rfdd.items():
                 v.price = v.price * 1.5
                 wfdd[k+' with inflation'] = v
 
         with RFDD(self.test_file2) as rfdd:
             self.assertEqual(rfdd['house1 with inflation'].name, 'house1')
@@ -139,20 +140,20 @@
             self.assertEqual(rfdd['house2 with inflation'].area, 200)
             self.assertEqual(rfdd['house2 with inflation'].price, 300000)
             self.assertEqual(rfdd['house3 with inflation'].name, 'house3')
             self.assertEqual(rfdd['house3 with inflation'].area, 300)
             self.assertEqual(rfdd['house3 with inflation'].price, 450000)
 
     def test_modify_and_write_use_indices(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
 
-        with WFDD(self.test_file2, columns=('name','area', 'price'), overwrite=True) as wfdd,\
+        with WFDD(self.test_file2, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd,\
              RFDD(self.test_file) as rfdd:
              for k,v in rfdd.items():
                 v[2] = v[2] * 1.5
                 wfdd[k+' with inflation'] = v
 
         with RFDD(self.test_file2) as rfdd:
             self.assertEqual(rfdd['house1 with inflation'].name, 'house1')
@@ -164,15 +165,15 @@
             self.assertEqual(rfdd['house3 with inflation'].name, 'house3')
             self.assertEqual(rfdd['house3 with inflation'].area, 300)
             self.assertEqual(rfdd['house3 with inflation'].price, 450000)
 
             
     def test_custom_attributes(self):
         # Test setting and getting custom attributes
-        with WFDD(self.test_file, overwrite=True, columns=('value',)) as fdd:
+        with WFDD(self.test_file, overwrite=True, columns={'value':'any'}) as fdd:
             fdd.property_one = 'initial'
             fdd.property_two = 123
             fdd.property_one = 'changed'
             fdd.property_3 = 3.14159
 
             self.assertEqual(fdd.property_one, 'changed')
 
@@ -199,15 +200,15 @@
             self.assertEqual(fdd.property_two, 'new')
             dct = {}
             for k,v in fdd.items():
                 dct[k] = v.value
             self.assertEqual(dct, {'key1': 'value1', 'key2': 'value2', 'key3': 'value3'})
 
     def test_incomplete_columns(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100}
             wfdd['house2'] = {'name': 'house2', 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
         
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['house1'].name, 'house1')
             self.assertEqual(rfdd['house1'].area, 100)
@@ -216,15 +217,15 @@
             self.assertEqual(rfdd['house2'].area, None)
             self.assertEqual(rfdd['house2'].price, 200000)
             self.assertEqual(rfdd['house3'].name, 'house3')
             self.assertEqual(rfdd['house3'].area, 300)
             self.assertEqual(rfdd['house3'].price, 300000)
 
     def test_single_column_functionality(self):
-        with WFDD(self.test_file, columns=('value',), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'value':'any'}, overwrite=True) as wfdd:
             wfdd['key1'].value='value1'
             wfdd['key2']['value'] ='value2'
             wfdd['key3'] = ('value3',)
 
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['key1'].value, 'value1')
             self.assertEqual(rfdd['key2'].value, 'value2')
@@ -233,34 +234,34 @@
             rfdd['key1'].value = 'new_value1'
             self.assertEqual(rfdd['key1'].value, 'new_value1')
 
             rfdd['key1']['value'] = 'new_value2'
             self.assertEqual(rfdd['key1'].value, 'new_value2')
 
     def test_set_all_of_column(self):
-        with WFDD(self.test_file, columns=('value','area'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'value':'float','area':'float'}, overwrite=True) as wfdd:
             for i in range(100):
                 wfdd[f'key{i}'].value = i
                 wfdd[f'key{i}'].area = i+1
         
         with RFDD(self.test_file) as rfdd:
-            with WFDD(self.test_file2, columns=('value','area'), overwrite=True) as wfdd2:
+            with WFDD(self.test_file2, columns={'value':'float','area':'float'}, overwrite=True) as wfdd2:
                 for k,v in rfdd.items():
                     v.value = v.value * 1.1
                     wfdd2[k] = v
 
         with RFDD(self.test_file2) as rfdd2:
             for i, (k,v) in enumerate(rfdd2.items()):
                 self.assertEqual(v.value, i*1.1)
                 self.assertEqual(v.area, i+1)
 
 
 
     def test_set_columns_by_attribute_or_item(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'].name = 'house1'
             wfdd['house1'].area = 100
             wfdd['house1'].price = 100000
             wfdd['house2']["name"] = 'house2'
             wfdd['house2']["area"] = 200
             wfdd['house2']["price"] = 200000
             wfdd['house3'] = ('house3', 300, 300000)
@@ -274,15 +275,15 @@
             self.assertEqual(rfdd['house2'].price, 200000)
             self.assertEqual(rfdd['house3'].name, 'house3')
             self.assertEqual(rfdd['house3'].area, 300)
             self.assertEqual(rfdd['house3'].price, 300000)
 
 
     def test_out_of_order_writes(self):
-        with WFDD(self.test_file, columns=('first', 'second'),overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'first':'int', 'second':'int'},overwrite=True) as wfdd:
             for i in range(100):
                 wfdd[f'key{i}'].first = i
             for i in range(50):
                 wfdd[f'key{i}'].second = i+1
 
         with RFDD(self.test_file) as rfdd:
             for i in range(100):
@@ -337,15 +338,16 @@
             self.assertEqual(len(items), 3)
             keys = wfdd.keys()
             self.assertEqual(len(keys), 3)
 
 
     def test_splits(self):
 
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             for i in range(100):
                 wfdd[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i, 'price': 1000+100*i}
 
             wfdd.make_split('odds', [f'house_{i}' for i in range(1,100,2)])
             wfdd.make_split('evens', [f'house_{i}' for i in range(0,100,2)])
             wfdd.make_split('big houses', [f'house_{i}' for i in range(80,100)])
             wfdd.make_split('reverse_order', [f'house_{i}' for i in range(99,-1,-1)])
@@ -417,15 +419,15 @@
 
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(len(list(rfdd.keys())), num_records)
             for key, value in data.items():
                 self.assertEqual(rfdd[key], value)
 
     def test_column_not_found(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
             wfdd['house4'].name = 'house4'
             with self.assertRaises(AttributeError):
                 wfdd['house4'].nonexistent = 3
 
@@ -437,15 +439,15 @@
                 _ = rfdd['house1'].nonexistent
             
             with self.assertRaises(AttributeError):
                 rfdd['house1'].nonexistent = 3
         
     def test_print_finalize_warning(self):
         with self.assertWarns(UserWarning):
-            with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+            with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
                 for i in range(1100):
                     wfdd[f'house_{i}'].name = f'house_{i}' # we only set the name attribute
             # we should get a warning upon exiting the context
 
         # rows should be written to disk anyway
         with RFDD(self.test_file) as rfdd:
             for i in range(1100):
@@ -463,15 +465,15 @@
     def test_key_already_exists(self):
         with WFDD(self.test_file, overwrite=True) as wfdd:
             wfdd['key1']= 'value1'
             with self.assertRaises(KeyError):
                 wfdd['key1'] = 'value2'
             
     def test_invalid_object_for_column_mode(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             with self.assertRaises(ValueError):
                 wfdd['house3'] = 15
 
         with WFDD(self.test_file, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
@@ -487,32 +489,32 @@
 
         class Test2:
             def __init__(self, time, location):
                 self.time = time
                 self.location = location
 
 
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = Test('house1', 100, 100000)
             wfdd['house2'] = Test('house2', 200, 200000)
             with self.assertRaises(ValueError):
                 wfdd['house3'] = Test2('house3', 300)
 
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             with self.assertRaises(ValueError):
                 wfdd['house1'] = {"happy": "birthday"}
             
 
         
 
     def test_reaads_in_between_writes_with_columns(self):
         num_records = 1000
         data = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(num_records)}
         
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             for i, (k, v) in enumerate(data.items()):
                 wfdd[k] = v
                 where_read = random.choice(list(data.keys())[:i+1])
                 self.assertEqual(wfdd[where_read].name, data[where_read]['name'])
                 self.assertEqual(wfdd[where_read].area, data[where_read]['area'])
                 self.assertEqual(wfdd[where_read].price, data[where_read]['price'])
 
@@ -555,18 +557,23 @@
         import torch
         import ctypes
 
         import json
 
 
         def json_serializer(obj):
+            if isinstance(obj, FDDIndexBase):
+                return pkl.dumps(obj)
             return json.dumps(obj).encode('utf-8')
 
         def json_deserializer(data):
-            return json.loads(data.decode('utf-8'))
+            try:
+                return json.loads(data.decode('utf-8'))
+            except:
+                return pkl.loads(data)
         
         custom_deserialize_list = [lambda x:pkl.loads(x[:-1]), lambda x: pkl.loads(zlib.decompress(x)), lambda x: pkl.loads(bz2.decompress(x)), lambda x: pkl.loads(gzip.decompress(x)), json_deserializer]
         custom_serialize_list = [lambda x:pkl.dumps(x)+b'\n', lambda x: zlib.compress(pkl.dumps(x)), lambda x: bz2.compress(pkl.dumps(x)), lambda x: gzip.compress(pkl.dumps(x)), json_serializer]
 
 
         for custom_serialize, custom_deserialize in zip(custom_serialize_list, custom_deserialize_list):
             with WFDD(self.test_file, overwrite=True, system_serialize=custom_serialize) as wfdd:
@@ -575,68 +582,60 @@
                 wfdd['key3'] = 'value3'
 
             with RFDD(self.test_file, system_deserialize=custom_deserialize) as rfdd:
                 self.assertEqual(rfdd['key1'], 'value1')
                 self.assertEqual(rfdd['key2'], 'value2')
                 self.assertEqual(rfdd['key3'], 'value3')
 
-            with WFDD(self.test_file, overwrite=True, no_columns_serialize=custom_serialize) as wfdd:
+
+
+            
+            with WFDD(self.test_file, overwrite=True, system_serialize=custom_serialize) as wfdd:
                 wfdd['key1'] = 'value1'
                 wfdd['key2'] = 'value2'
                 wfdd['key3'] = 'value3'
 
-            with RFDD(self.test_file, no_columns_deserialize=custom_deserialize) as rfdd:
+            with RFDD(self.test_file, system_deserialize=custom_deserialize) as rfdd:
                 self.assertEqual(rfdd['key1'], 'value1')
                 self.assertEqual(rfdd['key2'], 'value2')
                 self.assertEqual(rfdd['key3'], 'value3')
 
-            for custom_serialize2, custom_deserialize2 in zip(custom_serialize_list, custom_deserialize_list):
-                with WFDD(self.test_file, overwrite=True, system_serialize=custom_serialize, no_columns_serialize=custom_serialize2) as wfdd:
-                    wfdd['key1'] = 'value1'
-                    wfdd['key2'] = 'value2'
-                    wfdd['key3'] = 'value3'
-
-                with RFDD(self.test_file, system_deserialize=custom_deserialize, no_columns_deserialize=custom_deserialize2) as rfdd:
-                    self.assertEqual(rfdd['key1'], 'value1')
-                    self.assertEqual(rfdd['key2'], 'value2')
-                    self.assertEqual(rfdd['key3'], 'value3')
-
-                with WFDD(self.test_file, overwrite=True, columns=('name', 'salary', 'position'), system_serialize=custom_serialize, column_to_serialize=(pkl.dumps, pkl.dumps, custom_serialize)) as wfdd:
-                    wfdd['employee1'] = {'name': 'Alice', 'salary': 100000, 'position': 'manager'}
-                    wfdd['employee2'] = {'name': 'Bob', 'salary': 80000, 'position': 'engineer'}
-                    wfdd['employee3'] = {'name': 'Charlie', 'salary': 60000, 'position': 'assistant'}
-                
-                with RFDD(self.test_file, system_deserialize=custom_deserialize, column_to_deserialize=(pkl.loads, pkl.loads, custom_deserialize)) as rfdd:
-                    self.assertEqual(rfdd['employee1'].name, 'Alice')
-                    self.assertEqual(rfdd['employee1'].salary, 100000)
-                    self.assertEqual(rfdd['employee1'].position, 'manager')
-                    self.assertEqual(rfdd['employee2'].name, 'Bob')
-                    self.assertEqual(rfdd['employee2'].salary, 80000)
-                    self.assertEqual(rfdd['employee2'].position, 'engineer')
-                    self.assertEqual(rfdd['employee3'].name, 'Charlie')
-                    self.assertEqual(rfdd['employee3'].salary, 60000)
-                    self.assertEqual(rfdd['employee3'].position, 'assistant')
+            with WFDD(self.test_file, overwrite=True, columns={'name':'str', 'salary':'int', 'position':(custom_serialize, custom_deserialize)}, system_serialize=custom_serialize) as wfdd:
+                wfdd['employee1'] = {'name': 'Alice', 'salary': 100000, 'position': 'manager'}
+                wfdd['employee2'] = {'name': 'Bob', 'salary': 80000, 'position': 'engineer'}
+                wfdd['employee3'] = {'name': 'Charlie', 'salary': 60000, 'position': 'assistant'}
+            
+            with RFDD(self.test_file, system_deserialize=custom_deserialize) as rfdd:
+                self.assertEqual(rfdd['employee1'].name, 'Alice')
+                self.assertEqual(rfdd['employee1'].salary, 100000)
+                self.assertEqual(rfdd['employee1'].position, 'manager')
+                self.assertEqual(rfdd['employee2'].name, 'Bob')
+                self.assertEqual(rfdd['employee2'].salary, 80000)
+                self.assertEqual(rfdd['employee2'].position, 'engineer')
+                self.assertEqual(rfdd['employee3'].name, 'Charlie')
+                self.assertEqual(rfdd['employee3'].salary, 60000)
+                self.assertEqual(rfdd['employee3'].position, 'assistant')
 
         for custom_serialize, custom_deserialize in zip(custom_serialize_list, custom_deserialize_list):
-            with WFDD(self.test_file, overwrite=True, columns=('hash', 'tensor', 'label'), column_to_serialize=(pkl.dumps, custom_serialize, pkl.dumps), column_to_deserialize=(pkl.loads, custom_deserialize, pkl.loads)) as wfdd:
+            with WFDD(self.test_file, overwrite=True, columns={'hash':'str', 'tensor':(custom_serialize, custom_deserialize), 'label':'str'}) as wfdd:
                 wfdd['hash1'] = {'hash': 'hash1', 'tensor': 1, 'label': 'dog'}
                 wfdd['hash2'] = {'hash': 'hash2', 'tensor': 2, 'label': 'cat'}
                 wfdd['hash3'] = {'hash': 'hash3', 'tensor': 2, 'label': 'dog'}
                 self.assertEqual(wfdd['hash3'].hash, 'hash3')
                 self.assertEqual(wfdd['hash3'].tensor, 2)
                 self.assertEqual(wfdd['hash3'].label, 'dog')
                 self.assertEqual(wfdd['hash1'].hash, 'hash1')
                 self.assertEqual(wfdd['hash1'].tensor, 1)
                 self.assertEqual(wfdd['hash1'].label, 'dog')
                 self.assertEqual(wfdd['hash2'].hash, 'hash2')
                 self.assertEqual(wfdd['hash2'].tensor, 2)
                 self.assertEqual(wfdd['hash2'].label, 'cat')
                 
 
-            with RFDD(self.test_file, column_to_deserialize=(pkl.loads, custom_deserialize, pkl.loads)) as rfdd:
+            with RFDD(self.test_file,) as rfdd:
                 for k,v in rfdd.items():
                     self.assertEqual(v.hash, k)
                     self.assertEqual(v.tensor, 1 if k == 'hash1' else 2)
                     self.assertEqual(v.label, 'dog' if k == 'hash1' or k == 'hash3' else 'cat')
 
         data ={'hash1': {'hash': 'hash1', 'tensor': torch.randn(10,10,dtype=torch.bfloat16), 'label': 'dog'},
                'hash2': {'hash': 'hash2', 'tensor': torch.randn(10,10,dtype=torch.bfloat16), 'label': 'cat'},
@@ -655,26 +654,26 @@
         
         def bytes_to_tensor(byte_data, shape=(10,10)):
             byte_data = bytearray(byte_data)
             tensor = torch.frombuffer(byte_data, dtype=torch.bfloat16, )
             return tensor.view(shape)
         
         for custom_serialize, custom_deserialize in zip(custom_serialize_list, custom_deserialize_list):
-            with WFDD(self.test_file, overwrite=True, columns=('hash', 'tensor', 'label'),system_serialize=custom_serialize, column_to_serialize=(pkl.dumps,tensor_to_bytes,pkl.dumps)) as wfdd:
+            with WFDD(self.test_file, overwrite=True, columns={'hash':'str', 'tensor':(tensor_to_bytes,bytes_to_tensor), 'label':'any'},system_serialize=custom_serialize, ) as wfdd:
                 for k,v in data.items():
                     wfdd[k] = v
 
-            with RFDD(self.test_file, system_deserialize=custom_deserialize, column_to_deserialize=(pkl.loads,bytes_to_tensor,pkl.loads)) as rfdd:
+            with RFDD(self.test_file, system_deserialize=custom_deserialize) as rfdd:
                 for k,v in data.items():
                     self.assertEqual(rfdd[k].hash, v['hash'])
                     self.assertTrue(torch.allclose(rfdd[k].tensor, v['tensor']))
                     self.assertEqual(rfdd[k].label, v['label'])
 
     def test_row_has_already_been_finalized(self):
-        with WFDD(self.test_file,columns=('col1','col2'),overwrite=True) as wfdd:
+        with WFDD(self.test_file,columns={'col1':'any','col2':'any'},overwrite=True) as wfdd:
             wfdd['key1'].col1 = 1
             wfdd['key1'].col2 = 2
             with self.assertRaises(AttributeError):
                 wfdd['key1'].col1 = 3
 
     def test_reopen_file(self):
         data = {f'key{i}': f'value{i}' for i in range(1000)}
@@ -733,15 +732,15 @@
             self.assertEqual(rfdd.custom_attribute1, 're-written custom1')
             self.assertEqual(rfdd.custom_attribute2, 'custom2')
             self.assertEqual(rfdd.custom_attribute3, 'custom3')
 
 
     def test_reopen_file_with_columns(self):
         data = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(1000)}
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             for k, v in data.items():
                 wfdd[k] = v
 
             wfdd.custom_attribute1 = 'custom1'
             wfdd.custom_attribute2 = 'custom2'
             wfdd.make_split('evens', [f'key{i}' for i in range(0,1000,2)])
         with RFDD(self.test_file) as rfdd:
@@ -754,15 +753,15 @@
             for i, (k,v) in enumerate(rfdd.items()):
                 self.assertEqual(k, f'key{2*i}')
                 self.assertEqual(v.name, f'name{2*i}')
                 self.assertEqual(v.area, data[f'key{2*i}']['area'])
                 self.assertEqual(v.price, data[f'key{2*i}']['price'])
 
         data_2 = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(1000,2000)}
-        with WFDD(self.test_file, columns=('name','area', 'price'), reopen=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, reopen=True) as wfdd:
 
             for k, v in data_2.items():
                 wfdd[k] = v
             
             wfdd.custom_attribute1 = 're-written custom1'
             wfdd.custom_attribute3 = 'custom3'
             wfdd.add_to_split('evens', [f'key{i}' for i in range(1000,2000,2)])
@@ -770,76 +769,78 @@
                 wfdd.add_to_split('fake_split', ['key1'])
             with self.assertRaises(ValueError):
                 wfdd.add_to_split('evens', 234234)
             wfdd.make_split('odds', [f'key{i}' for i in range(1,2000,2)])
 
 
     def test_columns_with_partial_dicts(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100}
             wfdd['house2'] = {'name': 'house2', 'price': 200000}
 
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['house1'].name, 'house1')
             self.assertEqual(rfdd['house1'].area, 100)
             self.assertEqual(rfdd['house1'].price, None)
             self.assertEqual(rfdd['house2'].name, 'house2')
             self.assertEqual(rfdd['house2'].area, None)
             self.assertEqual(rfdd['house2'].price, 200000)
 
     def test_columns_with_dicts_with_extra_keys(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             with self.assertRaises(ValueError):
                 wfdd['house1'] = {'name': 'house1', 'area': 100, 'extra': 'extra'}
             with self.assertRaises(ValueError):
                 wfdd['house2'] = {'name': 'house2', 'price': 200000, 'extra': 'extra'}
 
     def test_get_dict(self):
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
 
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['house1'].get_dict(), {'name': 'house1', 'area': 100, 'price': 100000})
             self.assertEqual(rfdd['house2'].get_dict(), {'name': 'house2', 'area': 200, 'price': 200000})
             self.assertEqual(rfdd['house3'].get_dict(), {'name': 'house3', 'area': 300, 'price': 300000})
 
-    def test_add_column(self):
+    # def test_add_column(self):
         
-        with WFDD(self.test_file, columns=('name','area'), overwrite=True) as wfdd:
-            for i in range(100):
-                wfdd[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i}
+    #     with WFDD(self.test_file, columns={'name':'str','area':'float'}, overwrite=True) as wfdd:
+    #         for i in range(100):
+    #             wfdd[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i}
 
-            wfdd.custom_attribute1 = 'custom1'
+    #         wfdd.custom_attribute1 = 'custom1'
 
-            wfdd.make_split('evens', [f'house_{i}' for i in range(0,100,2)])
+    #         wfdd.make_split('evens', [f'house_{i}' for i in range(0,100,2)])
 
-        new_col = {}
-        for i in range(100):
-            new_col[f'house_{i}'] = 1000+100*i
+    #     new_col = {}
+    #     for i in range(100):
+    #         new_col[f'house_{i}'] = 1000+100*i
         
         
-        if os.path.exists(self.test_file3):
-            os.remove(self.test_file3)
+    #     if os.path.exists(self.test_file3):
+    #         os.remove(self.test_file3)
 
-        add_column(self.test_file, self.test_file3, 'price', new_col)
+    #     add_column(self.test_file, self.test_file3, 'price', new_col)
 
-        with RFDD(self.test_file3) as rfdd:
-            for i in range(100):
-                self.assertEqual(rfdd[f'house_{i}'].price, 1000+100*i)
+    #     with RFDD(self.test_file3) as rfdd:
+    #         for i in range(100):
+    #             self.assertEqual(rfdd[f'house_{i}'].price, 1000+100*i)
 
-            rfdd.load_new_split('evens')
-            for i in range(50):
-                self.assertEqual(rfdd[f'house_{2*i}'].price, 1000+200*i)
+    #         rfdd.load_new_split('evens')
+    #         for i in range(50):
+    #             self.assertEqual(rfdd[f'house_{2*i}'].price, 1000+200*i)
 
-            self.assertEqual(rfdd.custom_attribute1, 'custom1')
+    #         self.assertEqual(rfdd.custom_attribute1, 'custom1')
 
-        with self.assertRaises(ValueError):
-            add_column(self.test_file3, self.test_file4, 'price', new_col)
+    #     with self.assertRaises(ValueError):
+    #         add_column(self.test_file3, self.test_file4, 'price', new_col)
 
             
 
     def test_dataloader_integration(self):
         from torch.utils.data import DataLoader, Dataset
 
         num_records = 100000
@@ -870,15 +871,16 @@
 
     def test_dataloader_integration_with_columns(self):
         from torch.utils.data import DataLoader, Dataset
         import torch
 
         num_records = 100000
         data = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(num_records)}
-        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+        
+        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
             for k, v in data.items():
                 wfdd[k] = v
 
         class FDDDataset(Dataset):
             def __init__(self, filename):
                 self.rfdd = RFDD(filename)
                 self.keys = list(self.rfdd.keys())
```

### Comparing `freeze_dried_data-2.1.4/freeze_dried_data/test_freeze_dried_data_old.py` & `freeze_dried_data-2.2.0/freeze_dried_data/test_freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.4/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: freeze-dried-data
-Version: 2.1.4
+Name: freeze_dried_data
+Version: 2.2.0
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.1.4/setup.py` & `freeze_dried_data-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='freeze_dried_data',
-    version='2.1.4',
+    version='2.2.0',
     description='A simple format for machine learning datasets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
```

