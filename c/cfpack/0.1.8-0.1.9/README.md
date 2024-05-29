# Comparing `tmp/cfpack-0.1.8.tar.gz` & `tmp/cfpack-0.1.9.tar.gz`

## Comparing `cfpack-0.1.8.tar` & `cfpack-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack.browser_control.html
--rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack.html
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.8/pyproject.toml.new
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.8/pyproject.toml.old
--rw-r--r--   0        0        0    57571 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/__init__.py
--rwxr-xr-x   0        0        0     6551 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/automator.py
--rwxr-xr-x   0        0        0     5236 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/browser_control.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/constants.py
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/hdfio.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/matplotlibrc.py
--rwxr-xr-x   0        0        0     2772 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/tests.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.1.8/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.1.8/LICENSE
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cfpack-0.1.8/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 cfpack-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.9/pyproject.toml.new
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.9/pyproject.toml.old
+-rw-r--r--   0        0        0    57644 2020-02-02 00:00:00.000000 cfpack-0.1.9/cfpack/__init__.py
+-rwxr-xr-x   0        0        0     6551 2020-02-02 00:00:00.000000 cfpack-0.1.9/cfpack/automator.py
+-rwxr-xr-x   0        0        0     5236 2020-02-02 00:00:00.000000 cfpack-0.1.9/cfpack/browser_control.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.1.9/cfpack/constants.py
+-rwxr-xr-x   0        0        0     3463 2020-02-02 00:00:00.000000 cfpack-0.1.9/cfpack/hdfio.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 cfpack-0.1.9/cfpack/matplotlibrc.py
+-rwxr-xr-x   0        0        0     2772 2020-02-02 00:00:00.000000 cfpack-0.1.9/cfpack/tests.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.1.9/LICENSE
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cfpack-0.1.9/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 cfpack-0.1.9/PKG-INFO
```

### Comparing `cfpack-0.1.8/pyproject.toml.new` & `cfpack-0.1.9/pyproject.toml.old`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.1.8/pyproject.toml.old` & `cfpack-0.1.9/pyproject.toml.new`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.1.7"
+version = "0.1.9"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.1.8/cfpack/__init__.py` & `cfpack-0.1.9/cfpack/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# written by Christoph Federrath, 2019-2023
+# written by Christoph Federrath, 2019-2024
 
 import numpy as np
 np.set_printoptions(linewidth=200) # increase the numpy printing linewidth a bit
 
 from . import constants as const # physical constants
-from . import matplotlibrc # set default plotting style
 
 # so we can call stop() to drop a script into interactive mode
 try:
     from ipdb import set_trace as stop # interactive python debugger
 except:
     from pdb import set_trace as stop # python debugger
 
+
+# === setup default cfpack plot styles ===
+def load_plot_styles():
+    from . import matplotlibrc # set default plotting style
+
 # === START print ===
 # custom print() function override to show caller (module and function) information before actual print string,
 # plus options colourised output
 def print(*args, error=False, warn=False, highlight=False, color="", input=False, no_prefix=False, **kwargs):
     from builtins import print as builtin_print, input as builtin_input
     from inspect import currentframe, getouterframes
     from colorama import Fore, Style
```

### Comparing `cfpack-0.1.8/cfpack/automator.py` & `cfpack-0.1.9/cfpack/automator.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.8/cfpack/browser_control.py` & `cfpack-0.1.9/cfpack/browser_control.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.8/cfpack/constants.py` & `cfpack-0.1.9/cfpack/constants.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.8/cfpack/hdfio.py` & `cfpack-0.1.9/cfpack/hdfio.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,24 +16,31 @@
     dset = f[datasetname]
     shape = dset.shape
     f.close()
     return shape
 # ============= end: get_shape =============
 
 # ============= read =============
-# ind should be of type slice or np.s_ to index into the dataset,
-# order to take hyperslabs
-def read(filename, datasetname, ind=()):
+# ind should be of type slice or np.s_ to index into the dataset, in order to select hyperslabs;
+# return_attributes=True will return the dataset's attributes as a dictionary
+def read(filename, datasetname, ind=(), return_attributes=False):
     # open HDF5 file
     f = h5py.File(filename, "r")
     # grab the dataset as a numpy array (with requested index ind, if provided, else all)
     dset = f[datasetname]
-    data = np.array(dset[ind])
+    if return_attributes: # return attributes of this dataset as a dict
+        ret = {}
+        attr_keys = dset.attrs.keys()
+        for key in attr_keys:
+            val = dset.attrs.get(key)
+            ret[key] = val # add key and value
+    else: # return dataset content
+        ret = np.array(dset[ind])
     f.close()
-    return data
+    return ret
 # ============= end: read =============
 
 # ============= write =============
 def write(data, filename, datasetname, overwrite_file=False, overwrite_dataset=False):
     # first test if file exists
     openflag = "w"
     if os.path.isfile(filename):
```

### Comparing `cfpack-0.1.8/cfpack/matplotlibrc.py` & `cfpack-0.1.9/cfpack/matplotlibrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 rcParams['ytick.minor.pad'] = 5
 # legend
 rcParams['legend.fontsize'] = rcParams['font.size']
 rcParams['legend.labelspacing'] = 0.2
 rcParams['legend.loc'] = 'upper left'
 rcParams['legend.frameon'] = False
 # figure
-rcParams['figure.figsize'] = (7.0, 4.5)
+rcParams['figure.figsize'] = (5.5, 3.5)
 rcParams['figure.dpi'] = 150
 rcParams['savefig.dpi'] = 200
 rcParams['savefig.bbox'] = 'tight'
 # errorbars
 rcParams['errorbar.capsize'] = 1.5
```

### Comparing `cfpack-0.1.8/cfpack/tests.py` & `cfpack-0.1.9/cfpack/tests.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.8/LICENSE` & `cfpack-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.8/pyproject.toml` & `cfpack-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.1.8/PKG-INFO` & `cfpack-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cfpack
-Version: 0.1.8
+Version: 0.1.9
 Summary: Christoph Federrath (CF) python package (cfpack)
 Project-URL: Homepage, https://www.mso.anu.edu.au/~chfeder/codes/cfpack/cfpack.html
 Author-email: Christoph Federrath <christoph.federrath@anu.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Christoph Federrath
```

