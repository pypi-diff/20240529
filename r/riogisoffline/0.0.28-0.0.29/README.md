# Comparing `tmp/riogisoffline-0.0.28.tar.gz` & `tmp/riogisoffline-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riogisoffline-0.0.28.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riogisoffline-0.0.29.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riogisoffline-0.0.28.tar` & `riogisoffline-0.0.29.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      717 2024-05-28 08:14:16.832396 riogisoffline-0.0.28/pyproject.toml
--rw-r--r--   0        0        0     1071 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/LICENSE
--rw-r--r--   0        0        0     7264 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/Makefile
--rw-r--r--   0        0        0      261 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/README.md
--rw-r--r--   0        0        0     2239 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/__init__.py
--rw-r--r--   0        0        0      158 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/compile.bat
--rw-r--r--   0        0        0     2810 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/dialog/riogis_dialog_settings.ui
--rw-r--r--   0        0        0     6143 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/dialog/riogis_dockwidget.ui
--rw-r--r--   0        0        0    30219 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/icon.png
--rw-r--r--   0        0        0     1505 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/metadata.txt
--rw-r--r--   0        0        0     1723 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/pb_tool.cfg
--rw-r--r--   0        0        0      195 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/__init__.py
--rw-r--r--   0        0        0     1283 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/azure_blob_storage_connection.py
--rw-r--r--   0        0        0      424 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/dependency_installer.py
--rw-r--r--   0        0        0    17046 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/refresh_map.py
--rw-r--r--   0        0        0   126345 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/resources.py
--rw-r--r--   0        0        0    14047 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/riogis.py
--rw-r--r--   0        0        0     1313 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/riogis_dockedwidget.py
--rw-r--r--   0        0        0     1310 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/settings_dialog.py
--rw-r--r--   0        0        0     7700 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/syncronizer.py
--rw-r--r--   0        0        0     2436 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/user_settings_generator.py
--rw-r--r--   0        0        0     2635 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/utils.py
--rw-r--r--   0        0        0      947 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/worker.py
--rw-r--r--   0        0        0     3559 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin_upload.py
--rw-r--r--   0        0        0     8798 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/pylintrc
--rw-r--r--   0        0        0       18 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/requirements.txt
--rw-r--r--   0        0        0      102 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/resources.qrc
--rw-r--r--   0        0        0     2740 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/settings.json
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 riogisoffline-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0      717 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/pyproject.toml
+-rw-r--r--   0        0        0     1071 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/LICENSE
+-rw-r--r--   0        0        0     7264 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/Makefile
+-rw-r--r--   0        0        0      261 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/README.md
+-rw-r--r--   0        0        0     2239 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/compile.bat
+-rw-r--r--   0        0        0     2810 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/dialog/riogis_dialog_settings.ui
+-rw-r--r--   0        0        0     6143 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/dialog/riogis_dockwidget.ui
+-rw-r--r--   0        0        0    30219 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/icon.png
+-rw-r--r--   0        0        0     1505 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/metadata.txt
+-rw-r--r--   0        0        0     1723 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/pb_tool.cfg
+-rw-r--r--   0        0        0      195 2024-05-29 12:37:52.889579 riogisoffline-0.0.29/riogisoffline/plugin/__init__.py
+-rw-r--r--   0        0        0     1283 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/azure_blob_storage_connection.py
+-rw-r--r--   0        0        0      424 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/dependency_installer.py
+-rw-r--r--   0        0        0    17046 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/refresh_map.py
+-rw-r--r--   0        0        0   126345 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/resources.py
+-rw-r--r--   0        0        0    14702 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/riogis.py
+-rw-r--r--   0        0        0     1313 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/riogis_dockedwidget.py
+-rw-r--r--   0        0        0     1310 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/settings_dialog.py
+-rw-r--r--   0        0        0     7700 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/syncronizer.py
+-rw-r--r--   0        0        0     2436 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/user_settings_generator.py
+-rw-r--r--   0        0        0     2635 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/utils.py
+-rw-r--r--   0        0        0      947 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin/worker.py
+-rw-r--r--   0        0        0     3559 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/plugin_upload.py
+-rw-r--r--   0        0        0     8798 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/pylintrc
+-rw-r--r--   0        0        0       18 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/requirements.txt
+-rw-r--r--   0        0        0      102 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/resources.qrc
+-rw-r--r--   0        0        0     2740 2024-05-29 12:37:52.893579 riogisoffline-0.0.29/riogisoffline/settings.json
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 riogisoffline-0.0.29/PKG-INFO
```

### Comparing `riogisoffline-0.0.28/pyproject.toml` & `riogisoffline-0.0.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "riogisoffline"
-version = "0.0.28"
+version = "0.0.29"
 description = "This Exports attributes of a given feature to a Wincan consumable text file."
 authors = [
   { name = "Vann- og avløpsetaten Oslo kommune", email = "gis@vav.oslo.kommune.no" },
 ]
 license = { file = "riogisoffline/LICENSE" }
 readme = "riogisoffline/README.md"
 classifiers = [
```

### Comparing `riogisoffline-0.0.28/riogisoffline/LICENSE` & `riogisoffline-0.0.29/riogisoffline/LICENSE`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/Makefile` & `riogisoffline-0.0.29/riogisoffline/Makefile`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/__init__.py` & `riogisoffline-0.0.29/riogisoffline/__init__.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/dialog/riogis_dialog_settings.ui` & `riogisoffline-0.0.29/riogisoffline/dialog/riogis_dialog_settings.ui`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/dialog/riogis_dockwidget.ui` & `riogisoffline-0.0.29/riogisoffline/dialog/riogis_dockwidget.ui`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/icon.png` & `riogisoffline-0.0.29/riogisoffline/icon.png`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/metadata.txt` & `riogisoffline-0.0.29/riogisoffline/metadata.txt`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/pb_tool.cfg` & `riogisoffline-0.0.29/riogisoffline/pb_tool.cfg`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/azure_blob_storage_connection.py` & `riogisoffline-0.0.29/riogisoffline/plugin/azure_blob_storage_connection.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/refresh_map.py` & `riogisoffline-0.0.29/riogisoffline/plugin/refresh_map.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/resources.py` & `riogisoffline-0.0.29/riogisoffline/plugin/resources.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/riogis.py` & `riogisoffline-0.0.29/riogisoffline/plugin/riogis.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,31 @@
         def _handle_settings_button_click():
             selectFileDialog.exec_()
             self.dlg.refresh_dialog()
             self.setup_user_settings()
         
         self.dlg.btnSelectSettingsFile.clicked.connect(_handle_settings_button_click)
 
+        self.show_necessary_panels()
+
+    def show_necessary_panels(self):
+        from qgis.PyQt.QtWidgets import QDockWidget, QToolBar
+        
+        needed_panels = ['Layers', 'mPluginToolBar', 'mAttributesToolBar', 'mMapNavToolBar']
+        from qgis.core import Qgis
+        for x in self.iface.mainWindow().findChildren(QDockWidget) + self.iface.mainWindow().findChildren(QToolBar):
+
+            if x.objectName() in ["MessageLog", "RioGIS2"]:
+                continue
+
+            if x.objectName() in needed_panels:
+                x.setVisible(True)
+            else:
+                x.setVisible(False)
+
     def _handle_export(self):
         if self.map_has_been_clicked:
             self.iface.mapCanvas().unsetMapTool(self.mapTool)
         
         if self.map_has_been_clicked and self.data and self.data.get("PipeID"):
                 self.write_output_file()
                 self.update_feature_status()
@@ -181,15 +198,15 @@
 
         data["operator"] = self.settings["operator"]
         data["orderid"] = ""
         data["workorder"] = ""
         if not data.get('form'):
             data['form'] = ""
 
-        utils.printInfoMessage(f'Ledning valgt: LSID {data["lsid"]} (fra PSID {data["from_psid"]} til {data["to_psid"]}), {data["streetname"]}, {data["fcodegroup"]}')
+        utils.printInfoMessage(f'Ledning valgt: LSID {data["lsid"]} (fra PSID {data["from_psid"]} til {data["to_psid"]}), {data["streetname"]}, {data["fcodegroup"]}', message_duration=5)
 
         old_keys = set(data.keys())
         map_keys = set(self.mapper.keys())
         auto_keys = old_keys.intersection(map_keys)
 
         new_data = {}
         for k in auto_keys:
@@ -219,15 +236,15 @@
 
     def show_selected_feature(self, data):
         if not data:
             text = "Ingen ledning er valgt"
             self.dlg.textLedningValgt.setText(text) 
             return
         
-        text = f"<strong>LSID: {data['lsid']}, Gate: {data['streetname']}</strong>"
+        text = f"LSID: <strong>{data['lsid']}</strong>, Gate: <strong>{data['streetname']}</strong>"
         self.dlg.textLedningValgt.setText(text)
 
     def select_feature(self, point):
         """Select layer and get nearest feature
 
         Args:
             point (point): point
@@ -354,14 +371,15 @@
 
         if self.first_start:
             self.first_start = False
         self.initiate_gui_elements()
 
         self.iface.addDockWidget(Qt.RightDockWidgetArea, self.dlg) 
 
+
     def startSyncWorker(self):
 
         # TODO move out of riogis maybe?
 
         if not os.path.exists(utils.get_user_settings_path()): 
             utils.printWarningMessage("Legg til bruker-innstillinger (bruker_settings.json)!")
             return
@@ -428,8 +446,8 @@
 
     def workerError(self, e, exception_string):
         utils.printCriticalMessage('Worker thread raised an exception:\n{}'.format(exception_string))
 
         self.workerFinished()
 
     def workerWarning(self, msg):
-        utils.printWarningMessage(msg)
+        utils.printWarningMessage(msg)
```

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/riogis_dockedwidget.py` & `riogisoffline-0.0.29/riogisoffline/plugin/riogis_dockedwidget.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/settings_dialog.py` & `riogisoffline-0.0.29/riogisoffline/plugin/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/syncronizer.py` & `riogisoffline-0.0.29/riogisoffline/plugin/syncronizer.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/user_settings_generator.py` & `riogisoffline-0.0.29/riogisoffline/plugin/user_settings_generator.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/utils.py` & `riogisoffline-0.0.29/riogisoffline/plugin/utils.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin/worker.py` & `riogisoffline-0.0.29/riogisoffline/plugin/worker.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/plugin_upload.py` & `riogisoffline-0.0.29/riogisoffline/plugin_upload.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/pylintrc` & `riogisoffline-0.0.29/riogisoffline/pylintrc`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/riogisoffline/settings.json` & `riogisoffline-0.0.29/riogisoffline/settings.json`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.28/PKG-INFO` & `riogisoffline-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riogisoffline
-Version: 0.0.28
+Version: 0.0.29
 Summary: This Exports attributes of a given feature to a Wincan consumable text file.
 Author-email: Vann- og avløpsetaten Oslo kommune <gis@vav.oslo.kommune.no>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

