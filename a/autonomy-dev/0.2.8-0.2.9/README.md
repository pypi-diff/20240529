# Comparing `tmp/autonomy_dev-0.2.8.tar.gz` & `tmp/autonomy_dev-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.2.8.tar", max compression
+gzip compressed data, was "autonomy_dev-0.2.9.tar", max compression
```

## Comparing `autonomy_dev-0.2.8.tar` & `autonomy_dev-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0      578 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/LICENSE
--rw-r--r--   0        0        0      967 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/README.md
--rw-r--r--   0        0        0        0 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/__init__.py
--rw-r--r--   0        0        0     2716 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/base.py
--rw-r--r--   0        0        0      242 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/cli.py
--rw-r--r--   0        0        0     2758 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/cli_executor.py
--rw-r--r--   0        0        0     3456 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/augment.py
--rw-r--r--   0        0        0     5823 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/deps.py
--rw-r--r--   0        0        0     1890 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/fmt.py
--rw-r--r--   0        0        0     1372 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/fsm.py
--rw-r--r--   0        0        0     2144 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/lint.py
--rw-r--r--   0        0        0     3538 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/release.py
--rw-r--r--   0        0        0     5195 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/repo.py
--rw-r--r--   0        0        0     3525 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/scaffold.py
--rw-r--r--   0        0        0     1450 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/commands/test.py
--rw-r--r--   0        0        0      515 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/constants.py
--rw-r--r--   0        0        0     1482 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/block_explorer.py
--rw-r--r--   0        0        0     5786 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/contract.py
--rw-r--r--   0        0        0     2914 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/contract_functions.py
--rw-r--r--   0        0        0     2238 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/contract_scafolder.py
--rw-r--r--   0        0        0     6102 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/contract_templates.py
--rw-r--r--   0        0        0     1788 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/function.py
--rw-r--r--   0        0        0      791 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/param_type.py
--rw-r--r--   0        0        0     1811 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/utils.py
--rw-r--r--   0        0        0     1636 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/contracts/variable.py
--rw-r--r--   0        0        0     1158 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/data/contracts/header.py
--rw-r--r--   0        0        0      173 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/data/mermaid.py
--rw-r--r--   0        0        0      636 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      532 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/data/repo/templates/python/readme.py
--rw-r--r--   0        0        0     2550 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/fmt.py
--rw-r--r--   0        0        0     3090 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/fsm/chain.py
--rw-r--r--   0        0        0     8257 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/fsm/fsm.py
--rw-r--r--   0        0        0      464 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/lint.py
--rw-r--r--   0        0        0     2153 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/local_fork.py
--rw-r--r--   0        0        0      470 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/test.py
--rw-r--r--   0        0        0     2542 2023-08-26 18:40:03.729771 autonomy_dev-0.2.8/auto_dev/utils.py
--rw-r--r--   0        0        0     2671 2023-08-26 18:40:03.733772 autonomy_dev-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      296 2023-08-26 18:40:03.733772 autonomy_dev-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     1634 2023-08-26 18:40:03.733772 autonomy_dev-0.2.8/tests/test_augmenter.py
--rw-r--r--   0        0        0     1084 2023-08-26 18:40:03.733772 autonomy_dev-0.2.8/tests/test_cli.py
--rw-r--r--   0        0        0     2459 2023-08-26 18:40:03.733772 autonomy_dev-0.2.8/tests/test_contracts.py
--rw-r--r--   0        0        0     5241 2023-08-26 18:40:03.733772 autonomy_dev-0.2.8/tests/test_fsm.py
--rw-r--r--   0        0        0     1562 2023-08-26 18:40:03.733772 autonomy_dev-0.2.8/tests/test_local_fork.py
--rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 autonomy_dev-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/LICENSE
+-rw-r--r--   0        0        0      967 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/__init__.py
+-rw-r--r--   0        0        0     2716 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/base.py
+-rw-r--r--   0        0        0      242 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/cli.py
+-rw-r--r--   0        0        0     2758 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0     3456 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/augment.py
+-rw-r--r--   0        0        0     5823 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/deps.py
+-rw-r--r--   0        0        0     1890 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/fmt.py
+-rw-r--r--   0        0        0     1372 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/fsm.py
+-rw-r--r--   0        0        0     2144 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/lint.py
+-rw-r--r--   0        0        0    11560 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/metadata.py
+-rw-r--r--   0        0        0     3538 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/release.py
+-rw-r--r--   0        0        0     5195 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/repo.py
+-rw-r--r--   0        0        0     3525 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/scaffold.py
+-rw-r--r--   0        0        0     1450 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/commands/test.py
+-rw-r--r--   0        0        0      515 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/constants.py
+-rw-r--r--   0        0        0     1482 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/block_explorer.py
+-rw-r--r--   0        0        0     5786 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/contract.py
+-rw-r--r--   0        0        0     2914 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/contract_functions.py
+-rw-r--r--   0        0        0     2238 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/contract_scafolder.py
+-rw-r--r--   0        0        0     6102 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/contract_templates.py
+-rw-r--r--   0        0        0     1788 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/function.py
+-rw-r--r--   0        0        0      791 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/param_type.py
+-rw-r--r--   0        0        0     1811 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/utils.py
+-rw-r--r--   0        0        0     1636 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/contracts/variable.py
+-rw-r--r--   0        0        0     1158 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/data/contracts/header.py
+-rw-r--r--   0        0        0     1693 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/data/mapping.txt
+-rw-r--r--   0        0        0      173 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/data/mermaid.py
+-rw-r--r--   0        0        0      637 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      532 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/data/repo/templates/python/readme.py
+-rw-r--r--   0        0        0     2550 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/fmt.py
+-rw-r--r--   0        0        0     3090 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/fsm/chain.py
+-rw-r--r--   0        0        0     8257 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/fsm/fsm.py
+-rw-r--r--   0        0        0      464 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/lint.py
+-rw-r--r--   0        0        0     2153 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/local_fork.py
+-rw-r--r--   0        0        0      470 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/test.py
+-rw-r--r--   0        0        0     2542 2023-09-04 10:03:38.946632 autonomy_dev-0.2.9/auto_dev/utils.py
+-rw-r--r--   0        0        0     2671 2023-09-04 10:03:38.950632 autonomy_dev-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      296 2023-09-04 10:03:38.950632 autonomy_dev-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     1634 2023-09-04 10:03:38.950632 autonomy_dev-0.2.9/tests/test_augmenter.py
+-rw-r--r--   0        0        0     1084 2023-09-04 10:03:38.950632 autonomy_dev-0.2.9/tests/test_cli.py
+-rw-r--r--   0        0        0     2459 2023-09-04 10:03:38.950632 autonomy_dev-0.2.9/tests/test_contracts.py
+-rw-r--r--   0        0        0     5241 2023-09-04 10:03:38.950632 autonomy_dev-0.2.9/tests/test_fsm.py
+-rw-r--r--   0        0        0     1562 2023-09-04 10:03:38.950632 autonomy_dev-0.2.9/tests/test_local_fork.py
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 autonomy_dev-0.2.9/PKG-INFO
```

### Comparing `autonomy_dev-0.2.8/LICENSE` & `autonomy_dev-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/README.md` & `autonomy_dev-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/base.py` & `autonomy_dev-0.2.9/auto_dev/base.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/cli_executor.py` & `autonomy_dev-0.2.9/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/augment.py` & `autonomy_dev-0.2.9/auto_dev/commands/augment.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/deps.py` & `autonomy_dev-0.2.9/auto_dev/commands/deps.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/fmt.py` & `autonomy_dev-0.2.9/auto_dev/commands/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/fsm.py` & `autonomy_dev-0.2.9/auto_dev/commands/fsm.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/lint.py` & `autonomy_dev-0.2.9/auto_dev/commands/lint.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/release.py` & `autonomy_dev-0.2.9/auto_dev/commands/release.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/repo.py` & `autonomy_dev-0.2.9/auto_dev/commands/repo.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/scaffold.py` & `autonomy_dev-0.2.9/auto_dev/commands/scaffold.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/commands/test.py` & `autonomy_dev-0.2.9/auto_dev/commands/test.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/constants.py` & `autonomy_dev-0.2.9/auto_dev/constants.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/block_explorer.py` & `autonomy_dev-0.2.9/auto_dev/contracts/block_explorer.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/contract.py` & `autonomy_dev-0.2.9/auto_dev/contracts/contract.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/contract_functions.py` & `autonomy_dev-0.2.9/auto_dev/contracts/contract_functions.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/contract_scafolder.py` & `autonomy_dev-0.2.9/auto_dev/contracts/contract_scafolder.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/contract_templates.py` & `autonomy_dev-0.2.9/auto_dev/contracts/contract_templates.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/function.py` & `autonomy_dev-0.2.9/auto_dev/contracts/function.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/param_type.py` & `autonomy_dev-0.2.9/auto_dev/contracts/param_type.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/utils.py` & `autonomy_dev-0.2.9/auto_dev/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/contracts/variable.py` & `autonomy_dev-0.2.9/auto_dev/contracts/variable.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/data/contracts/header.py` & `autonomy_dev-0.2.9/auto_dev/data/contracts/header.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/data/pylama.ini` & `autonomy_dev-0.2.9/auto_dev/data/pylama.ini`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 min-confidence = 90
 
 [pylama:mypy]
 ignore_missing_imports = True
 strict = False
 
 [pylama:radon]
-complexity = 18
+complexity = 25
```

