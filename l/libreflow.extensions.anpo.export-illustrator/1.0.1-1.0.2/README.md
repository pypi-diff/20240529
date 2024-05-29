# Comparing `tmp/libreflow_extensions_anpo_export_illustrator-1.0.1.tar.gz` & `tmp/libreflow_extensions_anpo_export_illustrator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_extensions_anpo_export_illustrator-1.0.1.tar", last modified: Tue May 28 08:21:03 2024, max compression
+gzip compressed data, was "libreflow_extensions_anpo_export_illustrator-1.0.2.tar", last modified: Wed May 29 20:39:53 2024, max compression
```

## Comparing `libreflow_extensions_anpo_export_illustrator-1.0.1.tar` & `libreflow_extensions_anpo_export_illustrator-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:21:03.987673 libreflow_extensions_anpo_export_illustrator-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1323 2024-05-28 08:21:03.987673 libreflow_extensions_anpo_export_illustrator-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-28 08:21:03.987673 libreflow_extensions_anpo_export_illustrator-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1278 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:21:03.982673 libreflow_extensions_anpo_export_illustrator-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:21:03.984673 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:21:03.985673 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/extensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:21:03.986673 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/extensions/anpo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/extensions/anpo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:21:03.986673 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/extensions/anpo/export_illustrator/
--rw-rw-rw-   0 root         (0) root         (0)     5137 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/extensions/anpo/export_illustrator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-28 08:21:03.987673 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/extensions/anpo/export_illustrator/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:21:03.986673 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow.extensions.anpo.export_illustrator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1323 2024-05-28 08:21:03.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 08:21:03.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 08:21:03.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow.extensions.anpo.export_illustrator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 08:21:03.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow.extensions.anpo.export_illustrator.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-28 08:20:54.000000 libreflow_extensions_anpo_export_illustrator-1.0.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-29 20:39:53.854260 libreflow_extensions_anpo_export_illustrator-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.848260 libreflow_extensions_anpo_export_illustrator-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.851260 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.852259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.852259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/
+-rw-rw-rw-   0 root         (0) root         (0)     5467 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-29 20:39:53.854260 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     9765 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/scripts/layers2png.jsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-05-29 20:39:53.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 20:39:53.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 20:39:53.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 20:39:53.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/versioneer.py
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.1/CHANGELOG.md` & `libreflow_extensions_anpo_export_illustrator-1.0.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.1/PKG-INFO` & `libreflow_extensions_anpo_export_illustrator-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.export-illustrator
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://gitlab.com/lfs.coop/libreflow/
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.1/setup.py` & `libreflow_extensions_anpo_export_illustrator-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow/extensions/anpo/export_illustrator/__init__.py` & `libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,19 @@
         return self.root().project().kitsu_api()
     
     def get_illustrator_path(self):
         _envs = self.root().project().get_current_site().site_environment
         return _envs["ILLUSTRATOR_EXEC_PATH"].value.get() if "ILLUSTRATOR_EXEC_PATH" in _envs.mapped_names() else None
     
     def get_illustrator_script(self):
-        return os.path.join(os.path.dirname(__file__), "scripts", "layers2png.jsx")
+        path = os.path.join(os.path.dirname(__file__), "scripts", "layers2png.jsx")
+        if not os.path.exists(path):
+            print('ERROR : COULD NOT FIND THE ILLUSTRATOR SCRIPT @:')
+            print(path)
+        return path
     
     def create_layers(self, assets):
         ai_files_list = []
         
         #assets = self.assets
         print(assets)
         
@@ -107,15 +111,20 @@
             
         
         os.environ["LIBREFLOW_AI2LAYERS_AILIST"] = ";".join(ai_files_list).replace("\\", "/")
         os.environ["LIBREFLOW_ROOT_FOLDER"] = self.get_project_root_folder().replace("\\", "/")
         if not ai_files_list:
             print("No AI Files to Process in this selection")
         else: 
-            _run = subprocess.run([self.get_illustrator_path(), "/run", self.get_illustrator_script()], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            script_path = self.get_illustrator_script()
+            if not script_path:
+                print("script jsx was not found... stopping action now")
+                return
+            
+            _run = subprocess.run([self.get_illustrator_path(), "/run", script_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             print(_run.stderr)
             print(_run.stdout)
 
     def select_assets(self):
         return self.parent.assets.mapped_items() 
 
     def needs_dialog(self):
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO` & `libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.export-illustrator
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://gitlab.com/lfs.coop/libreflow/
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.1/src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt` & `libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO
 src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt
 src/libreflow.extensions.anpo.export_illustrator.egg-info/dependency_links.txt
 src/libreflow.extensions.anpo.export_illustrator.egg-info/top_level.txt
 src/libreflow/extensions/__init__.py
 src/libreflow/extensions/anpo/__init__.py
 src/libreflow/extensions/anpo/export_illustrator/__init__.py
-src/libreflow/extensions/anpo/export_illustrator/_version.py
+src/libreflow/extensions/anpo/export_illustrator/_version.py
+src/libreflow/extensions/anpo/export_illustrator/scripts/layers2png.jsx
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.1/versioneer.py` & `libreflow_extensions_anpo_export_illustrator-1.0.2/versioneer.py`

 * *Files identical despite different names*

