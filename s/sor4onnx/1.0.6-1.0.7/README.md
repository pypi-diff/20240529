# Comparing `tmp/sor4onnx-1.0.6.tar.gz` & `tmp/sor4onnx-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sor4onnx-1.0.6.tar", last modified: Tue Apr 30 06:35:06 2024, max compression
+gzip compressed data, was "sor4onnx-1.0.7.tar", last modified: Tue May 28 23:38:55 2024, max compression
```

## Comparing `sor4onnx-1.0.6.tar` & `sor4onnx-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:06.283565 sor4onnx-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-30 06:35:06.279565 sor4onnx-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:35:06.283565 sor4onnx-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:06.279565 sor4onnx-1.0.6/sor4onnx/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/sor4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/sor4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-04-30 06:35:00.000000 sor4onnx-1.0.6/sor4onnx/onnx_opname_renamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:06.279565 sor4onnx-1.0.6/sor4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 06:35:06.000000 sor4onnx-1.0.6/sor4onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:38:55.819225 sor4onnx-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 23:38:46.000000 sor4onnx-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-28 23:38:55.819225 sor4onnx-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-28 23:38:46.000000 sor4onnx-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:38:55.819225 sor4onnx-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-28 23:38:46.000000 sor4onnx-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:38:55.819225 sor4onnx-1.0.7/sor4onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-28 23:38:46.000000 sor4onnx-1.0.7/sor4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 23:38:46.000000 sor4onnx-1.0.7/sor4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-28 23:38:46.000000 sor4onnx-1.0.7/sor4onnx/onnx_opname_renamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:38:55.819225 sor4onnx-1.0.7/sor4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-28 23:38:55.000000 sor4onnx-1.0.7/sor4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 23:38:55.000000 sor4onnx-1.0.7/sor4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:38:55.000000 sor4onnx-1.0.7/sor4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 23:38:55.000000 sor4onnx-1.0.7/sor4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 23:38:55.000000 sor4onnx-1.0.7/sor4onnx.egg-info/top_level.txt
```

### Comparing `sor4onnx-1.0.6/LICENSE` & `sor4onnx-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sor4onnx-1.0.6/PKG-INFO` & `sor4onnx-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sor4onnx
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple OP Renamer for ONNX.
 Home-page: https://github.com/PINTO0309/sor4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `sor4onnx-1.0.6/README.md` & `sor4onnx-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sor4onnx-1.0.6/setup.py` & `sor4onnx-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `sor4onnx-1.0.6/sor4onnx/onnx_opname_renamer.py` & `sor4onnx-1.0.7/sor4onnx/onnx_opname_renamer.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,18 @@
     # onnx_graph If specified, onnx_graph is processed first
     if not onnx_graph:
         onnx_graph = onnx.load(input_onnx_file_path)
 
     # domain, ir_version
     domain: str = onnx_graph.domain
     ir_version: int = onnx_graph.ir_version
+    meta_data = {'domain': domain, 'ir_version': ir_version}
+    metadata_props = None
+    if hasattr(onnx_graph, 'metadata_props'):
+        metadata_props = onnx_graph.metadata_props
 
     graph = gs.import_onnx(onnx_graph)
     graph.cleanup().toposort()
 
     if mode in ['full', 'inputs']:
         for graph_input in graph.inputs:
             if search_mode == 'exact_match':
@@ -214,18 +218,21 @@
             graph_node.name = f'sor_{graph_node.op}_{supplementation_idx}'
             supplementation_idx += 1
 
     graph.cleanup().toposort()
 
     # Shape Estimation
     renamed_graph = None
+    exported_onnx_graph = gs.export_onnx(graph, do_type_check=False, **meta_data)
+    if metadata_props is not None:
+        exported_onnx_graph.metadata_props.extend(metadata_props)
     try:
-        renamed_graph = onnx.shape_inference.infer_shapes(gs.export_onnx(graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version}))
+        renamed_graph = onnx.shape_inference.infer_shapes(exported_onnx_graph)
     except:
-        renamed_graph = gs.export_onnx(graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version})
+        renamed_graph = exported_onnx_graph
         if not non_verbose:
             print(
                 f'{Color.YELLOW}WARNING:{Color.RESET} '+
                 'The input shape of the next OP does not match the output shape. '+
                 'Be sure to open the .onnx file to verify the certainty of the geometry.'
             )
```

### Comparing `sor4onnx-1.0.6/sor4onnx.egg-info/PKG-INFO` & `sor4onnx-1.0.7/sor4onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sor4onnx
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple OP Renamer for ONNX.
 Home-page: https://github.com/PINTO0309/sor4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

