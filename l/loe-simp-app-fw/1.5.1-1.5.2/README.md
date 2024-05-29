# Comparing `tmp/loe_simp_app_fw-1.5.1.tar.gz` & `tmp/loe_simp_app_fw-1.5.2.tar.gz`

## Comparing `loe_simp_app_fw-1.5.1.tar` & `loe_simp_app_fw-1.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/config-example.yaml
--rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/.github/workflows/workflow.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/config-example.yaml
+-rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.2/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.5.1/.github/workflows/workflow.yaml` & `loe_simp_app_fw-1.5.2/.github/workflows/workflow.yaml`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.5.2/src/loe_simp_app_fw/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,12 +169,13 @@
             with open(abs_example_config_path, "r", encoding="utf-8") as f:
                 config = yaml.safe_load(f)
             Logger.debug(f"Config: {json.dumps(config, indent=2)}")
         
         return config
 
 # -------------------------------
+Logger.debug(f"isCLI is set to {isCLI}")
 
 # Init Config if CLI arguments are parsed successfully
 if __name__ != "__main__" and isCLI:
     Logger.info(f"Receive CLI arguments")
     Config(config_dir)
```

### Comparing `loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.5.2/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.1/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.5.2/src/loe_simp_app_fw/logger.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.1/tests/test_import.py` & `loe_simp_app_fw-1.5.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.1/.gitignore` & `loe_simp_app_fw-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.1/LICENSE` & `loe_simp_app_fw-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.1/README.md` & `loe_simp_app_fw-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.5.1/pyproject.toml` & `loe_simp_app_fw-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.5.1/PKG-INFO` & `loe_simp_app_fw-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.5.1
+Version: 1.5.2
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

