# Comparing `tmp/winterapi-1.4.0.tar.gz` & `tmp/winterapi-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winterapi-1.4.0.tar", last modified: Mon May 20 21:29:29 2024, max compression
+gzip compressed data, was "winterapi-1.4.1.tar", last modified: Wed May 29 06:16:27 2024, max compression
```

## Comparing `winterapi-1.4.0.tar` & `winterapi-1.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.367559 winterapi-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/continuous_integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/isort.yml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-20 21:27:34.000000 winterapi-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-20 21:27:34.000000 winterapi-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 21:27:34.000000 winterapi-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 21:29:29.367559 winterapi-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-20 21:27:34.000000 winterapi-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_1_Setting_Up_Credentials.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_2_Submitting_a_ToO.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_3_Interacting_with_Observatory_Queue.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   102674 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_4_Finding_Observatory_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_5_Downloading_Observatory_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Info_1_Introduction_To_Credentials.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Info_2a_ToO_Parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19222 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Info_2b_Submitting_ToOs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-20 21:27:34.000000 winterapi-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:29:29.367559 winterapi-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-20 21:27:34.000000 winterapi-1.4.0/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-20 21:27:34.000000 winterapi-1.4.0/tests/test_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-20 21:27:34.000000 winterapi-1.4.0/tests/testdata/test_schedule.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.367559 winterapi-1.4.0/winterapi/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/base_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/configure_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/fidelius.py
--rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/messenger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.367559 winterapi-1.4.0/winterapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:16:27.975262 winterapi-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:16:27.971262 winterapi-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-29 06:14:20.000000 winterapi-1.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:16:27.971262 winterapi-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-29 06:14:20.000000 winterapi-1.4.1/.github/workflows/automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-29 06:14:20.000000 winterapi-1.4.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-29 06:14:20.000000 winterapi-1.4.1/.github/workflows/continuous_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-29 06:14:20.000000 winterapi-1.4.1/.github/workflows/isort.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-29 06:14:20.000000 winterapi-1.4.1/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-29 06:14:20.000000 winterapi-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-29 06:14:20.000000 winterapi-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-29 06:14:20.000000 winterapi-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-29 06:16:27.975262 winterapi-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-29 06:14:20.000000 winterapi-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:16:27.971262 winterapi-1.4.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-29 06:14:20.000000 winterapi-1.4.1/notebooks/Example_1_Setting_Up_Credentials.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-05-29 06:14:20.000000 winterapi-1.4.1/notebooks/Example_2_Submitting_a_ToO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-29 06:14:20.000000 winterapi-1.4.1/notebooks/Example_3_Interacting_with_Observatory_Queue.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   102674 2024-05-29 06:14:20.000000 winterapi-1.4.1/notebooks/Example_4_Finding_Observatory_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-05-29 06:14:20.000000 winterapi-1.4.1/notebooks/Example_5_Downloading_Observatory_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-05-29 06:14:20.000000 winterapi-1.4.1/notebooks/Info_1_Introduction_To_Credentials.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-05-29 06:14:20.000000 winterapi-1.4.1/notebooks/Info_2a_ToO_Parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19222 2024-05-29 06:14:20.000000 winterapi-1.4.1/notebooks/Info_2b_Submitting_ToOs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-29 06:14:20.000000 winterapi-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:16:27.975262 winterapi-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:16:27.971262 winterapi-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-29 06:14:20.000000 winterapi-1.4.1/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-29 06:14:20.000000 winterapi-1.4.1/tests/test_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:16:27.971262 winterapi-1.4.1/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-29 06:14:20.000000 winterapi-1.4.1/tests/testdata/test_schedule.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:16:27.975262 winterapi-1.4.1/winterapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 06:14:20.000000 winterapi-1.4.1/winterapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-29 06:14:20.000000 winterapi-1.4.1/winterapi/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-29 06:14:20.000000 winterapi-1.4.1/winterapi/configure_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-29 06:14:20.000000 winterapi-1.4.1/winterapi/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-29 06:14:20.000000 winterapi-1.4.1/winterapi/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-29 06:14:20.000000 winterapi-1.4.1/winterapi/fidelius.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-05-29 06:14:20.000000 winterapi-1.4.1/winterapi/messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:16:27.975262 winterapi-1.4.1/winterapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-29 06:16:27.000000 winterapi-1.4.1/winterapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 06:16:27.000000 winterapi-1.4.1/winterapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:16:27.000000 winterapi-1.4.1/winterapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 06:16:27.000000 winterapi-1.4.1/winterapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 06:16:27.000000 winterapi-1.4.1/winterapi.egg-info/top_level.txt
```

### Comparing `winterapi-1.4.0/.github/workflows/automerge.yml` & `winterapi-1.4.1/.github/workflows/automerge.yml`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/.github/workflows/black.yml` & `winterapi-1.4.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/.github/workflows/continuous_integration.yml` & `winterapi-1.4.1/.github/workflows/continuous_integration.yml`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/.github/workflows/pylint.yml` & `winterapi-1.4.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/.gitignore` & `winterapi-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/.pre-commit-config.yaml` & `winterapi-1.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/LICENSE` & `winterapi-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/PKG-INFO` & `winterapi-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winterapi
-Version: 1.4.0
+Version: 1.4.1
 Author-email: Robert Stein <rdstein@caltech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/winter-telescope/winterapi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +24,15 @@
 Requires-Dist: packaging
 Requires-Dist: keyring
 Requires-Dist: cryptography
 Requires-Dist: pre-commit
 Requires-Dist: jupyter
 Requires-Dist: backoff
 Requires-Dist: pydantic
