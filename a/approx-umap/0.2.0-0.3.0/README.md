# Comparing `tmp/approx_umap-0.2.0.tar.gz` & `tmp/approx_umap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approx_umap-0.2.0.tar", max compression
+gzip compressed data, was "approx_umap-0.3.0.tar", max compression
```

## Comparing `approx_umap-0.2.0.tar` & `approx_umap-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1505 2024-04-03 17:09:04.702968 approx_umap-0.2.0/LICENSE
--rw-r--r--   0        0        0     2279 2024-05-22 21:58:28.949239 approx_umap-0.2.0/README.md
--rw-r--r--   0        0        0       46 2024-04-14 07:53:15.581717 approx_umap-0.2.0/approx_umap/__init__.py
--rw-r--r--   0        0        0     9282 2024-05-22 21:43:34.075895 approx_umap-0.2.0/approx_umap/approx_umap.py
--rw-r--r--   0        0        0      751 2024-05-22 21:57:02.008039 approx_umap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 approx_umap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-04-03 17:09:04.702968 approx_umap-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3254 2024-05-29 15:06:55.050278 approx_umap-0.3.0/README.md
+-rw-r--r--   0        0        0      109 2024-05-29 12:50:34.415840 approx_umap-0.3.0/approx_umap/__init__.py
+-rw-r--r--   0        0        0     8176 2024-05-29 14:47:21.789882 approx_umap-0.3.0/approx_umap/approx_aligned_umap.py
+-rw-r--r--   0        0        0     8784 2024-05-29 14:23:01.272888 approx_umap-0.3.0/approx_umap/approx_umap.py
+-rw-r--r--   0        0        0      960 2024-05-29 14:35:35.781364 approx_umap-0.3.0/approx_umap/functions.py
+-rw-r--r--   0        0        0    10902 2024-05-29 12:25:23.877307 approx_umap-0.3.0/approx_umap/temp.py
+-rw-r--r--   0        0        0      751 2024-05-29 15:07:30.780884 approx_umap-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 approx_umap-0.3.0/PKG-INFO
```

### Comparing `approx_umap-0.2.0/LICENSE` & `approx_umap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `approx_umap-0.2.0/README.md` & `approx_umap-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Approximate UMAP
 
 Modification of the UMAP algorithm to allow for fast approximate projections of
 new data points.
 
 ## Description
 
-This package provides a class `ApproxUMAP` that allows for fast approximate projections of new data points in the target
+This package provides the classes `ApproxUMAP` and `ApproxAlignedUMAP` that allow for fast approximate projections of
+new data points in the target
 space.
 
 The `fit` and `fit_transform` methods of `ApproxUMAP` are nearly identical to those of `umap.UMAP`;
 they simply fit an additional `sklearn.neighbors.NearestNeighbors` estimator.
 
 Only the `transform` method significantly differs; it approximates the projection of new data points
 in the embedding space to improve the projection speed.
@@ -20,14 +21,16 @@
 Formally, the projection of a new point $x$ is approximated as follows:
 $$u=\sum_i^k\frac{f(k d_i)}{\sum_j^kf(k d_j)}u_i$$
 with $x_1\dots x_k$ the $k$ nearest neighbours of $x$ in the source space
 among the points used for training (i.e., passed to `fit` or `fit_transform`),
 $d_i=distance(x, x_i)$, $u_1\dots u_i$ the exact UMAP projections of $x_1\dots x_k$, and $k$ the temperature parameter.
 The function $f(\cdot)$ corresponds to $\frac{1}{\cdot}$ if `fn='inv'`, and to $\frac{1}{e^{\cdot}}$ if `fn='exp'`.
 
+The original behavior of UMAP's `transform` method can be obtained using the `transform_exact` method.
+
 ## Installation
 
 The package can be installed via pip:
 
 ```bash
 pip install approx-umap
 ```
@@ -38,16 +41,40 @@
 transformer:
 
 ```python
 import numpy as np
 from approx_umap import ApproxUMAP
 
 X = np.random.rand(100, 10)
+
 emb_exact = ApproxUMAP(fn='exp', k=1).fit_transform(X)  # exact UMAP projections
