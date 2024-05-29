# Comparing `tmp/loe_simp_app_fw-1.5.0.tar.gz` & `tmp/loe_simp_app_fw-1.5.1.tar.gz`

## Comparing `loe_simp_app_fw-1.5.0.tar` & `loe_simp_app_fw-1.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/config-example.yaml
--rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/.github/workflows/workflow.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/config-example.yaml
+-rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.5.0/.github/workflows/workflow.yaml` & `loe_simp_app_fw-1.5.1/.github/workflows/workflow.yaml`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 # CLI Parser (Only runs once)
 config_dir = ""
 if not isNotebook():
     # Add CLI
     arguments = ArgumentParser()
 
     parser = ArgumentParser()
-    parser.add_argument("--config", type=str, default="", help="config file overwrites commandline arguments. if not present, a new one will be created")
+    parser.add_argument("--config", type=str, default="", help="config file overwrites command line arguments. if not present, a new one will be created")
     
     try:
         args = parser.parse_args()
     except:
         parser.print_help()
         sys.exit(0)
     config_dir = args.config
@@ -77,15 +77,15 @@
     isCLI = True
 elif not config_dir.startswith("/") and config_dir:
     # Start from current working dir
     config_dir = f"{current_working_dir}/{config_dir}"
     Logger.info(f"Loading config from {config_dir}")
     isCLI = True
 else:
-    Logger.debug("No config information can be inffered from the CLI")
+    Logger.debug("No config information can be inferred from the CLI")
 # print(f"isCLI is {isCLI}")
     
 # -------------------------------
 
 class Config:
     # Following parameters should be set at the top-level environment of the project
     _project_root_path = ""
@@ -99,19 +99,19 @@
 
         Args:
             config_path (str): path to config, should be a yaml file
             project_root_path (str, optional): path to project top level. Defaults to current working directory.
             example_config_path (str, optional): path to config example. Defaults to "".
             respect_CLI (CLI, optional): whether CLI will overwrite the config choice of config_path. Defaults to False.
         """
-        # Senity check
+        # Sanity check
         ## No on-the-fly update of project root path
         if Config._project_root_path and project_root_path and not os.path.samefile(project_root_path, Config._project_root_path):
             Logger.error("One should not change project root path twice.")
-            Logger.error(f"Orignial project root path: {Config._project_root_path}")
+            Logger.error(f"Original project root path: {Config._project_root_path}")
             Logger.error(f"Updated project root path: {project_root_path}")
             raise ProjectRootChanged
 
         ## Check example config file
         if not example_config_path or not os.path.isfile(example_config_path):
             Logger.warning("Example config path not valid")
 
@@ -172,8 +172,9 @@
         
         return config
 
 # -------------------------------
 
 # Init Config if CLI arguments are parsed successfully
 if __name__ != "__main__" and isCLI:
+    Logger.info(f"Receive CLI arguments")
     Config(config_dir)
```

### Comparing `loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,14 @@
     @staticmethod
     def _log_composer(level: LogLevels, msg: str) -> str:
         return f"{datetime.datetime.now()} {level.upper()}: {msg}\n"
         
 
 @atexit.register
 def clean_log_buffer():
-    Logger.error("Uncatched error! Panic! Exit!")
     # Clean up logger buffer when crashing
     Logger._log_file_handle.close()
 
 def logger_showoff() -> None:
     # Demonstrate the logger
     Logger("log")
     print(f"Today is {datetime.date.today()}")
```

### Comparing `loe_simp_app_fw-1.5.0/tests/test_import.py` & `loe_simp_app_fw-1.5.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.0/.gitignore` & `loe_simp_app_fw-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.0/LICENSE` & `loe_simp_app_fw-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.0/README.md` & `loe_simp_app_fw-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.0/pyproject.toml` & `loe_simp_app_fw-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.5.0"
+version = "1.5.1"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.5.0/PKG-INFO` & `loe_simp_app_fw-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.5.0
+Version: 1.5.1
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