### Comparing `autonomy_dev-0.2.8/auto_dev/data/repo/templates/python/readme.py` & `autonomy_dev-0.2.9/auto_dev/data/repo/templates/python/readme.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/fmt.py` & `autonomy_dev-0.2.9/auto_dev/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/fsm/chain.py` & `autonomy_dev-0.2.9/auto_dev/fsm/chain.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/fsm/fsm.py` & `autonomy_dev-0.2.9/auto_dev/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/local_fork.py` & `autonomy_dev-0.2.9/auto_dev/local_fork.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/auto_dev/utils.py` & `autonomy_dev-0.2.9/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/pyproject.toml` & `autonomy_dev-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.2.8"
+version = "0.2.9"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `autonomy_dev-0.2.8/tests/test_augmenter.py` & `autonomy_dev-0.2.9/tests/test_augmenter.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/tests/test_cli.py` & `autonomy_dev-0.2.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/tests/test_contracts.py` & `autonomy_dev-0.2.9/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/tests/test_fsm.py` & `autonomy_dev-0.2.9/tests/test_fsm.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/tests/test_local_fork.py` & `autonomy_dev-0.2.9/tests/test_local_fork.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.8/PKG-INFO` & `autonomy_dev-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomy_dev
-Version: 0.2.8
+Version: 0.2.9
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.7.2,<=3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

