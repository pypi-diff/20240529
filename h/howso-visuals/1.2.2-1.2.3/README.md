# Comparing `tmp/howso_visuals-1.2.2.tar.gz` & `tmp/howso_visuals-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "howso_visuals-1.2.2.tar", last modified: Tue Apr 30 13:36:01 2024, max compression
+gzip compressed data, was "howso_visuals-1.2.3.tar", last modified: Wed May 29 13:49:08 2024, max compression
```

## Comparing `howso_visuals-1.2.2.tar` & `howso_visuals-1.2.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.224062 howso_visuals-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.216062 howso_visuals-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.216062 howso_visuals-1.2.2/.github/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/templates/version_summary.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/workflows/build-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/workflows/build-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/workflows/rebuild-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)   199837 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33893 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    40889 2024-04-30 13:36:01.224062 howso_visuals-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/bin/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-mt-debug-howso.yml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-mt-howso.yml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-mt-noavx-debug-howso.yml
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-st-debug-howso.yml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-st-howso.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/config/powershell/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/powershell/Download-Tzdata.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/powershell/Helper-Functions.ps1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.212062 howso_visuals-1.2.2/howso/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/howso/visuals/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/howso/visuals/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/data/iris.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/howso/visuals/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    24016 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/howso_visuals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40889 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    65614 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.10-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)    65365 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.11-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)    65365 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.12-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.12.txt
--rw-r--r--   0 runner    (1001) docker     (127)    65866 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.9-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35209 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:36:01.224062 howso_visuals-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.498695 howso_visuals-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.490695 howso_visuals-1.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.490695 howso_visuals-1.2.3/.github/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/.github/templates/version_summary.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.490695 howso_visuals-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/.github/workflows/build-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/.github/workflows/build-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/.github/workflows/rebuild-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)   199837 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33893 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    40889 2024-05-29 13:49:08.494695 howso_visuals-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.490695 howso_visuals-1.2.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/bin/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.494695 howso_visuals-1.2.3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/config/latest-mt-debug-howso.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/config/latest-mt-howso.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/config/latest-mt-noavx-debug-howso.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/config/latest-st-debug-howso.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/config/latest-st-howso.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.494695 howso_visuals-1.2.3/config/powershell/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/config/powershell/Download-Tzdata.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/config/powershell/Helper-Functions.ps1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.486695 howso_visuals-1.2.3/howso/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.494695 howso_visuals-1.2.3/howso/visuals/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/howso/visuals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.494695 howso_visuals-1.2.3/howso/visuals/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/howso/visuals/data/iris.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.494695 howso_visuals-1.2.3/howso/visuals/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/howso/visuals/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/howso/visuals/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23995 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/howso/visuals/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:08.494695 howso_visuals-1.2.3/howso_visuals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40889 2024-05-29 13:49:08.000000 howso_visuals-1.2.3/howso_visuals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-29 13:49:08.000000 howso_visuals-1.2.3/howso_visuals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:49:08.000000 howso_visuals-1.2.3/howso_visuals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 13:49:08.000000 howso_visuals-1.2.3/howso_visuals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 13:49:08.000000 howso_visuals-1.2.3/howso_visuals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    65614 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/requirements-3.10-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/requirements-3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    65365 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/requirements-3.11-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/requirements-3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    65365 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/requirements-3.12-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/requirements-3.12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    65866 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/requirements-3.9-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35209 2024-05-29 13:49:04.000000 howso_visuals-1.2.3/requirements-3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:49:08.498695 howso_visuals-1.2.3/setup.cfg
```

### Comparing `howso_visuals-1.2.2/.github/templates/version_summary.md` & `howso_visuals-1.2.3/.github/templates/version_summary.md`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/.github/workflows/build-pr.yml` & `howso_visuals-1.2.3/.github/workflows/build-pr.yml`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/.github/workflows/build-release.yml` & `howso_visuals-1.2.3/.github/workflows/build-release.yml`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/.github/workflows/build.yml` & `howso_visuals-1.2.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/.github/workflows/rebuild-requirements.yml` & `howso_visuals-1.2.3/.github/workflows/rebuild-requirements.yml`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/.gitignore` & `howso_visuals-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/LICENSE-3RD-PARTY.txt` & `howso_visuals-1.2.3/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/LICENSE.txt` & `howso_visuals-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/PKG-INFO` & `howso_visuals-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: howso-visuals
-Version: 1.2.2
+Version: 1.2.3
 Summary: Visualization utilities for use with Howso Engine.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
            Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
         of this license document, but changing it is not allowed.
