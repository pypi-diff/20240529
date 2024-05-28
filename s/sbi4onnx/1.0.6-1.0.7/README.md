# Comparing `tmp/sbi4onnx-1.0.6.tar.gz` & `tmp/sbi4onnx-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbi4onnx-1.0.6.tar", last modified: Tue Apr 30 05:52:04 2024, max compression
+gzip compressed data, was "sbi4onnx-1.0.7.tar", last modified: Tue May 28 23:43:49 2024, max compression
```

## Comparing `sbi4onnx-1.0.6.tar` & `sbi4onnx-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:04.108938 sbi4onnx-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 05:51:57.000000 sbi4onnx-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-30 05:52:04.108938 sbi4onnx-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-30 05:51:57.000000 sbi4onnx-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:04.108938 sbi4onnx-1.0.6/sbi4onnx/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 05:51:57.000000 sbi4onnx-1.0.6/sbi4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 05:51:57.000000 sbi4onnx-1.0.6/sbi4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-30 05:51:57.000000 sbi4onnx-1.0.6/sbi4onnx/onnx_batchsize_initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:52:04.108938 sbi4onnx-1.0.6/sbi4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-30 05:52:04.000000 sbi4onnx-1.0.6/sbi4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 05:52:04.000000 sbi4onnx-1.0.6/sbi4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:52:04.000000 sbi4onnx-1.0.6/sbi4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 05:52:04.000000 sbi4onnx-1.0.6/sbi4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 05:52:04.000000 sbi4onnx-1.0.6/sbi4onnx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 05:52:04.108938 sbi4onnx-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-30 05:51:57.000000 sbi4onnx-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:43:49.170888 sbi4onnx-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 23:43:43.000000 sbi4onnx-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-28 23:43:49.170888 sbi4onnx-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-28 23:43:43.000000 sbi4onnx-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:43:49.166888 sbi4onnx-1.0.7/sbi4onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 23:43:43.000000 sbi4onnx-1.0.7/sbi4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 23:43:43.000000 sbi4onnx-1.0.7/sbi4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-28 23:43:43.000000 sbi4onnx-1.0.7/sbi4onnx/onnx_batchsize_initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:43:49.170888 sbi4onnx-1.0.7/sbi4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-28 23:43:49.000000 sbi4onnx-1.0.7/sbi4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 23:43:49.000000 sbi4onnx-1.0.7/sbi4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:43:49.000000 sbi4onnx-1.0.7/sbi4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 23:43:49.000000 sbi4onnx-1.0.7/sbi4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 23:43:49.000000 sbi4onnx-1.0.7/sbi4onnx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:43:49.170888 sbi4onnx-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-28 23:43:43.000000 sbi4onnx-1.0.7/setup.py
```

### Comparing `sbi4onnx-1.0.6/LICENSE` & `sbi4onnx-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sbi4onnx-1.0.6/PKG-INFO` & `sbi4onnx-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbi4onnx
-Version: 1.0.6
+Version: 1.0.7
 Summary: A very simple script that only initializes the batch size of ONNX. Simple Batchsize Initialization for ONNX.
 Home-page: https://github.com/PINTO0309/sbi4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `sbi4onnx-1.0.6/README.md` & `sbi4onnx-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sbi4onnx-1.0.6/sbi4onnx/onnx_batchsize_initialize.py` & `sbi4onnx-1.0.7/sbi4onnx/onnx_batchsize_initialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,18 +103,24 @@
             onnx_graph, _ = simplify(onnx_graph)
     except:
         pass
 
     # domain, ir_version
     domain: str = onnx_graph.domain
     ir_version: int = onnx_graph.ir_version
+    meta_data = {'domain': domain, 'ir_version': ir_version}
+    metadata_props = None
+    if hasattr(onnx_graph, 'metadata_props'):
+        metadata_props = onnx_graph.metadata_props
 
     graph = gs.import_onnx(onnx_graph)
     graph.cleanup().toposort()
-    target_model = gs.export_onnx(graph, do_type_check=False, **{'domain': domain, 'ir_version': ir_version})
+    target_model = gs.export_onnx(graph, do_type_check=False, **meta_data)
+    if metadata_props is not None:
+        target_model.metadata_props.extend(metadata_props)
     target_graph = target_model.graph
 
     # Change batch size in input, output and value_info
     taget_nodes = \
         list(target_graph.input) + \
         list(target_graph.value_info) + \
         list(target_graph.output)
```

### Comparing `sbi4onnx-1.0.6/sbi4onnx.egg-info/PKG-INFO` & `sbi4onnx-1.0.7/sbi4onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbi4onnx
-Version: 1.0.6
+Version: 1.0.7
 Summary: A very simple script that only initializes the batch size of ONNX. Simple Batchsize Initialization for ONNX.
 Home-page: https://github.com/PINTO0309/sbi4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
```

### Comparing `sbi4onnx-1.0.6/setup.py` & `sbi4onnx-1.0.7/setup.py`

 * *Files identical despite different names*

