# Comparing `tmp/ctapipe_io_nectarcam-0.1.4.tar.gz` & `tmp/ctapipe_io_nectarcam-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctapipe_io_nectarcam-0.1.4.tar", last modified: Wed Mar  6 09:50:52 2024, max compression
+gzip compressed data, was "ctapipe_io_nectarcam-0.1.5.tar", last modified: Wed May 29 07:22:54 2024, max compression
```

## Comparing `ctapipe_io_nectarcam-0.1.4.tar` & `ctapipe_io_nectarcam-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:50:52.894627 ctapipe_io_nectarcam-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:50:52.890627 ctapipe_io_nectarcam-0.1.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:50:52.890627 ctapipe_io_nectarcam-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-06 09:50:52.894627 ctapipe_io_nectarcam-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 09:50:52.894627 ctapipe_io_nectarcam-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:50:52.890627 ctapipe_io_nectarcam-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:50:52.890627 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/
--rw-r--r--   0 runner    (1001) docker     (127)    41118 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-06 09:50:52.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/anyarray_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:50:52.890627 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat
--rw-r--r--   0 runner    (1001) docker     (127)   881677 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   882754 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155_ctapipe018.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:50:52.894627 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/tests/test_nectarcameventsource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/tests/test_trigger_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-06 09:50:48.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:50:52.894627 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-06 09:50:52.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-06 09:50:52.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 09:50:52.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-06 09:50:52.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-06 09:50:52.000000 ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:22:54.311297 ctapipe_io_nectarcam-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:22:54.303297 ctapipe_io_nectarcam-0.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:22:54.303297 ctapipe_io_nectarcam-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-29 07:22:54.311297 ctapipe_io_nectarcam-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:22:54.311297 ctapipe_io_nectarcam-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:22:54.303297 ctapipe_io_nectarcam-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:22:54.303297 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/
+-rw-r--r--   0 runner    (1001) docker     (127)    53769 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 07:22:54.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/anyarray_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:22:54.307297 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   881677 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   882754 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155_ctapipe018.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:22:54.307297 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/tests/test_nectarcameventsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/tests/test_trigger_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-29 07:22:49.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:22:54.311297 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-29 07:22:54.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 07:22:54.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:22:54.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 07:22:54.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 07:22:54.000000 ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam.egg-info/top_level.txt
```

### Comparing `ctapipe_io_nectarcam-0.1.4/.github/workflows/ci.yml` & `ctapipe_io_nectarcam-0.1.5/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 name: CI
 
 # by not building all branches on push, we avoid the duplicated builds in PRs
 on:
   push:
     branches:
-      - master
+      - main
     tags:
       - '**'
   pull_request:
 
 env:
   NUMBA_NUM_THREADS: 1
   MPLBACKEND: Agg
   PYTEST_ADDOPTS: --color=yes
 
 jobs:
+  lint:
+    runs-on: ubuntu-latest
+    name: Lint
+    steps:
+      - name: Check out source repository
+        uses: actions/checkout@v3
+      - name: Set up Python environment
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.9"
+      - name: Runs pre-commit hooks
+        uses: pre-commit/action@v3.0.0
+        with:
+          extra_args: --files $(git diff origin/main --name-only)
+
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.9", "3.10", "3.11"]
         ctapipe-version: [v0.19.3]
 
@@ -48,15 +63,15 @@
         env:
           PYTHON_VERSION: ${{ matrix.python-version }}
           CTAPIPE_VERSION: ${{ matrix.ctapipe-version }}
 
         run: |
           python --version
           echo "Installing additional pip packages"
-          # we install ctapipe using pip to be able to select any commit, e.g. the current master
+          # we install ctapipe using pip to be able to select any commit, e.g. the current main
           pip install \
              "git+https://github.com/cta-observatory/ctapipe@$CTAPIPE_VERSION" \
               pytest-cov
 
           echo "pip install -e ."
           pip install -e .
```

### Comparing `ctapipe_io_nectarcam-0.1.4/.github/workflows/deploy.yml` & `ctapipe_io_nectarcam-0.1.5/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/.gitignore` & `ctapipe_io_nectarcam-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/LICENSE.md` & `ctapipe_io_nectarcam-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/PKG-INFO` & `ctapipe_io_nectarcam-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctapipe_io_nectarcam
-Version: 0.1.4
+Version: 0.1.5
 Summary: ctapipe plugin for reading NectarCam files
 Author: NectarCAM collaboration
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/cta-observatory/ctapipe_io_nectarcam/issues
 Project-URL: Source Code, https://github.com/cta-observatory/ctapipe_io_nectarcam
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -24,23 +24,24 @@
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Provides-Extra: all
 Requires-Dist: ctapipe_io_nectarcam[dev,test]; extra == "all"
 