```

### Comparing `howso_visuals-1.2.2/README.md` & `howso_visuals-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/config/powershell/Download-Tzdata.ps1` & `howso_visuals-1.2.3/config/powershell/Download-Tzdata.ps1`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/config/powershell/Helper-Functions.ps1` & `howso_visuals-1.2.3/config/powershell/Helper-Functions.ps1`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/howso/visuals/data/iris.csv` & `howso_visuals-1.2.3/howso/visuals/data/iris.csv`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/howso/visuals/tests/conftest.py` & `howso_visuals-1.2.3/howso/visuals/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/howso/visuals/tests/test_plot.py` & `howso_visuals-1.2.3/howso/visuals/tests/test_plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         generative_reacts = result["action"].loc[:, action_feature].values.tolist()
         generative_reacts[0] = generative_reacts[0] + 0.2
     else:
         generative_reacts = None
 
     if do_residual:
         iris_trainee.react_into_trainee(residuals=True)
-        residual = iris_trainee.get_prediction_stats(stats=["mae"])[action_feature][0]
+        residual = iris_trainee.get_prediction_stats(stats=["mae"])[action_feature].iloc[0]
     else:
         residual = None
 
     fig = plot_interpretable_prediction(
         react,
         actual_value=actual_value,
         generative_reacts=generative_reacts,
@@ -106,29 +106,29 @@
 
     # We will only get the most similar cases if there"s one or more highlight cases to
     # react to. This will add another trace.
     most_similar_cases = None
     if do_most_similar_cases and highlight_cases is not None:
         most_similar_cases = iris_trainee.react(contexts=highlight_cases, details={"most_similar_cases": True})
         most_similar_cases = pd.concat(
-            [pd.DataFrame(mscs) for mscs in most_similar_cases["explanation"]["most_similar_cases"]]
+            [pd.DataFrame(mscs) for mscs in most_similar_cases["details"]["most_similar_cases"]]
         ).reset_index(drop=True)
         num_expected_traces += 1
 
     # Same for bounary cases.
     boundary_cases = None
     if do_boundary_cases and highlight_cases is not None:
         context_features = iris_features.get_names(without=["target"])
         boundary_cases = iris_trainee.react(
             contexts=highlight_cases[context_features],
             action_features=["target"],
             details={"boundary_cases": True}
         )
         boundary_cases = pd.concat(
-            [pd.DataFrame(bcs) for bcs in boundary_cases["explanation"]["boundary_cases"]]
+            [pd.DataFrame(bcs) for bcs in boundary_cases["details"]["boundary_cases"]]
         ).reset_index(drop=True)
         num_expected_traces += 1
 
     # Hue groups by the requested feature and then creates one trace per group.
     if hue is not None:
         num_expected_traces += iris_test[hue].nunique()
     else:
@@ -158,23 +158,22 @@
 
     outliers_indices = outliers[['.session', '.session_training_index']].values
     convictions = iris_trainee.react(
         case_indices=outliers_indices,
         preserve_feature_values=iris_features.get_names(),
         leave_case_out=True,
         details={
-            "robust_computation": True,
             "boundary_cases": True,
             "influential_cases": True,
             "global_case_feature_residual_convictions": True,
             "local_case_feature_residual_convictions": True,
         }
     )
     convictions = pd.DataFrame(
-        convictions["explanation"]["global_case_feature_residual_convictions"]
+        convictions["details"]["global_case_feature_residual_convictions"]
     )
 
     yield outliers, convictions
 
 
 @pytest.mark.parametrize("num_cases_to_plot", [1, 5, 10])
 def test_plot_anomalies(
```

### Comparing `howso_visuals-1.2.2/howso/visuals/visuals.py` & `howso_visuals-1.2.3/howso/visuals/visuals.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 from __future__ import annotations
 
-from typing import (
-    Any,
-    Dict,
-    List,
-    Optional,
-    TYPE_CHECKING,
-    Tuple,
-)
+import typing as t
 
 import numpy as np
 from pandas import (
     DataFrame,
     Series,
 )
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from scipy.stats import gaussian_kde
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from howso.engine.trainee import Reaction
 
 
 def plot_feature_importances(
     feature_importances: DataFrame,
     *,
-    num_features_to_plot: Optional[int] = None,
+    num_features_to_plot: t.Optional[int] = None,
     sort_values: bool = True,
-    title: Optional[str] = "Feature Importances",
-    xaxis_title: Optional[str] = "Feature",
-    yaxis_title: Optional[str] = "Importance",
+    title: t.Optional[str] = "Feature Importances",
+    xaxis_title: t.Optional[str] = "Feature",
+    yaxis_title: t.Optional[str] = "Importance",
 ) -> go.Figure:
     """
     Plot feature importances (either MDA or feature contributions) from :meth:`Trainee.get_prediction_stats`.
 
     Parameters
     ----------
     feature_contributions : DataFrame
@@ -79,15 +72,15 @@
     anomalies: DataFrame,
     convictions: DataFrame,
     *,
     colorbar_title: str = "Conviction",
     num_cases_to_plot: int = 5,
     title: str = "Anomalies",
     xaxis_title: str = "Feature",
-    yaxis_title: Optional[str] = None,
+    yaxis_title: t.Optional[str] = None,
 ) -> go.Figure:
     """
     Plot anomalous cases using a heat map which shows conviction values for each feature.
 
     Parameters
     ----------
     anomalies : DataFrame
