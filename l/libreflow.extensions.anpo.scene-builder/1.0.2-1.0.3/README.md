# Comparing `tmp/libreflow_extensions_anpo_scene_builder-1.0.2.tar.gz` & `tmp/libreflow_extensions_anpo_scene_builder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_extensions_anpo_scene_builder-1.0.2.tar", last modified: Tue May 21 10:28:45 2024, max compression
+gzip compressed data, was "libreflow_extensions_anpo_scene_builder-1.0.3.tar", last modified: Wed May 29 09:04:49 2024, max compression
```

## Comparing `libreflow_extensions_anpo_scene_builder-1.0.2.tar` & `libreflow_extensions_anpo_scene_builder-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.428262 libreflow_extensions_anpo_scene_builder-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1561 2024-05-21 10:28:45.428262 libreflow_extensions_anpo_scene_builder-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-21 10:28:45.429262 libreflow_extensions_anpo_scene_builder-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.423262 libreflow_extensions_anpo_scene_builder-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.426262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.427262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.427262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.428262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/
--rw-rw-rw-   0 root         (0) root         (0)    19915 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-21 10:28:45.429262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/build_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:28:45.428262 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1561 2024-05-21 10:28:45.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-21 10:28:45.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:28:45.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-21 10:28:45.000000 libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-21 10:28:36.000000 libreflow_extensions_anpo_scene_builder-1.0.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:04:49.678693 libreflow_extensions_anpo_scene_builder-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1786 2024-05-29 09:04:49.677693 libreflow_extensions_anpo_scene_builder-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-29 09:04:49.678693 libreflow_extensions_anpo_scene_builder-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:04:49.673693 libreflow_extensions_anpo_scene_builder-1.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:04:49.675693 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:04:49.676693 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:04:49.676693 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/anpo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/anpo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:04:49.677693 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/anpo/scene_builder/
+-rw-rw-rw-   0 root         (0) root         (0)    26881 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/anpo/scene_builder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-29 09:04:49.678693 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/anpo/scene_builder/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/anpo/scene_builder/build_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:04:49.677693 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow.extensions.anpo.scene_builder.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1786 2024-05-29 09:04:49.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow.extensions.anpo.scene_builder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-29 09:04:49.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow.extensions.anpo.scene_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 09:04:49.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow.extensions.anpo.scene_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 09:04:49.000000 libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow.extensions.anpo.scene_builder.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-29 09:04:40.000000 libreflow_extensions_anpo_scene_builder-1.0.3/versioneer.py
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.2/PKG-INFO` & `libreflow_extensions_anpo_scene_builder-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.scene-builder
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://gitlab.com/lfs.coop/libreflow/extensions/anpo/scene_builder
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -34,14 +34,24 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.3] - 2024-05-29
+
+### Fixed
+
+* Layout and blocking files are created with the path format of their corresponding presets in the task manager (when defined).
+
+### Added
+
+* New action to build a Blender blocking scene.
+
 ## [1.0.2] - 2024-05-21
 
 ### Added
 
 * An option to refresh dependencies (which might be updated in Kitsu before the cache invalidates).
 
 ## [1.0.1] - 2024-05-16
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.2/setup.py` & `libreflow_extensions_anpo_scene_builder-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow/extensions/anpo/scene_builder/__init__.py` & `libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow/extensions/anpo/scene_builder/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class AssetStatus(flow.values.ChoiceValue):
 
     CHOICES = ["NotAvailable", "Downloadable", "Available"]
 
 
-class LayoutDependency(flow.Object):
+class TaskFileDependency(flow.Object):
 
     _parent = flow.Parent()
     _shot = flow.Parent(3)
     
     asset_type = flow.Computed(store_value=False)
     asset_family = flow.Computed(store_value=False)
     asset_code = flow.Computed(store_value=False)
@@ -122,65 +122,68 @@
     def needs_dialog(self):
         return False
 
     def run(self, button):
         self._map.refresh()
 
 
