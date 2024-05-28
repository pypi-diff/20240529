# Comparing `tmp/tdta-0.1.0.dev7.tar.gz` & `tmp/tdta-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdta-0.1.0.dev7.tar", last modified: Tue May 28 13:17:00 2024, max compression
+gzip compressed data, was "tdta-0.1.0.dev9.tar", last modified: Tue May 28 15:33:19 2024, max compression
```

## Comparing `tdta-0.1.0.dev7.tar` & `tdta-0.1.0.dev9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:17:00.545024 tdta-0.1.0.dev7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/src/tdta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/anndata_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/purl_publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/tdt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 13:16:12.000000 tdta-0.1.0.dev7/src/tdta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:17:00.549024 tdta-0.1.0.dev7/src/tdta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 13:17:00.000000 tdta-0.1.0.dev7/src/tdta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:33:19.705873 tdta-0.1.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 15:33:19.705873 tdta-0.1.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:33:19.705873 tdta-0.1.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:33:19.701873 tdta-0.1.0.dev9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:33:19.705873 tdta-0.1.0.dev9/src/tdta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/src/tdta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/src/tdta/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/src/tdta/anndata_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/src/tdta/purl_publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/src/tdta/tdt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 15:32:28.000000 tdta-0.1.0.dev9/src/tdta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:33:19.705873 tdta-0.1.0.dev9/src/tdta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 15:33:19.000000 tdta-0.1.0.dev9/src/tdta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-28 15:33:19.000000 tdta-0.1.0.dev9/src/tdta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:33:19.000000 tdta-0.1.0.dev9/src/tdta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 15:33:19.000000 tdta-0.1.0.dev9/src/tdta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 15:33:19.000000 tdta-0.1.0.dev9/src/tdta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 15:33:19.000000 tdta-0.1.0.dev9/src/tdta.egg-info/top_level.txt
```

### Comparing `tdta-0.1.0.dev7/LICENSE` & `tdta-0.1.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev7/PKG-INFO` & `tdta-0.1.0.dev9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdta
-Version: 0.1.0.dev7
+Version: 0.1.0.dev9
 Summary: The aim of this project is to provide taxonomy development tools custom actions.
 Home-page: https://github.com/hkir-dev/taxonomy-development-tools-actions
 Author: 
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tdta-0.1.0.dev7/src/tdta/__main__.py` & `tdta-0.1.0.dev9/src/tdta/__main__.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev7/src/tdta/anndata_export.py` & `tdta-0.1.0.dev9/src/tdta/anndata_export.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev7/src/tdta/purl_publish.py` & `tdta-0.1.0.dev9/src/tdta/purl_publish.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev7/src/tdta/tdt_export.py` & `tdta-0.1.0.dev9/src/tdta/tdt_export.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sqlite3
 import ast
 import json
 from contextlib import closing
 from pathlib import Path
 
 from tdta.utils import read_project_config
-from cas.model import (CellTypeAnnotation, Annotation, Labelset, AnnotationTransfer, UserAnnotation, AutomatedAnnotation)
+from cas.model import (CellTypeAnnotation, Annotation, Labelset, AnnotationTransfer, AutomatedAnnotation, Review)
 from cas.file_utils import write_json_file
 from cas.matrix_file.resolver import resolve_matrix_file
 from cas.populate_cell_ids import add_cell_ids
 
 CONFLICT_TBL_EXT = "_conflict"
 
 cas_table_names = ["annotation", "labelset", "metadata", "annotation_transfer"]
@@ -30,15 +30,17 @@
         if table_name == "metadata":
             parse_metadata_data(cta, sqlite_db, table_name)
         elif table_name == "annotation":
             parse_annotation_data(cta, sqlite_db, table_name)
         elif table_name == "labelset":
             parse_labelset_data(cta, sqlite_db, table_name)
         elif table_name == "annotation_transfer":
-            parse__annotation_transfer_data(cta, sqlite_db, table_name)
+            parse_annotation_transfer_data(cta, sqlite_db, table_name)
+        elif table_name == "review":
+            parse_review_data(cta, sqlite_db, table_name)
 
     project_config = read_project_config(Path(output_file).parent.absolute())
 
     if "matrix_file_id" in project_config:
         matrix_file_id = str(project_config["matrix_file_id"]).strip()
         anndata = resolve_matrix_file(matrix_file_id, dataset_cache_folder)
         labelsets = cta.labelsets.copy()
