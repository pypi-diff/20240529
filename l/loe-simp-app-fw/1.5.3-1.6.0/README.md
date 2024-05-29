# Comparing `tmp/loe_simp_app_fw-1.5.3.tar.gz` & `tmp/loe_simp_app_fw-1.6.0.tar.gz`

## Comparing `loe_simp_app_fw-1.5.3.tar` & `loe_simp_app_fw-1.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/config-example.yaml
--rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/.github/workflows/workflow.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/config-example.yaml
+-rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.6.0/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.5.3/.github/workflows/workflow.yaml` & `loe_simp_app_fw-1.6.0/.github/workflows/workflow.yaml`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.3/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.6.0/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.3/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.6.0/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.3/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.6.0/src/loe_simp_app_fw/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     @classmethod
     def _create_log_file(cls):
         if not os.path.isfile(cls._log_location()) and not os.path.isdir(cls._log_location()):
             with open(cls._log_location(), "w", encoding="utf-8") as f:
                 print("Create log file successfully.")
 
-    def __init__(self, log_folder_path: str, project_root_path: str = os.getcwd(), log_level: LogLevels = "INFO"):
+    def __init__(self, log_folder_path: str, project_root_path: str = os.getcwd(), log_level: LogLevels = "INFO", buffering: int = 1024):
         """Init Logger
 
         Args:
             log_folder_path (str): path to log folder relative to project root path
             project_root_path (str, optional): path to project top-level directory. Defaults to os.getcwd().
                                                 The parent folder of that would be os.path.dirname(os.path.realpath(__file__)).
 
@@ -63,15 +63,15 @@
         # Create log folder
         folder_name = os.path.join(self._project_root_path, self._log_folder_path)
         if not os.path.isfile(folder_name) and not os.path.isdir(folder_name):
             create_folder_if_not_exists(folder_name)
 
         # Create file IO handle
         self._log_file_handle.close()
-        type(self)._log_file_handle = open(self._log_location(), "a", encoding="utf-8", buffering=0)
+        type(self)._log_file_handle = open(self._log_location(), "a", encoding="utf-8", buffering=buffering)
 
         # Save previous logs
         self._log_file_handle.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
         for entry in self._log_buffer:
             composed_log_entry = self._log_composer(*entry)
             print(composed_log_entry)
             self._log_file_handle.writelines(composed_log_entry)
```

### Comparing `loe_simp_app_fw-1.5.3/tests/test_import.py` & `loe_simp_app_fw-1.6.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.3/.gitignore` & `loe_simp_app_fw-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.3/LICENSE` & `loe_simp_app_fw-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.3/README.md` & `loe_simp_app_fw-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.3/pyproject.toml` & `loe_simp_app_fw-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.5.3"
+version = "1.6.0"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.5.3/PKG-INFO` & `loe_simp_app_fw-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.5.3
+Version: 1.6.0
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

