# Comparing `tmp/pyswxf-0.6.5.tar.gz` & `tmp/pyswxf-0.6.6.tar.gz`

## Comparing `pyswxf-0.6.5.tar` & `pyswxf-0.6.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyswxf-0.6.5/PyPI-Recovery-Codes-luriol-2023-10-13T13_43_44.046510.txt
--rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.6.5/cbwe.py
--rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pyswxf-0.6.5/dot_pypirc
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 pyswxf-0.6.5/instructions
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 pyswxf-0.6.5/pyproject.bak
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.5/pyproject.new
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pyswxf-0.6.5/token
--rwxr-xr-x   0        0        0     5451 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py
--rwxr-xr-x   0        0        0    10605 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/AuI_funs.py
--rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/__init__.py
--rwxr-xr-x   0        0        0     8356 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/fluor_fit.py
--rwxr-xr-x   0        0        0     6752 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/niu_multilayer_fit_params_3_LBL.json
--rwxr-xr-x   0        0        0     6863 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/refl_funs.py
--rwxr-xr-x   0        0        0    23866 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/spec_utils.py
--rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/view_new_multilayer.ipynb
--rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/xray_utils.py
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.6.5/LICENSE
--rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 pyswxf-0.6.5/README.md
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 pyswxf-0.6.5/PKG-INFO
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyswxf-0.6.6/PyPI-Recovery-Codes-luriol-2023-10-13T13_43_44.046510.txt
+-rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.6.6/cbwe.py
+-rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pyswxf-0.6.6/dot_pypirc
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 pyswxf-0.6.6/instructions
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 pyswxf-0.6.6/pyproject.bak
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.6/pyproject.new
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pyswxf-0.6.6/token
+-rwxr-xr-x   0        0        0     5451 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py
+-rwxr-xr-x   0        0        0    13162 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/AuI_funs.py
+-rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/__init__.py
+-rwxr-xr-x   0        0        0     8356 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/fluor_fit.py
+-rwxr-xr-x   0        0        0     6752 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/niu_multilayer_fit_params_3_LBL.json
+-rwxr-xr-x   0        0        0     6863 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/refl_funs.py
+-rwxr-xr-x   0        0        0    24080 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/spec_utils.py
+-rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/view_new_multilayer.ipynb
+-rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 pyswxf-0.6.6/src/pySWXF/xray_utils.py
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.6.6/LICENSE
+-rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 pyswxf-0.6.6/README.md
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 pyswxf-0.6.6/PKG-INFO
```

### Comparing `pyswxf-0.6.5/dot_pypirc` & `pyswxf-0.6.6/dot_pypirc`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/pyproject.bak` & `pyswxf-0.6.6/pyproject.bak`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/pyproject.new` & `pyswxf-0.6.6/pyproject.new`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py` & `pyswxf-0.6.6/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json` & `pyswxf-0.6.6/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/src/pySWXF/fluor_fit.py` & `pyswxf-0.6.6/src/pySWXF/fluor_fit.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/src/pySWXF/niu_multilayer_fit_params_3_LBL.json` & `pyswxf-0.6.6/src/pySWXF/niu_multilayer_fit_params_3_LBL.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/src/pySWXF/refl_funs.py` & `pyswxf-0.6.6/src/pySWXF/refl_funs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/src/pySWXF/spec_utils.py` & `pyswxf-0.6.6/src/pySWXF/spec_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -694,11 +694,16 @@
      y += Au_L_peak(A_Au,sig,x)
      return y
 
 Br_background = LinearModel()
 Br_peak_mod = Model(Br_peak_sim)+Br_background
 
 def list_scans(filename):
-    with open(filename,'r') as fd:
-        for line in fd:
-            if line[0:2] == '#S':
-                print('{0:s}'.format(line))
+    try:
+        with open(filename, 'r') as fd:
+            for line in fd:
+                if line.startswith('#S'):
+                    print(line.strip())
+    except FileNotFoundError:
+        print(f"Error: The file '{filename}' was not found.")
+    except IOError:
+        print(f"Error: An error occurred while reading the file '{filename}'.")
```

### Comparing `pyswxf-0.6.5/src/pySWXF/view_new_multilayer.ipynb` & `pyswxf-0.6.6/src/pySWXF/view_new_multilayer.ipynb`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/src/pySWXF/xray_utils.py` & `pyswxf-0.6.6/src/pySWXF/xray_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/LICENSE` & `pyswxf-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/README.md` & `pyswxf-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.5/pyproject.toml` & `pyswxf-0.6.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling==1.17.1"]
 build-backend = "hatchling.build"
 [project]
 name = "pySWXF"
-version = "0.6.5"
+version = "0.6.6"
 authors = [
 	{name="Laurence Lurio", email="llurio@niu.edu" },
 ]
 description = "Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity"
 readme = "README.md"
 requires-python = ">3.7"
 classifiers = [
```

### Comparing `pyswxf-0.6.5/PKG-INFO` & `pyswxf-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySWXF
-Version: 0.6.5
+Version: 0.6.6
 Summary: Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity
 Project-URL: Homepage, https://github.com/pypa/pySWXF
 Project-URL: Bug Tracker, https://github.com/pypa/pySWXF/issues
 Author-email: Laurence Lurio <llurio@niu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