-Requires-Dist: wintertoo>=1.6.1
+Requires-Dist: wintertoo>=1.6.2
 Provides-Extra: dev
 Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: pylint==3.2.2; extra == "dev"
 Requires-Dist: coveralls; extra == "dev"
 
 # winterapi
```

### Comparing `winterapi-1.4.0/README.md` & `winterapi-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/notebooks/Example_1_Setting_Up_Credentials.ipynb` & `winterapi-1.4.1/notebooks/Example_1_Setting_Up_Credentials.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/notebooks/Example_2_Submitting_a_ToO.ipynb` & `winterapi-1.4.1/notebooks/Example_2_Submitting_a_ToO.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/notebooks/Example_3_Interacting_with_Observatory_Queue.ipynb` & `winterapi-1.4.1/notebooks/Example_3_Interacting_with_Observatory_Queue.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/notebooks/Example_4_Finding_Observatory_Data.ipynb` & `winterapi-1.4.1/notebooks/Example_4_Finding_Observatory_Data.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/notebooks/Example_5_Downloading_Observatory_Data.ipynb` & `winterapi-1.4.1/notebooks/Example_5_Downloading_Observatory_Data.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/notebooks/Info_1_Introduction_To_Credentials.ipynb` & `winterapi-1.4.1/notebooks/Info_1_Introduction_To_Credentials.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/notebooks/Info_2a_ToO_Parameters.ipynb` & `winterapi-1.4.1/notebooks/Info_2a_ToO_Parameters.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/notebooks/Info_2b_Submitting_ToOs.ipynb` & `winterapi-1.4.1/notebooks/Info_2b_Submitting_ToOs.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/pyproject.toml` & `winterapi-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "winterapi"
-version = "1.4.0"
+version = "1.4.1"
 description = ""
 authors = [
     {name = "Robert Stein", email = "rdstein@caltech.edu"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
@@ -32,15 +32,15 @@
     "packaging",
     "keyring",
     "cryptography",
     "pre-commit",
     "jupyter",
     "backoff",
     "pydantic",
-    "wintertoo>=1.6.1"
+    "wintertoo>=1.6.2"
 ]
 [project.optional-dependencies]
 dev = [
     "black == 24.4.2",
     "isort == 5.13.2",
     "pylint == 3.2.2",
     "coveralls",
```

### Comparing `winterapi-1.4.0/tests/test_schedule.py` & `winterapi-1.4.1/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/tests/testdata/test_schedule.csv` & `winterapi-1.4.1/tests/testdata/test_schedule.csv`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/winterapi/base_api.py` & `winterapi-1.4.1/winterapi/base_api.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/winterapi/configure_tests.py` & `winterapi-1.4.1/winterapi/configure_tests.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/winterapi/credentials.py` & `winterapi-1.4.1/winterapi/credentials.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/winterapi/endpoints.py` & `winterapi-1.4.1/winterapi/endpoints.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/winterapi/fidelius.py` & `winterapi-1.4.1/winterapi/fidelius.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/winterapi/messenger.py` & `winterapi-1.4.1/winterapi/messenger.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.4.0/winterapi.egg-info/PKG-INFO` & `winterapi-1.4.1/winterapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winterapi
-Version: 1.4.0
+Version: 1.4.1
 Author-email: Robert Stein <rdstein@caltech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/winter-telescope/winterapi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +24,15 @@
 Requires-Dist: packaging
 Requires-Dist: keyring
 Requires-Dist: cryptography
 Requires-Dist: pre-commit
 Requires-Dist: jupyter
 Requires-Dist: backoff
 Requires-Dist: pydantic
-Requires-Dist: wintertoo>=1.6.1
+Requires-Dist: wintertoo>=1.6.2
 Provides-Extra: dev
 Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: pylint==3.2.2; extra == "dev"
 Requires-Dist: coveralls; extra == "dev"
 
 # winterapi
```

### Comparing `winterapi-1.4.0/winterapi.egg-info/SOURCES.txt` & `winterapi-1.4.1/winterapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

