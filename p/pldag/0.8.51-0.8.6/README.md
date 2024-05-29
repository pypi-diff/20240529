# Comparing `tmp/pldag-0.8.51.tar.gz` & `tmp/pldag-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.51.tar", max compression
+gzip compressed data, was "pldag-0.8.6.tar", max compression
```

## Comparing `pldag-0.8.51.tar` & `pldag-0.8.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.51/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.51/README.md
--rw-r--r--   0        0        0    46384 2024-05-29 12:38:45.208109 pldag-0.8.51/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.51/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.51/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      400 2024-05-29 12:38:59.513284 pldag-0.8.51/pyproject.toml
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 pldag-0.8.51/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-29 06:53:14.527873 pldag-0.8.6/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-29 06:53:14.528024 pldag-0.8.6/README.md
+-rw-r--r--   0        0        0    46473 2024-05-29 14:33:40.433748 pldag-0.8.6/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 06:53:14.528571 pldag-0.8.6/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-05-29 06:53:14.528701 pldag-0.8.6/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-05-29 14:33:40.434169 pldag-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.6/PKG-INFO
```

### Comparing `pldag-0.8.51/LICENSE` & `pldag-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.51/README.md` & `pldag-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.51/pldag/__init__.py` & `pldag-0.8.6/pldag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,18 +351,21 @@
         model._amap = self._amap.copy()
         return model
     
     def get(self, *id: str) -> np.ndarray:
         """Get the bounds of the given ID(s)"""
         return self._dvec[list(map(self._col, id))]
     
-    def delete(self, id: str) -> True:
+    def delete(self, *id: str) -> bool:
         """
             Delete the given ID.
         """
+        if len(id)>1:
+            return tuple(map(self.delete, id))
+        id = id[0]
         try:
             if id in self.composites:
                 row_id = self._row(id)
                 self._bvec = np.delete(self._bvec, row_id)
                 self._nvec = np.delete(self._nvec, row_id)
                 self._amap = dict(filter(lambda x: x[1] != id, self._amap.items()))
                 self._amat = np.delete(self._amat, row_id, axis=0)
```

### Comparing `pldag-0.8.51/pldag/solver/glpk_solver.py` & `pldag-0.8.6/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.51/PKG-INFO` & `pldag-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.51
+Version: 0.8.6
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