-emb_approx = ApproxUMAP(fn='exp', k=1).fit(X).transform(X)  # approximate UMAP projection
+
+projector = ApproxUMAP(fn='exp', k=1).fit(X)
+emb_approx = projector.transform(X)  # approximate UMAP projection
+emb_approx_exact = projector.transform_exact(X)  # exact UMAP projection
+```
+
+The class `ApproxAlignedUMAP` additionally implements the methods `update` and `update_transform`
+to created aligned embeddings of new data points with respect to the training data.
+
+```python
+import numpy as np
+from approx_umap import ApproxAlignedUMAP
+
+X = np.random.rand(100, 10)
+X_new = np.random.rand(10, 10)
+
+emb_exact = ApproxAlignedUMAP(fn='exp', k=1).fit_transform(X)  # exact UMAP projections
+
+projector = ApproxAlignedUMAP(fn='exp', k=1).fit(X)
+
+emb_aligned = projector.update_transform(X_new)  # exact aligned UMAP projections
+assert emb_aligned.shape[0] == X.shape[0] + X_new.shape[0]  # returns the aligned embeddings of the whole history
+
+emb_approx_aligned = projector.transform(X_new)  # approximate aligned UMAP projections
 ```
 
 ## Citation
 
 Please, cite this work as:
 
 ```bibtex
```

### Comparing `approx_umap-0.2.0/approx_umap/approx_umap.py` & `approx_umap-0.3.0/approx_umap/approx_umap.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 #
 # License: BSD 3 clause
 import numpy as np
 from umap import UMAP
 from sklearn.neighbors import NearestNeighbors
 from docstring_inheritance import NumpyDocstringInheritanceMeta
 
+from approx_umap.functions import approximate_embedding
+
 
 class ApproxUMAP(UMAP, metaclass=NumpyDocstringInheritanceMeta):
     """Approximate UMAP
 
     Parameters
     ----------
     k: float
@@ -102,34 +104,26 @@
             dens_frac=dens_frac,
             dens_var_shift=dens_var_shift,
             output_dens=output_dens,
             disconnection_distance=disconnection_distance,
             precomputed_knn=precomputed_knn,
         )
         self.k = k
-        self._fn = fn
+        self.fn = fn
         self._knn = NearestNeighbors(
             n_neighbors=self.n_neighbors,
             # radius=1.0,
             # leaf_size=30,
             algorithm="auto",
             metric=self.metric,
             # p=2, Use  metric_params={'p': 3} instead
             metric_params=self.metric_kwds,
             n_jobs=self.n_jobs,
         )
 
-    def fn(self, d):
-        epsilon = 1e-8
-        if self._fn == "inv":
-            return 1 / (d + epsilon)
-        if self._fn == "exp":
-            return np.exp(-d) + epsilon
-        return self._fn(d)
-
     def fit(self, X, y=None, force_all_finite=True):
         """Fit X into an embedded space.
 
         Optionally use y for supervised dimension reduction.
 
         Parameters
         ----------
