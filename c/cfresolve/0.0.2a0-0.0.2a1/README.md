# Comparing `tmp/cfresolve-0.0.2a0.tar.gz` & `tmp/cfresolve-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfresolve-0.0.2a0.tar", last modified: Wed May 29 15:31:15 2024, max compression
+gzip compressed data, was "cfresolve-0.0.2a1.tar", last modified: Wed May 29 15:43:15 2024, max compression
```

## Comparing `cfresolve-0.0.2a0.tar` & `cfresolve-0.0.2a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.954160 cfresolve-0.0.2a0/
--rw-rw-r--   0 smz       (1000) smz       (1000)       68 2024-05-29 15:22:36.000000 cfresolve-0.0.2a0/.gitignore
--rw-r--r--   0 smz       (1000) smz       (1000)      700 2024-05-29 15:31:15.953160 cfresolve-0.0.2a0/PKG-INFO
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.951160 cfresolve-0.0.2a0/assets/
--rw-rw-r--   0 smz       (1000) smz       (1000)   296778 2024-05-29 08:08:36.000000 cfresolve-0.0.2a0/assets/domains.csv
--rw-rw-r--   0 smz       (1000) smz       (1000)     3268 2024-05-29 15:30:02.000000 cfresolve-0.0.2a0/pyproject.toml
--rw-rw-r--   0 smz       (1000) smz       (1000)       38 2024-05-29 15:31:15.954160 cfresolve-0.0.2a0/setup.cfg
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.951160 cfresolve-0.0.2a0/src/
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.952160 cfresolve-0.0.2a0/src/cfresolve/
--rw-rw-r--   0 smz       (1000) smz       (1000)       49 2024-05-29 14:58:39.000000 cfresolve-0.0.2a0/src/cfresolve/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)       68 2024-05-29 14:58:56.000000 cfresolve-0.0.2a0/src/cfresolve/__main__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      413 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve/_version.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     6034 2024-05-29 15:17:11.000000 cfresolve-0.0.2a0/src/cfresolve/cli.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      296 2024-05-29 10:08:39.000000 cfresolve-0.0.2a0/src/cfresolve/exceptions.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.953160 cfresolve-0.0.2a0/src/cfresolve.egg-info/
--rw-r--r--   0 smz       (1000) smz       (1000)      700 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/PKG-INFO
--rw-rw-r--   0 smz       (1000) smz       (1000)      395 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/SOURCES.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)        1 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/dependency_links.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       44 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/entry_points.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       86 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/requires.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       10 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/top_level.txt
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:43:15.225454 cfresolve-0.0.2a1/
+-rw-rw-r--   0 smz       (1000) smz       (1000)       68 2024-05-29 15:22:36.000000 cfresolve-0.0.2a1/.gitignore
+-rw-r--r--   0 smz       (1000) smz       (1000)      700 2024-05-29 15:43:15.225454 cfresolve-0.0.2a1/PKG-INFO
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:43:15.223454 cfresolve-0.0.2a1/assets/
+-rw-rw-r--   0 smz       (1000) smz       (1000)   296778 2024-05-29 08:08:36.000000 cfresolve-0.0.2a1/assets/domains.csv
+-rw-rw-r--   0 smz       (1000) smz       (1000)     3268 2024-05-29 15:39:10.000000 cfresolve-0.0.2a1/pyproject.toml
+-rw-rw-r--   0 smz       (1000) smz       (1000)       38 2024-05-29 15:43:15.225454 cfresolve-0.0.2a1/setup.cfg
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:43:15.223454 cfresolve-0.0.2a1/src/
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:43:15.224454 cfresolve-0.0.2a1/src/cfresolve/
+-rw-rw-r--   0 smz       (1000) smz       (1000)       49 2024-05-29 14:58:39.000000 cfresolve-0.0.2a1/src/cfresolve/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)       68 2024-05-29 14:58:56.000000 cfresolve-0.0.2a1/src/cfresolve/__main__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      413 2024-05-29 15:43:15.000000 cfresolve-0.0.2a1/src/cfresolve/_version.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     6049 2024-05-29 15:39:12.000000 cfresolve-0.0.2a1/src/cfresolve/cli.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      296 2024-05-29 10:08:39.000000 cfresolve-0.0.2a1/src/cfresolve/exceptions.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:43:15.225454 cfresolve-0.0.2a1/src/cfresolve.egg-info/
+-rw-r--r--   0 smz       (1000) smz       (1000)      700 2024-05-29 15:43:15.000000 cfresolve-0.0.2a1/src/cfresolve.egg-info/PKG-INFO
+-rw-rw-r--   0 smz       (1000) smz       (1000)      395 2024-05-29 15:43:15.000000 cfresolve-0.0.2a1/src/cfresolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)        1 2024-05-29 15:43:15.000000 cfresolve-0.0.2a1/src/cfresolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       44 2024-05-29 15:43:15.000000 cfresolve-0.0.2a1/src/cfresolve.egg-info/entry_points.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       86 2024-05-29 15:43:15.000000 cfresolve-0.0.2a1/src/cfresolve.egg-info/requires.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       10 2024-05-29 15:43:15.000000 cfresolve-0.0.2a1/src/cfresolve.egg-info/top_level.txt
```

### Comparing `cfresolve-0.0.2a0/PKG-INFO` & `cfresolve-0.0.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfresolve
-Version: 0.0.2a0
+Version: 0.0.2a1
 Summary: Pings domains that use cloudflare to retrieve edge ips
 Author-email: tempookian <tempookian@gmail.com>
 Project-URL: Homepage, https://github.com/tempookian/cfresolve/
 Project-URL: Bug Tracker, https://github.com/tempookian/cfresolve/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `cfresolve-0.0.2a0/assets/domains.csv` & `cfresolve-0.0.2a1/assets/domains.csv`

 * *Files identical despite different names*

