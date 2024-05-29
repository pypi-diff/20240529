# Comparing `tmp/py_distance_transforms-0.2.2.tar.gz` & `tmp/py_distance_transforms-0.2.3.tar.gz`

## Comparing `py_distance_transforms-0.2.2.tar` & `py_distance_transforms-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/.gitattributes
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/.python-version
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/requirements-dev.lock
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/requirements.lock
--rw-r--r--   0        0        0   361292 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/docs/getting_started.ipynb
--rw-r--r--   0        0        0   233221 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/docs/hausdorff_loss.ipynb
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/py_distance_transforms/__init__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/py_distance_transforms/julia_import.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/py_distance_transforms/juliapkg.json
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/py_distance_transforms/transform.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/py_distance_transforms/transform_cuda.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/.gitignore
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/.gitattributes
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/.python-version
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/requirements-dev.lock
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/requirements.lock
+-rw-r--r--   0        0        0   361292 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/docs/getting_started.ipynb
+-rw-r--r--   0        0        0   235100 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/docs/hausdorff_loss.ipynb
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/py_distance_transforms/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/py_distance_transforms/julia_import.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/py_distance_transforms/juliapkg.json
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/py_distance_transforms/transform.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/py_distance_transforms/transform_cuda.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/.gitignore
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 py_distance_transforms-0.2.3/PKG-INFO
```

### Comparing `py_distance_transforms-0.2.2/requirements-dev.lock` & `py_distance_transforms-0.2.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `py_distance_transforms-0.2.2/requirements.lock` & `py_distance_transforms-0.2.3/requirements.lock`

 * *Files identical despite different names*

### Comparing `py_distance_transforms-0.2.2/docs/getting_started.ipynb` & `py_distance_transforms-0.2.3/docs/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `py_distance_transforms-0.2.2/README.md` & `py_distance_transforms-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `py_distance_transforms-0.2.2/pyproject.toml` & `py_distance_transforms-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py_distance_transforms"
-version = "0.2.2"
+version = "0.2.3"
 description = "Add your description here"
 authors = [
     { name = "Dale Black", email = "djblack@uci.edu" }
 ]
 dependencies = [
     "juliacall>=0.9.20",
     "numpy>=1.25.0",
```

### Comparing `py_distance_transforms-0.2.2/PKG-INFO` & `py_distance_transforms-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py_distance_transforms
-Version: 0.2.2
+Version: 0.2.3
 Summary: Add your description here
 Author-email: Dale Black <djblack@uci.edu>
 Requires-Python: >=3.8
 Requires-Dist: juliacall>=0.9.20
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: torch>=2.2.0
 Description-Content-Type: text/markdown
```

