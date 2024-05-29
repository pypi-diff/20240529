# Comparing `tmp/nadl-1.4.9.tar.gz` & `tmp/nadl-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.4.9.tar", last modified: Mon May 27 18:52:56 2024, max compression
+gzip compressed data, was "nadl-1.5.0.tar", last modified: Wed May 29 18:07:16 2024, max compression
```

## Comparing `nadl-1.4.9.tar` & `nadl-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2275 2024-05-27 18:52:56.966776 nadl-1.4.9/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.9/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.4.9/src/nadl/.DS_Store
--rw-r--r--   0        0        0     1806 2024-05-27 18:52:28.004484 nadl-1.4.9/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.9/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.4.9/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.9/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.4.9/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.9/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.9/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.9/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.9/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.9/src/nadl/py.typed
--rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.4.9/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.9/src/nadl/transformers.py
--rw-r--r--   0        0        0     2478 2024-05-27 18:52:03.349585 nadl-1.4.9/src/nadl/utils.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0     2275 2024-05-29 18:07:16.710528 nadl-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.0/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.0/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     1806 2024-05-29 18:06:54.894671 nadl-1.5.0/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.0/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.0/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.0/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.0/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.0/src/nadl/loops.py
+-rw-r--r--   0        0        0     5751 2024-05-29 18:06:13.669773 nadl-1.5.0/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.0/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.0/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.0/src/nadl/py.typed
+-rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.0/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.0/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2699 2024-05-29 17:08:54.829295 nadl-1.5.0/src/nadl/utils.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.5.0/PKG-INFO
```

### Comparing `nadl-1.4.9/pyproject.toml` & `nadl-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.11",
 ]
 requires-python = ">=3.12"
-version = "1.4.9"
+version = "1.5.0"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.4.9/readme.org` & `nadl-1.5.0/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/.DS_Store` & `nadl-1.5.0/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/__init__.py` & `nadl-1.5.0/src/nadl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from .states import BaseTrainState, state_fn
 from .utils import (
   classit,
   rle,
   rle_array,
 )
 
-__version__ = "1.4.9"
+__version__ = "1.5.0"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "BaseTrainState",
   "DState",
```

### Comparing `nadl-1.4.9/src/nadl/blocks.py` & `nadl-1.5.0/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/data.py` & `nadl-1.5.0/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/images.py` & `nadl-1.5.0/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/keys.py` & `nadl-1.5.0/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/loops.py` & `nadl-1.5.0/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/nets.py` & `nadl-1.5.0/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/preprocessing.py` & `nadl-1.5.0/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/states.py` & `nadl-1.5.0/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/transformers.py` & `nadl-1.5.0/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.9/src/nadl/utils.py` & `nadl-1.5.0/src/nadl/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 filename : utils.py
 project  : nadl
 license  : GPL-3.0+
 
 Utils
 """
 
-from collections.abc import Mapping
-from typing import Literal
+from collections.abc import Callable, Mapping, Sequence
+from typing import Any, Literal
 import jax
 import jax.numpy as jnp
 from rich.console import Console
+from jaxtyping import PyTree
+import equinox as eqx
 
 
 def rle_array(x: jax.Array, shift: int = 1) -> jax.Array:
   """Run length encoding array."""
   x = x.flatten()
   x = jnp.pad(x, (1, 1), mode="constant")
   x = jnp.argwhere(x[1:] != x[:-1]).flatten() + shift
@@ -69,19 +71,24 @@
       return jnp.argmax(x, axis=-1, keepdims=True)
     case "threshold":
       return x > threshold
     case _:
       raise ValueError(f"Unknown method {method}")
 
 
-def pformat(xs: Mapping[str, jax.Array | float | int | str | None]) -> str:
+def pformat(xs: PyTree, short_arrays: bool = False) -> str:
   """Pretty format."""
   with (console := Console()).capture() as capture:
-    nxs = jax.tree.map(
-      lambda x: float(f"{x:.4f}")
-      if isinstance(x, float)
-      or (isinstance(x, jax.Array) and x.ndim <= 1 and x.shape[0] == 1)
-      else x,
-      xs,
-    )
+    nxs = eqx.tree_pformat(xs, short_arrays=short_arrays)
     console.print(nxs, soft_wrap=True, justify="left", no_wrap=True, width=40)
   return capture.get()
+
+
+def filter_concat[T](
+  xs: Sequence[T],
+  filter_spec: Callable[[Any], bool] = eqx.is_array,
+  select_idx: int = -1,
+) -> T:
+  """Filter concat."""
+  t1, t2 = eqx.partition(xs, filter_spec=filter_spec)
+  t1 = jax.tree.map(lambda *x: jnp.r_[x], *t1)
+  return eqx.combine(t1, t2[select_idx])
```

### Comparing `nadl-1.4.9/PKG-INFO` & `nadl-1.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.4.9
+Version: 1.5.0
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

