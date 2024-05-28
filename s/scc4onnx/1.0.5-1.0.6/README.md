# Comparing `tmp/scc4onnx-1.0.5.tar.gz` & `tmp/scc4onnx-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scc4onnx-1.0.5.tar", last modified: Fri Sep  9 16:36:36 2022, max compression
+gzip compressed data, was "scc4onnx-1.0.6.tar", last modified: Tue May 28 23:07:38 2024, max compression
```

## Comparing `scc4onnx-1.0.5.tar` & `scc4onnx-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:36:36.564049 scc4onnx-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-09 16:36:28.000000 scc4onnx-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9648 2022-09-09 16:36:36.564049 scc4onnx-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9108 2022-09-09 16:36:28.000000 scc4onnx-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:36:36.560049 scc4onnx-1.0.5/scc4onnx/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-09 16:36:28.000000 scc4onnx-1.0.5/scc4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 16:36:28.000000 scc4onnx-1.0.5/scc4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20822 2022-09-09 16:36:28.000000 scc4onnx-1.0.5/scc4onnx/onnx_input_order_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:36:36.564049 scc4onnx-1.0.5/scc4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9648 2022-09-09 16:36:36.000000 scc4onnx-1.0.5/scc4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-09 16:36:36.000000 scc4onnx-1.0.5/scc4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 16:36:36.000000 scc4onnx-1.0.5/scc4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-09 16:36:36.000000 scc4onnx-1.0.5/scc4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-09 16:36:36.000000 scc4onnx-1.0.5/scc4onnx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-09 16:36:36.564049 scc4onnx-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-09 16:36:28.000000 scc4onnx-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:38.419218 scc4onnx-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 23:07:32.000000 scc4onnx-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-05-28 23:07:38.419218 scc4onnx-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-05-28 23:07:32.000000 scc4onnx-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:38.419218 scc4onnx-1.0.6/scc4onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 23:07:32.000000 scc4onnx-1.0.6/scc4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 23:07:32.000000 scc4onnx-1.0.6/scc4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-05-28 23:07:32.000000 scc4onnx-1.0.6/scc4onnx/onnx_input_order_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:38.419218 scc4onnx-1.0.6/scc4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-05-28 23:07:38.000000 scc4onnx-1.0.6/scc4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 23:07:38.000000 scc4onnx-1.0.6/scc4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:07:38.000000 scc4onnx-1.0.6/scc4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 23:07:38.000000 scc4onnx-1.0.6/scc4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 23:07:38.000000 scc4onnx-1.0.6/scc4onnx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:07:38.419218 scc4onnx-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-28 23:07:32.000000 scc4onnx-1.0.6/setup.py
```

### Comparing `scc4onnx-1.0.5/LICENSE` & `scc4onnx-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scc4onnx-1.0.5/PKG-INFO` & `scc4onnx-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scc4onnx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Very simple NCHW and NHWC conversion tool for ONNX. Change to the specified input order for each and every input OP. Also, change the channel order of RGB and BGR. Simple Channel Converter for ONNX. Simple Channel Conversion for ONNX.
 Home-page: https://github.com/PINTO0309/scc4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `scc4onnx-1.0.5/README.md` & `scc4onnx-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `scc4onnx-1.0.5/scc4onnx/onnx_input_order_converter.py` & `scc4onnx-1.0.6/scc4onnx/onnx_input_order_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,14 +214,23 @@
         )
         sys.exit(1)
 
     # Loading Graphs
     # onnx_graph If specified, onnx_graph is processed first
     if not onnx_graph:
         onnx_graph = onnx.load(input_onnx_file_path)
+
+    # domain, ir_version
+    domain: str = onnx_graph.domain
+    ir_version: int = onnx_graph.ir_version
+    meta_data = {'domain': domain, 'ir_version': ir_version}
+    metadata_props = None
+    if hasattr(onnx_graph, 'metadata_props'):
+        metadata_props = onnx_graph.metadata_props
+
     graph = gs.import_onnx(onnx_graph)
 
     # input_op_names_and_order_dims check
     # input_op_names_and_order_dims = {"name": shape, ...}
     inverted_list = {}
     new_input_shapes = {}
     if input_op_names_and_order_dims:
@@ -392,15 +401,17 @@
                 graph.nodes.append(slice_op)
         for concat_op in concat_list:
             graph.nodes.append(concat_op)
 
 
     # Cleanup
     graph.cleanup().toposort()
-    order_converted_graph = gs.export_onnx(graph)
+    order_converted_graph = gs.export_onnx(graph, do_type_check=False, **meta_data)
+    if metadata_props is not None:
+        order_converted_graph.metadata_props.extend(metadata_props)
 
     # Optimize
     new_model = None
     try:
         new_model = onnx.shape_inference.infer_shapes(order_converted_graph)
     except Exception as e:
         new_model = order_converted_graph
```

### Comparing `scc4onnx-1.0.5/scc4onnx.egg-info/PKG-INFO` & `scc4onnx-1.0.6/scc4onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scc4onnx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Very simple NCHW and NHWC conversion tool for ONNX. Change to the specified input order for each and every input OP. Also, change the channel order of RGB and BGR. Simple Channel Converter for ONNX. Simple Channel Conversion for ONNX.
 Home-page: https://github.com/PINTO0309/scc4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `scc4onnx-1.0.5/setup.py` & `scc4onnx-1.0.6/setup.py`

 * *Files identical despite different names*

