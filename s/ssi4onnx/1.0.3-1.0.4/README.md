# Comparing `tmp/ssi4onnx-1.0.3.tar.gz` & `tmp/ssi4onnx-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssi4onnx-1.0.3.tar", last modified: Tue Apr 30 06:29:15 2024, max compression
+gzip compressed data, was "ssi4onnx-1.0.4.tar", last modified: Tue May 28 23:51:06 2024, max compression
```

## Comparing `ssi4onnx-1.0.3.tar` & `ssi4onnx-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:15.948312 ssi4onnx-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 06:29:07.000000 ssi4onnx-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-30 06:29:15.948312 ssi4onnx-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-30 06:29:07.000000 ssi4onnx-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:29:15.948312 ssi4onnx-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-30 06:29:07.000000 ssi4onnx-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:15.948312 ssi4onnx-1.0.3/ssi4onnx/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 06:29:07.000000 ssi4onnx-1.0.3/ssi4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 06:29:07.000000 ssi4onnx-1.0.3/ssi4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-30 06:29:07.000000 ssi4onnx-1.0.3/ssi4onnx/onnx_shape_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:15.948312 ssi4onnx-1.0.3/ssi4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-30 06:29:15.000000 ssi4onnx-1.0.3/ssi4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-30 06:29:15.000000 ssi4onnx-1.0.3/ssi4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:29:15.000000 ssi4onnx-1.0.3/ssi4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 06:29:15.000000 ssi4onnx-1.0.3/ssi4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 06:29:15.000000 ssi4onnx-1.0.3/ssi4onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:51:06.719067 ssi4onnx-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 23:51:00.000000 ssi4onnx-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-28 23:51:06.719067 ssi4onnx-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-28 23:51:00.000000 ssi4onnx-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:51:06.719067 ssi4onnx-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-28 23:51:00.000000 ssi4onnx-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:51:06.715067 ssi4onnx-1.0.4/ssi4onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 23:51:00.000000 ssi4onnx-1.0.4/ssi4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 23:51:00.000000 ssi4onnx-1.0.4/ssi4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-28 23:51:00.000000 ssi4onnx-1.0.4/ssi4onnx/onnx_shape_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:51:06.719067 ssi4onnx-1.0.4/ssi4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-28 23:51:06.000000 ssi4onnx-1.0.4/ssi4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 23:51:06.000000 ssi4onnx-1.0.4/ssi4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:51:06.000000 ssi4onnx-1.0.4/ssi4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 23:51:06.000000 ssi4onnx-1.0.4/ssi4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 23:51:06.000000 ssi4onnx-1.0.4/ssi4onnx.egg-info/top_level.txt
```

### Comparing `ssi4onnx-1.0.3/LICENSE` & `ssi4onnx-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ssi4onnx-1.0.3/PKG-INFO` & `ssi4onnx-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi4onnx
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple Shape Inference tool for ONNX.
 Home-page: https://github.com/PINTO0309/ssi4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `ssi4onnx-1.0.3/README.md` & `ssi4onnx-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ssi4onnx-1.0.3/setup.py` & `ssi4onnx-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `ssi4onnx-1.0.3/ssi4onnx/onnx_shape_inference.py` & `ssi4onnx-1.0.4/ssi4onnx/onnx_shape_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,24 +78,31 @@
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
 
     # Shape Estimation
     estimated_graph = None
+    exported_onnx_graph = gs.export_onnx(graph, do_type_check=False, **meta_data)
+    if metadata_props is not None:
+        exported_onnx_graph.metadata_props.extend(metadata_props)
     try:
-        estimated_graph = onnx.shape_inference.infer_shapes(gs.export_onnx(graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version}))
+        estimated_graph = onnx.shape_inference.infer_shapes(exported_onnx_graph)
     except:
-        estimated_graph = gs.export_onnx(graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version})
+        estimated_graph = exported_onnx_graph
         if not non_verbose:
             print(
                 f'{Color.YELLOW}WARNING:{Color.RESET} '+
                 'The input shape of the next OP does not match the output shape. '+
                 'Be sure to open the .onnx file to verify the certainty of the geometry.'
             )
```

### Comparing `ssi4onnx-1.0.3/ssi4onnx.egg-info/PKG-INFO` & `ssi4onnx-1.0.4/ssi4onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi4onnx
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple Shape Inference tool for ONNX.
 Home-page: https://github.com/PINTO0309/ssi4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

