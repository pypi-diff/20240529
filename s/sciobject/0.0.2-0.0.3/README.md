# Comparing `tmp/sciobject-0.0.2.tar.gz` & `tmp/sciobject-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciobject-0.0.2.tar", max compression
+gzip compressed data, was "sciobject-0.0.3.tar", max compression
```

## Comparing `sciobject-0.0.2.tar` & `sciobject-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1298 2024-05-27 08:59:13.510264 sciobject-0.0.2/LICENSE
--rw-r--r--   0        0        0      200 2024-05-27 08:59:13.514264 sciobject-0.0.2/README.md
--rw-r--r--   0        0        0      644 2024-05-29 11:28:22.507874 sciobject-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 11:04:55.328502 sciobject-0.0.2/sciobject/__init__.py
--rw-r--r--   0        0        0    12947 2024-05-29 11:28:02.439598 sciobject-0.0.2/sciobject/sciobject.py
--rw-r--r--   0        0        0     1006 2024-05-29 09:55:24.615094 sciobject-0.0.2/sciobject/test_sciobject.py
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 sciobject-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1298 2024-05-27 08:59:13.510264 sciobject-0.0.3/LICENSE
+-rw-r--r--   0        0        0      200 2024-05-27 08:59:13.514264 sciobject-0.0.3/README.md
+-rw-r--r--   0        0        0      644 2024-05-29 12:03:51.829214 sciobject-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 11:04:55.328502 sciobject-0.0.3/sciobject/__init__.py
+-rw-r--r--   0        0        0    12999 2024-05-29 12:03:19.032762 sciobject-0.0.3/sciobject/sciobject.py
+-rw-r--r--   0        0        0     1006 2024-05-29 09:55:24.615094 sciobject-0.0.3/sciobject/test_sciobject.py
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 sciobject-0.0.3/PKG-INFO
```

### Comparing `sciobject-0.0.2/LICENSE` & `sciobject-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sciobject-0.0.2/pyproject.toml` & `sciobject-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sciobject"
-version = "0.0.2"
+version = "0.0.3"
 description = "Abstract objects that save and log calculations."
 authors = ["Hana Zupan <h.zupan@fu-berlin.de>"]
 license = "LICENSE"
 readme = "README.md"
 keywords = ["scientific computing", "logging"]
 repository = "https://github.com/hanazupan/sciobject"
 homepage = "https://www.bcp.fu-berlin.de/en/chemie/chemie/forschung/PhysTheoChem/agkeller/index.html"
```

### Comparing `sciobject-0.0.2/sciobject/sciobject.py` & `sciobject-0.0.3/sciobject/sciobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         """
         Returns:
             A pandas dataframe including all instances that have been constructed so far.
         """
         return self._load_current_logbook()
 
     def get_class_index(self, use_saved: bool, parameter_names: list, parameter_values: list):
-        assert len(parameter_names) == len(parameter_values)
+        assert len(parameter_names) == len(parameter_values), f"len({parameter_values})!=len({parameter_names})"
         parameter_names_values = {n: v for n, v in zip(parameter_names, parameter_values)}
         new_entry = self._get_new_entry(parameter_names_values)
         if use_saved is True:
             # try finding an existing set of data
             existing_index = None
             for index, data in self.current_logbook.iterrows():
                 for i, row in new_entry.iterrows():
```

### Comparing `sciobject-0.0.2/sciobject/test_sciobject.py` & `sciobject-0.0.3/sciobject/test_sciobject.py`

 * *Files identical despite different names*

### Comparing `sciobject-0.0.2/PKG-INFO` & `sciobject-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciobject
-Version: 0.0.2
+Version: 0.0.3
 Summary: Abstract objects that save and log calculations.
 Home-page: https://www.bcp.fu-berlin.de/en/chemie/chemie/forschung/PhysTheoChem/agkeller/index.html
 License: LICENSE
 Keywords: scientific computing,logging
 Author: Hana Zupan
 Author-email: h.zupan@fu-berlin.de
 Requires-Python: >=3.9,<3.13
```

