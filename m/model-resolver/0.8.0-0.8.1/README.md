# Comparing `tmp/model_resolver-0.8.0.tar.gz` & `tmp/model_resolver-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.8.0.tar", max compression
+gzip compressed data, was "model_resolver-0.8.1.tar", max compression
```

## Comparing `model_resolver-0.8.0.tar` & `model_resolver-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-05-29 17:57:42.179849 model_resolver-0.8.0/LICENSE
--rw-r--r--   0        0        0     1752 2024-05-29 17:57:42.179849 model_resolver-0.8.0/README.md
--rw-r--r--   0        0        0       36 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/__main__.py
--rw-r--r--   0        0        0     2749 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    14955 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/plugin.py
--rw-r--r--   0        0        0    20952 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/render.py
--rw-r--r--   0        0        0      461 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem/assets/debug/models/block/all_white.json
--rw-r--r--   0        0        0      559 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem/assets/debug/textures/block/white.png
--rw-r--r--   0        0        0      780 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem/render.png
--rw-r--r--   0        0        0     1062 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem/target.png
--rw-r--r--   0        0        0     1753 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem.py
--rw-r--r--   0        0        0      391 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/special_filter.py
--rw-r--r--   0        0        0     1248 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/utils.py
--rw-r--r--   0        0        0      762 2024-05-29 17:57:58.603922 model_resolver-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-29 18:14:51.091942 model_resolver-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1752 2024-05-29 18:14:51.091942 model_resolver-0.8.1/README.md
+-rw-r--r--   0        0        0       36 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/__main__.py
+-rw-r--r--   0        0        0     2749 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14987 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/plugin.py
+-rw-r--r--   0        0        0    20952 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/render.py
+-rw-r--r--   0        0        0      461 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/tests/mini_problem/assets/debug/models/block/all_white.json
+-rw-r--r--   0        0        0      559 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/tests/mini_problem/assets/debug/textures/block/white.png
+-rw-r--r--   0        0        0      780 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/tests/mini_problem/render.png
+-rw-r--r--   0        0        0     1062 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/tests/mini_problem/target.png
+-rw-r--r--   0        0        0     1753 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/tests/mini_problem.py
+-rw-r--r--   0        0        0      391 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/tests/special_filter.py
+-rw-r--r--   0        0        0     1248 2024-05-29 18:14:51.095942 model_resolver-0.8.1/model_resolver/utils.py
+-rw-r--r--   0        0        0      762 2024-05-29 18:15:06.411949 model_resolver-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.8.1/PKG-INFO
```

### Comparing `model_resolver-0.8.0/LICENSE` & `model_resolver-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/README.md` & `model_resolver-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/model_resolver/cli.py` & `model_resolver-0.8.1/model_resolver/cli.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/model_resolver/my_glutinit.py` & `model_resolver-0.8.1/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/model_resolver/plugin.py` & `model_resolver-0.8.1/model_resolver/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     use_cache = ctx.meta.get("model_resolver", {}).get("use_cache", False)
     render_size = ctx.meta.get("model_resolver", {}).get("render_size", 1024)
     minecraft_version = ctx.meta.get("model_resolver", {}).get(
         "minecraft_version", "latest"
     )
     filter = ctx.meta.get("model_resolver", {}).get("filter", None)
     __special_filter__ = ctx.meta.get("model_resolver", {}).get("__special_filter__", None)
-    if __special_filter__ is not None:
+    if __special_filter__ is not None and len(__special_filter__) > 0:
         filter = __special_filter__.keys()
 
     vanilla = ctx.inject(Vanilla)
     if not minecraft_version == "latest":
         vanilla = vanilla.releases[minecraft_version]
     generated_models = set()
     generated_textures = set()
```

### Comparing `model_resolver-0.8.0/model_resolver/render.py` & `model_resolver-0.8.1/model_resolver/render.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/model_resolver/tests/mini_problem/assets/debug/textures/block/white.png` & `model_resolver-0.8.1/model_resolver/tests/mini_problem/assets/debug/textures/block/white.png`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/model_resolver/tests/mini_problem/render.png` & `model_resolver-0.8.1/model_resolver/tests/mini_problem/render.png`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/model_resolver/tests/mini_problem/target.png` & `model_resolver-0.8.1/model_resolver/tests/mini_problem/target.png`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/model_resolver/tests/mini_problem.py` & `model_resolver-0.8.1/model_resolver/tests/mini_problem.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/model_resolver/utils.py` & `model_resolver-0.8.1/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.8.0/pyproject.toml` & `model_resolver-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-resolver"
-version = "0.8.0"
+version = "0.8.1"
 description = ""
 authors = ["edayot <pro.e.dayot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `model_resolver-0.8.0/PKG-INFO` & `model_resolver-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.8.0
+Version: 0.8.1
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