@@ -92,21 +94,21 @@
                 if not cta.annotations:
                     annotations = list()
                 else:
                     annotations = cta.annotations
                 for row in rows:
                     annotation = Annotation("", "")
                     auto_fill_object_from_row(annotation, columns, row)
-                    # handle user_annotations
-                    user_annotations = list()
+                    # handle author_annotation_fields
+                    author_annotation_fields = dict()
                     obj_fields = vars(annotation)
                     for column in columns:
                         if column not in obj_fields and column not in ["row_number", "message"]:
-                            user_annotations.append(UserAnnotation(column, str(row[columns.index(column)])))
-                    annotation.user_annotations = user_annotations
+                            author_annotation_fields[column] = str(row[columns.index(column)])
+                    annotation.author_annotation_fields = author_annotation_fields
 
                     annotations.append(annotation)
                 cta.annotations = annotations
 
 
 def parse_labelset_data(cta, sqlite_db, table_name):
     """
@@ -133,15 +135,15 @@
                         automated_annotation = AutomatedAnnotation("", "", "", "")
                         auto_fill_object_from_row(automated_annotation, renamed_columns, row)
                         labelset.automated_annotation = automated_annotation
                     labelsets.append(labelset)
                 cta.labelsets = labelsets
 
 
-def parse__annotation_transfer_data(cta, sqlite_db, table_name):
+def parse_annotation_transfer_data(cta, sqlite_db, table_name):
     """
     Reads 'Annotation Transfer' table data into the CAS object
     :param cta: cell type annotation schema object.
     :param sqlite_db: db file path
     :param table_name: name of the metadata table
     """
     with closing(sqlite3.connect(sqlite_db)) as connection:
@@ -157,14 +159,37 @@
                             at = AnnotationTransfer("", "", "", "", "")
                             auto_fill_object_from_row(at, columns, row)
                             if filtered_annotations[0].transferred_annotations:
                                 filtered_annotations[0].transferred_annotations.append(at)
                             else:
                                 filtered_annotations[0].transferred_annotations = [at]
 
+def parse_review_data(cta, sqlite_db, table_name):
+    """
+    Reads 'Annotation Review' table data into the CAS object
+    :param cta: cell type annotation schema object.
+    :param sqlite_db: db file path
+    :param table_name: name of the metadata table
+    """
+    with closing(sqlite3.connect(sqlite_db)) as connection:
+        with closing(connection.cursor()) as cursor:
+            rows = cursor.execute("SELECT * FROM {}_view".format(table_name)).fetchall()
+            columns = list(map(lambda x: x[0], cursor.description))
+            if len(rows) > 0:
+                for row in rows:
+                    if "target_node_accession" in columns and row[columns.index("target_node_accession")]:
+                        filtered_annotations = [a for a in cta.annotations
+                                                if a.cell_set_accession == row[columns.index("target_node_accession")]]
+                        if filtered_annotations:
+                            ar = Review("", "", "", "", "")
+                            auto_fill_object_from_row(ar, columns, row)
+                            if filtered_annotations[0].reviews:
+                                filtered_annotations[0].reviews.append(ar)
+                            else:
+                                filtered_annotations[0].reviews = [ar]
 
 def get_table_names(sqlite_db):
     """
     Queries 'table' table to get all CAS related table names
     :param sqlite_db: db file path
     :return: list of CAS related table names
     """
```

### Comparing `tdta-0.1.0.dev7/src/tdta/utils.py` & `tdta-0.1.0.dev9/src/tdta/utils.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev7/src/tdta.egg-info/PKG-INFO` & `tdta-0.1.0.dev9/src/tdta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdta
-Version: 0.1.0.dev7
+Version: 0.1.0.dev9
 Summary: The aim of this project is to provide taxonomy development tools custom actions.
 Home-page: https://github.com/hkir-dev/taxonomy-development-tools-actions
 Author: 
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