@@ -155,22 +148,22 @@
 
 def plot_dataset(
     data: DataFrame,
     x: str,
     y: str,
     *,
     alpha: float = 1.0,
-    boundary_cases: Optional[DataFrame] = None,
-    highlight_index: Optional[Any | List[Any]] = None,
-    highlight_label: Optional[str] = None,
-    highlight_selection_conditions: Optional[Dict[str, Any]] = None,
-    hue: Optional[str] = None,
-    most_similar_cases: Optional[DataFrame] = None,
-    size: Optional[str] = None,
-    title: Optional[str] = None,
+    boundary_cases: t.Optional[DataFrame] = None,
+    highlight_index: t.Optional[t.Any | list[t.Any]] = None,
+    highlight_label: t.Optional[str] = None,
+    highlight_selection_conditions: t.Optional[dict[str, t.Any]] = None,
+    hue: t.Optional[str] = None,
+    most_similar_cases: t.Optional[DataFrame] = None,
+    size: t.Optional[str] = None,
+    title: t.Optional[str] = None,
 ) -> go.Figure:
     """
     Create a figure which displays an entire dataset with certain cases being specifically highlighted.
 
     Namely, the cases which can be specifically highlighted are:
 
     - A particular case index/set of indices,
@@ -188,20 +181,20 @@
         The feature to place on the x axis.
     y : str
         The feature to place on the y axis.
     alpha : float, default 1.0
         The transparency to assign to each marker when plotting the dataset.
     boundary_cases: DataFrame, optional
         The boundary cases to plot, if any.
-    highlight_index : Any | List[Any], optional
+    highlight_index : Any or list of Any, optional
         The index of one or more individual cases to highlight. Takes priority over
         ``highlight_selection_conditions``.
     highlight_label : str, Optional
         The label to assign to the highlighted case.
-    highlight_selection_conditions : Dict[str, Any], optional
+    highlight_selection_conditions : dict of str -> Any, optional
         A mapping of feature names to feature values that describes conditions for selecting case(s)
         to highlight.
     hue : str, optional
         The feature to use when determining the hue of the plotted dataset.
     most_similar_cases : DataFrame, optional
         The most similar cases to plot, if any.
     size : str, optional
@@ -328,30 +321,30 @@
     return fig
 
 
 def plot_drift(
     df: DataFrame,
     *,
     compute_rolling_mean: bool = True,
-    line_positions: List[int] = None,
+    line_positions: list[int] = None,
     rolling_window: int = 10,
     title: str = "Model Drift \u2014 Conviction Over Time",
     xaxis_title: str = "Case Index",
     yaxis_title: str = "Conviction",
 ) -> go.Figure:
     """
     Plot model drift over time.
 
     Parameters
     ----------
     df : DataFrame
         A DataFrame containing the drift measures to plot.
     compute_rolling_mean : bool, default True
         Whether to compute the rolling mean for the variable to plot.
-    line_positions : List[int], optional
+    line_positions : list of int, optional
         Positions along the X axis to plot black lines.
     rolling_window : int, default 10
         The window to use when computing the rolling mean.
     title : str, "Model Drift \u2014 Conviction Over Time"
         The title for the figure.
     xaxis_title : str, "Case Index"
         The title for the figure's x axis.