### Comparing `cfresolve-0.0.2a0/pyproject.toml` & `cfresolve-0.0.2a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [project.scripts]
 cfresolve = "cfresolve:app"
 
 [tool.setuptools_scm]
 version_file = "src/cfresolve/_version.py"
 
 [tool.ruff]
-target-version = "py312"
+target-version = "py310"
 line-length = 88
 output-format = "grouped"
 show-fixes = true
 extend-exclude = ["*venv*/", "*.bak.*", "temp.py"]
 src = ["src", "tests"]
 
 [tool.ruff.format]
```

### Comparing `cfresolve-0.0.2a0/src/cfresolve/cli.py` & `cfresolve-0.0.2a1/src/cfresolve/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     def csv_row(self) -> tuple[str]:
         if self.result == ResolveResultType.OK:
             return (self.domain, str(self.ip), "")
         return (self.domain, "FAIL", self.result.value)
 
 
 console = Console()
-dt_str = datetime.datetime.now(tz=datetime.UTC).strftime(r"%Y%m%d_%H%M%S")
+dt_str = datetime.datetime.now(tz=datetime.timezone.utc).strftime(
+    r"%Y%m%d_%H%M%S"
+)
 
 
 class TabularProgress(Progress):
     def __init__(  # noqa: PLR0913
         self,
         *columns: str | ProgressColumn,
         table_max_rows: int,
```

### Comparing `cfresolve-0.0.2a0/src/cfresolve.egg-info/PKG-INFO` & `cfresolve-0.0.2a1/src/cfresolve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfresolve
-Version: 0.0.2a0
+Version: 0.0.2a1
 Summary: Pings domains that use cloudflare to retrieve edge ips
 Author-email: tempookian <tempookian@gmail.com>
 Project-URL: Homepage, https://github.com/tempookian/cfresolve/
 Project-URL: Bug Tracker, https://github.com/tempookian/cfresolve/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

