# Comparing `tmp/pytest_dashboard-0.0.8.tar.gz` & `tmp/pytest_dashboard-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dashboard-0.0.8.tar", max compression
+gzip compressed data, was "pytest_dashboard-0.1.0.tar", max compression
```

## Comparing `pytest_dashboard-0.0.8.tar` & `pytest_dashboard-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1495 2024-04-22 11:08:28.243756 pytest_dashboard-0.0.8/LICENSE
--rw-r--r--   0        0        0     1232 2024-04-22 11:08:28.243756 pytest_dashboard-0.0.8/README.md
--rw-r--r--   0        0        0      775 2024-04-22 11:08:39.659715 pytest_dashboard-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-22 11:08:39.663715 pytest_dashboard-0.0.8/pytest_dashboard/__init__.py
--rw-r--r--   0        0        0     4262 2024-04-22 11:08:28.243756 pytest_dashboard-0.0.8/pytest_dashboard/_tally_progresses.py
--rw-r--r--   0        0        0     2184 2024-04-22 11:08:28.243756 pytest_dashboard-0.0.8/pytest_dashboard/conftest.py
--rw-r--r--   0        0        0      136 2024-04-22 11:08:28.243756 pytest_dashboard-0.0.8/pytest_dashboard/tally.py
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 pytest_dashboard-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1495 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1642 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/README.md
+-rw-r--r--   0        0        0      770 2024-05-29 06:12:47.703161 pytest_dashboard-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-29 06:12:47.703161 pytest_dashboard-0.1.0/pytest_dashboard/__init__.py
+-rw-r--r--   0        0        0     4183 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/pytest_dashboard/_tally_progresses.py
+-rw-r--r--   0        0        0      216 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/pytest_dashboard/config.py
+-rw-r--r--   0        0        0     2184 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/pytest_dashboard/conftest.py
+-rw-r--r--   0        0        0      165 2024-05-29 06:12:34.667029 pytest_dashboard-0.1.0/pytest_dashboard/tally.py
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 pytest_dashboard-0.1.0/PKG-INFO
```

### Comparing `pytest_dashboard-0.0.8/LICENSE` & `pytest_dashboard-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_dashboard-0.0.8/pyproject.toml` & `pytest_dashboard-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "pytest-dashboard"
-version = "0.0.8"  # ignored by versioning plugin
+version = "0.1.0"  # ignored by versioning plugin
 description = ""
 authors = ["kazuma.naito <kazuma.naito@murata.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/pyfemtet/pytest-dashboard"
 
 [tool.poetry.dependencies]
 python = " >= 3.9, < 4.0.0"
-dash = "^2.14.2"
-plotly = "^5.18.0"
-dash-bootstrap-components = "^1.5.0"
 pytest = "^7.4.3"
 pyyaml = "^6.0.1"
 fire = "^0.6.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.plugins]
 pytest11 = { pytest_dashboard_plugin = "pytest_dashboard.conftest" }  # by add this, work without conftest.py.
+
+[tool.poetry.scripts]
+tally-pytest = "pytest_dashboard.tally:main"
```

### Comparing `pytest_dashboard-0.0.8/pytest_dashboard/_tally_progresses.py` & `pytest_dashboard-0.1.0/pytest_dashboard/_tally_progresses.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,21 +126,19 @@
     while not should_stop:
         merge_progress_files(progresses_dir, entire_progress_path, notification)
         sleep(UPDATE_INTERVAL)
 
 
 def monitor_progress(
         progresses_dir:str,
-        entire_progress_path:str or None=None,
+        entire_progress_path:str='./entire-progress.yaml',
         notification:bool=False,
 ):
     global should_stop
 
-    if entire_progress_path is None:
-        entire_progress_path = 'entire-progress.yaml'
     entire_progress_path = os.path.abspath(entire_progress_path)
 
     t = Thread(
         target=_update_forever,
         args=(progresses_dir, entire_progress_path, notification,),
         daemon=True
     )
```

### Comparing `pytest_dashboard-0.0.8/pytest_dashboard/conftest.py` & `pytest_dashboard-0.1.0/pytest_dashboard/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_dashboard-0.0.8/PKG-INFO` & `pytest_dashboard-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 Metadata-Version: 2.1
 Name: pytest-dashboard
-Version: 0.0.8
+Version: 0.1.0
 Summary: 
 Home-page: https://github.com/pyfemtet/pytest-dashboard
 License: BSD-3-Clause
 Author: kazuma.naito
 Author-email: kazuma.naito@murata.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: dash (>=2.14.2,<3.0.0)
-Requires-Dist: dash-bootstrap-components (>=1.5.0,<2.0.0)
 Requires-Dist: fire (>=0.6.0,<0.7.0)
-Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Project-URL: Repository, https://github.com/pyfemtet/pytest-dashboard
 Description-Content-Type: text/markdown
 
 # pytest-dashboard
 
+## example
+- Download project
+- Run some pytest with `--progress-path` option. The value should end with `-progress.yaml`.
+    - i.e.) `pytest <path_to_project>\sample-tests --progress-path=<path_to_project>\sample-tests\sample-progress.yaml`
+    - You will get a `sample-progress.yaml` file.
+- Run pytest dashboard
+    - i.e.) `tally-pytest <path_to_project>\sample-tests`
+    - You will get a `entire-progress.yaml` file in working folder.
+
 ## usage
-`python -m pytest`
+`pytest`
 by this command, you get `[datetime]-progress.yaml` file on working directory as realtime pytest progress report.
 
-`python -m pytest --progress-path=[path/to/some-progress.yaml]`
+`pytest --progress-path=[path/to/some-progress.yaml]`
 by this command, you get `path/to/some-progress.yaml` file.
+The value should end with `-progress.yaml`.
 
-`python -m pytest-dashboard.tally PROGRESSES_DIR --entire_progress_path=[path/to/entire-progress.yaml]`
+`tally-pytest PROGRESSES_DIR --entire_progress_path=[path/to/entire-progress.yaml]`
 by this command, you get started to monitor changes of
 the progress files (ends with `-progress.yaml`)
 inside `PROGRESS_DIR` and save the state summary
 to `path/to/entire-progress.yaml`.
 
 So it is necessary to set `--progress-path` option of pytest
 ending with `-progress.yaml`.
 For example, `2024-04-22-progress.yaml`,
 
 > **Note**
 > if your `entire_progress_path` is ends with `-progress.yaml`,
 > you cannot save the entire progress file to
 > the same directory with each progress file.
 
-
-`python -m pytest_dashboard.tally PROGRESS_DIR --notification=True`
+`tally-pytest PROGRESS_DIR --notification=True`
 By this command, you will get mail notification when entire progress is finished.
 > **Note**
-> Please make and implement pytest_dashboard.config
+> Please implement pytest_dashboard.config
 > that contains information abaout mail address and SMTP server.
-
-
-`python -m pytest_dashboard.launch_pytest_dashboard`
-NOT IMPLEMENTED!
+> This command works with powershell `Send-MailMessage` command.
```

