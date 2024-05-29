# Comparing `tmp/eth_gtd_cli-0.0.98.tar.gz` & `tmp/eth_gtd_cli-0.0.99.tar.gz`

## Comparing `eth_gtd_cli-0.0.98.tar` & `eth_gtd_cli-0.0.99.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/deploy.sh
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/pyproject.toml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/deploy.sh
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.99/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.98/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.99/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.98/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.99/src/ETH_GTD_cli/main.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.98/LICENSE` & `eth_gtd_cli-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.98/pyproject.toml` & `eth_gtd_cli-0.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.98"
+version = "0.0.99"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.98/PKG-INFO` & `eth_gtd_cli-0.0.99/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.98
+Version: 0.0.99
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

