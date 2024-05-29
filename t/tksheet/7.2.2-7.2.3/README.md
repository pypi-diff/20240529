# Comparing `tmp/tksheet-7.2.2.tar.gz` & `tmp/tksheet-7.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-7.2.2.tar", last modified: Mon May 27 15:51:37 2024, max compression
+gzip compressed data, was "tksheet-7.2.3.tar", last modified: Tue May 28 18:12:41 2024, max compression
```

## Comparing `tksheet-7.2.2.tar` & `tksheet-7.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-27 15:51:37.406540 tksheet-7.2.2/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.2.2/LICENSE.txt
--rw-r--r--   0 rg        (1000) rg        (1000)     6319 2024-05-27 15:51:37.406540 tksheet-7.2.2/PKG-INFO
--rw-r--r--   0 rg        (1000) rg        (1000)     4222 2024-05-25 15:33:08.000000 tksheet-7.2.2/README.md
--rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-05-22 17:27:00.000000 tksheet-7.2.2/pyproject.toml
--rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-05-27 15:51:37.406540 tksheet-7.2.2/setup.cfg
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-27 15:51:37.402540 tksheet-7.2.2/tksheet/
--rw-rw-r--   0 rg        (1000) rg        (1000)     2124 2024-05-22 17:27:00.000000 tksheet-7.2.2/tksheet/__init__.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.2.2/tksheet/colors.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   102039 2024-05-27 15:41:38.000000 tksheet-7.2.2/tksheet/column_headers.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.2.2/tksheet/formatters.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    40835 2024-05-20 07:30:00.000000 tksheet-7.2.2/tksheet/functions.py
--rw-r--r--   0 rg        (1000) rg        (1000)   324868 2024-05-27 15:41:21.000000 tksheet-7.2.2/tksheet/main_table.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-05-17 10:30:02.000000 tksheet-7.2.2/tksheet/other_classes.py
--rw-r--r--   0 rg        (1000) rg        (1000)   108213 2024-05-27 15:41:55.000000 tksheet-7.2.2/tksheet/row_index.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   268309 2024-05-27 15:43:20.000000 tksheet-7.2.2/tksheet/sheet.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    12262 2024-05-20 09:45:04.000000 tksheet-7.2.2/tksheet/sheet_options.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     6548 2024-05-21 08:53:42.000000 tksheet-7.2.2/tksheet/text_editor.py
--rw-r--r--   0 rg        (1000) rg        (1000)    14474 2024-05-21 08:36:35.000000 tksheet-7.2.2/tksheet/themes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     8436 2024-05-26 07:23:05.000000 tksheet-7.2.2/tksheet/top_left_rectangle.py
--rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.2.2/tksheet/types.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     3452 2024-05-20 09:29:16.000000 tksheet-7.2.2/tksheet/vars.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-27 15:51:37.406540 tksheet-7.2.2/tksheet.egg-info/
--rw-r--r--   0 rg        (1000) rg        (1000)     6319 2024-05-27 15:51:37.000000 tksheet-7.2.2/tksheet.egg-info/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-05-27 15:51:37.000000 tksheet-7.2.2/tksheet.egg-info/SOURCES.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-05-27 15:51:37.000000 tksheet-7.2.2/tksheet.egg-info/dependency_links.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-05-27 15:51:37.000000 tksheet-7.2.2/tksheet.egg-info/top_level.txt
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-28 18:12:41.586196 tksheet-7.2.3/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.2.3/LICENSE.txt
+-rw-r--r--   0 rg        (1000) rg        (1000)     6319 2024-05-28 18:12:41.586196 tksheet-7.2.3/PKG-INFO
+-rw-r--r--   0 rg        (1000) rg        (1000)     4222 2024-05-25 15:33:08.000000 tksheet-7.2.3/README.md
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-05-27 15:52:09.000000 tksheet-7.2.3/pyproject.toml
+-rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-05-28 18:12:41.586196 tksheet-7.2.3/setup.cfg
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-28 18:12:41.586196 tksheet-7.2.3/tksheet/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     2124 2024-05-27 15:52:09.000000 tksheet-7.2.3/tksheet/__init__.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.2.3/tksheet/colors.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   102039 2024-05-27 15:41:38.000000 tksheet-7.2.3/tksheet/column_headers.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.2.3/tksheet/formatters.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    40835 2024-05-20 07:30:00.000000 tksheet-7.2.3/tksheet/functions.py
+-rw-r--r--   0 rg        (1000) rg        (1000)   325631 2024-05-28 18:00:11.000000 tksheet-7.2.3/tksheet/main_table.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-05-17 10:30:02.000000 tksheet-7.2.3/tksheet/other_classes.py
+-rw-r--r--   0 rg        (1000) rg        (1000)   108213 2024-05-28 11:18:06.000000 tksheet-7.2.3/tksheet/row_index.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   268536 2024-05-28 17:46:18.000000 tksheet-7.2.3/tksheet/sheet.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    12262 2024-05-20 09:45:04.000000 tksheet-7.2.3/tksheet/sheet_options.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     6548 2024-05-21 08:53:42.000000 tksheet-7.2.3/tksheet/text_editor.py
+-rw-r--r--   0 rg        (1000) rg        (1000)    14474 2024-05-21 08:36:35.000000 tksheet-7.2.3/tksheet/themes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     8436 2024-05-26 07:23:05.000000 tksheet-7.2.3/tksheet/top_left_rectangle.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.2.3/tksheet/types.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3452 2024-05-20 09:29:16.000000 tksheet-7.2.3/tksheet/vars.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-28 18:12:41.586196 tksheet-7.2.3/tksheet.egg-info/
+-rw-r--r--   0 rg        (1000) rg        (1000)     6319 2024-05-28 18:12:41.000000 tksheet-7.2.3/tksheet.egg-info/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-05-28 18:12:41.000000 tksheet-7.2.3/tksheet.egg-info/SOURCES.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-05-28 18:12:41.000000 tksheet-7.2.3/tksheet.egg-info/dependency_links.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-05-28 18:12:41.000000 tksheet-7.2.3/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-7.2.2/LICENSE.txt` & `tksheet-7.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/PKG-INFO` & `tksheet-7.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.2.2
+Version: 7.2.3
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `tksheet-7.2.2/README.md` & `tksheet-7.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/pyproject.toml` & `tksheet-7.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tksheet"
 description = "Tkinter table / sheet widget"
 readme = "README.md"
-version = "7.2.2"
+version = "7.2.3"
 authors = [{ name = "ragardner", email = "github@ragardner.simplelogin.com" }]
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["tkinter", "table", "widget", "sheet", "grid", "tk"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `tksheet-7.2.2/tksheet/__init__.py` & `tksheet-7.2.3/tksheet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 
 """
 tksheet - A Python tkinter table widget
 """
 