-class LayoutDependencies(flow.DynamicMap):
+class TaskFileDependencies(flow.DynamicMap):
     refresh_action = flow.Child(RefreshDependencies).ui(
         label="Refresh")
     _task = flow.Parent(2)
     _shot = flow.Parent(4)
     _sequence = flow.Parent(6)
     _updated = flow.BoolParam(False)
 
     def __init__(self, parent, name):
-        super(LayoutDependencies, self).__init__(parent, name)
+        super(TaskFileDependencies, self).__init__(parent, name)
         self._assets_data_time = time.time()
         self._assets_data = None
 
     def mapped_names(self, page_num=0, page_size=None):
         if not self._assets_data or time.time() - self._assets_data_time > 30.0:
             self._assets_data = self._get_assets_data()
             self._assets_data_time = time.time()
 
         return list(self._assets_data.keys())
 
-    def _get_assets_data(self):
+    def get_kitsu_casting(self, casting):
         kitsu_api = self.root().project().kitsu_api()
         kitsu_casting = kitsu_api.get_shot_casting(self._shot.name(), self._sequence.name())
-        casting = dict()
-        
+        if kitsu_casting is None:
+            return
+
         # Kitsu assets
         for asset in kitsu_casting:
             asset_name = asset['asset_name']
             asset_type = asset['asset_type_name']
             asset_family = kitsu_api.get_asset_data(asset_name)['data'].get('category', asset_type.lower())
 
             casting[asset_name.replace('-', '_')] = dict(
                 asset_type=asset_type.lower(),
                 asset_family=asset_family.lower(),
                 asset_number=asset['nb_occurences']
             )
 
+    def get_animatic_casting(self, casting):
         # Animatic
         casting['animatic'] = dict(
             asset_type='animatic',
             asset_family='',
         )
-        
-        return casting
+
+    def _get_assets_data(self):
+        raise NotImplementedError
 
     def asset_data(self, asset_name):
         return self._assets_data[asset_name]
 
     @classmethod
     def mapped_type(cls):
-        return LayoutDependency
+        return TaskFileDependency
 
     def columns(self):
         return ["Name", "Type", "Family", "Revision"]
     
     def asset_type_file_name(self, asset_type):
         return {
             "sets": "layers",
@@ -190,15 +193,15 @@
             "animatic": "animatic_mov",
         }[asset_type]
     
     def files_from_asset_type(self, asset, asset_type):
         if asset_type == 'sets' and asset.tasks.has_mapped_name('design'):
             return asset.tasks['design'].files
         elif asset_type == 'animatic':
-            return self._task.files
+            return asset.files
         elif asset.tasks.has_mapped_name('rigging'):
             return asset.tasks['rigging'].files
         else:
             return None
 
     def refresh(self):
         self._assets_data = None
@@ -225,16 +228,14 @@
 class BuildBlenderScene(GenericRunAction):
     ICON = ('icons.libreflow', 'blender')
 
     _task = flow.Parent()
     _shot = flow.Parent(3)
     _sequence = flow.Parent(5)
 
-    dependencies = flow.Child(LayoutDependencies).ui(expanded=True)
-
     def runner_name_and_tags(self):
         return 'Blender', []
     
     def get_run_label(self):
         return "Build scene"
 
     def get_buttons(self):
@@ -248,65 +249,78 @@
         return {
             "ROOT_PATH": self.root().project().get_root()
         }
     
     def target_file_extension(self):
         return 'blend'
 
-    def get_template_path(self, filename):
-        file_mapped_name = filename.replace('.', '_')
-        template_path = resources.get("file_templates", "template.blend")
-        mng = self.root().project().get_task_manager()
-        if not mng.default_tasks.has_mapped_name(self._task.name()): # check default task
-            print(f'Scene Builder - no default task {self._task.name()} -> use default template')
-            return template_path
-
-        default_task = mng.default_tasks[self._task.name()]
-        if not default_task.files.has_mapped_name(file_mapped_name): # check default file
-            print(f'Scene Builder - default task {self._task.name()} has no default file {filename} -> use default template')
-            return template_path
-
-        default_file = default_task.files[file_mapped_name]
+    def get_template_path(self, default_file):
         template_oid = default_file.template_file.get()
         if template_oid is None or not self.root().session().cmds.Flow.exists(template_oid): # check file template
