# Comparing `tmp/pytest_ditto-0.0.3.tar.gz` & `tmp/pytest_ditto-0.1.0.tar.gz`

## Comparing `pytest_ditto-0.0.3.tar` & `pytest_ditto-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/_unittest.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/_version.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/exceptions.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/plugin.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/snapshot.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_json.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_pandas_parquet.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_pickle.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_protocol.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_yaml.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/LICENSE
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/README.md
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/_unittest.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/_version.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/exceptions.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/marks.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/plugin.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/snapshot.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/io/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/io/_json.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/io/_pickle.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/io/_plugins.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/io/_protocol.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/ditto/io/_yaml.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/README.md
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 pytest_ditto-0.1.0/PKG-INFO
```

### Comparing `pytest_ditto-0.0.3/ditto/_unittest.py` & `pytest_ditto-0.1.0/ditto/_unittest.py`

 * *Files identical despite different names*

### Comparing `pytest_ditto-0.0.3/ditto/plugin.py` & `pytest_ditto-0.1.0/ditto/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_ditto-0.0.3/ditto/snapshot.py` & `pytest_ditto-0.1.0/ditto/snapshot.py`

 * *Files identical despite different names*

### Comparing `pytest_ditto-0.0.3/LICENSE` & `pytest_ditto-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_ditto-0.0.3/pyproject.toml` & `pytest_ditto-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,43 +23,48 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pytest>=3.5.0",
     "pyyaml",
-    "pandas",
-    "pyarrow",
 ]
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "hatch>=1.9.4",
     "hatch-vcs>=0.4.0",
 ]
 
 [project.entry-points.pytest11]
 recording = "ditto.plugin"
 
+[project.entry-points.ditto]
+pickle = "ditto.io._pickle:Pickle"
+yaml = "ditto.io._yaml:Yaml"
+json = "ditto.io._json:Json"
+
+[project.entry-points.ditto_marks]
+# placeholder for ditto IO plugins to use to register marks.
+
 
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 
 [tool.hatch.build]
-hooks.vcs.version-file = "ditto/_version.py"
+hooks.vcs.version-file = "src/ditto/_version.py"
 hooks.vcs.template = "__version__ = {version!r}"
-targets.wheel.packages = ["ditto"]
+targets.wheel.packages = ["src/ditto"]
 targets.wheel.strict-naming = false
-targets.sdist.packages = ["ditto"]
+targets.sdist.packages = ["src/ditto"]
 targets.sdist.strict-naming = false
 
 [tool.hatch.version]
-#source = "vcs"
 source = "code"
 path = "version_builder.py"
 expression = "_version()"
 
 
 [tool.hatch.envs.default]
 python = "3.10"
@@ -106,15 +111,15 @@
     | dist
   )/
 )
 '''
 
 [tool.coverage.run]
 branch = true
-source = ["ditto"]
+source = ["src/ditto"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 80
 
 [tool.ruff]
 line-length = 88  # same as Black.
```