-__version__ = "7.2.2"
+__version__ = "7.2.3"
 
 from .colors import (
     color_map,
 )
 from .column_headers import ColumnHeaders
 from .formatters import (
     Formatter,
```

### Comparing `tksheet-7.2.2/tksheet/colors.py` & `tksheet-7.2.3/tksheet/colors.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/column_headers.py` & `tksheet-7.2.3/tksheet/column_headers.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/formatters.py` & `tksheet-7.2.3/tksheet/formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/functions.py` & `tksheet-7.2.3/tksheet/functions.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/main_table.py` & `tksheet-7.2.3/tksheet/main_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -848,14 +848,15 @@
                         ctr += 1
             if ctr:
                 event_data = self.add_rows(
                     rows=rows,
                     index=index,
                     row_heights=row_heights,
                     event_data=event_data,
+                    mod_event_boxes=False,
                 )
         if added_cols:
             ctr = 0
             if total_data_cols is None:
                 total_data_cols = self.total_data_cols()
             data_ins_col = total_data_cols
             displayed_ins_col = len(self.col_positions) - 1
@@ -897,34 +898,37 @@
                         ctr += 1
             if ctr:
                 event_data = self.add_columns(
                     columns=columns,
                     header=headers,
                     column_widths=column_widths,
                     event_data=event_data,
+                    mod_event_boxes=False,
                 )
-        self.deselect("all", redraw=False)
-        if event_data["cells"]["table"] or event_data["added"]["rows"] or event_data["added"]["columns"]:
-            self.undo_stack.append(pickled_event_dict(event_data))
         if added_rows:
             selboxr = selected_r + new_data_numrows
         else:
             selboxr = selected_r_adjusted_new_data_numrows
         if added_cols:
             selboxc = selected_c + new_data_numcols
         else:
             selboxc = selected_c_adjusted_new_data_numcols
+        self.deselect("all", redraw=False)
         self.create_selection_box(
             selected_r,
             selected_c,
             selboxr,
             selboxc,
             "cells",
             run_binding=True,
         )
+        event_data["selection_boxes"] = self.get_boxes()
+        event_data["selected"] = self.selected
+        if event_data["cells"]["table"] or event_data["added"]["rows"] or event_data["added"]["columns"]:
+            self.undo_stack.append(pickled_event_dict(event_data))
         self.see(
             r=selected_r,
             c=selected_c,
             keep_yscroll=False,
             keep_xscroll=False,
             bottom_right_corner=False,
             check_cell_visibility=True,
@@ -1557,15 +1561,14 @@
             name=modification["eventname"],
             sheet=self.PAR.name,
             widget=self,
         )
         event_data["selection_boxes"] = modification["selection_boxes"]
         event_data["selected"] = modification["selected"]
         saved_cells = False
-
         if modification["added"]["rows"] or modification["added"]["columns"]:
             event_data = self.save_cells_using_modification(modification, event_data)
             saved_cells = True
 
         if modification["moved"]["columns"]:
             totalcols = max(self.equalize_data_row_lengths(), max(modification["moved"]["columns"]["data"].values()))
             data_new_idxs, disp_new_idxs, event_data = self.move_columns_adjust_options_dict(
@@ -1623,91 +1626,73 @@
                 event_data=event_data,
             )
             event_data = self.delete_rows_displayed(
                 rows=tuple(reversed(modification["added"]["rows"]["row_heights"])),
                 event_data=event_data,
             )
             self.displayed_rows = modification["added"]["rows"]["displayed_rows"]
-            if len(self.row_positions) > 1:
-                self.reselect_from_get_boxes(
-                    modification["selection_boxes"],
-                    modification["selected"],
-                )
 
         if modification["added"]["columns"]:
             self.deselect("all", run_binding=False, redraw=False)
             event_data = self.delete_columns_data(
                 cols=tuple(reversed(modification["added"]["columns"]["table"])),
                 event_data=event_data,
             )
             event_data = self.delete_columns_displayed(
                 cols=tuple(reversed(modification["added"]["columns"]["column_widths"])),
                 event_data=event_data,
             )
             self.displayed_columns = modification["added"]["columns"]["displayed_columns"]
-            if len(self.col_positions) > 1:
-                self.reselect_from_get_boxes(
-                    modification["selection_boxes"],
-                    modification["selected"],
-                )
 
-        if modification["deleted"]["rows"]:
+        if modification["deleted"]["rows"] or modification["deleted"]["row_heights"]:
             self.add_rows(
                 rows=modification["deleted"]["rows"],
                 index=modification["deleted"]["index"],
                 row_heights=modification["deleted"]["row_heights"],
                 event_data=event_data,
                 displayed_rows=modification["deleted"]["displayed_rows"],
                 create_ops=False,
                 create_selections=not modification["eventname"].startswith("edit"),
                 add_col_positions=False,
             )
             self.restore_options_named_spans(modification)
 
-        if modification["deleted"]["columns"]:
+        if modification["deleted"]["columns"] or modification["deleted"]["column_widths"]:
             self.add_columns(
                 columns=modification["deleted"]["columns"],
                 header=modification["deleted"]["header"],
                 column_widths=modification["deleted"]["column_widths"],
                 event_data=event_data,
                 displayed_columns=modification["deleted"]["displayed_columns"],
                 create_ops=False,
                 create_selections=not modification["eventname"].startswith("edit"),
                 add_row_positions=False,
             )
             self.restore_options_named_spans(modification)
 
-        if modification["eventname"].startswith("edit") and (
-            modification["deleted"]["columns"] or modification["deleted"]["rows"]
-        ):
-            self.reselect_from_get_boxes(
-                modification["selection_boxes"],
-                modification["selected"],
-            )
-
         if modification["eventname"].startswith(("edit", "move")):
             if not saved_cells:
                 event_data = self.save_cells_using_modification(modification, event_data)
             event_data = self.edit_cells_using_modification(modification, event_data)
-            if (
-                not modification["deleted"]["columns"]
-                and not modification["deleted"]["rows"]
-                and not modification["eventname"].startswith("move")
-            ):
-                self.reselect_from_get_boxes(
-                    modification["selection_boxes"],
-                    modification["selected"],
-                )
 
         elif modification["eventname"].startswith("add"):
             event_data["eventname"] = modification["eventname"].replace("add", "delete")
 
         elif modification["eventname"].startswith("delete"):
             event_data["eventname"] = modification["eventname"].replace("delete", "add")
 
+        if not modification["eventname"].startswith("move") and (
+            len(self.row_positions) > 1 or len(self.col_positions) > 1
+        ):
+            self.deselect("all", redraw=False)
+            self.reselect_from_get_boxes(
+                modification["selection_boxes"],
+                modification["selected"],
+            )
+
         if self.selected:
             self.see(
                 r=self.selected.row,
                 c=self.selected.column,
                 keep_yscroll=False,
                 keep_xscroll=False,
                 bottom_right_corner=False,
@@ -3745,17 +3730,18 @@
                     h = int(self.max_row_height)
                 if h > rhs[datarn]:
                     rhs[datarn] = h
         added_w_space = 1 if slim else 7
         for datacn in itercols:
             if (hw := self.CH.get_cell_dimensions(datacn)[0]) > w:
                 w = hw
+            else:
+                w = min_column_width
             for datarn in iterrows:
-                txt = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
-                if txt:
+                if txt := self.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True):
                     qconf(qtxtm, text=txt, font=qfont)
                     b = qbbox(qtxtm)
                     tw = b[2] - b[0] + added_w_space
                     h = b[3] - b[1] + 5
                 else:
                     tw = min_column_width
                     h = min_rh
@@ -4296,14 +4282,15 @@
         column_widths: dict,
         event_data: dict,
         displayed_columns: None | list[int] = None,
         create_ops: bool = True,
         create_selections: bool = True,
         add_row_positions: bool = True,
         push_ops: bool = True,
+        mod_event_boxes: bool = True,
     ) -> EventDataDict:
         self.saved_column_widths = {}
         saved_displayed_columns = list(self.displayed_columns)
         if isinstance(displayed_columns, list):
             self.displayed_columns = displayed_columns
         elif not self.all_columns_displayed:
             # push displayed indexes by one for every inserted column