-            print(f'Scene Builder -  template of {self._task.name()}/{filename} is undefined -> use default template')
+            print(f'Scene Builder -  template of {self._task.name()}/{default_file.name()} is undefined -> use default template')
             return template_path
 
         template = self.root().get_object(template_oid)
         if template is None: # check file template
-            print(f'Scene Builder - template of {self._task.name()}/{filename} is undefined -> use default template')
+            print(f'Scene Builder - template of {self._task.name()}/{default_file.name()} is undefined -> use default template')
             return template_path
 
         rev_name = default_file.template_file_revision.get()
         if rev_name == 'Latest': # check template revision
             rev = template.get_head_revision()
         else:
             rev = template.get_revision(rev_name)
         if rev is None or rev.get_sync_status() != 'Available':
-            print(f'Scene Builder - template of {self._task.name()}/{filename} is not available -> use default template')
+            print(f'Scene Builder - template of {self._task.name()}/{default_file.name()} is not available -> use default template')
             return template_path
 
         rev_path = rev.get_path()
         if not os.path.exists(rev_path):
-            print(f'Scene Builder - template of {self._task.name()}/{filename} is not available -> use default template')
+            print(f'Scene Builder - template of {self._task.name()}/{default_file.name()} is not available -> use default template')
             return template_path
 
-        print(f'Scene Builder - custom template found: {rev_path}')
+        print(f'Scene Builder - custom template found: {self._task.name()}/{default_file.name()} -> {rev_path}')
         return rev_path
+
+    def get_default_file(self, task_name, filename):
+        file_mapped_name = filename.replace('.', '_')
+        template_path = resources.get("file_templates", "template.blend")
+        mng = self.root().project().get_task_manager()
+        if not mng.default_tasks.has_mapped_name(task_name): # check default task
+            # print(f'Scene Builder - no default task {task_name} -> use default template')
+            return None
+
+        dft_task = mng.default_tasks[task_name]
+        if not dft_task.files.has_mapped_name(file_mapped_name): # check default file
+            # print(f'Scene Builder - default task {task_name} has no default file {filename} -> use default template')
+            return None
+
+        dft_file = dft_task.files[file_mapped_name]
+        return dft_file
+
+    def get_path_format(self, task_name, filename):
+        dft_file = self.get_default_file(task_name, filename)
+        if dft_file is None:
+            return None
+
+        return dft_file.path_format.get()
     
-    def _ensure_file(self, name, format, to_edit=False, src_path=None, publish_comment=""):
+    def _ensure_file(self, name, format, path_format, to_edit=False, src_path=None, publish_comment=""):
         files = self._task.files
         file_name = "%s_%s" % (name, format)
 
-        if not files.has_mapped_name(file_name):
-            files.create_file.file_name.set(name)
-            files.create_file.file_format.set(format)
-            files.create_file.run(None)
-        
-        file = files[file_name]
+        if files.has_file(name, format):
+            file = files[file_name]
+        else:
+            file = files.add_file(
+                name=name,
+                extension=format,
+                tracked=True,
+                default_path_format=path_format,
+            )
 
         if not to_edit and not src_path:
             return None
         
         if to_edit:
             revision = file.create_working_copy(source_path=src_path)
         else:
