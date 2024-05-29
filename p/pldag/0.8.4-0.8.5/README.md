# Comparing `tmp/pldag-0.8.4.tar.gz` & `tmp/pldag-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.4.tar", max compression
+gzip compressed data, was "pldag-0.8.5.tar", max compression
```

## Comparing `pldag-0.8.4.tar` & `pldag-0.8.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-05-29 06:53:14.527873 pldag-0.8.4/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-29 06:53:14.528024 pldag-0.8.4/README.md
--rw-r--r--   0        0        0    45839 2024-05-29 07:14:45.518551 pldag-0.8.4/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 06:53:14.528571 pldag-0.8.4/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-05-29 06:53:14.528701 pldag-0.8.4/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-05-29 07:14:10.308536 pldag-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.5/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.5/README.md
+-rw-r--r--   0        0        0    46376 2024-05-29 11:16:58.151828 pldag-0.8.5/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.5/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.5/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-05-29 11:17:07.674390 pldag-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.5/PKG-INFO
```

### Comparing `pldag-0.8.4/LICENSE` & `pldag-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.4/README.md` & `pldag-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.4/pldag/__init__.py` & `pldag-0.8.5/pldag/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -940,14 +940,15 @@
             Returns
             -------
             PLDAG
                 The sub-PLDAG.
         """
         sub_model = PLDAG()
         sub_model._amat = self._amat[row_idxs][:, col_idxs]
+        sub_model._wmat = self._wmat[row_idxs][:, col_idxs]
         sub_model._nvec = self._nvec[row_idxs]
         sub_model._dvec = self._dvec[col_idxs]
         sub_model._bvec = self._bvec[row_idxs]
         sub_model._cvec = self._cvec[col_idxs]
         sub_model._imap = dict(map(lambda x: (x[1], x[0]), enumerate(self._col_vars[col_idxs])))
         sub_model._amap = dict(filter(lambda x: x[1] in sub_model._imap, self._amap.items()))
         return sub_model
@@ -1144,14 +1145,27 @@
 
 class Puan(PLDAG):
 
     def __init__(self):
         super().__init__()
         self.data: dict = {}
 
+    def copy(self) -> "Puan":
+        new_model = Puan()
+        new_model._amat = self._amat.copy()
+        new_model._wmat = self._wmat.copy()
+        new_model._dvec = self._dvec.copy()
+        new_model._bvec = self._bvec.copy()
+        new_model._nvec = self._nvec.copy()
+        new_model._cvec = self._cvec.copy()
+        new_model._imap = self._imap.copy()
+        new_model._amap = self._amap.copy()
+        new_model.data = self.data.copy()
+        return new_model
+
     def set_meta(self, id: str, props: dict):
         self.data.setdefault(id, {}).update(props)
 
     def del_meta(self, id: str, key: str):
         self.data[id].pop(key, None)
 
     def set_primitive(self, id: str, properties: dict = {}, bound: complex = complex(0,1)) -> str:
```

### Comparing `pldag-0.8.4/pldag/solver/glpk_solver.py` & `pldag-0.8.5/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.4/PKG-INFO` & `pldag-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.4
+Version: 0.8.5
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

