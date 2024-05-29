# Comparing `tmp/pldag-0.8.5.tar.gz` & `tmp/pldag-0.8.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.5.tar", max compression
+gzip compressed data, was "pldag-0.8.51.tar", max compression
```

## Comparing `pldag-0.8.5.tar` & `pldag-0.8.51.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.5/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.5/README.md
--rw-r--r--   0        0        0    46376 2024-05-29 11:16:58.151828 pldag-0.8.5/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.5/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.5/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-05-29 11:17:07.674390 pldag-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.51/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.51/README.md
+-rw-r--r--   0        0        0    46384 2024-05-29 12:38:45.208109 pldag-0.8.51/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.51/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.51/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      400 2024-05-29 12:38:59.513284 pldag-0.8.51/pyproject.toml
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 pldag-0.8.51/PKG-INFO
```

### Comparing `pldag-0.8.5/LICENSE` & `pldag-0.8.51/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.5/README.md` & `pldag-0.8.51/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.5/pldag/__init__.py` & `pldag-0.8.51/pldag/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1282,9 +1282,9 @@
     def sub(self, roots: List[str], max_iterations: int = 1000) -> 'Puan':
         new_model = self.from_super(super().sub(roots, max_iterations))
         new_model.data = dict(filter(lambda k: k[0] in new_model._imap, self.data.items()))
         return new_model
         
     def cut(self, cuts: Dict[str, str]) -> "Puan":
         new_model = self.from_super(super().cut(cuts))
-        new_model.data = dict(filter(lambda k: k[0] in new_model._imap, self.data))
+        new_model.data = dict(filter(lambda k: k[0] in new_model._imap, self.data.items()))
         return new_model
```

### Comparing `pldag-0.8.5/pldag/solver/glpk_solver.py` & `pldag-0.8.51/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.5/PKG-INFO` & `pldag-0.8.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.5
+Version: 0.8.51
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