@@ -4326,26 +4313,34 @@
                 column_widths,
             )
         )
         # rn needed for indexing but cn insert
         maxrn = 0
         for cn, rowdict in reversed(columns.items()):
             for rn, v in rowdict.items():
-                if rn >= len(self.data):
+                if rn < len(self.data) and cn > len(self.data[rn]):
+                    self.fix_row_len(rn, cn - 1)
+                elif rn >= len(self.data):
                     self.fix_data_len(rn, cn - 1)
                 if rn > maxrn:
                     maxrn = rn
                 self.data[rn].insert(cn, v)
         # if not hiding rows then we can extend row positions if necessary
-        if add_row_positions and self.all_rows_displayed and maxrn + 1 > len(self.row_positions) - 1:
-            default_row_height = self.get_default_row_height()
+        if add_row_positions and self.all_rows_displayed and maxrn >= len(self.row_positions) - 1:
+            default_height = self.get_default_row_height()
+            event_data["added"]["rows"] = {
+                "table": {},
+                "index": {},
+                "row_heights": {rn: default_height for rn in range(len(self.row_positions) - 1, maxrn + 1)},
+                "displayed_rows": self.displayed_rows,
+            }
             self.set_row_positions(
                 itr=chain(
                     self.gen_row_heights(),
-                    repeat(default_row_height, len(self.row_positions) - 1, maxrn + 1),
+                    repeat(default_height, maxrn + 1 - (len(self.row_positions) - 1)),
                 )
             )
         if isinstance(self._headers, list) and header:
             self._headers = insert_items(self._headers, header, self.CH.fix_header)
         if push_ops:
             self.adjust_options_post_add_columns(
                 cols=tuple(reversed(columns)),
@@ -4358,14 +4353,17 @@
                     0,
                     boxst,
                     len(self.row_positions) - 1,
                     boxend,
                     "columns",
                     run_binding=True,
                 )
