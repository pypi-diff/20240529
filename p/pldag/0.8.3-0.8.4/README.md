# Comparing `tmp/pldag-0.8.3.tar.gz` & `tmp/pldag-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.3.tar", max compression
+gzip compressed data, was "pldag-0.8.4.tar", max compression
```

## Comparing `pldag-0.8.3.tar` & `pldag-0.8.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.3/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.3/README.md
--rw-r--r--   0        0        0    44814 2024-05-20 12:18:33.057582 pldag-0.8.3/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.3/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.3/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-05-20 12:31:45.429037 pldag-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-29 06:53:14.527873 pldag-0.8.4/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-29 06:53:14.528024 pldag-0.8.4/README.md
+-rw-r--r--   0        0        0    45839 2024-05-29 07:14:45.518551 pldag-0.8.4/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 06:53:14.528571 pldag-0.8.4/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-05-29 06:53:14.528701 pldag-0.8.4/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-05-29 07:14:10.308536 pldag-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.4/PKG-INFO
```

### Comparing `pldag-0.8.3/LICENSE` & `pldag-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.3/README.md` & `pldag-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.3/pldag/__init__.py` & `pldag-0.8.4/pldag/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,25 @@
         self._imap = {}
         # Alias to id mapping
         self._amap = {}
 
     def __hash__(self) -> int:
         return hash(self.sha1())
     
+    def __eq__(self, other: "PLDAG") -> bool:
+        return (self.sha1() == other.sha1()
+                and np.array_equal(self._amat, other._amat)
+                and np.array_equal(self._wmat, other._wmat)
+                and np.array_equal(self._nvec, other._nvec)
+                and np.array_equal(self._dvec, other._dvec)
+                and np.array_equal(self._bvec, other._bvec)
+                and np.array_equal(self._cvec, other._cvec)
+                and self._imap == other._imap
+                and self._amap == other._amap)
+
     def sha1(self) -> str:
         return sha1(("".join(self._imap.keys()) + "".join(map(lambda c: f"{c.real}{c.imag}", self._dvec))).encode()).hexdigest()
 
     @property
     def bounds(self) -> np.ndarray:
         """Get the bounds of all aliases"""
         return self._dvec
@@ -1036,43 +1047,49 @@
     
     def cut_sub(self, cuts: Dict[str, str], roots: List[str]) -> "PLDAG":
         """
             Cuts graph on given nodes in `cuts` and then creates a sub graph from the given root IDs.
         """
         return self.cut(cuts).sub(roots)
     
-    def solve(self, objectives: List[Dict[str, int]], assume: Dict[str, complex], solver: Solver) -> List[Dict[str, complex]]:
+    def solve(self, objectives: List[Dict[str, int]], assume: Dict[str, complex], solver: Solver, double_bind_constraints: bool = True) -> List[Dict[str, complex]]:
         """
             Solves the model with the given objectives.
 
             Parameters
             ----------
             objectives : List[Dict[str, int]]
                 The objectives to solve for.
 
             assume : Dict[str, complex]
                 Assume new bounds for variables.
 
             solver : Solver
                 The solver to use.
 
+            double_bind_constraints: bool = True
+                If the constraints should be double binded. That is, a constraint A -> x & y & z will become two constraints:
+                1 ) -dA + x + y + z >= 0
+                2 ) +mA - x - y - z >= -1
+                Saying that if A is 1 then x, y and z must be 1, and if A is 0 then x, y and z must be 0.
+
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xyz")
             >>> a = model.set_atleast("xyz", 1)
             >>> model.solve([{"x": 0, "y": 1, "z": 0}], {}, Solver.GLPK)
             [{'x': 0j, 'y': 1+1j, 'z': 0j}]
 
             Returns
             -------
             List[Dict[str, complex]]
                 The solutions for the objectives.
         """
-        A, b = self.to_polyhedron(double_binding=True, **assume)
+        A, b = self.to_polyhedron(double_binding=double_bind_constraints, **assume)
         variables = self._col_vars
         obj_mat = np.zeros((len(objectives), len(variables)), dtype=np.int64)
         for i, obj in enumerate(objectives):
             obj_mat[i, [self._col(k) for k in obj]] = list(obj.values())
 
         if solver == Solver.GLPK:
             from pldag.solver.glpk_solver import solve_lp
@@ -1206,26 +1223,26 @@
                         )
                     ),
                     self.data.items()
                 )
             )
         )
     
-    def solve(self, objectives: List[dict], assume: Dict[str, complex], solver: Solver) -> List[dict]:
+    def solve(self, objectives: List[dict], assume: Dict[str, complex], solver: Solver, double_bind_constraints: bool = True) -> List[dict]:
         return list(
             map(
                 lambda solution: Solution(
                     variables=list(
                         starmap(
                             lambda k,v: Variable(k, v, self.data.get(k, {}), self.id_to_alias(k) or None),
                             solution.items()
                         )
                     )
                 ),
-                super().solve(objectives, assume, solver)
+                super().solve(objectives, assume, solver, double_bind_constraints)
             )
         )
     
     def propagate(self, query: dict = {}, freeze: bool = True) -> Solution:
         return Solution(
             variables=list(
                 starmap(
@@ -1253,8 +1270,7 @@
         new_model.data = dict(filter(lambda k: k[0] in new_model._imap, self.data.items()))
         return new_model
         
     def cut(self, cuts: Dict[str, str]) -> "Puan":
         new_model = self.from_super(super().cut(cuts))
         new_model.data = dict(filter(lambda k: k[0] in new_model._imap, self.data))
         return new_model
-
```

### Comparing `pldag-0.8.3/pldag/solver/glpk_solver.py` & `pldag-0.8.4/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.3/PKG-INFO` & `pldag-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.3
+Version: 0.8.4
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

