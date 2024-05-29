# Comparing `tmp/model_resolver-0.7.0.tar.gz` & `tmp/model_resolver-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.7.0.tar", max compression
+gzip compressed data, was "model_resolver-0.8.0.tar", max compression
```

## Comparing `model_resolver-0.7.0.tar` & `model_resolver-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-05-25 15:22:29.323684 model_resolver-0.7.0/LICENSE
--rw-r--r--   0        0        0     1752 2024-05-25 15:22:29.323684 model_resolver-0.7.0/README.md
--rw-r--r--   0        0        0       36 2024-05-25 15:22:29.327684 model_resolver-0.7.0/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-25 15:22:29.327684 model_resolver-0.7.0/model_resolver/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-25 15:22:29.327684 model_resolver-0.7.0/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-25 15:22:29.327684 model_resolver-0.7.0/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    14955 2024-05-25 15:22:29.327684 model_resolver-0.7.0/model_resolver/plugin.py
--rw-r--r--   0        0        0    20600 2024-05-25 15:22:29.327684 model_resolver-0.7.0/model_resolver/render.py
--rw-r--r--   0        0        0      391 2024-05-25 15:22:29.327684 model_resolver-0.7.0/model_resolver/tests/special_filter.py
--rw-r--r--   0        0        0     1248 2024-05-25 15:22:29.327684 model_resolver-0.7.0/model_resolver/utils.py
--rw-r--r--   0        0        0      762 2024-05-25 15:22:45.599699 model_resolver-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-29 17:57:42.179849 model_resolver-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1752 2024-05-29 17:57:42.179849 model_resolver-0.8.0/README.md
+-rw-r--r--   0        0        0       36 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/__main__.py
+-rw-r--r--   0        0        0     2749 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14955 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/plugin.py
+-rw-r--r--   0        0        0    20952 2024-05-29 17:57:42.179849 model_resolver-0.8.0/model_resolver/render.py
+-rw-r--r--   0        0        0      461 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem/assets/debug/models/block/all_white.json
+-rw-r--r--   0        0        0      559 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem/assets/debug/textures/block/white.png
+-rw-r--r--   0        0        0      780 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem/render.png
+-rw-r--r--   0        0        0     1062 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem/target.png
+-rw-r--r--   0        0        0     1753 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/mini_problem.py
+-rw-r--r--   0        0        0      391 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/tests/special_filter.py
+-rw-r--r--   0        0        0     1248 2024-05-29 17:57:42.183849 model_resolver-0.8.0/model_resolver/utils.py
+-rw-r--r--   0        0        0      762 2024-05-29 17:57:58.603922 model_resolver-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.8.0/PKG-INFO
```

### Comparing `model_resolver-0.7.0/LICENSE` & `model_resolver-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.7.0/README.md` & `model_resolver-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `model_resolver-0.7.0/model_resolver/cli.py` & `model_resolver-0.8.0/model_resolver/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,39 +19,45 @@
     output_dir: Annotated[Path, typer.Option(help="Where you want to save the new resourcepack, with new textures corresponding to the model")] = Path.cwd() / "build", 
     save_namespace: Annotated[str, typer.Option(help="Namespace to save the rendered models, default is the namespace the model is in")] = None,
     filter: Annotated[list[str], typer.Option(help="Filter models in directory")] = None,
     use_cache: Annotated[bool, typer.Option(help="Use cache for model rendering)")] = False,
     load_vanilla: Annotated[bool, typer.Option(help="Load vanilla model")] = False,
     resolve_vanilla_atlas: Annotated[bool, typer.Option(help="Resolve vanilla model textures, True if load_vanilla is True")] = False,
     minecraft_version: Annotated[str, typer.Option(help="Minecraft version to use for vanilla models")] = "latest",
-    __special_filter__ = typer.Option(None, hidden=True),
+    __special_filter__ : Annotated[str, typer.Option(hidden=True)] = "",
+    __light__ : Annotated[str, typer.Option(hidden=True)] = "",
     # fmt: on
 ):
     """
     A simple CLI to render models from a resourcepack, can also load vanilla models.
     """
     t_start = perf_counter()
     if isinstance(load_dir, str):
         load_dir = Path(load_dir)
     if isinstance(output_dir, str):
         output_dir = Path(output_dir)
+    if isinstance(__special_filter__, str):
+        __special_filter__ = {}
+    if isinstance(__light__, str):
+        __light__ = {}
     config = ProjectConfig(
         pipeline=["model_resolver"],
         output=output_dir,
         resource_pack={"load": load_dir, "name": load_dir.name},
         meta={
             "model_resolver": {
                 "load_vanilla": load_vanilla,
                 "use_cache": use_cache,
                 "render_size": render_size,
                 "minecraft_version": minecraft_version,
                 "resolve_vanilla_atlas": resolve_vanilla_atlas,
                 "filter": filter,
                 "__special_filter__": __special_filter__,
                 "save_namespace": save_namespace,
+                "__light__": __light__,
             },
         },
     )
     with run_beet(config=config) as ctx:
         pass
     t_end = perf_counter()
     print(f"[green][bold]✔️[/bold]  Finished in {t_end - t_start:.2f} seconds [/green]")
```

### Comparing `model_resolver-0.7.0/model_resolver/my_glutinit.py` & `model_resolver-0.8.0/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.7.0/model_resolver/plugin.py` & `model_resolver-0.8.0/model_resolver/plugin.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.7.0/model_resolver/render.py` & `model_resolver-0.8.0/model_resolver/render.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,18 +131,18 @@
         glutInitWindowPosition(100, 100)
         glutCreateWindow(b"Isometric View")
         glutHideWindow()
         glutSetOption(GLUT_ACTION_ON_WINDOW_CLOSE, GLUT_ACTION_GLUTMAINLOOP_RETURNS)
         glClearColor(0.0, 0.0, 0.0, 0.0)
 
         # Enable lighting
-        MINECRAFT_LIGHT_POWER = 1.0
-        MINECRAFT_AMBIENT_LIGHT = 0.4
+        MINECRAFT_LIGHT_POWER = self.ctx.meta.get("model_resolver", {}).get("__light__", {}).get("minecraft_light_power", 0.6727302277118515)
+        MINECRAFT_AMBIENT_LIGHT = self.ctx.meta.get("model_resolver", {}).get("__light__", {}).get("minecraft_ambient_light", 0.197261163686041)
 
-        glLightfv(GL_LIGHT0, GL_POSITION, [-0.5, -1.0, 0.35, 0.0])
+        glLightfv(GL_LIGHT0, GL_POSITION, self.ctx.meta.get("model_resolver", {}).get("__light__", {}).get("minecraft_light_position", [-0.42341569107908505, -0.6577205642540358, 0.4158725999762756, 0.0]))
         glLightfv(GL_LIGHT0, GL_AMBIENT, [MINECRAFT_AMBIENT_LIGHT] * 4)
         glLightfv(GL_LIGHT0, GL_DIFFUSE, [MINECRAFT_LIGHT_POWER] * 4)
 
         glLightfv(GL_LIGHT1, GL_POSITION, [0.0, 0.0, 10.0, 0.0])
         glLightfv(GL_LIGHT1, GL_DIFFUSE, [1.0] * 4)
         
         self.reload()
```

### Comparing `model_resolver-0.7.0/model_resolver/utils.py` & `model_resolver-0.8.0/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.7.0/pyproject.toml` & `model_resolver-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-resolver"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = ["edayot <pro.e.dayot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `model_resolver-0.7.0/PKG-INFO` & `model_resolver-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