+            if mod_event_boxes:
+                event_data["selection_boxes"] = self.get_boxes()
+                event_data["selected"] = self.selected
         event_data["added"]["columns"] = {
             "table": columns,
             "header": header,
             "column_widths": column_widths,
             "displayed_columns": saved_displayed_columns,
         }
         return event_data
@@ -4429,14 +4427,15 @@
         row_heights: dict,
         event_data: dict,
         displayed_rows: None | list[int] = None,
         create_ops: bool = True,
         create_selections: bool = True,
         add_col_positions: bool = True,
         push_ops: bool = True,
+        mod_event_boxes: bool = True,
     ) -> EventDataDict:
         self.saved_row_heights = {}
         saved_displayed_rows = list(self.displayed_rows)
         if isinstance(displayed_rows, list):
             self.displayed_rows = displayed_rows
         elif not self.all_rows_displayed:
             # push displayed indexes by one for every inserted column
@@ -4468,19 +4467,26 @@
                 self.fix_data_len(rn - 1, cn)
             self.data.insert(rn, row)
             if cn > maxcn:
                 maxcn = cn
         if isinstance(self._row_index, list) and index:
             self._row_index = insert_items(self._row_index, index, self.RI.fix_index)
         # if not hiding columns then we can extend col positions if necessary