@@ -328,15 +342,15 @@
         `cleanup`, `save`.
         '''
 
         blender_operators = {
             "setup": {'operator_command': "bpy.ops.pipeline.scene_builder_setup",
                       'args': "frame_start={frame_start}, frame_end={frame_end}, resolution_x={resolution_x}, resolution_y={resolution_y}, fps={fps}, create_camera=False"},
             "setup_anim": {'operator_command': "bpy.ops.pipeline.scene_builder_setup_animation",
-                           'args': 'alembic_filepath="{alembic_filepath}", assets={assets}, do_automate={do_automate}'},
+                           'args': 'alembic_filepath="{alembic_filepath}", assets={assets}, create_ghost={create_ghost}'},
 
             "add_asset": {'operator_command': 'bpy.ops.pipeline.scene_builder_import_asset',
                           'args': 'filepath="{filepath}", asset_name="{asset_name}", target_collection="{asset_type}"'},
             "add_animatic": {'operator_command': 'bpy.ops.pipeline.scene_builder_add_animatic',
                              'args': 'filepath="{filepath}"'},
             "add_set": {'operator_command': 'bpy.ops.pipeline.scene_builder_import_set',
                         'args': 'directory="{set_dir}", files={set_dicts}'},
@@ -367,32 +381,44 @@
         op = blender_operators[operator]
         operator_command = op['operator_command']
         args = op['args'].format(**kwargs)
         command = f"if {operator_command}.poll(): {operator_command}({args})\n"
         return command
 
 
+class LayoutDependencies(TaskFileDependencies):
+
+    def _get_assets_data(self):
+        casting = dict()
+        self.get_kitsu_casting(casting)
+        self.get_animatic_casting(casting)
+        return casting
+
+
 class BuildLayoutScene(BuildBlenderScene):
 
+    dependencies = flow.Child(LayoutDependencies).ui(expanded=True)
+
     def get_run_label(self):
         return 'Build layout scene'
 
     def extra_argv(self):
         # Get scene builder arguments
         frame_start = 101
-        frame_end = 101 + self._shot_data.get("nb_frames", 0) - 1
+        frame_end = 101 + self._shot_data["nb_frames"] - 1
         resolution_x = 2048
         resolution_y = 858
         fps = 24
 
-        assets = self._shot_data.get("assets_data", [])
-        sets = self._shot_data.get("sets_data", [])
+        assets = self._shot_data["assets_data"]
+        sets = self._shot_data["sets_data"]
         animatic_path = self._shot_data.get("animatic_path", None)
-        layout_path = self._shot_data["layout_path"] # Mandatory
-        template_path = self.get_template_path("layout.blend")
+        layout_path = self._shot_data["layout_scene_path"] # Mandatory
+        template_path = self._shot_data.get("layout_template_path", \
+            resources.get("file_templates", "template.blend"))
 
         # Build Blender Python expression
         python_expr = "import bpy\n"
         python_expr += self._blender_cmd("setup", frame_start=frame_start, frame_end=frame_end, resolution_x=resolution_x, resolution_y=resolution_y, fps=fps)
         python_expr += self._blender_cmd("save", filepath=layout_path)
         
         for name, path, asset_type, asset_number in assets:
@@ -443,14 +469,16 @@
         # Get shot data
         kitsu_api = self.root().project().kitsu_api()
         shot_data = kitsu_api.get_shot_data(shot_name, sequence_name)
 
         # Store dependencies file paths for Blender script building
         self._shot_data = {}
         self._shot_data["nb_frames"] = shot_data["nb_frames"]
+        if self._shot_data["nb_frames"] is None:
+            self._shot_data["nb_frames"] = 0
         self._shot_data["assets_data"] = []
         self._shot_data["sets_data"] = []
 
         for dep in self.dependencies.mapped_items():
             if dep.available.get() != "Available":
                 continue
 
@@ -465,40 +493,199 @@
                     (path, [{"name": name} for name in set_names])
                 )
             elif asset_type == "animatic":
                 self._shot_data["animatic_path"] = path
             else: # characters/props/animals
                 self._shot_data["assets_data"].append((dep.asset_code.get(), path, asset_type, asset_number))
 
+        # Get layout file preset to resolve template and path format
+        default_file = self.get_default_file(self._task.name(), "layout.blend")
+        path_format = None
+        if default_file is not None:
+            self._shot_data["layout_template_path"] = self.get_template_path(default_file)
+            path_format = default_file.path_format.get()
         # Configure layout file
         layout_path = self._ensure_file(
             name='layout',
             format='blend',
+            path_format=path_format,
             to_edit=(button == 'Build and edit'),
             src_path=resources.get("file_templates", "template.blend"),
             publish_comment="Created with scene builder"
         )
 
         self._task.touch()
 
         # Store layout output path
         layout_path = layout_path.replace("\\", "/")
         layout_path = re.sub(r"^//([^/]+)/", r"\\\\\\\\\1\\\\", layout_path) # check drive name
-        self._shot_data["layout_path"] = layout_path
+        self._shot_data["layout_scene_path"] = layout_path
 
         # Build
         super(BuildLayoutScene, self).run(button)
 
 
-def build_layout_scene_action(parent):
+class BlockingDependencies(TaskFileDependencies):
+
+    def _get_assets_data(self):
+        casting = dict()
+        self.get_kitsu_casting(casting)
+        return casting
+
+
+class BuildBlockingScene(BuildBlenderScene):
+
+    dependencies = flow.Child(BlockingDependencies).ui(expanded=True)
+
+    create_ghost = flow.SessionParam(True).ui(editor='bool')
+
+    def get_run_label(self):
+        return 'Build blocking scene'
+
+    def extra_argv(self):
+        # Get scene builder arguments
+        anim_path = self._shot_data.get("anim_path", None)
+        alembic_path = self._shot_data.get("alembic_path", None)
+        assets_data = self._shot_data.get("assets_data", [])
+        assets = []
+        create_ghost = self.create_ghost.get()
+
+        for name, path, asset_type, asset_number in assets_data:
+            for i in range(asset_number):
+                assets.append({"name": name,
+                                "filepath": path,
+                                "target_collection": asset_type})
+
+        # Build Blender Python expression
+        python_expr = "import bpy\n"
+        python_expr += self._blender_cmd("setup_anim",
+                                         alembic_filepath=alembic_path, assets=assets, create_ghost=create_ghost)
+
+        # Update reference files
+        python_expr += self._blender_cmd("update_animatic")
+
+        python_expr += self._blender_cmd("cleanup")
+        python_expr += self._blender_cmd("save", filepath=anim_path)
+
+        return [
+            "-b", anim_path,
+            "--addons", "io_import_images_as_planes,camera_plane,lfs_scene_builder,add_camera_rigs",
+            "--python-expr", wrap_python_expr(python_expr)
+        ]
+
+    def get_buttons(self):
+        latest_revision = None
+        files = self._shot.tasks['layout'].files
+
+        if "layout_blend" in files.mapped_names():
+            latest_revision = files["layout_blend"].get_head_revision()
+
+        if (latest_revision is None or latest_revision.get_sync_status() != 'Available'):
+            msg = "<h2><font color=#D5000D>Last revision of layout file not available</font></h2>"
+            buttons =  ["Cancel"]
+        else:
+            msg = "<h2>Build animation shot</h2>"
+            buttons = ["Build and edit", "Cancel"]
+
+            for dep in self.dependencies.mapped_items():
+                if dep.available.get() in ["Downloadable", "NotAvailable"]:
+                    msg += (
+                        "<h3><font color=#D66700>"
+                        "Some dependencies are still missing, either because they do not already exists or need to be downloaded on your site.\n"
+                        "You can build the scene anyway, but you will have to manually update it when missing dependencies will be available."
+                        "</font></h3>"
+                    )
+                    break
+
+        self.message.set(msg)
+
+        return buttons
+
+    def run(self, button):
+        if button == 'Cancel':
+            return
+
+        if button == "Refresh":
+            self.dependencies.touch()
+            return self.get_result(refresh=True, close=False)
+
+        shot_name = self._shot.name()
+        sequence_name = self._sequence.name()
+
+        # Store dependencies file paths for Blender script building
+        self._shot_data = {}
+        self._shot_data["assets_data"] = []
+
+        for dep in self.dependencies.mapped_items():
+            if dep.available.get() != "Available":
+                continue
+
+            asset_type = dep.asset_type.get()
+            asset_number = dep.asset_number.get()
+            path = dep.asset_path.get().replace("\\", "/")
+            path = re.sub(r"^//([^/]+)/", r"\\\\\1\\", path) # check drive name
+
+            if asset_type in ["sets", "animatic"]:
+                continue
+            # if asset_type == "animatic":
+            #     self._shot_data["animatic_path"] = path
+            self._shot_data["assets_data"].append((dep.asset_code.get(), path, asset_type, asset_number))
+
+        # Configure anim file
+        latest_revision = self._shot.tasks['layout'].files["layout_blend"].get_head_revision()
+        layout_path = latest_revision.get_path()
+
+        # Create empty file
+        anim_path = self._ensure_file(
+            name='anim_blocking',
+            format='blend',
+            path_format=self.get_path_format(self._task.name(), 'anim_blocking.blend'),
+            to_edit=True,
+            src_path=layout_path,
+            publish_comment="Created with anim scene builder"
+        )
+
+        create_ghost = self.create_ghost.get()
+        if create_ghost:
+            # Configure alembic file
+            alembic_path = self._ensure_file(
+                name='ref_layout',
+                format='abc',
+                path_format=self.get_path_format(self._task.name(), 'ref_layout.abc'),
+                src_path=resources.get("file_templates", "template.abc"),
+                publish_comment="Created with anim scene builder"
+            )
+
+        # Store anim and alembic output path
+        anim_path = anim_path.replace("\\", "/")
+        anim_path = re.sub(r"^//([^/]+)/", r"\\\\\\\\\1\\\\", anim_path) # check drive name
+        self._shot_data["anim_path"] = anim_path
+
+        if create_ghost:
+            alembic_path = alembic_path.replace("\\", "/")
+            alembic_path = re.sub(r"^//([^/]+)/", r"\\\\\\\\\1\\\\", alembic_path) # check drive name
+            self._shot_data["alembic_path"] = alembic_path
+
+        # Build
+        super(BuildBlockingScene, self).run(button)
+
+
+def build_scene_action(parent):
     if isinstance(parent, Task) and parent.name() == "layout":
         r = flow.Child(BuildLayoutScene)
         r.name = 'build_layout_scene'
         r.index = None
         return r
 
-def install_extensions(session): 
+    if isinstance(parent, Task) and parent.name() == "animblock":
+        r = flow.Child(BuildBlockingScene)
+        r.name = 'build_blocking_scene'
+        r.index = None
+        return r
+
+
+def install_extensions(session):
     return {
         "scene_builder": [
-            build_layout_scene_action
+            build_scene_action
         ]
     }
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/PKG-INFO` & `libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow.extensions.anpo.scene_builder.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.scene-builder
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://gitlab.com/lfs.coop/libreflow/extensions/anpo/scene_builder
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -34,14 +34,24 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.3] - 2024-05-29
+
+### Fixed
+
+* Layout and blocking files are created with the path format of their corresponding presets in the task manager (when defined).
+
+### Added
+
+* New action to build a Blender blocking scene.
+
 ## [1.0.2] - 2024-05-21
 
 ### Added
 
 * An option to refresh dependencies (which might be updated in Kitsu before the cache invalidates).
 
 ## [1.0.1] - 2024-05-16
```

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.2/src/libreflow.extensions.anpo.scene_builder.egg-info/SOURCES.txt` & `libreflow_extensions_anpo_scene_builder-1.0.3/src/libreflow.extensions.anpo.scene_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_scene_builder-1.0.2/versioneer.py` & `libreflow_extensions_anpo_scene_builder-1.0.3/versioneer.py`

 * *Files identical despite different names*

