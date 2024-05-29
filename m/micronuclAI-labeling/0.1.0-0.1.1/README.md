# Comparing `tmp/micronuclai_labeling-0.1.0.tar.gz` & `tmp/micronuclai_labeling-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micronuclai_labeling-0.1.0.tar", last modified: Thu May 23 08:05:23 2024, max compression
+gzip compressed data, was "micronuclai_labeling-0.1.1.tar", last modified: Wed May 29 13:22:23 2024, max compression
```

## Comparing `micronuclai_labeling-0.1.0.tar` & `micronuclai_labeling-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:05:23.174118 micronuclai_labeling-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-23 08:05:16.000000 micronuclai_labeling-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-23 08:05:16.000000 micronuclai_labeling-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-23 08:05:23.174118 micronuclai_labeling-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 08:05:16.000000 micronuclai_labeling-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-23 08:05:16.000000 micronuclai_labeling-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:05:23.174118 micronuclai_labeling-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:05:23.170118 micronuclai_labeling-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:05:16.000000 micronuclai_labeling-0.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:05:23.174118 micronuclai_labeling-0.1.0/src/micronuclAI_labeling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-23 08:05:23.000000 micronuclai_labeling-0.1.0/src/micronuclAI_labeling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-23 08:05:23.000000 micronuclai_labeling-0.1.0/src/micronuclAI_labeling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:05:23.000000 micronuclai_labeling-0.1.0/src/micronuclAI_labeling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 08:05:23.000000 micronuclai_labeling-0.1.0/src/micronuclAI_labeling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 08:05:23.000000 micronuclai_labeling-0.1.0/src/micronuclAI_labeling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:05:23.170118 micronuclai_labeling-0.1.0/src/micronuclai_labeling/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 08:05:16.000000 micronuclai_labeling-0.1.0/src/micronuclai_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-23 08:05:16.000000 micronuclai_labeling-0.1.0/src/micronuclai_labeling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-23 08:05:16.000000 micronuclai_labeling-0.1.0/src/micronuclai_labeling/_labeling_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:22:23.374619 micronuclai_labeling-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-29 13:22:15.000000 micronuclai_labeling-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 13:22:15.000000 micronuclai_labeling-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-29 13:22:23.374619 micronuclai_labeling-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-29 13:22:15.000000 micronuclai_labeling-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-29 13:22:15.000000 micronuclai_labeling-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:22:23.374619 micronuclai_labeling-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:22:23.370619 micronuclai_labeling-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:22:15.000000 micronuclai_labeling-0.1.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:22:23.370619 micronuclai_labeling-0.1.1/src/micronuclAI_labeling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-29 13:22:23.000000 micronuclai_labeling-0.1.1/src/micronuclAI_labeling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-29 13:22:23.000000 micronuclai_labeling-0.1.1/src/micronuclAI_labeling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:22:23.000000 micronuclai_labeling-0.1.1/src/micronuclAI_labeling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 13:22:23.000000 micronuclai_labeling-0.1.1/src/micronuclAI_labeling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 13:22:23.000000 micronuclai_labeling-0.1.1/src/micronuclAI_labeling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:22:23.370619 micronuclai_labeling-0.1.1/src/micronuclai_labeling/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 13:22:15.000000 micronuclai_labeling-0.1.1/src/micronuclai_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-29 13:22:15.000000 micronuclai_labeling-0.1.1/src/micronuclai_labeling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-29 13:22:15.000000 micronuclai_labeling-0.1.1/src/micronuclai_labeling/_labeling_tool.py
```

### Comparing `micronuclai_labeling-0.1.0/LICENSE` & `micronuclai_labeling-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micronuclai_labeling-0.1.0/PKG-INFO` & `micronuclai_labeling-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micronuclAI_labeling
-Version: 0.1.0
+Version: 0.1.1
 Summary: GUI tool for labeling micronuclei images
 Author-email: "Miguel A. Ibarra-Arellano" <c180l058j@mozmail.com>
 Project-URL: Homepage, https://github.com/SchapiroLabor/micronuclAI_labeling
 Project-URL: Issues, https://github.com/SchapiroLabor/micronuclAI_labeling/issues
 Keywords: micronuclei,labeling,gui
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,26 +25,19 @@
 # micronuclAI labeling tool
 [![PyPI](https://img.shields.io/pypi/v/micronuclAI_labeling?style=flat-square)](https://pypi.org/project/micronuclAI_labeling/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/micronuclAI_labeling?style=flat-square)](https://pypi.org/project/micronuclAI_labeling/)
 [![PyPI - License](https://img.shields.io/pypi/l/micronuclAI_labeling?style=flat-square)](https://pypi.org/project/micronuclAI_labeling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/micronuclAI_labeling?style=flat-square)](https://pypi.org/project/micronuclAI_labeling/)
 
 ## Installation
+On your preferred python environment, run the following command:
+
 ``` bash
 pip install micronuclAI-labeling
 ```
-
-## Requirements
-- Python >= 3.9
-- numpy
-- matplotlib
-- scikit-image
-- PySimpleGUI
-- mask2bbox
-
 ## Usage
 
 To launch micronuclAI labeling tool, run the following command:
 
 ``` bash
 python -m micronuclai_labeling --input path/to/image --mask path/to/mask --out path/to/outfile.csv
 ```
@@ -55,8 +48,12 @@
 
 The key 0 for no micro-nuclei present.  
 The keys 1-9 for the number of observed micro-nuclei in the image.  
 The key r is used to go back one image (in case any labeling mistake occurs).  
 
 **NOTE:** Labeling doesn't have to be done in one session, it can be resumed later on.  
 **NOTE:** Once labeling is complete the tool will not initiate.  
-**NOTE:** Output, Input and Mask paths are required and must be the same in order to resume labeling.  
+**NOTE:** Output, Input and Mask paths are required and must be the same in order to resume labeling.
+
+## License
+
+micronuclAI labeling tool offers a dual licensing mode the [GNU Affero General Public License v3.0](LICENSE) - see [LICENSE](LICENSE) and [ESSENTIAL_LICENSE_CONDITIONS.txt](ESSENTIAL_LICENSE_CONDITIONS.txt)
```

### Comparing `micronuclai_labeling-0.1.0/pyproject.toml` & `micronuclai_labeling-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micronuclAI_labeling"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Miguel A. Ibarra-Arellano", email="c180l058j@mozmail.com"},
 ]
 description = "GUI tool for labeling micronuclei images"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `micronuclai_labeling-0.1.0/src/micronuclAI_labeling.egg-info/PKG-INFO` & `micronuclai_labeling-0.1.1/src/micronuclAI_labeling.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micronuclAI_labeling
-Version: 0.1.0
+Version: 0.1.1
 Summary: GUI tool for labeling micronuclei images
 Author-email: "Miguel A. Ibarra-Arellano" <c180l058j@mozmail.com>
 Project-URL: Homepage, https://github.com/SchapiroLabor/micronuclAI_labeling
 Project-URL: Issues, https://github.com/SchapiroLabor/micronuclAI_labeling/issues
 Keywords: micronuclei,labeling,gui
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,26 +25,19 @@
 # micronuclAI labeling tool
 [![PyPI](https://img.shields.io/pypi/v/micronuclAI_labeling?style=flat-square)](https://pypi.org/project/micronuclAI_labeling/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/micronuclAI_labeling?style=flat-square)](https://pypi.org/project/micronuclAI_labeling/)
 [![PyPI - License](https://img.shields.io/pypi/l/micronuclAI_labeling?style=flat-square)](https://pypi.org/project/micronuclAI_labeling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/micronuclAI_labeling?style=flat-square)](https://pypi.org/project/micronuclAI_labeling/)
 
 ## Installation
+On your preferred python environment, run the following command:
+
 ``` bash
 pip install micronuclAI-labeling
 ```
-
-## Requirements
-- Python >= 3.9
-- numpy
-- matplotlib
-- scikit-image
-- PySimpleGUI
-- mask2bbox
-
 ## Usage
 
 To launch micronuclAI labeling tool, run the following command:
 
 ``` bash
 python -m micronuclai_labeling --input path/to/image --mask path/to/mask --out path/to/outfile.csv
 ```
@@ -55,8 +48,12 @@
 
 The key 0 for no micro-nuclei present.  
 The keys 1-9 for the number of observed micro-nuclei in the image.  
 The key r is used to go back one image (in case any labeling mistake occurs).  
 
 **NOTE:** Labeling doesn't have to be done in one session, it can be resumed later on.  
 **NOTE:** Once labeling is complete the tool will not initiate.  
-**NOTE:** Output, Input and Mask paths are required and must be the same in order to resume labeling.  
+**NOTE:** Output, Input and Mask paths are required and must be the same in order to resume labeling.
+
+## License
+
+micronuclAI labeling tool offers a dual licensing mode the [GNU Affero General Public License v3.0](LICENSE) - see [LICENSE](LICENSE) and [ESSENTIAL_LICENSE_CONDITIONS.txt](ESSENTIAL_LICENSE_CONDITIONS.txt)
```

### Comparing `micronuclai_labeling-0.1.0/src/micronuclai_labeling/__main__.py` & `micronuclai_labeling-0.1.1/src/micronuclai_labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `micronuclai_labeling-0.1.0/src/micronuclai_labeling/_labeling_tool.py` & `micronuclai_labeling-0.1.1/src/micronuclai_labeling/_labeling_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # labeling_tool.py
 import PySimpleGUI as sg
 from PIL import Image
 from os.path import dirname, exists
 from pathlib import Path
-from matplotlib import cm
+from matplotlib import colormaps as cm
 from mask2bbox import BBoxes
 import numpy as np
 import io
 
 
 def array2image(array, cmap="gray", size=(256, 256)):
     # https: // stackoverflow.com / questions / 10965417 / how - to - convert - a - numpy - array - to - pil - image - applying - matplotlib - colormap
```