-        if add_col_positions and self.all_columns_displayed and maxcn + 1 > len(self.col_positions) - 1:
+        if add_col_positions and self.all_columns_displayed and maxcn >= len(self.col_positions) - 1:
+            default_width = self.PAR.ops.default_column_width
+            event_data["added"]["columns"] = {
+                "table": {},
+                "header": {},
+                "column_widths": {cn: default_width for cn in range(len(self.col_positions) - 1, maxcn + 1)},
+                "displayed_columns": self.displayed_columns,
+            }
             self.set_col_positions(
                 itr=chain(
                     self.gen_column_widths(),
-                    repeat(self.PAR.ops.default_column_width, len(self.col_positions) - 1, maxcn + 1),
+                    repeat(default_width, maxcn + 1 - (len(self.col_positions) - 1)),
                 )
             )
         if push_ops:
             self.adjust_options_post_add_rows(
                 rows=tuple(reversed(rows)),
                 create_ops=create_ops,
             )
@@ -4491,14 +4497,17 @@
                     boxst,
                     0,
                     boxend,
                     len(self.col_positions) - 1,
                     "rows",
                     run_binding=True,
                 )
+            if mod_event_boxes:
+                event_data["selection_boxes"] = self.get_boxes()
+                event_data["selected"] = self.selected
         event_data["added"]["rows"] = {
             "table": rows,
             "index": index,
             "row_heights": row_heights,
             "displayed_rows": saved_displayed_rows,
         }
         return event_data
@@ -5336,26 +5345,29 @@
                         heights[i] = min_row_height
                 if diffs and len(diffs) < len(heights):
                     change = sum(diffs.values()) / (len(heights) - len(diffs))
                     for i, h in enumerate(heights):
                         if i not in diffs:
                             heights[i] -= change
                 self.row_positions = list(accumulate(chain([0], heights)))
-        if self.PAR.ops.auto_resize_row_index is not True:
-            if can_width >= self.col_positions[-1] + self.PAR.ops.empty_horizontal and self.PAR.xscroll_showing:
-                self.PAR.xscroll.grid_forget()
-                self.PAR.xscroll_showing = False
-            elif (
-                can_width < self.col_positions[-1] + self.PAR.ops.empty_horizontal
-                and not self.PAR.xscroll_showing
-                and not self.PAR.xscroll_disabled
-                and can_height > 40
-            ):
-                self.PAR.xscroll.grid(row=2, column=0, columnspan=2, sticky="nswe")
-                self.PAR.xscroll_showing = True
+        if (
+            self.PAR.ops.auto_resize_row_index is not True
+            and can_width >= self.col_positions[-1] + self.PAR.ops.empty_horizontal
+            and self.PAR.xscroll_showing
+        ):
+            self.PAR.xscroll.grid_forget()
+            self.PAR.xscroll_showing = False
+        elif (
+            can_width < self.col_positions[-1] + self.PAR.ops.empty_horizontal
+            and not self.PAR.xscroll_showing
+            and not self.PAR.xscroll_disabled
+            and can_height > 40
+        ):
+            self.PAR.xscroll.grid(row=2, column=0, columnspan=2, sticky="nswe")
+            self.PAR.xscroll_showing = True
         if can_height >= self.row_positions[-1] + self.PAR.ops.empty_vertical and self.PAR.yscroll_showing:
             self.PAR.yscroll.grid_forget()
             self.PAR.yscroll_showing = False
         elif (
             can_height < self.row_positions[-1] + self.PAR.ops.empty_vertical
             and not self.PAR.yscroll_showing
             and not self.PAR.yscroll_disabled
@@ -5825,15 +5837,16 @@
                         r,
                         c,
                         selection_box.type_,
                         selection_box.fill_iid,
                     )
                     return
             # wasn't provided an item and couldn't find a box at coords so select cell