@@ -212,25 +206,18 @@
             New data to be transformed.
 
         Returns
         -------
         X_new : array, shape (n_samples, n_components)
             Approximate embedding of the new data in low-dimensional space.
         """
-        n_neighbors = min(self._knn.n_neighbors, self.embedding_.shape[0])
-        neigh_dist, neigh_ind = self._knn.kneighbors(
-            X, n_neighbors=n_neighbors, return_distance=True)
-        neigh_emb = self.embedding_[neigh_ind]
-        neigh_sim = self.fn(neigh_dist * self.k)
-        emb = np.sum(neigh_sim[:, :, None] / neigh_sim.sum(axis=1)[:, None, None] * neigh_emb,
-                     axis=1)
-        return emb
+        return approximate_embedding(X, self._knn, self.embedding_, self.k, self.fn)
 
     def transform_exact(self, X, force_all_finite=True):
-        """Original exact tronsform method from UMAP.
+        """Original exact transform method from UMAP.
 
         Parameters
         ----------
         X : array, shape (n_samples, n_features)
             New data to be transformed.
 
         force_all_finite : Whether to raise an error on np.inf, np.nan, pd.NA in array.
```

### Comparing `approx_umap-0.2.0/pyproject.toml` & `approx_umap-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "approx-umap"
-version = "0.2.0"
+version = "0.3.0"
 description = "Modification of the UMAP algorithm to allow for fast approximate projections of new data points."
 authors = [
     "Pierre Guetschel <pierre.guetschel@donders.ru.nl>",
     "Peter Wassenaar <peter.wassenaar@ru.nl>",
 ]
 readme = "README.md"
 packages = [{ include = "approx_umap" }]
```

### Comparing `approx_umap-0.2.0/PKG-INFO` & `approx_umap-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approx-umap
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modification of the UMAP algorithm to allow for fast approximate projections of new data points.
 Home-page: https://github.com/PierreGtch/approx-umap
 License: BSD-3-Clause
 Author: Pierre Guetschel
 Author-email: pierre.guetschel@donders.ru.nl
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: BSD License
@@ -19,15 +19,16 @@
 # Approximate UMAP
 
 Modification of the UMAP algorithm to allow for fast approximate projections of
 new data points.
 
 ## Description
 
-This package provides a class `ApproxUMAP` that allows for fast approximate projections of new data points in the target
+This package provides the classes `ApproxUMAP` and `ApproxAlignedUMAP` that allow for fast approximate projections of
+new data points in the target
 space.
 
 The `fit` and `fit_transform` methods of `ApproxUMAP` are nearly identical to those of `umap.UMAP`;
 they simply fit an additional `sklearn.neighbors.NearestNeighbors` estimator.
 
 Only the `transform` method significantly differs; it approximates the projection of new data points
 in the embedding space to improve the projection speed.
@@ -38,14 +39,16 @@
 Formally, the projection of a new point $x$ is approximated as follows:
 $$u=\sum_i^k\frac{f(k d_i)}{\sum_j^kf(k d_j)}u_i$$
 with $x_1\dots x_k$ the $k$ nearest neighbours of $x$ in the source space
 among the points used for training (i.e., passed to `fit` or `fit_transform`),
 $d_i=distance(x, x_i)$, $u_1\dots u_i$ the exact UMAP projections of $x_1\dots x_k$, and $k$ the temperature parameter.
 The function $f(\cdot)$ corresponds to $\frac{1}{\cdot}$ if `fn='inv'`, and to $\frac{1}{e^{\cdot}}$ if `fn='exp'`.
 
+The original behavior of UMAP's `transform` method can be obtained using the `transform_exact` method.
+
 ## Installation
 
 The package can be installed via pip:
 
 ```bash
 pip install approx-umap
 ```
@@ -56,16 +59,40 @@
 transformer:
 
 ```python
 import numpy as np
 from approx_umap import ApproxUMAP
 
 X = np.random.rand(100, 10)
+
 emb_exact = ApproxUMAP(fn='exp', k=1).fit_transform(X)  # exact UMAP projections
-emb_approx = ApproxUMAP(fn='exp', k=1).fit(X).transform(X)  # approximate UMAP projection
+
+projector = ApproxUMAP(fn='exp', k=1).fit(X)
+emb_approx = projector.transform(X)  # approximate UMAP projection
+emb_approx_exact = projector.transform_exact(X)  # exact UMAP projection
+```
+
+The class `ApproxAlignedUMAP` additionally implements the methods `update` and `update_transform`
+to created aligned embeddings of new data points with respect to the training data.
+
+```python
+import numpy as np
+from approx_umap import ApproxAlignedUMAP
+
+X = np.random.rand(100, 10)
+X_new = np.random.rand(10, 10)
+
+emb_exact = ApproxAlignedUMAP(fn='exp', k=1).fit_transform(X)  # exact UMAP projections
+
+projector = ApproxAlignedUMAP(fn='exp', k=1).fit(X)
+
+emb_aligned = projector.update_transform(X_new)  # exact aligned UMAP projections
+assert emb_aligned.shape[0] == X.shape[0] + X_new.shape[0]  # returns the aligned embeddings of the whole history
+
+emb_approx_aligned = projector.transform(X_new)  # approximate aligned UMAP projections
 ```
 
 ## Citation
 
 Please, cite this work as:
 
 ```bibtex
```

