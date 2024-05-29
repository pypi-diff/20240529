# Comparing `tmp/sdss_yao-1.3.1.tar.gz` & `tmp/sdss_yao-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_yao-1.3.1.tar", max compression
+gzip compressed data, was "sdss_yao-1.3.2.tar", max compression
```

## Comparing `sdss_yao-1.3.1.tar` & `sdss_yao-1.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1504 2024-02-27 18:45:04.938167 sdss_yao-1.3.1/LICENSE.md
--rw-r--r--   0        0        0      386 2024-02-27 18:45:04.938167 sdss_yao-1.3.1/README.md
--rw-r--r--   0        0        0     2407 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      450 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/__init__.py
--rw-r--r--   0        0        0     1410 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/__main__.py
--rw-r--r--   0        0        0     4797 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/actor.py
--rw-r--r--   0        0        0     7106 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/alerts.py
--rw-r--r--   0        0        0     4893 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/commands.py
--rw-r--r--   0        0        0     3831 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/controller.py
--rw-r--r--   0        0        0    19491 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/delegate.py
--rw-r--r--   0        0        0    32902 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/BOSS_extra.acf
--rw-r--r--   0        0        0    49124 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v2.acf
--rw-r--r--   0        0        0    49106 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v3.acf
--rw-r--r--   0        0        0    55310 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v4.acf
--rw-r--r--   0        0        0    57565 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v5.acf
--rw-r--r--   0        0        0    55553 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v6.acf
--rw-r--r--   0        0        0    55599 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v8.acf
--rw-r--r--   0        0        0     1258 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/README.md
--rw-r--r--   0        0        0     2649 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/schema.json
--rw-r--r--   0        0        0     2155 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/etc/yao.yml
--rw-r--r--   0        0        0     1062 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/exceptions.py
--rw-r--r--   0        0        0    15564 2024-02-27 18:45:04.942167 sdss_yao-1.3.1/yao/mech_commands.py
--rw-r--r--   0        0        0    19662 2024-02-27 18:45:04.946167 sdss_yao-1.3.1/yao/mech_controller.py
--rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 sdss_yao-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-29 17:33:11.128754 sdss_yao-1.3.2/LICENSE.md
+-rw-r--r--   0        0        0      386 2024-05-29 17:33:11.128754 sdss_yao-1.3.2/README.md
+-rw-r--r--   0        0        0     2440 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      450 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/__init__.py
+-rw-r--r--   0        0        0     1410 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/__main__.py
+-rw-r--r--   0        0        0     4797 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/actor.py
+-rw-r--r--   0        0        0     7106 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/alerts.py
+-rw-r--r--   0        0        0     4893 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/commands.py
+-rw-r--r--   0        0        0     3831 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/controller.py
+-rw-r--r--   0        0        0    19491 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/delegate.py
+-rw-r--r--   0        0        0    32902 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/etc/BOSS_extra.acf
+-rw-r--r--   0        0        0    49124 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v2.acf
+-rw-r--r--   0        0        0    49106 2024-05-29 17:33:11.132754 sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v3.acf
+-rw-r--r--   0        0        0    55310 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v4.acf
+-rw-r--r--   0        0        0    57565 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v5.acf
+-rw-r--r--   0        0        0    55553 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v6.acf
+-rw-r--r--   0        0        0    55599 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v8.acf
+-rw-r--r--   0        0        0     1258 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/etc/README.md
+-rw-r--r--   0        0        0     2649 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/etc/schema.json
+-rw-r--r--   0        0        0     2155 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/etc/yao.yml
+-rw-r--r--   0        0        0     1062 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/exceptions.py
+-rw-r--r--   0        0        0    15564 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/mech_commands.py
+-rw-r--r--   0        0        0    19662 2024-05-29 17:33:11.136754 sdss_yao-1.3.2/yao/mech_controller.py
+-rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 sdss_yao-1.3.2/PKG-INFO
```

### Comparing `sdss_yao-1.3.1/LICENSE.md` & `sdss_yao-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/pyproject.toml` & `sdss_yao-1.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-yao"
-version = "1.3.1"
+version = "1.3.2"
 description = "BOSS spectrograph actor that uses an STA Archon controller"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Aidan Gray <aidan.gray@idg.jhu.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/yao"
 repository = "https://github.com/sdss/yao"
 documentation = "https://sdss-yao.readthedocs.org"
@@ -25,15 +25,15 @@
 include = ["yao/etc/*"]
 
 [tool.poetry.scripts]
 yao = "yao.__main__:yao"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
-sdss-archon = "^0.13.2"
+sdss-archon = "^0.13.5"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=8.0.0"
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.10.0"
 pytest-cov = ">=2.8.1"
 pytest-mock = ">=1.13.0"
@@ -55,26 +55,28 @@
 line-length = 88
 target-version = ['py312']
 fast = true
 
 [tool.ruff]
 line-length = 88
 target-version = 'py312'
+
+[tool.ruff.lint]
 select = ["E", "F", "I"]
 unfixable = ["F841"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F403", "E402", "F401"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["yao"]
 lines-after-imports = 2
 section-order = ["future", "standard-library", "typing", "third-party", "sdss", "first-party", "local-folder"]
 
-[tool.ruff.isort.sections]
+[tool.ruff.lint.isort.sections]
 typing = ["typing"]
 sdss = ["sdsstools", "archon"]
 
 [tool.pytest.ini_options]
 addopts = "--cov yao --cov-report xml --cov-report html --cov-report term"
 
 [tool.coverage.run]
```

### Comparing `sdss_yao-1.3.1/yao/__main__.py` & `sdss_yao-1.3.2/yao/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/actor.py` & `sdss_yao-1.3.2/yao/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/alerts.py` & `sdss_yao-1.3.2/yao/alerts.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/commands.py` & `sdss_yao-1.3.2/yao/commands.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/controller.py` & `sdss_yao-1.3.2/yao/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/delegate.py` & `sdss_yao-1.3.2/yao/delegate.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/BOSS_extra.acf` & `sdss_yao-1.3.2/yao/etc/BOSS_extra.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v2.acf` & `sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v2.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v3.acf` & `sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v3.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v4.acf` & `sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v4.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v5.acf` & `sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v5.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v6.acf` & `sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v6.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/BOSS_extra_purge_erase_v8.acf` & `sdss_yao-1.3.2/yao/etc/BOSS_extra_purge_erase_v8.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/README.md` & `sdss_yao-1.3.2/yao/etc/README.md`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/schema.json` & `sdss_yao-1.3.2/yao/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/etc/yao.yml` & `sdss_yao-1.3.2/yao/etc/yao.yml`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/exceptions.py` & `sdss_yao-1.3.2/yao/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/mech_commands.py` & `sdss_yao-1.3.2/yao/mech_commands.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/yao/mech_controller.py` & `sdss_yao-1.3.2/yao/mech_controller.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.3.1/PKG-INFO` & `sdss_yao-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-yao
-Version: 1.3.1
+Version: 1.3.2
 Summary: BOSS spectrograph actor that uses an STA Archon controller
 Home-page: https://github.com/sdss/yao
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<3.13
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: sdss-archon (>=0.13.2,<0.14.0)
+Requires-Dist: sdss-archon (>=0.13.5,<0.14.0)
 Project-URL: Documentation, https://sdss-yao.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/yao
 Description-Content-Type: text/markdown
 
 # yao
 
 ![Versions](https://img.shields.io/badge/python->3.9-blue)
```