-[![CI](https://github.com/cta-observatory/ctapipe_io_nectarcam/workflows/CI/badge.svg?branch=master)](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions?query=workflow%3ACI+branch%3Amaster)
+[![CI](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions/workflows/ci.yml?query=workflow%3ACI+branch%3Amain)
 
 EventSource Plugin for ctapipe, able to read NectarCam zfits files
 and calibrate them to R1 as needed for ctapipe tools.
 
 To install into an existing environment, just do:
 ```shell
 pip install .
 ```
 
 For development, create a new environment and run the development install:
 ```shell
 conda env create -n nectar-dev -f environment.yml
 conda activate nectar-dev
 pip install -e .
+pre-commit install
 ```
```

### Comparing `ctapipe_io_nectarcam-0.1.4/README.md` & `ctapipe_io_nectarcam-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-[![CI](https://github.com/cta-observatory/ctapipe_io_nectarcam/workflows/CI/badge.svg?branch=master)](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions?query=workflow%3ACI+branch%3Amaster)
+[![CI](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions/workflows/ci.yml?query=workflow%3ACI+branch%3Amain)
 
 EventSource Plugin for ctapipe, able to read NectarCam zfits files
 and calibrate them to R1 as needed for ctapipe tools.
 
 To install into an existing environment, just do:
 ```shell
 pip install .
 ```
 
 For development, create a new environment and run the development install:
 ```shell
 conda env create -n nectar-dev -f environment.yml
 conda activate nectar-dev
 pip install -e .
-```
+pre-commit install
+```
```

### Comparing `ctapipe_io_nectarcam-0.1.4/pyproject.toml` & `ctapipe_io_nectarcam-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/__init__.py` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,81 +2,91 @@
 """
 EventSource for NectarCAM protobuf-fits.fz-files.
 
 Needs protozfits v1.5.0 from github.com/cta-sst-1m/protozfitsreader
 """
 
 import glob
-import numpy as np
+import re
 import struct
+from enum import IntFlag, auto
+
+import numpy as np
 from astropy import units as u
 from astropy.io import fits
 from astropy.time import Time
 from ctapipe.containers import (
-    PixelStatusContainer, EventType, R0CameraContainer, R1CameraContainer,
-    CoordinateFrameType, PointingMode, SchedulingBlockContainer, ObservationBlockContainer, # VIM : line of things in lst equivalent
+    EventType,
+    ObservationBlockContainer,
+    PixelStatusContainer,
+    PointingMode,
+    R0CameraContainer,
+    R1CameraContainer,
+    SchedulingBlockContainer,
 )
 from ctapipe.coordinates import CameraFrame
 from ctapipe.core import Provenance
-from ctapipe.core.traits import Int, Bool, Enum
+from ctapipe.core.traits import Bool, Enum, Int
 from ctapipe.instrument import (
-    TelescopeDescription,
-    SubarrayDescription,
     CameraDescription,
-    CameraReadout,
     CameraGeometry,
+    CameraReadout,
     OpticsDescription,
+    ReflectorShape,
     SizeType,
-    ReflectorShape
+    SubarrayDescription,
+    TelescopeDescription,
 )
-
-from ctapipe.io import EventSource, DataLevel
-from enum import IntFlag, auto
+from ctapipe.io import DataLevel, EventSource
 from pkg_resources import resource_filename
 
+from .anyarray_dtypes import CDTS_AFTER_37201_DTYPE, CDTS_BEFORE_37201_DTYPE, TIB_DTYPE
 from .calibration import NectarCAMR0Corrections
-from .constants import (
-    N_GAINS, N_PIXELS, N_SAMPLES
-)
-from .containers import NectarCAMDataContainer, NectarCAMServiceContainer, \
-    NectarCAMEventContainer
-from .anyarray_dtypes import (
-    CDTS_AFTER_37201_DTYPE,
-    CDTS_BEFORE_37201_DTYPE,
-    TIB_DTYPE,
+from .constants import N_GAINS, N_PIXELS, N_SAMPLES
+from .containers import (
+    NectarCAMDataContainer,
+    NectarCAMDataStreamContainer,
+    NectarCAMEventContainer,
+    NectarCAMServiceContainer,
 )
+
+from traitlets.config import Config
+
 from .version import __version__
 
-__all__ = ['NectarCAMEventSource', '__version__']
+__all__ = ["LightNectarCAMEventSource", "NectarCAMEventSource", "__version__"]
 
 S_TO_NS = np.uint64(1e9)
 
+
 class TriggerBits(IntFlag):
-    '''
+    """
     See TIB User manual
-    '''
+    """
+
     UNKNOWN = 0
     MONO = auto()
     STEREO = auto()
     CALIBRATION = auto()
     SINGLE_PE = auto()
     SOFTWARE = auto()
     PEDESTAL = auto()
     SLOW_CONTROL = auto()
 
     PHYSICS = MONO | STEREO
     OTHER = CALIBRATION | SINGLE_PE | SOFTWARE | PEDESTAL | SLOW_CONTROL
 
 
 class PixelStatus(IntFlag):
-    '''
+    """
     Pixel status information
     See Section A.5 of the CTA R1 Data Model:
     https://forge.in2p3.fr/dmsf/files/8627
-    '''
+    """
+
     RESERVED_0 = auto()
     RESERVED_1 = auto()
     HIGH_GAIN_STORED = auto()
     LOW_GAIN_STORED = auto()
     SATURATED = auto()
     PIXEL_TRIGGER_1 = auto()
     PIXEL_TRIGGER_2 = auto()
@@ -84,170 +94,179 @@
 
     BOTH_GAINS_STORED = HIGH_GAIN_STORED | LOW_GAIN_STORED
 
 
 OPTICS = OpticsDescription(
     # https://gitlab.cta-observatory.org/cta-science/simulations/simulation-model/verification/verification-process/mst-structure/-/blob/master/Appendix-MST-Structure.pdf
     # version from 20 Jan 2022
-    'MST',
+    "MST",
     size_type=SizeType.MST,
-    equivalent_focal_length=u.Quantity(16., u.m),
-    effective_focal_length=u.Quantity(16.44505,u.m), # from https://www.mpi-hd.mpg.de/hfm/CTA/MC/Prod5/Config/PSF/fov_prod4.pdf mentioned in the link above
+    equivalent_focal_length=u.Quantity(16.0, u.m),
+    effective_focal_length=u.Quantity(
+        16.44505, u.m
+    ),  # from https://www.mpi-hd.mpg.de/hfm/CTA/MC/Prod5/Config/PSF/fov_prod4.pdf
+    # mentioned in the link above
     n_mirrors=1,
-    mirror_area=u.Quantity(106., u.m ** 2),  # no shadowing, uncertainty is 0.5 m2
+    mirror_area=u.Quantity(106.0, u.m**2),  # no shadowing, uncertainty is 0.5 m2
     n_mirror_tiles=86,  # Garczarczyk 2017
-    reflector_shape=ReflectorShape.HYBRID #according to Dan Parsons
+    reflector_shape=ReflectorShape.HYBRID,  # according to Dan Parsons
 )
 
 
-
-def nectar_trigger_patches(geometry,pix_mid_module):
-    '''
+def nectar_trigger_patches(geometry, pix_mid_module):
+    """
     Input:
-        camera geometry  
+        camera geometry
             e.g. `source.subarray.tel[10].camera.geometry`
         pix_mid_module
             list of pixels at the centre of the modules (from `module_central` routine)
     Returns:
         trigger_patches
             list of trigger_patches, each consisting of a list of pixels in that patch
-        
+
     Requires to have 7-pixel modules.
     Neighbours gets lazy-loaded by the main ctapipe function in camera.geometry.
-    '''
-    
+    """
+
     from copy import copy
-    from scipy import sparse    
 
-    trigger_patches = []    
+    trigger_patches = []
 
     for patch_pix in pix_mid_module:
         trigger_patch = patch_pix
         # Use a set to avoid repeating pixels
-        trigger_patch = set([patch_pix]+geometry.neighbors[patch_pix])
+        trigger_patch = set([patch_pix] + geometry.neighbors[patch_pix])
         for nbrs in geometry.neighbors[patch_pix]:
             trigger_patch |= set(geometry.neighbors[nbrs])
         for nbrs in copy(trigger_patch):
             trigger_patch |= set(geometry.neighbors[nbrs])
         trigger_patch = list(trigger_patch)
-        #type(trigger_patch),trigger_patch,len(trigger_patch)
-                
+
         # Just for tidiness
         trigger_patch.sort()
         trigger_patches.append(trigger_patch)
-    
-        
+
     return trigger_patches
 
+
 def module_central(geometry):
-    '''
+    """
     Input:
-        camera geometry  
+        camera geometry
             e.g. `source.subarray.tel[10].camera.geometry`
     Returns:
         pix_mid_module
             list of pixels at the centre of each module (sorted)
-        
+
     Requires the geometry to have pixel_x and pixel_y, and to have 7-pixel modules.
     Neighbours gets lazy-loaded by the main ctapipe function in camera.geometry.
-    
+
     Find central pixels of all the modules, as follows:
 
-    Finds the most distant PMT and which still has 6 neighbours, 
+    Finds the most distant PMT and which still has 6 neighbours,
       which must be the central pixel of a module.
-    Then elimates that module and repeats, until no modules left.
+    Then eliminates that module and repeats, until no modules left.
+
+    """
+
+    from copy import deepcopy
 
-    '''
-    
     import numpy as np
-    from copy import copy,deepcopy
-    
-    # Bug out right away if the number of pixels is not divisible by 7 (for 7-pixel modules)
-    if geometry.n_pixels%7 != 0:
-        raise ValueError("n_pixels is not divisible by 7, so not full 7-pixel modules. \n"+
-            "... Incompatible with expected NectarCAM geometry.")
-    
+
+    # Bug out right away if the number of pixels is not divisible by 7
+    # (for 7-pixel modules)
+    if geometry.n_pixels % 7 != 0:
+        raise ValueError(
+            "n_pixels is not divisible by 7, so not full 7-pixel modules. \n"
+            + "... Incompatible with expected NectarCAM geometry."
+        )
+
     pix_mid_module = []
-    
-    pixel_dist = np.hypot(geometry.pix_x,geometry.pix_y).value
+
+    pixel_dist = np.hypot(geometry.pix_x, geometry.pix_y).value
 
     # Make a dictionary by pixel index, so that pixels can be deleted later
-    pixel_dist_dict = dict(zip(range(geometry.n_pixels),pixel_dist))
-    
-    # geometry.neighbours gets lazy-loaded by the main ctapipe function in camera.geometry
-    pixel_nbrs_dict = dict(zip(range(geometry.n_pixels),deepcopy(geometry.neighbors)))
+    pixel_dist_dict = dict(zip(range(geometry.n_pixels), pixel_dist))
 
-    while len(pixel_dist_dict)>0:
+    # geometry.neighbours gets lazy-loaded by the main ctapipe function in
+    # camera.geometry
+    pixel_nbrs_dict = dict(zip(range(geometry.n_pixels), deepcopy(geometry.neighbors)))
 
+    while len(pixel_dist_dict) > 0:
         # Find the farthest pixel which still has 6 neighbours
-        
+
         # This holds the index within the dictionary
         pixdist_order = np.argsort(list(pixel_dist_dict.values()))
 
-        for pix_idx in pixdist_order[::-1]: # Go backwards
+        for pix_idx in pixdist_order[::-1]:  # Go backwards
             pix_key = list(pixel_dist_dict.keys())[pix_idx]
             if len(pixel_nbrs_dict[pix_key]) == 6:
                 break
         pix_cent = pix_key
-        
+
         pix_mid_module.append(pix_cent)
-        
+
         module = [pix_cent] + pixel_nbrs_dict[pix_key]
-        
+
         for pix_key in module:
-            
             # remove all the current module pixels from the neighbours list values
             for nbr_key in pixel_nbrs_dict:
                 if pix_key in pixel_nbrs_dict[nbr_key]:
                     pixel_nbrs_dict[nbr_key].remove(pix_key)
 
             # remove the current module pixels from the neighbours dictionary itself
             if pix_key in pixel_nbrs_dict:
                 pixel_nbrs_dict.pop(pix_key)
-            
+
             # remove the current module pixels from the distance dictionary
             if pix_key in pixel_dist_dict:
                 pixel_dist_dict.pop(pix_key)
-                
-    # Bug out right away if the number of central pixels is not == n_pixels/7 (for 7-pixel modules)
-    if len(pix_mid_module) != geometry.n_pixels/7:
-        raise ValueError("Number of module central pixels != n_pixels/7. \n"+
-            "... Incompatible with expected NectarCAM geometry.")
 
-                
+    # Bug out right away if the number of central pixels is not == n_pixels/7
+    # (for 7-pixel modules)
+    if len(pix_mid_module) != geometry.n_pixels / 7:
+        raise ValueError(
+            "Number of module central pixels != n_pixels/7. \n"
+            + "... Incompatible with expected NectarCAM geometry."
+        )
+
     # Just for tidiness
     pix_mid_module.sort()
-        
+
     return pix_mid_module
 
+
 def find_central_pixels(cam: CameraGeometry):
-    '''
+    """
     Input:
-        camera geometry  
+        camera geometry
             e.g. `source.subarray.tel[10].camera.geometry`
     Returns:
         central_pixel_ids
             list of pixels at the centre of each module (sorted)
-        
+
     Requires the geometry to have pixel_x and pixel_y, and to have 7-pixel modules.
     Neighbours gets lazy-loaded by the main ctapipe function in camera.geometry.
-    
+
     Find central pixels of all the modules, as follows:
 
-    Finds the most distant PMT and which still has 6 neighbours, 
+    Finds the most distant PMT and which still has 6 neighbours,
       which must be the central pixel of a module.
     Then elimates that module and repeats, until no modules left.
 
-    '''
+    """
     # Max's version of the above
 
-    # Bug out right away if the number of pixels is not divisible by 7 (for 7-pixel modules)
-    if cam.n_pixels%7 != 0:
-        raise ValueError("n_pixels is not divisible by 7, so not full 7-pixel modules. \n"+
-                         " -> Incompatible with expected NectarCAM geometry.")
+    # Bug out right away if the number of pixels is not divisible by 7
+    # (for 7-pixel modules)
+    if cam.n_pixels % 7 != 0:
+        raise ValueError(
+            "n_pixels is not divisible by 7, so not full 7-pixel modules. \n"
+            + " -> Incompatible with expected NectarCAM geometry."
+        )
 
     # distance to the camera center
     distance = np.hypot(cam.pix_x, cam.pix_y).to_value(cam.pix_x.unit)
 
     # pixel indices sorted from farthest to closest to the center
     order = np.argsort(distance)[::-1]
 
@@ -262,136 +281,150 @@
 
     while n_unassigned > 0:
         # Next pixel center is the furthest pixel from the center that has 6 neighbors
         try:
             center = order[(n_neighbors[order] == 6)][0]
         except IndexError:
             print(center)
-            raise IndexError("Search for module central pixels failed.\n"+
-                             " -> Probably incompatible with expected NectarCAM geometry")
+            raise IndexError(
+                "Search for module central pixels failed.\n"
+                + " -> Probably incompatible with expected NectarCAM geometry"
+            )
 
         central_pixel_ids.append(center)
 
-        # remove that pixel and the pixels that belong to this module, i.e. the neighbors
-        # of the central pixel, from the calculation
+        # remove that pixel and the pixels that belong to this module,
+        # i.e. the neighbors of the central pixel, from the calculation
         other = neighbors[center]
         n_neighbors[center] -= 7
         n_neighbors -= neighbors[other].sum(axis=0)
 
         neighbors[:, center] = False
         neighbors[center, :] = False
         neighbors[:, other] = False
         neighbors[other, :] = False
 
         n_unassigned -= 7
 
-    # Bug out right away if the number of central pixels is not == n_pixels/7 (for 7-pixel modules)
-    if len(central_pixel_ids) != cam.n_pixels/7:
-        raise ValueError("Number of module central pixels != n_pixels/7. \n"+
-                         " -> Incompatible with expected NectarCAM geometry.")
+    # Bug out right away if the number of central pixels is not == n_pixels/7
+    # (for 7-pixel modules)
+    if len(central_pixel_ids) != cam.n_pixels / 7:
+        raise ValueError(
+            "Number of module central pixels != n_pixels/7. \n"
+            + " -> Incompatible with expected NectarCAM geometry."
+        )
 
     central_pixel_ids = np.array(central_pixel_ids)
     central_pixel_ids.sort()
 
     return central_pixel_ids
 
+
 def add_nectar_trigger_patches_to_geom(cam: CameraGeometry):
-    '''
-        Does what it says on the tin
-        Adds the trigger patches as an attribute on-the-fly for now.
-            Input:
-        camera geometry  
-            e.g. `source.subarray.tel[10].camera.geometry`
-        Returns:
-            No return, just "cam" gets modified with added: 
-            * pix_mid_module: list of pixel IDs
-            * trigger_patches: list of list of pixel IDs
-            * trigger_patches_mask: list of list of boolean masks (n_pixels x n_pixels)
-            * trigger_patches_mask_sparse: sparse array of trigger_patches
-    '''
-    from scipy.sparse import csr_matrix, lil_matrix
-    
+    """
+    Does what it says on the tin
+    Adds the trigger patches as an attribute on-the-fly for now.
+        Input:
+    camera geometry
+        e.g. `source.subarray.tel[10].camera.geometry`
+    Returns:
+        No return, just "cam" gets modified with added:
+        * pix_mid_module: list of pixel IDs
+        * trigger_patches: list of list of pixel IDs
+        * trigger_patches_mask: list of list of boolean masks (n_pixels x n_pixels)
+        * trigger_patches_mask_sparse: sparse array of trigger_patches
+    """
+    from scipy.sparse import lil_matrix
+
     # Find central pixels of all the modules
     pix_mid_module = find_central_pixels(cam)
     cam.pix_mid_module = pix_mid_module
-    # Get a list of trigger patches, with the PMTs in each patch (up to 37 = 7 + 6*5, but fewer at edges)
-    trigger_patches = nectar_trigger_patches(cam,pix_mid_module)
+    # Get a list of trigger patches, with the PMTs in each patch (up to 37 = 7 + 6*5,
+    # but fewer at edges)
+    trigger_patches = nectar_trigger_patches(cam, pix_mid_module)
     cam.trigger_patches = trigger_patches
-    
+
     # Using a mask can be faster (tested with %%timeit), so calculate it here
 
     # Usage then is as follows:
-    # e.g. # sum(np.array(patch_masks) & np.array(mask_trig)) is the number of patches triggered
+    # e.g. # sum(np.array(patch_masks) & np.array(mask_trig)) is the number of patches
+    # triggered
     # > triggers = (np.sum(np.array(patch_masks) & np.array(mask_trig),axis=1))
     # > patch_count = sum(triggers>2)
     # # Where patch_count is the number of patches in triggered.
-                
+
     patch_masks = []
     for patch in trigger_patches:
-        patch_mask = np.array([False]*cam.n_pixels)
+        patch_mask = np.array([False] * cam.n_pixels)
         patch_mask[np.array(patch)] = True
-        patch_masks.append(patch_mask)        
+        patch_masks.append(patch_mask)
     cam.trigger_patches_mask = patch_masks
-    
+
     # Max suggestion to use sparse array
-    # Usage as above, but need to convert from sparse array to array with patch_masks_sparse.toarray()
+    # Usage as above, but need to convert from sparse array to array with
+    # patch_masks_sparse.toarray()
     # ... and then it is 4 times slower than using just the boolean mask array
     lil = lil_matrix((cam.n_pixels, cam.n_pixels), dtype=bool)
     for pix_id, patches in enumerate(trigger_patches):
         lil[pix_id, patches] = True
     patch_masks_sparse = lil.tocsr()
     cam.trigger_patches_mask_sparse = patch_masks_sparse
-    
+
     return
 
+
 def load_camera_geometry(version=3):
-    ''' Load camera geometry from bundled resources of this repo,
-         and find central pixels of the modules and trigger patches.'''
-         
-    #from ctapipe_io_nectarcam import nectar_trigger_patches,find_central_pixels
-    
+    """Load camera geometry from bundled resources of this repo,
+    and find central pixels of the modules and trigger patches."""
+
+    # from ctapipe_io_nectarcam import nectar_trigger_patches,find_central_pixels
+
     f = resource_filename(
-        'ctapipe_io_nectarcam', f'resources/NectarCam-{version:03d}.camgeom.fits.gz'
+        "ctapipe_io_nectarcam", f"resources/NectarCam-{version:03d}.camgeom.fits.gz"
     )
     Provenance().add_input_file(f, role="CameraGeometry")
     geom = CameraGeometry.from_table(f)
     geom.frame = CameraFrame(focal_length=OPTICS.equivalent_focal_length)
 
     # Add the trigger patches as an attribute on-the-fly for now.
-    add_nectar_trigger_patches_to_geom(geom)    
-    
+    add_nectar_trigger_patches_to_geom(geom)
+
     return geom
 
 
 def read_pulse_shapes():
-    '''
+    """
     Reads in the data on the pulse shapes from an external file
     Returns
     -------
     (daq_time_per_sample, pulse_shape_time_step, pulse shapes)
-        daq_time_per_sample: time between samples in the actual DAQ (ns, astropy quantity)
-        pulse_shape_time_step: time between samples in the returned single-p.e pulse shape (ns, astropy
-    quantity)
+        daq_time_per_sample: time between samples in the actual DAQ
+        (ns, astropy quantity)
+        pulse_shape_time_step: time between samples in the returned single-p.e
+        pulse shape (ns, astropy quantity)
         pulse shapes: Single-p.e. pulse shapes, ndarray of shape (2, 1640)
-    '''
+    """
 
-    # https://gitlab.cta-observatory.org/cta-consortium/aswg/simulations/simulation-model/simulation-model-description/-/blob/master/datFiles/Pulse_template_nectarCam_17042020.dat
+    # https://gitlab.cta-observatory.org/cta-consortium/aswg/simulations/
+    # simulation-model/simulation-model-description/-/blob/master/datFiles/
+    # Pulse_template_nectarCam_17042020.dat
     infilename = resource_filename(
-        'ctapipe_io_nectarcam',
-        'resources/Pulse_template_nectarCam_17042020.dat'
+        "ctapipe_io_nectarcam", "resources/Pulse_template_nectarCam_17042020.dat"
     )
 
-    data = np.genfromtxt(infilename, dtype='float', comments='#')
+    data = np.genfromtxt(infilename, dtype="float", comments="#")
     Provenance().add_input_file(infilename, role="PulseShapes")
-    pulse_shape_time_step = 0.125 * u.ns  # file specific, change if model file is changed
+    pulse_shape_time_step = (
+        0.125 * u.ns
+    )  # file specific, change if model file is changed
     # TODO read automatically from file
 
     # https://gitlab.cta-observatory.org/cta-science/simulations/simulation-model/verification/verification-process/mst-nectarcam/-/blob/master/Appendix-NectarCam.pdf
     # version from 13 Jan 2022
-    daq_time_per_sample = 1. * u.ns
+    daq_time_per_sample = 1.0 * u.ns
 
     # Note we have to transpose the pulse shapes array to provide what ctapipe
     # expects:
     return daq_time_per_sample, pulse_shape_time_step, data[:, 1:].T
 
 
 def time_from_unix_tai_ns(unix_tai_ns):
@@ -402,41 +435,66 @@
     """
     # make sure input is really uint64
     unix_tai_ns = np.asanyarray(unix_tai_ns, dtype=np.uint64)
 
     seconds, nanoseconds = np.divmod(unix_tai_ns, S_TO_NS)
     return Time(seconds, nanoseconds / S_TO_NS, format="unix_tai")
 
+
 class NectarCAMEventSource(EventSource):
     """
     EventSource for NectarCam r0 data.
     """
 
-    baseline = Int(
-        250,
-        help='r0 waveform baseline '
-    ).tag(config=True)
+    baseline = Int(250, help="r0 waveform baseline ").tag(config=True)
 
     trigger_information = Bool(
-        default_value=True,
-        help='Fill trigger information.'
+        default_value=True, help="Fill trigger information."
     ).tag(config=True)
 
     default_trigger_type = Enum(
-        ['ucts', 'tib'], default_value='ucts',
-        help=(
-            'Default source for trigger type information.'
-        )
+        ["ucts", "tib"],
+        default_value="ucts",
+        help=("Default source for trigger type information."),
     ).tag(config=True)
 
     calibrate_flatfields_and_pedestals = Bool(
         default_value=True,
-        help='If True, flat field and pedestal events are also calibrated.'
+        help="If True, flat field and pedestal events are also calibrated.",
+    ).tag(config=True)
+
+    skip_empty_events = Bool(
+        default_value=True,
+        help="If True, remove the empty events from the analysis (not loading"
+        "information from them).",
+    )
+
+    show_empty_stats = Bool(
+        default_value=False,
+        help="If True, show statistics on the empty events that were present in file"
+        "(only if empty events are skipped)",
     ).tag(config=True)
 
+    load_feb_info = Bool(
+        default_value=True,
+        help="If False, skip the decoding of FEB info"
+    )
+
+    def _correct_tel_id(self, tel_id, run):
+        if run >= 5047 and run <= 5085 and tel_id == 14:
+            # For the first data with EVB v6, the Telescope ID was set to 14 in the
+            # config but many other code (like monitoring script) expect tel_id at 0
+            # (hardcoded) so apply a correction to be sure that data are consistent
+            # for this data range
+            print(f"Correcting Telescope ID from {tel_id} to 0")
+            cor_tel_id = 0
+        else:
+            cor_tel_id = tel_id
+        return cor_tel_id
+
     def __init__(self, **kwargs):
         """
         Constructor
         Parameters
         ----------
         config: traitlets.loader.Config
             Configuration specified by config file or cmdline arguments.
@@ -450,84 +508,109 @@
             Additional parameters to be passed.
             NOTE: The file mask of the data to read can be passed with
             the 'input_url' parameter.
         """
         # EventSource can not handle file wild cards as input_url
         # To overcome this we substitute the input_url with first file matching
         # the specified file mask (copied from  MAGICEventSourceROOT).
-
-        if 'input_url' in kwargs.keys():
-            self.file_list = glob.glob(str(kwargs['input_url']))
+        if "input_url" in kwargs.keys():
+            self.file_list = glob.glob(str(kwargs["input_url"]))
             self.file_list.sort()
-            kwargs['input_url'] = self.file_list[0]
+            kwargs["input_url"] = self.file_list[0]
             super().__init__(**kwargs)
-        elif 'input_filelist' in kwargs.keys():
-            input_filelist = kwargs['input_filelist']
-            if isinstance(input_filelist,str):
+        elif "input_filelist" in kwargs.keys():
+            input_filelist = kwargs["input_filelist"]
+            if isinstance(input_filelist, str):
                 self.file_list = [input_filelist]
             else:
                 self.file_list = list(input_filelist)
             self.file_list.sort()
-            kwargs['input_url'] = self.file_list[0]
-            del kwargs['input_filelist']
+            kwargs["input_url"] = self.file_list[0]
+            del kwargs["input_filelist"]
             super().__init__(**kwargs)
         else:
             super().__init__(**kwargs)
             self.file_list = [self.input_url]
 
-        self.multi_file = MultiFiles(self.file_list)
+        self.multi_file = MultiFiles(self.file_list, self.skip_empty_events)
+        self._pre_v6_data = self.multi_file._pre_v6_file
         self.camera_config = self.multi_file.camera_config
         self.log.info("Read {} input files".format(self.multi_file.num_inputs()))
-        self.run_id = self.camera_config.configuration_id
-        self.tel_id = self.camera_config.telescope_id #VIM : Change the _tel_id to tel_id to be consistent with lst
-        self.run_start = Time(self.camera_config.date, format='unix')
+        self.run_id = (
+            self.camera_config.configuration_id
+            if self._pre_v6_data
+            else self.camera_config.local_run_id
+        )
+        self.tel_id = (
+            self.camera_config.telescope_id
+            if self._pre_v6_data
+            else self.camera_config.tel_id
+        )
+        self.tel_id = self._correct_tel_id(self.tel_id, self.run_id)
+        self.run_start = (
+            Time(self.camera_config.date, format="unix")
+            if self._pre_v6_data
+            else self.camera_config.config_time_s
+        )
         self.geometry_version = 3
         self._subarray = self.create_subarray(self.geometry_version, self.tel_id)
         self.r0_r1_calibrator = NectarCAMR0Corrections(
-             subarray=self._subarray, parent=self
-         )
-        self.nectarcam_service = self.fill_nectarcam_service_container_from_zfile(self.tel_id,
-                                                                                  self.camera_config)
+            subarray=self._subarray, parent=self
+        )
+        self.nectarcam_service = self.fill_nectarcam_service_container_from_zfile(
+            self.tel_id, self.camera_config, self._pre_v6_data
+        )
+        self.nectarcam_datastream = self.fill_nectarcam_datastream_container_from_zfile(
+            self.tel_id, self.multi_file.camera_datastream, self._pre_v6_data
+        )
 
         target_info = {}
 
-        # VIM : Put some pointing info to be filled as a reminder that it should be done at some point
-        #self.pointing_source = PointingSource(subarray=self.subarray, parent=self)
+        # VIM : Put some pointing info to be filled as a reminder that it should be done
+        # at some point
+        # self.pointing_source = PointingSource(subarray=self.subarray, parent=self)
         pointing_mode = PointingMode.UNKNOWN
-        #if self.pointing_information:
-        #    target = self.pointing_source.get_target(tel_id=self.tel_id, time=self.run_start)
+        # if self.pointing_information:
+        #    target = self.pointing_source.get_target(tel_id=self.tel_id,
+        #                                             time=self.run_start)
         #    if target is not None:
         #        target_info["subarray_pointing_lon"] = target["ra"]
         #        target_info["subarray_pointing_lat"] = target["dec"]
         #        target_info["subarray_pointing_frame"] = CoordinateFrameType.ICRS
         #        pointing_mode = PointingMode.TRACK
 
+        # TODO: Transfer the sb_id from the self.nectarcam_datastream when it will be
+        #  meaningful
         self._scheduling_blocks = {
             self.run_id: SchedulingBlockContainer(
                 sb_id=np.uint64(self.run_id),
                 producer_id=f"MST-{self.tel_id}",
                 pointing_mode=pointing_mode,
             )
         }
 
+        # TODO: Transfer the sb_id and obs_id from the self.nectarcam_datastream when it
+        #  will be meaningful
         self._observation_blocks = {
             self.run_id: ObservationBlockContainer(
                 obs_id=np.uint64(self.run_id),
                 sb_id=np.uint64(self.run_id),
                 producer_id=f"MST-{self.tel_id}",
                 actual_start_time=self.run_start,
-                **target_info
+                **target_info,
             )
         }
 
     def get_entries(self):
-        tot_events = 0
-        for v in self.multi_file._events_table.values():
-            tot_events += len(v)
-        return tot_events
+        n_total = len(self.multi_file)
+        n = n_total if self.max_events is None else min(n_total, self.max_events)
+        return n
+
+    def get_empty_entries(self):
+        return self.multi_file.get_empty_entries()
 
     def __len__(self):
         return self.get_entries()
 
     @property
     def is_simulation(self):
         return False
@@ -538,14 +621,18 @@
             return (DataLevel.R0, DataLevel.R1)
         return (DataLevel.R0,)
 
     @property
     def subarray(self):
         return self._subarray
 
+    @property
+    def pre_v6_data(self):
+        return self._pre_v6_data
+
     @staticmethod
     def create_subarray(geometry_version, tel_id=0):
         """
         Obtain the subarray from the EventSource
         Returns
         -------
         ctapipe.instrument.SubarrayDescription
@@ -554,204 +641,333 @@
         # camera info from NectarCAM-[geometry_version].camgeom.fits.gz file
         camera_geom = load_camera_geometry(version=geometry_version)
 
         # get info on the camera readout:
         daq_time_per_sample, pulse_shape_time_step, pulse_shapes = read_pulse_shapes()
 
         camera_readout = CameraReadout(
-            name = 'NectarCam',
+            name="NectarCam",
             n_pixels=N_PIXELS,
             n_channels=N_GAINS,
             n_samples=N_SAMPLES,
-            sampling_rate = (1 / daq_time_per_sample).to(u.GHz),
-            reference_pulse_shape = pulse_shapes,
-            reference_pulse_sample_width = pulse_shape_time_step,
+            sampling_rate=(1 / daq_time_per_sample).to(u.GHz),
+            reference_pulse_shape=pulse_shapes,
+            reference_pulse_sample_width=pulse_shape_time_step,
         )
 
-        camera = CameraDescription('NectarCam', camera_geom, camera_readout)
+        camera = CameraDescription("NectarCam", camera_geom, camera_readout)
 
         mst_tel_descr = TelescopeDescription(
-            name='NectarCam', optics=OPTICS, camera=camera
+            name="NectarCam", optics=OPTICS, camera=camera
         )
 
         tel_descriptions = {tel_id: mst_tel_descr}
 
         # MST telescope position
-        tel_positions = {tel_id: [0., 0., 0] * u.m}
+        tel_positions = {tel_id: [0.0, 0.0, 0] * u.m}
 
         subarray = SubarrayDescription(
             name=f"MST-{tel_id} subarray",
             tel_descriptions=tel_descriptions,
             tel_positions=tel_positions,
         )
 
         return subarray
 
-
     @property
     def observation_blocks(self):
         return self._observation_blocks
 
     @property
     def scheduling_blocks(self):
         return self._scheduling_blocks
 
     @property
     def obs_ids(self):
         # currently no obs id is available from the input files
-        return [self.camera_config.configuration_id, ]
+        # return [self.camera_config.configuration_id if self._pre_v6_data else
+        # self.camera_config.camera_config_id, ]
+        # change it to run_id from nectarcam_service (new) as camera_config_id is not
+        # the same as in pre_v6 data
+        return [
+            self.nectarcam_service.run_id,
+        ]
 
     def _generator(self):
-
         # container for NectarCAM data
         array_event = NectarCAMDataContainer()
-        array_event.meta['input_url'] = self.input_url
-        array_event.meta['max_events'] = self.max_events
-        array_event.meta['origin'] = 'NectarCAM'
+        array_event.meta["input_url"] = self.input_url
+        array_event.meta["max_events"] = self.max_events
+        array_event.meta["origin"] = "NectarCAM"
 
         # also add service container to the event section
         array_event.nectarcam.tel[self.tel_id].svc = self.nectarcam_service
+        array_event.nectarcam.tel[self.tel_id].dst = self.nectarcam_datastream
 
         # initialize general monitoring container
         self.initialize_mon_container(array_event)
 
         # loop on events
         for count, event in enumerate(self.multi_file):
-
             array_event.count = count
             array_event.index.event_id = event.event_id
             array_event.index.obs_id = self.obs_ids[0]
 
             # fill R0/R1 data
-            self.fill_r0r1_container(array_event, event)
-            # fill specific NectarCAM event data
+            self.fill_r0r1_container(
+                array_event, event
+            )  # svc or use self.nectarcam_service
+
             # fill specific NectarCAM event data
             self.fill_nectarcam_event_container_from_zfile(array_event, event)
 
             if self.trigger_information:
                 self.fill_trigger_info(array_event)
 
             # fill general monitoring data
             self.fill_mon_container_from_zfile(array_event, event)
 
             # gain select and calibrate to pe
-            if self.r0_r1_calibrator.calibration_path is not None:
+            if self.r0_r1_calibrator.calibration_path is not None:  # and not bad_event:
                 # skip flatfield and pedestal events if asked
                 if (
-                        self.calibrate_flatfields_and_pedestals
-                        or array_event.trigger.event_type not in {EventType.FLATFIELD,
-                                                                  EventType.SKY_PEDESTAL}
+                    self.calibrate_flatfields_and_pedestals
+                    or array_event.trigger.event_type
+                    not in {EventType.FLATFIELD, EventType.SKY_PEDESTAL}
                 ):
                     self.r0_r1_calibrator.calibrate(array_event)
 
             yield array_event
+        if self.show_empty_stats:
+            self.multi_file.show_empty_stats()
 
     @staticmethod
     def is_compatible(file_path):
         try:
-            # The file contains two tables:
+            # The file contains two tables for EVB v5:
             #  1: CameraConfig
             #  2: Events
-            h = fits.open(file_path)[2].header
-            ttypes = [
-                h[x] for x in h.keys() if 'TTYPE' in x
-            ]
+            # and 3 for EVB v6:
+            #  1: DataStream
+            #  2: CameraConfiguration
+            #  3: Events
+            # Modification for EVB v6 --> Going to search for the Events table
+            ffiles = fits.open(file_path)
+            event_names = ["Events"]
+            for i in range(1, len(ffiles)):  # start at 1 to avoid the PrimaryHDU
+                h = ffiles[i].header
+                if h["EXTNAME"] in event_names:
+                    break
+            ttypes = [h[x] for x in h.keys() if "TTYPE" in x]
         except OSError:
             # not even a fits file
             return False
 
         except IndexError:
             # A fits file of a different format
             return False
 
         is_protobuf_zfits_file = (
-                (h['XTENSION'] == 'BINTABLE') and
-                (h['EXTNAME'] == 'Events') and
-                (h['ZTABLE'] is True) and
-                (h['ORIGIN'] == 'CTA') and
-                (h['PBFHEAD'] == 'R1.CameraEvent')
+            (h["XTENSION"] == "BINTABLE")
+            and (h["EXTNAME"] == "Events")
+            and (h["ZTABLE"] is True)
+            and (h["ORIGIN"] == "CTA")
+            and (
+                h["PBFHEAD"] == "R1.CameraEvent" or h["PBFHEAD"] == "CTAR1.Event"
+            )  # The latter is from EVBv6
         )
 
-        is_nectarcam_file = 'nectarcam_counters' in ttypes
+        is_nectarcam_file = "nectarcam_counters" in ttypes
+        if not is_nectarcam_file:
+            # We might have a EVB v6 file, so let's try EVBv6
+            # EVBv6 format is similar to the one of LST... hard to distinguish... :-(
+            # I know that LST has 40 sample readout and NectarCAM 60,
+            # so use I'll use this
+            try:
+                nFields = int(h["TFIELDS"])
+                nWaveformBins = None
+                nPixels = None
+                for i in range(nFields):
+                    field = i + 1  # fields starts at 1
+                    if h[f"TTYPE{field}"] == "waveform":
+                        # ZFORM has letter to express the type, e.g  ZFORM11 = '221760I'
+                        # --> remove them
+                        nWaveformBins = int(re.sub("[^0-9]", "", h[f"ZFORM{field}"]))
+                    if h[f"TTYPE{field}"] == "pixel_status":
+                        nPixels = int(re.sub("[^0-9]", "", h[f"ZFORM{field}"]))
+                sample_per_pixel = nWaveformBins / nPixels
+                is_nectarcam_file = (
+                    sample_per_pixel == 120.0 or sample_per_pixel == 60.0
+                )
+                # 120 is for the case 2 channel are stored
+                # 60 is for the case 1 channel is stored (gain selection applied)
+            except (IndexError, TypeError, ValueError):
+                is_nectarcam_file = False
+        if not is_nectarcam_file:
+            # The last resort... Very ugly and likely won't work for
+            # non test bench data !!!!!!!
+            try:
+                if h["TARGET"] == "NectarCAM":
+                    is_nectarcam_file = True
+            except IndexError:
+                is_nectarcam_file = False
         return is_protobuf_zfits_file & is_nectarcam_file
 
     @staticmethod
-    def fill_nectarcam_service_container_from_zfile(tel_id, camera_config):
+    def fill_nectarcam_datastream_container_from_zfile(
+        tel_id, camera_datastream, pre_v6_data
+    ):
+        """
+        Fill NectarCAM DataStream container with specific NectarCAM data stream data
+        (from DataStream object) in the zfits file
+
         """
-        Fill NectarCAM Service container with specific NectarCAM service data data
+        ncdst = NectarCAMDataStreamContainer(telescope_id=tel_id)
+
+        if not pre_v6_data:
+            ncdst.sb_id = camera_datastream.sb_id
+            ncdst.obs_id = camera_datastream.obs_id
+            ncdst.waveform_scale = camera_datastream.waveform_scale
+            ncdst.waveform_offset = camera_datastream.waveform_offset
+        return ncdst
+
+    @staticmethod
+    def fill_nectarcam_service_container_from_zfile(tel_id, camera_config, pre_v6_data):
+        """
+        Fill NectarCAM Service container with specific NectarCAM service data
         (from the CameraConfig table of zfit file)
         """
-        return NectarCAMServiceContainer(
-            telescope_id=tel_id,
-            cs_serial=camera_config.cs_serial,
-            configuration_id=camera_config.configuration_id,
-            acquisition_mode=camera_config.nectarcam.acquisition_mode,
-            date=camera_config.date,
-            num_pixels=camera_config.num_pixels,
-            num_samples=camera_config.num_samples,
-            pixel_ids=camera_config.expected_pixels_id,
-            data_model_version=camera_config.data_model_version,
-            num_modules=camera_config.nectarcam.num_modules,
-            module_ids=camera_config.nectarcam.expected_modules_id,
-            idaq_version=camera_config.nectarcam.idaq_version,
-            cdhs_version=camera_config.nectarcam.cdhs_version,
-            algorithms=camera_config.nectarcam.algorithms,
-        )
 
-    def fill_nectarcam_event_container_from_zfile(self, array_event, event):
+        ncs = NectarCAMServiceContainer()
+        ncs.telescope_id = tel_id
+        ncs.num_pixels = camera_config.num_pixels
+        ncs.data_model_version = camera_config.data_model_version
+
+        if pre_v6_data:
+            ncs.cs_serial = camera_config.cs_serial
+            ncs.configuration_id = camera_config.configuration_id
+            ncs.acquisition_mode = camera_config.nectarcam.acquisition_mode
+            ncs.date = camera_config.date
+            ncs.num_samples = camera_config.num_samples
+            ncs.pixel_ids = camera_config.expected_pixels_id
+            ncs.num_modules = camera_config.nectarcam.num_modules
+            ncs.module_ids = camera_config.nectarcam.expected_modules_id
+            ncs.idaq_version = camera_config.nectarcam.idaq_version
+            ncs.cdhs_version = camera_config.nectarcam.cdhs_version
+            ncs.algorithms = camera_config.nectarcam.algorithms
+
+            # new variables since v6 but might have an interest to be filled with
+            # something meaningful:
+            ncs.num_channels = N_GAINS
 
+            # other
+            ncs.run_id = camera_config.nectarcam.run_id
+        else:
+            # Will debug always be there ?
+            has_debug = hasattr(camera_config, "debug")
+
+            ncs.configuration_id = camera_config.camera_config_id
+            ncs.acquisition_mode = None  # in v6 ? # VIM IMPORTANT
+            ncs.date = camera_config.config_time_s
+            ncs.num_samples = camera_config.num_samples_nominal
+            ncs.pixel_ids = camera_config.pixel_id_map
+            ncs.num_modules = camera_config.num_modules
+            ncs.module_ids = camera_config.module_id_map
+            ncs.algorithms = camera_config.calibration_algorithm_id
+
+            # new variables:
+            ncs.num_channels = camera_config.num_channels
+            ncs.calibration_service_id = camera_config.calibration_service_id
+
+            if has_debug:
+                ncs.cs_serial = camera_config.debug.cs_serial
+                ncs.idaq_version = camera_config.debug.evb_version
+                ncs.cdhs_version = camera_config.debug.cdhs_version
+                # new variables:
+                ncs.tdp_type = camera_config.debug.tdp_type
+                ncs.tdp_action = camera_config.debug.tdp_action
+                ncs.ttype_pattern = camera_config.debug.ttype_pattern
+
+            # other
+            ncs.run_id = camera_config.local_run_id
+
+        return ncs
+
+    def fill_nectarcam_event_container_from_zfile(self, array_event, event):
         tel_id = self.tel_id
         event_container = NectarCAMEventContainer()
         array_event.nectarcam.tel[tel_id].evt = event_container
 
-        event_container.configuration_id = event.configuration_id
+        if self.pre_v6_data:
+            nectarcam_data = event.nectarcam
+            event_container.configuration_id = event.configuration_id
+            event_container.tel_event_id = event.tel_event_id
+            event_container.ped_id = event.ped_id
+        else:
+            nectarcam_data = event.debug
+            event_container.configuration_id = self.nectarcam_service.configuration_id
+            # Above info not in Event for v6. Use the one from config. Is that right ?
+            event_container.tel_event_id = event.event_id
+            # Above info not in Event for v6. Use the event_id. is that right ?
+            event_container.ped_id = None
+            # Above info not in Event for v6. Put None instead
+
         event_container.event_id = event.event_id
-        event_container.tel_event_id = event.tel_event_id
         event_container.pixel_status = event.pixel_status
-        event_container.ped_id = event.ped_id
-        event_container.module_status = event.nectarcam.module_status
-        event_container.extdevices_presence = event.nectarcam.extdevices_presence
-        event_container.swat_data = event.nectarcam.swat_data
-        event_container.counters = event.nectarcam.counters
+
+        event_container.module_status = nectarcam_data.module_status
+        event_container.extdevices_presence = nectarcam_data.extdevices_presence
+        event_container.swat_data = nectarcam_data.swat_data
+        event_container.counters = nectarcam_data.counters
 
         # unpack TIB data
-        unpacked_tib = event.nectarcam.tib_data.view(TIB_DTYPE)[0]
+        unpacked_tib = nectarcam_data.tib_data.view(TIB_DTYPE)[0]
         event_container.tib_event_counter = unpacked_tib[0]
         event_container.tib_pps_counter = unpacked_tib[1]
         event_container.tib_tenMHz_counter = unpacked_tib[2]
         event_container.tib_stereo_pattern = unpacked_tib[3]
         event_container.tib_masked_trigger = unpacked_tib[4]
 
         # unpack CDTS data
-        is_old_cdts = len(event.nectarcam.cdts_data) < 36
+        is_old_cdts = len(nectarcam_data.cdts_data) < 36
         if is_old_cdts:
-            unpacked_cdts = event.nectarcam.cdts_data.view(CDTS_BEFORE_37201_DTYPE)[0]
+            unpacked_cdts = nectarcam_data.cdts_data.view(CDTS_BEFORE_37201_DTYPE)[0]
             event_container.ucts_event_counter = unpacked_cdts[0]
             event_container.ucts_pps_counter = unpacked_cdts[1]
             event_container.ucts_clock_counter = unpacked_cdts[2]
             event_container.ucts_timestamp = unpacked_cdts[3]
             event_container.ucts_camera_timestamp = unpacked_cdts[4]
             event_container.ucts_trigger_type = unpacked_cdts[5]
             event_container.ucts_white_rabbit_status = unpacked_cdts[6]
         else:
-            unpacked_cdts = event.nectarcam.cdts_data.view(CDTS_AFTER_37201_DTYPE)[0]
+            unpacked_cdts = nectarcam_data.cdts_data.view(CDTS_AFTER_37201_DTYPE)[0]
             event_container.ucts_timestamp = unpacked_cdts[0]
             event_container.ucts_address = unpacked_cdts[1]  # new
             event_container.ucts_event_counter = unpacked_cdts[2]
             event_container.ucts_busy_counter = unpacked_cdts[3]  # new
             event_container.ucts_pps_counter = unpacked_cdts[4]
             event_container.ucts_clock_counter = unpacked_cdts[5]
             event_container.ucts_trigger_type = unpacked_cdts[6]
             event_container.ucts_white_rabbit_status = unpacked_cdts[7]
             event_container.ucts_stereo_pattern = unpacked_cdts[8]  # new
             event_container.ucts_num_in_bunch = unpacked_cdts[9]  # new
             event_container.cdts_version = unpacked_cdts[10]  # new
 
+
+        if not self.pre_v6_data:
+            event_container.first_cell_id = np.full(
+                (N_PIXELS,), -1, dtype=event.first_cell_id.dtype
+            )
+            event_container.first_cell_id[
+                self.nectarcam_service.pixel_ids
+            ] = event.first_cell_id
+
         # Unpack FEB counters and trigger pattern
-        self.unpack_feb_data(event_container, event)
+        if self.load_feb_info:
+            self.unpack_feb_data(event_container, event, nectarcam_data)
 
     def fill_trigger_info(self, array_event):
         tel_id = self.tel_id
 
         nectarcam = array_event.nectarcam.tel[tel_id]
         tib_available = nectarcam.evt.extdevices_presence & 1
         ucts_available = nectarcam.evt.extdevices_presence & 2
@@ -761,189 +977,259 @@
         trigger_time = nectarcam.evt.ucts_timestamp
         trigger_time = time_from_unix_tai_ns(trigger_time)
         trigger.time = trigger_time
         trigger.tels_with_trigger = [tel_id]
         trigger.tel[tel_id].time = trigger.time
 
         # decide which source to use, if both are available,
-        # the option decides, if not, fallback to the avilable source
+        # the option decides, if not, fallback to the available source
         # if no source available, warn and do not fill trigger info
         if tib_available and ucts_available:
-            if self.default_trigger_type == 'ucts':
+            if self.default_trigger_type == "ucts":
                 trigger_bits = nectarcam.evt.ucts_trigger_type
             else:
                 trigger_bits = nectarcam.evt.tib_masked_trigger
-
         elif tib_available:
             trigger_bits = nectarcam.evt.tib_masked_trigger
-
         elif ucts_available:
             trigger_bits = nectarcam.evt.ucts_trigger_type
-
         else:
-            self.log.warning('No trigger info available.')
+            self.log.warning("No trigger info available.")
             trigger.event_type = EventType.UNKNOWN
             return
 
         if (
-                ucts_available
-                and nectarcam.evt.ucts_trigger_type == 42  # TODO check if it's correct
-                and self.default_trigger_type == "ucts"
+            ucts_available
+            and nectarcam.evt.ucts_trigger_type == 42  # TODO check if it's correct
+            and self.default_trigger_type == "ucts"
         ):
             self.log.warning(
-                'Event with UCTS trigger_type 42 found.'
-                ' Probably means unreliable or shifted UCTS data.'
+                "Event with UCTS trigger_type 42 found."
+                " Probably means unreliable or shifted UCTS data."
                 ' Consider switching to TIB using `default_trigger_type="tib"`'
             )
 
         # first bit mono trigger, second stereo.
         # If *only* those two are set, we assume it's a physics event
         # for all other we only check if the flag is present
-        if (trigger_bits & TriggerBits.PHYSICS) and not (trigger_bits & TriggerBits.OTHER):
+        if (trigger_bits & TriggerBits.PHYSICS) and not (
+            trigger_bits & TriggerBits.OTHER
+        ):
             trigger.event_type = EventType.SUBARRAY
         elif trigger_bits & TriggerBits.CALIBRATION:
             trigger.event_type = EventType.FLATFIELD
         elif trigger_bits & TriggerBits.PEDESTAL:
             trigger.event_type = EventType.SKY_PEDESTAL
         elif trigger_bits & TriggerBits.SINGLE_PE:
             trigger.event_type = EventType.SINGLE_PE
         else:
             self.log.warning(
-                f'Event {array_event.index.event_id} has unknown event type, trigger: {trigger_bits:08b}')
+                f"Event {array_event.index.event_id} has unknown event type,"
+                f"trigger: {trigger_bits:08b}"
+            )
             trigger.event_type = EventType.UNKNOWN
 
-    def unpack_feb_data(self, event_container, event):
-        '''Unpack FEB counters and trigger pattern'''
+    def unpack_feb_data(self, event_container, event, nectarcam_data):
+        """Unpack FEB counters and trigger pattern"""
 
         # Deduce data format version
-        bytes_per_module = len(
-            event.nectarcam.counters) // self.camera_config.nectarcam.num_modules
+        bytes_per_module = (
+            len(nectarcam_data.counters) // self.nectarcam_service.num_modules
+        )
+        # VIM NOTES> There is in v6 the num_modules per event... Use this one ?
+
         # Remain compatible with data before addition of trigger pattern
-        module_fmt = 'IHHIBBBBBBBB' if bytes_per_module > 16 else 'IHHIBBBB'
+        module_fmt = "IHHIBBBBBBBB" if bytes_per_module > 16 else "IHHIBBBB"
         n_fields = len(module_fmt)
-        rec_fmt = '=' + module_fmt * self.camera_config.nectarcam.num_modules
+        rec_fmt = "=" + module_fmt * self.nectarcam_service.num_modules
         # Unpack
-        unpacked_feb = struct.unpack(rec_fmt, event.nectarcam.counters)
+        unpacked_feb = struct.unpack(rec_fmt, nectarcam_data.counters)
+
         # Initialize field containers
         n_camera_modules = N_PIXELS // 7
-        event_container.feb_abs_event_id = np.zeros(shape=(n_camera_modules,), dtype=np.uint32)
-        event_container.feb_event_id = np.zeros(shape=(n_camera_modules,), dtype=np.uint16)
-        event_container.feb_pps_cnt = np.zeros(shape=(n_camera_modules,), dtype=np.uint16)
+        event_container.feb_abs_event_id = np.zeros(
+            shape=(n_camera_modules,), dtype=np.uint32
+        )
+        event_container.feb_event_id = np.zeros(
+            shape=(n_camera_modules,), dtype=np.uint16
+        )
+        event_container.feb_pps_cnt = np.zeros(
+            shape=(n_camera_modules,), dtype=np.uint16
+        )
         event_container.feb_ts1 = np.zeros(shape=(n_camera_modules,), dtype=np.uint32)
-        event_container.feb_ts2_trig = np.zeros(shape=(n_camera_modules,), dtype=np.int16)
-        event_container.feb_ts2_pps = np.zeros(shape=(n_camera_modules,), dtype=np.int16)
+        event_container.feb_ts2_trig = np.zeros(
+            shape=(n_camera_modules,), dtype=np.int16
+        )
+        event_container.feb_ts2_pps = np.zeros(
+            shape=(n_camera_modules,), dtype=np.int16
+        )
         if bytes_per_module > 16:
             n_patterns = 4
-            event_container.trigger_pattern = np.zeros(shape=(n_patterns, N_PIXELS),
-                                                       dtype=bool)
+            event_container.trigger_pattern = np.zeros(
+                shape=(n_patterns, N_PIXELS), dtype=bool
+            )
 
         # Unpack absolute event ID
         event_container.feb_abs_event_id[
-            self.camera_config.nectarcam.expected_modules_id] = unpacked_feb[0::n_fields]
+            self.nectarcam_service.module_ids
+        ] = unpacked_feb[0::n_fields]
         # Unpack PPS counter
-        event_container.feb_pps_cnt[
-            self.camera_config.nectarcam.expected_modules_id] = unpacked_feb[1::n_fields]
+        event_container.feb_pps_cnt[self.nectarcam_service.module_ids] = unpacked_feb[
+            1::n_fields
+        ]
         # Unpack relative event ID
-        event_container.feb_event_id[
-            self.camera_config.nectarcam.expected_modules_id] = unpacked_feb[2::n_fields]
+        event_container.feb_event_id[self.nectarcam_service.module_ids] = unpacked_feb[
+            2::n_fields
+        ]
         # Unpack TS1 counter
-        event_container.feb_ts1[
-            self.camera_config.nectarcam.expected_modules_id] = unpacked_feb[3::n_fields]
+        event_container.feb_ts1[self.nectarcam_service.module_ids] = unpacked_feb[
+            3::n_fields
+        ]
         # Unpack TS2 counters
         ts2_decimal = lambda bits: bits - (1 << 8) if bits & 0x80 != 0 else bits
         ts2_decimal_vec = np.vectorize(ts2_decimal)
         event_container.feb_ts2_trig[
-            self.camera_config.nectarcam.expected_modules_id] = ts2_decimal_vec(
-            unpacked_feb[4::n_fields])
+            self.nectarcam_service.module_ids
+        ] = ts2_decimal_vec(unpacked_feb[4::n_fields])
         event_container.feb_ts2_pps[
-            self.camera_config.nectarcam.expected_modules_id] = ts2_decimal_vec(
-            unpacked_feb[5::n_fields])
+            self.nectarcam_service.module_ids
+        ] = ts2_decimal_vec(unpacked_feb[5::n_fields])
         # Loop over modules
-        for module_idx, module_id in enumerate(
-                self.camera_config.nectarcam.expected_modules_id):
+        for module_idx, module_id in enumerate(self.nectarcam_service.module_ids):
             offset = module_id * 7
             if bytes_per_module > 16:
                 field_id = 8
                 # Decode trigger pattern
                 for pattern_id in range(n_patterns):
                     value = unpacked_feb[n_fields * module_idx + field_id + pattern_id]
-                    module_pattern = [int(digit) for digit in
-                                      reversed(bin(value)[2:].zfill(7))]
-                    event_container.trigger_pattern[pattern_id,
-                    offset:offset + 7] = module_pattern
+                    module_pattern = [
+                        int(digit) for digit in reversed(bin(value)[2:].zfill(7))
+                    ]
+                    event_container.trigger_pattern[
+                        pattern_id, offset : offset + 7
+                    ] = module_pattern
 
         # Unpack native charge
-        if len(event.nectarcam.charges_gain1) > 0:
-            event_container.native_charge = np.zeros(shape=(N_GAINS, N_PIXELS),
-                                                     dtype=np.uint16)
-            rec_fmt = '=' + 'H' * self.camera_config.num_pixels
+        if len(nectarcam_data.charges_gain1) > 0:
+            event_container.native_charge = np.zeros(
+                shape=(N_GAINS, N_PIXELS), dtype=np.uint16
+            )
+            rec_fmt = "=" + "H" * self.nectarcam_service.num_pixels
+
             for gain_id in range(N_GAINS):
-                unpacked_charge = struct.unpack(rec_fmt, getattr(event.nectarcam,
-                                                                 f'charges_gain{gain_id + 1}'))
+                unpacked_charge = struct.unpack(
+                    rec_fmt, getattr(nectarcam_data, f"charges_gain{gain_id + 1}")
+                )
                 event_container.native_charge[
-                    gain_id, self.camera_config.expected_pixels_id] = unpacked_charge
+                    gain_id, self.nectarcam_service.pixel_ids
+                ] = unpacked_charge
 
     def fill_r0r1_camera_container(self, zfits_event):
         """
         Fill the r0 or r1 container, depending on whether gain
         selection has already happened (r1) or not (r0)
         This will create waveforms of shape (N_GAINS, N_PIXELS, N_SAMPLES),
         or (N_PIXELS, N_SAMPLES) respectively regardless of the n_pixels, n_samples
         in the file.
         Missing or broken pixels are filled using maxval of the waveform dtype.
         """
-        n_pixels = self.camera_config.num_pixels
-        n_samples = self.camera_config.num_samples
-        expected_pixels = self.camera_config.expected_pixels_id
 
-        has_low_gain = (zfits_event.pixel_status & PixelStatus.LOW_GAIN_STORED).astype(bool)
-        has_high_gain = (zfits_event.pixel_status & PixelStatus.HIGH_GAIN_STORED).astype(bool)
+        # nectarcam_service contain the info from camera_config but in a "uniform" way
+        # between old and v6 data
+        n_pixels = (
+            self.nectarcam_service.num_pixels
+            if self.pre_v6_data
+            else zfits_event.num_pixels
+        )
+        n_samples = (
+            self.nectarcam_service.num_samples
+            if self.pre_v6_data
+            else zfits_event.num_samples
+        )
+        expected_pixels = self.nectarcam_service.pixel_ids
+
+        has_low_gain = (zfits_event.pixel_status & PixelStatus.LOW_GAIN_STORED).astype(
+            bool
+        )
+        has_high_gain = (
+            zfits_event.pixel_status & PixelStatus.HIGH_GAIN_STORED
+        ).astype(bool)
         not_broken = (has_low_gain | has_high_gain).astype(bool)
 
         # broken pixels have both false, so gain selected means checking
         # if there are any pixels where exactly one of high or low gain is stored
         gain_selected = np.any(has_low_gain != has_high_gain)
 
         # fill value for broken pixels
-        dtype = zfits_event.waveform.dtype
-        fill = np.iinfo(dtype).max
+
+        if self.pre_v6_data:
+            dtype = zfits_event.waveform.dtype
+            fill = np.iinfo(dtype).max
+        else:
+            dtype = np.float32
+            fill = np.finfo(dtype).max
+        # VIM : We received uint16 data from the EVB,
+        # but because of the scaling in v6 we gets back to a float, so let's use
+        # directly floats
+
         # we assume that either all pixels are gain selected or none
         # only broken pixels are allowed to be missing completely
+
         if gain_selected:
+            # print("GAIN SELECTED")
             selected_gain = np.where(has_high_gain, 0, 1)
-            waveform = np.full((n_pixels, n_samples), fill, dtype=dtype)
+            waveform = np.full(
+                (n_pixels, n_samples), fill, dtype=dtype
+            )  # VIM : Replace full by empty ?
             waveform[not_broken] = zfits_event.waveform.reshape((-1, n_samples))
 
-            reordered_waveform = np.full((N_PIXELS, N_SAMPLES), fill, dtype=dtype)
+            reordered_waveform = np.full(
+                (N_PIXELS, N_SAMPLES), fill, dtype=dtype
+            )  # VIM : Replace full by empty ?
             reordered_waveform[expected_pixels] = waveform
 
             reordered_selected_gain = np.full(N_PIXELS, -1, dtype=np.int8)
             reordered_selected_gain[expected_pixels] = selected_gain
 
             r0 = R0CameraContainer()
             r1 = R1CameraContainer(
                 waveform=reordered_waveform,
                 selected_gain_channel=reordered_selected_gain,
             )
         else:
-            reshaped_waveform = zfits_event.waveform.reshape(N_GAINS, n_pixels, n_samples)
+            reshaped_waveform = zfits_event.waveform.reshape(
+                N_GAINS, n_pixels, n_samples
+            )
             # re-order the waveform following the expected_pixels_id values
             #  could also just do waveform = reshaped_waveform[np.argsort(expected_ids)]
-            reordered_waveform = np.full((N_GAINS, N_PIXELS, N_SAMPLES), fill, dtype=dtype)
+            reordered_waveform = np.full(
+                (N_GAINS, N_PIXELS, N_SAMPLES), fill, dtype=dtype
+            )  # VIM : use empty ?
             reordered_waveform[:, expected_pixels, :] = reshaped_waveform
             r0 = R0CameraContainer(waveform=reordered_waveform)
             r1 = R1CameraContainer()
 
+        if not self.pre_v6_data:
+            if r0.waveform is not None:
+                r0.waveform = (
+                    r0.waveform - self.nectarcam_datastream.waveform_offset
+                ) / self.nectarcam_datastream.waveform_scale
+            if r1.waveform is not None:
+                r1.waveform = (
+                    r1.waveform - self.nectarcam_datastream.waveform_offset
+                ) / self.nectarcam_datastream.waveform_scale
+
         return r0, r1
 
     def fill_r0r1_container(self, array_event, zfits_event):
         """
         Fill with R0Container
         """
         r0, r1 = self.fill_r0r1_camera_container(zfits_event)
+
         array_event.r0.tel[self.tel_id] = r0
         array_event.r1.tel[self.tel_id] = r1
 
     def initialize_mon_container(self, array_event):
         """
         Fill with MonitoringContainer.
         For the moment, initialize only the PixelStatusContainer
@@ -969,88 +1255,174 @@
 
         """
 
         status_container = array_event.mon.tel[self.tel_id].pixel_status
 
         # reorder the array
         pixel_status = np.zeros(N_PIXELS)
-        pixel_status[self.camera_config.expected_pixels_id] = event.pixel_status
+        pixel_status[self.nectarcam_service.pixel_ids] = event.pixel_status
         status_container.hardware_failing_pixels[:] = pixel_status == 0
 
+
+
+class LightNectarCAMEventSource(NectarCAMEventSource):
+    """
+    EventSource for NectarCam r0 data.
+    Lighter version of the NectarCAMEventSource class but without FEB data nor gain selection.
+    """
+    def __init__(self,**kwargs):
+
+        if self.config is None:
+            self.config = Config()
+        self.config.NectarCAMEventSource.NectarCAMR0Corrections.calibration_path = None
+        self.config.NectarCAMEventSource.NectarCAMR0Corrections.apply_flatfield = False
+        self.config.NectarCAMEventSource.NectarCAMR0Corrections.select_gain = False
+        self.load_feb_info = False
+        super().__init__(**kwargs)
+
+    @staticmethod
+    def is_compatible(file_path):
+        '''
+        This version should only be called directly so return False 
+        such that it is not used when using EventSource
+        '''
+        return False
+
+
+
 class MultiFiles:
     """
     This class open all the files in file_list and read the events following
     the event_id order
     """
 
-    def __init__(self, file_list):
-
+    def __init__(self, file_list, skip_empty_events):
         self._file = {}
         self._events = {}
         self._events_table = {}
         self._camera_config = {}
+        self._camera_datastream = {}
         self.camera_config = None
+        self.camera_datastream = None
+        self._pre_v6_file = True
+        self._empty_per_file = dict()
+        self._skip_empty_events = skip_empty_events
 
         paths = []
         for file_name in file_list:
             paths.append(file_name)
-            Provenance().add_input_file(file_name, role='r0.sub.evt')
+            Provenance().add_input_file(file_name, role="r0.sub.evt")
 
         # open the files and get the first fits Tables
         from protozfits import File
 
         for path in paths:
-
             try:
                 self._file[path] = File(str(path))
-                self._events_table[path] = File(str(path)).Events
+                self._events_table[path] = File(
+                    str(path)
+                ).Events  # VIM : Why do we open the file a second time ?
                 self._events[path] = next(self._file[path].Events)
 
                 # verify where the CameraConfig is present
-                if 'CameraConfig' in self._file[path].__dict__.keys():
+                if "CameraConfig" in self._file[path].__dict__.keys():
+                    # File before EVB v6
                     self._camera_config[path] = next(self._file[path].CameraConfig)
-
-                    # for the moment it takes the first CameraConfig it finds (to be changed)
-                    if (self.camera_config is None):
-                        self.camera_config = self._camera_config[path]
-
+                elif "CameraConfiguration" in self._file[path].__dict__.keys():
+                    # File after EVB v6
+                    self._pre_v6_file = False
+                    self._camera_config[path] = next(
+                        self._file[path].CameraConfiguration
+                    )
+                    self._camera_datastream[path] = next(self._file[path].DataStream)
+
+                    # take the first datastream info it find (to be changed)
+                    if self.camera_datastream is None:
+                        self.camera_datastream = self._camera_datastream[path]
+
+                # for the moment it takes the first CameraConfig it finds
+                # (to be changed)
+                if self.camera_config is None:
+                    self.camera_config = self._camera_config[path]
 
             except StopIteration:
                 pass
 
         # verify that somewhere the CameraConfing is present
-        assert (self.camera_config)
+        assert self.camera_config
+
+    def show_empty_stats(self):
+        tot_zeros = sum(self._empty_per_file.values())
+        tot_events = self.__len__()
+        print(
+            f"WARNING> Empty events : {tot_zeros}/{tot_events} --> "
+            f"{100.*tot_zeros/tot_events:.2f} %"
+        )
+        # print("Files with empty events: ")
+        # for k, v in self._empty_per_file.items():
+        #    print(f'{os.path.basename(k)} : {v} empty events')
 
     def __iter__(self):
         return self
 
     def __next__(self):
         return self.next_event()
 
     def next_event(self):
         # check for the minimal event id
         if not self._events:
             raise StopIteration
 
+        if self._skip_empty_events:
+            # Attempt to skip the zero events
+            # Loop on all files. If there is an event_id at 0, then loop until there is
+            # one with a "normal id"
+            # Once done, go back to the normal behavior
+            # TODO : Think of a way to do it in on one pass over the files
+            files_with_zero = [k for k, v in self._events.items() if v.event_id == 0]
+            for f in files_with_zero:
+                # next until we find an event that is not 0
+                try:
+                    while self._events[f].event_id == 0:
+                        if f not in self._empty_per_file:
+                            self._empty_per_file[f] = 0
+                        self._empty_per_file[f] += 1
+                        self._events[f] = next(self._file[f].Events)
+                except StopIteration:
+                    # We have ended the file, remove it from the list so we don't
+                    # iterate/look at it anymore
+                    del self._events[f]
+
+        if len(self._events) == 0:
+            raise StopIteration
+
         min_path = min(
             self._events.items(),
             key=lambda item: item[1].event_id,
+            # biggest value for signed int on 64 bit (should be ok)
         )[0]
 
         # return the minimal event id
         next_event = self._events[min_path]
         try:
             self._events[min_path] = next(self._file[min_path].Events)
         except StopIteration:
             del self._events[min_path]
 
         return next_event
 
     def __len__(self):
-        total_length = sum(
-            len(table)
-            for table in self._events_table.values()
-        )
+        total_length = sum(len(table) for table in self._events_table.values())
         return total_length
 
     def num_inputs(self):
         return len(self._file)
+
+    def get_empty_entries(self):
+        # Compute the number of empty events. This is complete only once we've looped
+        # on all events
+        return sum(self._empty_per_file.values())
+
+
+
+
+
```

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/anyarray_dtypes.py` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/anyarray_dtypes.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/calibration.py` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/calibration.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,26 +87,28 @@
             self.mon_data = self._read_calibration_file(self.calibration_path)
 
     def calibrate(self, event: NectarCAMDataContainer):
         for tel_id in event.r0.tel:
             r1 = event.r1.tel[tel_id]
             # check if waveform is already filled
             if r1.waveform is None:
-                r1.waveform = event.r0.tel[tel_id].waveform
+                r1.waveform = event.r0.tel[tel_id].waveform.copy()
+                # Force a copy as v6 have waveform as float 
+                # so in this case r0 == r1 (in memory)
 
             r1.waveform = r1.waveform.astype(np.float32, copy=False)
-
             # do gain selection before converting to pe
             # like eventbuilder will do
             if self.select_gain and r1.selected_gain_channel is None:
                 r1.selected_gain_channel = self.gain_selector(r1.waveform)
                 r1.waveform = r1.waveform[r1.selected_gain_channel, PIXEL_INDEX]
 
             # apply monitoring data corrections,
             # subtract pedestal per sample and convert to pe
+
             if self.mon_data is not None:
                 calibration = self.mon_data.tel[tel_id].calibration
                 # pedestal subtraction and gain correction
                 convert_to_pe(
                     waveform=r1.waveform,
                     calibration=calibration,
                     selected_gain_channel=r1.selected_gain_channel
@@ -155,29 +157,26 @@
         mon = MonitoringContainer()
 
         with tables.open_file(path) as f:
             tel_ids = [
                 int(key[4:]) for key in f.root._v_children.keys()
                 if key.startswith('tel_')
             ]
-
         for tel_id in tel_ids:
             with HDF5TableReader(path) as h5_table:
-
                 mon.tel[tel_id] = MonitoringCameraContainer(
                     calibration=next(h5_table.read(f'/tel_{tel_id}/calibration', WaveformCalibrationContainer)),
                     flatfield=next(h5_table.read(f'/tel_{tel_id}/flatfield', FlatFieldContainer)),
-                    #pedestal=next(h5_table.read(f'/{base}/pedestal', PedestalContainer)),
-                    #pixel_status=next(h5_table.read(f"/{base}/pixel_status", PixelStatusContainer)),
                 )
 
         return mon
 
 
 def convert_to_pe(waveform, calibration, selected_gain_channel):
+
     if selected_gain_channel is None:
         waveform -= calibration.pedestal_per_sample
         waveform *= calibration.dc_to_pe[:, :, np.newaxis]
     else:
         waveform = waveform - calibration.pedestal_per_sample[selected_gain_channel]
         waveform *= calibration.dc_to_pe[selected_gain_channel, PIXEL_INDEX, np.newaxis]
```

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/containers.py` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/containers.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 from ctapipe.containers import ArrayEventContainer
 
 __all__ = [
     'NectarCAMContainer',
     'NectarCAMCameraContainer',
 ]
 
+class NectarCAMDataStreamContainer(Container):
+    """
+    Container for the Fields that are from the DataStream information (new from v6)
+    """
+    telescope_id = Field(-1,"telescope id")
+    sb_id = Field(-1,"Scheduling block ID")
+    obs_id = Field(-1,"Observation ID")
+    waveform_scale = Field(1.,"Scaling factor to apply to the waveform data from the EVB")
+    waveform_offset = Field(0.,"Offset to apply to the waveform data from the EVB")
 
 class NectarCAMServiceContainer(Container):
     """
     Container for Fields that are specific to each NectarCAM camera configuration
     """
 
     # Data from the CameraConfig table
@@ -29,14 +38,25 @@
     idaq_version = Field(0o0, "idaq version")
     cdhs_version = Field(0o0, "cdhs version")
     acquisition_mode = Field(-1, "acquisition mode")
     algorithms = Field(None, "algorithms")
     # pre_proc_algorithms = Field(None, "pre processing algorithms")
     module_ids = Field([], "module ids")
     num_modules = Field(-1, "number of modules")
+    ## Add new fields for the EVB v6 :
+    num_channels = Field(-1, "number of channels")
+    calibration_service_id = Field(-1,"calibration service id")
+    tdp_type = Field([],"tdp type")
+    tdp_action = Field([],"tdp action")
+    ttype_pattern = Field([],"tdp type")
+
+    run_id = Field(-1,"run number")
+
+
+
 
 
 class NectarCAMEventContainer(Container):
     """
     Container for Fields that are specific to each NectarCAM event
     """
 
@@ -79,21 +99,25 @@
     feb_pps_cnt = Field(None, "FEB count of PPS")
     feb_ts1 = Field(None, "FEB TS1")
     feb_ts2_trig = Field(None, "FEB TS2 Trigger Shift")
     feb_ts2_pps = Field(None, "FEB TS2 PPS Shift")
     trigger_pattern =  Field(None, "FEB L0 trigger pattern")
     native_charge = Field(None, "FEB native charge")
 
+    # new in v6
+    first_cell_id = Field(None,'ID of the first NECTAr read cell')
+
 class NectarCAMCameraContainer(Container):
     """
     Container for Fields that are specific to each NectarCAM camera
     """
     evt = Field(NectarCAMEventContainer(), "NectarCAM specific event Information")
     svc = Field(NectarCAMServiceContainer(), "NectarCAM specific camera_config "
                                              "Information")
+    dst = Field(NectarCAMDataStreamContainer(), "NectarCAM specific datastream Information")
 
 
 class NectarCAMContainer(Container):
     """
     Storage for the NectarCAMCameraContainer for each telescope
     """
     tels_with_data = Field([], "list of telescopes with data")
```

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155_ctapipe018.hdf5` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155_ctapipe018.hdf5`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/tests/test_trigger_patches.py` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/tests/test_trigger_patches.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam/version.py` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam/version.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam.egg-info/PKG-INFO` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctapipe_io_nectarcam
-Version: 0.1.4
+Version: 0.1.5
 Summary: ctapipe plugin for reading NectarCam files
 Author: NectarCAM collaboration
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/cta-observatory/ctapipe_io_nectarcam/issues
 Project-URL: Source Code, https://github.com/cta-observatory/ctapipe_io_nectarcam
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -24,23 +24,24 @@
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Provides-Extra: all
 Requires-Dist: ctapipe_io_nectarcam[dev,test]; extra == "all"
 
-[![CI](https://github.com/cta-observatory/ctapipe_io_nectarcam/workflows/CI/badge.svg?branch=master)](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions?query=workflow%3ACI+branch%3Amaster)
+[![CI](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions/workflows/ci.yml?query=workflow%3ACI+branch%3Amain)
 
 EventSource Plugin for ctapipe, able to read NectarCam zfits files
 and calibrate them to R1 as needed for ctapipe tools.
 
 To install into an existing environment, just do:
 ```shell
 pip install .
 ```
 
 For development, create a new environment and run the development install:
 ```shell
 conda env create -n nectar-dev -f environment.yml
 conda activate nectar-dev
 pip install -e .
+pre-commit install
 ```
```

### Comparing `ctapipe_io_nectarcam-0.1.4/src/ctapipe_io_nectarcam.egg-info/SOURCES.txt` & `ctapipe_io_nectarcam-0.1.5/src/ctapipe_io_nectarcam.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE.md
 MANIFEST.in
 README.md
 environment.yml
 pyproject.toml
 .github/release-drafter.yml
 .github/workflows/ci.yml
```