@@ -441,52 +434,52 @@
 
     return fig
 
 
 def plot_interpretable_prediction(
     react: Reaction,
     *,
-    actual_value: Optional[float] = None,
-    generative_reacts: Optional[List[float]] = None,
-    residual: Optional[float] = None,
+    actual_value: t.Optional[float] = None,
+    generative_reacts: t.Optional[list[float]] = None,
+    residual: t.Optional[float] = None,
     secondary_yaxis_title: str = "Influence Weight",
-    title: Optional[str] = None,
-    xaxis_title: Optional[str] = None,
+    title: t.Optional[str] = None,
+    xaxis_title: t.Optional[str] = None,
     yaxis_title: str = "Density",
-) -> go.Figure | List[go.Figure]:
+) -> go.Figure | list[go.Figure]:
     """
     Plot a prediction with additional information for interpreting the result.
 
     Parameters
     ----------
     react : Reaction
         The reaction predicting the action feature(s) to visualize. If this contains more than one action feature,
         each will be given its own plot.
-    generative_reacts : Optional[List[float]]
+    generative_reacts : list of float, optional
         An optional list of values for the action feature to visualize. This will be used to visualize a
         KDE plot to characterize the distribution of values around the predicted and actual values. If this is None,
         the distribution of influential cases in the react will be used instead, if present.
-    actual_value : Optional[float]
+    actual_value : float, optional
         The actual value for the point that was predicted. If this is None, only the predicted value will be
         visualized.
-    residual : Optional[float]
+    residual : float, optional
         The residual for the feature that was predicted, local or global. Used to display an error bar around the
         predicted value. If this is None, no error bar will be displayed
     secondary_yaxis_title : str, default "Influence Weight"
         The title for thefigure's secondary y axis.
     title : str, optional
         The title for the figure.
     xaxis_title : str, optional
         The title for the figure's x axis. If None, the action feature will be used.
     yaxis_title : str, default "Density"
         The title for the figure's y axis.
 
     Returns
     -------
-    Figure | List[Figure]
+    Figure or list of Figure
         The resultant `Plotly` figure(s).
     """
     figures = []
     for action_feature in react["action"].columns:
         predicted_value = react["action"][action_feature].iloc[0]
 
         influential_cases = react.get("details", {}).get("influential_cases")
@@ -602,15 +595,15 @@
     fairness_results : dict
         Dictionary of the fairness disparity ratios.
     reference_class : str
         The reference class for the metric calculation.
     fairness_threshold : float, default 0.75
         Threshold for values to be classified as fair. Values below this threshold are colored red when
         graphing while values above are colored green.
-    x_tickangle : bool | float, default False
+    x_tickangle : bool or float, default False
         Whether to rotate the x-axis labels. If False, the labels will not be rotated. If True,
         the default angle is 45 degrees. If float, then that angle of rotation will be used.
     fair_color : str, default '#9BBf85'
         The bar chart color for values that are above the ``fairness_threshold``. Accepts `Plotly` compatible
         values.
     unfair_color : str, default '#B3589A'
         The bar chart color for values that are below the ``fairness_threshold``. Accepts `Plotly` compatible
@@ -662,15 +655,15 @@
             x_tickangle = 45
         fig.update_xaxes(tickangle=x_tickangle)
 
     return fig
 
 
 def compose_figures(
-    figures: List[go.Figure],
+    figures: list[go.Figure],
     rows: int,
     cols: int,
     **make_subplots_kwargs,
 ) -> go.Figure:
     """
     Helper function for composing several plotly `Figure`s.
 
@@ -684,18 +677,18 @@
     rows : int
         The number of rows to include in the composed `Figure`.
     cols : int
         The number of columns to include in the composed `Figure`.
 
     Returns
     -------
-    go.Figure
+    Figure
         The composed `Figure`.
     """
-    figure_trace_map: Dict[Tuple[int, int], List] = {}
+    figure_trace_map: dict[tuple[int, int], list] = {}
     subplot_titles = []
 
     if rows < 1 or cols < 1:
         raise ValueError("Neither `rows` nor `cols` can be less than 1.")
 
     if rows * cols < len(figures):
         raise ValueError(f"A {rows}x{cols} grid of subplots cannot fit {len(figures)} figures.")
```

### Comparing `howso_visuals-1.2.2/howso_visuals.egg-info/PKG-INFO` & `howso_visuals-1.2.3/howso_visuals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: howso-visuals
-Version: 1.2.2
+Version: 1.2.3
 Summary: Visualization utilities for use with Howso Engine.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
            Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
         of this license document, but changing it is not allowed.
```

### Comparing `howso_visuals-1.2.2/howso_visuals.egg-info/SOURCES.txt` & `howso_visuals-1.2.3/howso_visuals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/pyproject.toml` & `howso_visuals-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/requirements-3.10-dev.txt` & `howso_visuals-1.2.3/requirements-3.10-dev.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/requirements-3.10.txt` & `howso_visuals-1.2.3/requirements-3.10.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/requirements-3.11-dev.txt` & `howso_visuals-1.2.3/requirements-3.11-dev.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/requirements-3.11.txt` & `howso_visuals-1.2.3/requirements-3.11.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/requirements-3.12-dev.txt` & `howso_visuals-1.2.3/requirements-3.12-dev.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/requirements-3.12.txt` & `howso_visuals-1.2.3/requirements-3.12.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/requirements-3.9-dev.txt` & `howso_visuals-1.2.3/requirements-3.9-dev.txt`

 * *Files identical despite different names*

### Comparing `howso_visuals-1.2.2/requirements-3.9.txt` & `howso_visuals-1.2.3/requirements-3.9.txt`

 * *Files identical despite different names*

