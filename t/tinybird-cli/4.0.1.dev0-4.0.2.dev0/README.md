# Comparing `tmp/tinybird-cli-4.0.1.dev0.tar.gz` & `tmp/tinybird-cli-4.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-4.0.1.dev0.tar", last modified: Tue May 28 07:16:19 2024, max compression
+gzip compressed data, was "tinybird-cli-4.0.2.dev0.tar", last modified: Wed May 29 11:11:20 2024, max compression
```

## Comparing `tinybird-cli-4.0.1.dev0.tar` & `tinybird-cli-4.0.2.dev0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:16:19.014757 tinybird-cli-4.0.1.dev0/
--rw-r--r--   0 root         (0) root         (0)    70608 2024-05-28 07:16:19.014757 tinybird-cli-4.0.1.dev0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 07:16:19.014757 tinybird-cli-4.0.1.dev0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:16:19.011757 tinybird-cli-4.0.1.dev0/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-28 07:16:18.000000 tinybird-cli-4.0.1.dev0/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:16:19.011757 tinybird-cli-4.0.1.dev0/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-05-28 07:16:04.000000 tinybird-cli-4.0.1.dev0/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-05-28 07:16:04.000000 tinybird-cli-4.0.1.dev0/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-28 07:16:04.000000 tinybird-cli-4.0.1.dev0/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46918 2024-05-28 07:16:04.000000 tinybird-cli-4.0.1.dev0/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-05-28 07:16:04.000000 tinybird-cli-4.0.1.dev0/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-28 07:16:04.000000 tinybird-cli-4.0.1.dev0/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-28 07:16:04.000000 tinybird-cli-4.0.1.dev0/tinybird/context.py
--rw-rw-rw-   0 root         (0) root         (0)   210873 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    60657 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41589 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    81800 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11523 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:16:19.013757 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    38296 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    13910 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64576 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78296 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    32368 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31968 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26132 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:16:19.013757 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    11064 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-05-28 07:16:05.000000 tinybird-cli-4.0.1.dev0/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:16:19.014757 tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    70608 2024-05-28 07:16:18.000000 tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-28 07:16:18.000000 tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 07:16:18.000000 tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-28 07:16:18.000000 tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-05-28 07:16:18.000000 tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-28 07:16:18.000000 tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.227909 tinybird-cli-4.0.2.dev0/
+-rw-r--r--   0 root         (0) root         (0)    70608 2024-05-29 11:11:20.227909 tinybird-cli-4.0.2.dev0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 11:11:20.228909 tinybird-cli-4.0.2.dev0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.225909 tinybird-cli-4.0.2.dev0/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-29 11:11:18.000000 tinybird-cli-4.0.2.dev0/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.225909 tinybird-cli-4.0.2.dev0/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46918 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/context.py
+-rw-rw-rw-   0 root         (0) root         (0)   210873 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    60657 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41589 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    81800 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11523 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.226909 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    38296 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    13910 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64576 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78632 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    32368 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31968 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26132 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.227909 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    11064 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.227909 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    70608 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-4.0.1.dev0/PKG-INFO` & `tinybird-cli-4.0.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 4.0.1.dev0
+Version: 4.0.2.dev0
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
```

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/ch_utils/constants.py` & `tinybird-cli-4.0.2.dev0/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/ch_utils/engine.py` & `tinybird-cli-4.0.2.dev0/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/check_pypi.py` & `tinybird-cli-4.0.2.dev0/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/client.py` & `tinybird-cli-4.0.2.dev0/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/config.py` & `tinybird-cli-4.0.2.dev0/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/connectors.py` & `tinybird-cli-4.0.2.dev0/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/context.py` & `tinybird-cli-4.0.2.dev0/tinybird/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,11 +8,10 @@
 use_gatherer: ContextVar[bool] = ContextVar("use_gatherer")
 allow_gatherer_fallback: ContextVar[bool] = ContextVar("allow_gatherer_fallback")
 disable_template_security_validation: ContextVar[bool] = ContextVar("disable_template_security_validation")
 origin: ContextVar[str] = ContextVar("origin")
 request_id: ContextVar[str] = ContextVar("request_id")
 engine: ContextVar[str] = ContextVar("engine")
 wait_parameter: ContextVar[bool] = ContextVar("wait_parameter")
-wait_for_gatherer: ContextVar[bool] = ContextVar("wait_for_gatherer")
 api_host: ContextVar[str] = ContextVar("api_host")
 ff_split_to_array_escape: ContextVar[bool] = ContextVar("ff_split_to_array_escape")
 ff_preprocess_parameters_circuit_breaker: ContextVar[bool] = ContextVar("ff_preprocess_parameters_circuit_breaker")
```

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/datafile.py` & `tinybird-cli-4.0.2.dev0/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/datatypes.py` & `tinybird-cli-4.0.2.dev0/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/feedback_manager.py` & `tinybird-cli-4.0.2.dev0/tinybird/feedback_manager.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/git_settings.py` & `tinybird-cli-4.0.2.dev0/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/sql.py` & `tinybird-cli-4.0.2.dev0/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/sql_template.py` & `tinybird-cli-4.0.2.dev0/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/sql_template_fmt.py` & `tinybird-cli-4.0.2.dev0/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/sql_toolset.py` & `tinybird-cli-4.0.2.dev0/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/syncasync.py` & `tinybird-cli-4.0.2.dev0/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/auth.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/cicd.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/common.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1170,19 +1170,31 @@
 class PlanName(Enum):
     DEV = "Build"
     PRO = "Pro"
     ENTERPRISE = "Enterprise"
 
 
 def _get_workspace_plan_name(plan):
+    """
+    >>> _get_workspace_plan_name("dev")
+    'Build'
+    >>> _get_workspace_plan_name("pro")
+    'Pro'
+    >>> _get_workspace_plan_name("enterprise")
+    'Enterprise'
+    >>> _get_workspace_plan_name("branch_enterprise")
+    'Enterprise'
+    >>> _get_workspace_plan_name("other_plan")
+    'Custom'
+    """
     if plan == "dev":
         return PlanName.DEV.value
     if plan == "pro":
         return PlanName.PRO.value
-    if plan == "enterprise":
+    if plan in ("enterprise", "branch_enterprise"):
         return PlanName.ENTERPRISE.value
     return "Custom"
 
 
 def get_format_from_filename_or_url(filename_or_url: str) -> str:
     """
     >>> get_format_from_filename_or_url('wadus_parquet.csv')
```

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/config.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/connection.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/job.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/test.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/token.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/workspace.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird/tornado_template.py` & `tinybird-cli-4.0.2.dev0/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 4.0.1.dev0
+Version: 4.0.2.dev0
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
```

### Comparing `tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.1.dev0/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*