-            self.select_cell(r, c, redraw=True)
+            if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
+                self.select_cell(r, c, redraw=True)
 
     def set_current_to_last(self) -> None:
         if self.selection_boxes:
             box = next(iter(reversed(self.selection_boxes.values())))
             r1, c1, r2, c2 = box.coords
             if r2 - r1 == 1 and c2 - c1 == 1:
                 self.itemconfig(box.fill_iid, state="hidden")
```

### Comparing `tksheet-7.2.2/tksheet/other_classes.py` & `tksheet-7.2.3/tksheet/other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/row_index.py` & `tksheet-7.2.3/tksheet/row_index.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/sheet.py` & `tksheet-7.2.3/tksheet/sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1499,14 +1499,15 @@
             self.MT.reset_tags()
         if undo_stack:
             self.reset_undos()
         if selections:
             self.MT.deselect(redraw=False)
         if sheet_options:
             self.ops = new_sheet_options()
+            self.change_theme(redraw=False)
         if tree:
             self.RI.tree_reset()
         if tree or row_heights or column_widths:
             self.MT.hide_dropdown_editor_all_canvases()
         return self.set_refresh_timer(redraw)
 
     def set_sheet_data(
@@ -4287,14 +4288,17 @@
             self.config(
                 highlightbackground=kwargs["outline_color"],
                 highlightcolor=kwargs["outline_color"],
             )
         if any(k in kwargs for k in scrollbar_options_keys):
             self.set_scrollbar_options()
         self.MT.create_rc_menus()
+        if "treeview" in kwargs:
+            self.set_options(auto_resize_row_index=True, redraw=False)
+            self.index_align("w", redraw=False)
         return self.set_refresh_timer(redraw)
 
     def set_scrollbar_options(self) -> Sheet:
         style = ttk.Style()
         for orientation in ("vertical", "horizontal"):
             style.configure(
                 f"Sheet{self.unique_id}.{orientation.capitalize()}.TScrollbar",
@@ -4789,17 +4793,19 @@
                 if index:
                     for count, cid in enumerate(self.get_children("")):
                         if count >= index:
                             break
                         idx += sum(1 for _ in self.RI.get_iid_descendants(cid)) + 1
             else:
                 idx = len(self.MT._row_index)
+        if values is None:
+            values = []
         self.insert_rows(
             idx=idx,
-            rows=[[self.RI.tree[iid]] + [] if values is None else values],
+            rows=[[self.RI.tree[iid]] + values],
             row_index=True,
             create_selections=create_selections,
             fill=False,
         )
         self.RI.tree_rns[iid] = idx
         if pid and (pid not in self.RI.tree_open_ids or not self.item_displayed(pid)):
             self.hide_rows(idx, deselect_all=False, data_indexes=True)
```

### Comparing `tksheet-7.2.2/tksheet/sheet_options.py` & `tksheet-7.2.3/tksheet/sheet_options.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/text_editor.py` & `tksheet-7.2.3/tksheet/text_editor.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/themes.py` & `tksheet-7.2.3/tksheet/themes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/top_left_rectangle.py` & `tksheet-7.2.3/tksheet/top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet/vars.py` & `tksheet-7.2.3/tksheet/vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.2/tksheet.egg-info/PKG-INFO` & `tksheet-7.2.3/tksheet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.2.2
+Version: 7.2.3
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

