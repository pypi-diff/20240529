# Comparing `tmp/DiffeRT-0.0.9.tar.gz` & `tmp/differt-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `DiffeRT-0.0.9.tar` & `differt-0.15.tar`

### file list

```diff
@@ -1,39 +1,25 @@
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 DiffeRT-0.0.9/Cargo.toml
--rw-r--r--   0     1001      127     1073 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/LICENSE.md
--rw-r--r--   0     1001      127     2838 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/README.md
--rw-r--r--   0     1001      127   239396 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/pdm.lock
--rw-r--r--   0     1001      127      139 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/__init__.py
--rw-r--r--   0     1001      127       92 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/_core/__init__.pyi
--rw-r--r--   0     1001      127       74 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/_core/geometry/__init__.pyi
--rw-r--r--   0     1001      127      247 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/_core/geometry/triangle_mesh.pyi
--rw-r--r--   0     1001      127       67 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/_core/rt/__init__.pyi
--rw-r--r--   0     1001      127     2291 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/_core/rt/graph.pyi
--rw-r--r--   0     1001      127      489 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/_core/rt/utils.pyi
--rw-r--r--   0     1001      127      108 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/geometry/__init__.py
--rw-r--r--   0     1001      127     5475 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/geometry/triangle_mesh.py
--rw-r--r--   0     1001      127     3430 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/geometry/utils.py
--rw-r--r--   0     1001      127     3196 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/plotting/__init__.py
--rw-r--r--   0     1001      127     6023 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/plotting/_core.py
--rw-r--r--   0     1001      127    11696 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/plotting/_utils.py
--rw-r--r--   0     1001      127        0 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/py.typed
--rw-r--r--   0     1001      127       29 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/rt/__init__.py
--rw-r--r--   0     1001      127     4571 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/rt/fermat.py
--rw-r--r--   0     1001      127      846 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/rt/graph.py
--rw-r--r--   0     1001      127     9370 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/rt/image_method.py
--rw-r--r--   0     1001      127     5759 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/rt/utils.py
--rw-r--r--   0     1001      127       36 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/scene/__init__.py
--rw-r--r--   0     1001      127       12 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/scene/scene.py
--rw-r--r--   0     1001      127     7531 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/utils.py
--rw-r--r--   0     1001      127      191 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/python/differt/version.py
--rw-r--r--   0     1001      127      244 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/src/geometry/mod.rs
--rw-r--r--   0     1001      127     3291 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/src/geometry/triangle_mesh.rs
--rw-r--r--   0     1001      127      444 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/src/lib.rs
--rw-r--r--   0     1001      127    32773 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/src/rt/graph.rs
--rw-r--r--   0     1001      127      288 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/src/rt/mod.rs
--rw-r--r--   0     1001      127     1859 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/src/rt/utils.rs
--rw-r--r--   0     1001      127     3064 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/static/favicon.png
--rw-r--r--   0     1001      127    11088 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/static/logo.svg
--rw-r--r--   0     1001      127    13997 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/static/logo_250px.png
--rw-r--r--   0     1001      127    31233 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/Cargo.lock
--rw-r--r--   0     1001      127     4086 2024-02-28 14:55:13.000000 DiffeRT-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     5629 1970-01-01 00:00:00.000000 DiffeRT-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 differt-0.15/differt/__init__.py
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 differt-0.15/differt/utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 differt-0.15/differt/version.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 differt-0.15/differt/em/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 differt-0.15/differt/em/constants.py
+-rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 differt-0.15/differt/em/special.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 differt-0.15/differt/em/utd.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 differt-0.15/differt/em/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 differt-0.15/differt/geometry/__init__.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 differt-0.15/differt/geometry/triangle_mesh.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 differt-0.15/differt/geometry/utils.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 differt-0.15/differt/plotting/__init__.py
+-rw-r--r--   0        0        0    12785 2020-02-02 00:00:00.000000 differt-0.15/differt/plotting/_core.py
+-rw-r--r--   0        0        0    15051 2020-02-02 00:00:00.000000 differt-0.15/differt/plotting/_utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 differt-0.15/differt/rt/__init__.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 differt-0.15/differt/rt/fermat.py
+-rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 differt-0.15/differt/rt/image_method.py
+-rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 differt-0.15/differt/rt/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 differt-0.15/differt/scene/__init__.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 differt-0.15/differt/scene/sionna.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 differt-0.15/differt/scene/triangle_scene.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 differt-0.15/.gitignore
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 differt-0.15/LICENSE.md -> ../LICENSE.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 differt-0.15/pyproject.toml
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 differt-0.15/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `DiffeRT-0.0.9/python/differt/geometry/triangle_mesh.py` & `differt-0.15/differt/geometry/triangle_mesh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Mesh geometry made of triangles and utilities."""
+
 from functools import cached_property
 from typing import Any
 
 import equinox as eqx
 import jax.numpy as jnp
 import numpy as np
 from beartype import beartype as typechecker
 from jaxtyping import Array, Bool, Float, UInt, jaxtyped
 
-from .. import _core
+import differt_core.geometry.triangle_mesh
+
 from ..plotting import draw_mesh
 from ..rt.utils import rays_intersect_triangles
 from .utils import normalize
 
 
 @jaxtyped(typechecker=typechecker)
 def triangles_contain_vertices_assuming_inside_same_plane(
@@ -129,30 +131,65 @@
 
     @cached_property
     def diffraction_edges(self) -> UInt[Array, "num_edges 3"]:
         """The diffraction edges."""
         raise NotImplementedError
 
     @classmethod
+    def empty(cls) -> "TriangleMesh":
+        """
+        Create an empty scene.
+
+        Return:
+            A new empty scene.
+        """
+        return cls(
+            vertices=jnp.empty((0, 3)), triangles=jnp.empty((0, 3), dtype=jnp.uint32)
+        )
+
+    @property
+    def is_empty(self) -> bool:
+        """Whether this scene has no triangle."""
+        return self.triangles.size == 0
+
+    @classmethod
     def load_obj(cls, file: str) -> "TriangleMesh":
         """
         Load a triangle mesh from a Wavefront .obj file.
 
         Currently, only vertices and triangles are loaded. Triangle normals
         are computed afterward (when first accessed).
 
-        This method will fail if it contains any geometry that is not a triangle.
-
         Args:
             file: The path to the Wavefront .obj file.
 
         Return:
             The corresponding mesh containing only triangles.
         """
-        mesh = _core.geometry.triangle_mesh.TriangleMesh.load_obj(file)
+        mesh = differt_core.geometry.triangle_mesh.TriangleMesh.load_obj(file)
+        return cls(
+            vertices=mesh.vertices,
+            triangles=mesh.triangles,
+        )
+
+    @classmethod
+    def load_ply(cls, file: str) -> "TriangleMesh":
+        """
+        Load a triangle mesh from a Stanford PLY .ply file.
+
+        Currently, only vertices and triangles are loaded. Triangle normals
+        are computed afterward (when first accessed).
+
+        Args:
+            file: The path to the Stanford PLY .ply file.
+
+        Return:
+            The corresponding mesh containing only triangles.
+        """
+        mesh = differt_core.geometry.triangle_mesh.TriangleMesh.load_ply(file)
         return cls(
             vertices=mesh.vertices,
             triangles=mesh.triangles,
         )
 
     def plot(self, **kwargs: Any) -> Any:
         """
```

### Comparing `DiffeRT-0.0.9/python/differt/geometry/utils.py` & `differt-0.15/differt/geometry/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Utilities for working with 3D geometries."""
+
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 from beartype import beartype as typechecker
 from jaxtyping import Array, Float, jaxtyped
 
 
-@jaxtyped(typechecker=typechecker)
 @jax.jit
+@jaxtyped(typechecker=typechecker)
 def pairwise_cross(
     u: Float[Array, "m 3"], v: Float[Array, "n 3"]
 ) -> Float[Array, "m n 3"]:
     """
     Compute the pairwise cross product between two arrays of vectors.
 
     Args:
@@ -21,16 +22,16 @@
 
     Return:
         A 3D tensor with all cross products.
     """
     return jnp.cross(u[:, None, :], v[None, :, :])
 
 
-@jaxtyped(typechecker=typechecker)
 @jax.jit
+@jaxtyped(typechecker=typechecker)
 def normalize(
     vector: Float[Array, "*batch 3"],
 ) -> tuple[Float[Array, "*batch 3"], Float[Array, " *batch"]]:
     """
     Normalize vectors and also return their length.
 
     This function avoids division by zero by checking vectors
@@ -39,14 +40,17 @@
     Args:
         vector: An array of vectors.
 
     Return:
         The normalized vector and their length.
 
     Examples:
+        The following examples shows how normalization works and
+        its special behavior at zero.
+
         >>> from differt.geometry.utils import (
         ...     normalize,
         ... )
         >>>
         >>> vector = jnp.array([1.0, 1.0, 1.0])
         >>> normalize(vector)  # [1., 1., 1.] / sqrt(3), sqrt(3)
         (Array([0.5773503, 0.5773503, 0.5773503], dtype=float32),
@@ -57,16 +61,16 @@
     """
     length: Array = jnp.linalg.norm(vector, axis=-1, keepdims=True)
     length = jnp.where(length == 0.0, jnp.ones_like(length), length)
 
     return vector / length, jnp.squeeze(length, axis=-1)
 
 
-@jaxtyped(typechecker=typechecker)
 @partial(jax.jit, static_argnames=("normalize",))
+@jaxtyped(typechecker=typechecker)
 def orthogonal_basis(
     u: Float[Array, "*batch 3"], normalize: bool = True
 ) -> tuple[Float[Array, "*batch 3"], Float[Array, "*batch 3"]]:
     """
     Generate ``v`` and ``w``, two other arrays of unit vectors that form with input ``u`` an orthogonal basis.
 
     Args:
@@ -79,14 +83,16 @@
             that the vector lengths may diverge from the unit
             length by 10% or even more!
 
     Return:
         A pair of unit vectors, ``v`` and ``w``.
 
     Examples:
+        The following example shows how this function works on basic input vectors.
+
         >>> from differt.geometry.utils import (
         ...     normalize,
         ...     orthogonal_basis,
         ... )
         >>>
         >>> u = jnp.array([1.0, 0.0, 0.0])
         >>> orthogonal_basis(u)
@@ -101,7 +107,42 @@
     v = jnp.cross(w, u, axis=-1)
 
     if normalize:
         v = v / jnp.linalg.norm(v, axis=-1, keepdims=True)
         w = w / jnp.linalg.norm(w, axis=-1, keepdims=True)
 
     return v, w
+
+
+@jax.jit
+@jaxtyped(typechecker=typechecker)
+def path_lengths(
+    paths: Float[Array, "*batch path_length 3"],
+) -> Float[Array, " *batch"]:
+    """
+    Compute the path length of each path.
+
+    Each path is exactly made of ``path_length`` vertices.
+
+    Args:
+        paths: The array of path vertices.
+
+    Return:
+        The array of path lengths.
+
+    Examples:
+        The following example shows how to compute the length of a very simple path.
+
+        >>> from differt.geometry.utils import (
+        ...     path_lengths,
+        ... )
+        >>>
+        >>> path = jnp.array([[1.0, 0.0, 0.0], [1.0, 1.0, 0.0]])
+        >>> path_lengths(path)
+        Array(1., dtype=float32)
+        >>> path_lengths(jnp.vstack((path, path[::-1, :])))
+        Array(2., dtype=float32)
+    """
+    vectors = jnp.diff(paths, axis=-2)
+    lengths = jnp.linalg.norm(vectors, axis=-1)
+
+    return jnp.sum(lengths, axis=-1)
```

### Comparing `DiffeRT-0.0.9/python/differt/plotting/__init__.py` & `differt-0.15/differt/plotting/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 VisPy uses :py:class:`SceneCanvas<vispy.scene.canvas.SceneCanvas>` objects
 to display contents, on which a view is attached. The view
 (:py:class:`ViewBox<vispy.scene.widgets.viewbox.ViewBox>`)
 is what contains
 the data to be plotted.
 
-To re-use an existing ``canvas`` object, just pass it as a keyword
+To reuse an existing ``canvas`` object, just pass it as a keyword
 argument to any of the ``draw_*`` functions in this module, i.e.,
 with ``draw_*(..., canvas=canvas)``.
 In turn, each of those functions returns a figure on which you
 can later add data.
 
 It is also possible to pass an existing view
 on which data will be plotted: ``draw_*(..., view=view)``.
@@ -46,29 +46,29 @@
 Matplotlib
 ----------
 
 Matplotlib uses :py:class:`Figure<matplotlib.figure.Figure>` objects
 to display contents, on which multiple axes can be attached. In turn, each
 axis can contain data to be plotted.
 
-To re-use an existing ``figure`` object, just pass it as a keyword
+To reuse an existing ``figure`` object, just pass it as a keyword
 argument to any of the ``draw_*`` functions in this module, i.e.,
 with ``draw_*(..., figure=figure)``.
 In turn, each of those functions returns a figure on which you
 can later add data.
 
 It is also possible to pass an existing axis
 (:py:class:`Axes<matplotlib.axes.Axes>`)
 on which data will be plotted: ``draw_*(..., ax=ax)``.
 
 .. warning::
 
     By default, Matplotlib instantiates 2D axes, but this module
     extensively uses 3D plot methods. If an axis is provided,
-    it is your responsability to ensure that it can plot 3D data
+    it is your responsibility to ensure that it can plot 3D data
     when needed.
 
 By default, Matpotlib displays static images in Jupyter notebooks.
 To make them interactive, install ``ipympl`` and load the corresponding
 extension with ``%matplotlib widget``.
 
 Plotly
@@ -78,32 +78,38 @@
 outputs. Hence, Plotly is a very good choice for publishing
 nice interactive plots on webpages.
 
 Plots are fully contained inside
 :py:class:`Figure<plotly.graph_objects.Figure>` objects, and can be nicely
 displayed within Jupyter notebooks without further configuration.
 
-To re-use an existing ``figure`` object, you can do the same as with
+To reuse an existing ``figure`` object, you can do the same as with
 the Matplotlib backend.
 
 """
+
 __all__ = (
     "dispatch",
+    "set_defaults",
     "use",
+    "reuse",
+    "draw_image",
     "draw_markers",
     "draw_mesh",
     "draw_paths",
     "process_vispy_kwargs",
     "process_matplotlib_kwargs",
     "process_plotly_kwargs",
     "view_from_canvas",
 )
 
-from ._core import draw_markers, draw_mesh, draw_paths
+from ._core import draw_image, draw_markers, draw_mesh, draw_paths
 from ._utils import (
     dispatch,
     process_matplotlib_kwargs,
     process_plotly_kwargs,
     process_vispy_kwargs,
+    reuse,
+    set_defaults,
     use,
     view_from_canvas,
 )
```

### Comparing `DiffeRT-0.0.9/python/differt/plotting/_utils.py` & `differt-0.15/differt/plotting/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 """Useful decorators for plotting."""
 
 from __future__ import annotations
 
 import importlib
-from collections.abc import MutableMapping
+from collections.abc import Iterator, MutableMapping
+from contextlib import contextmanager
 from functools import wraps
+from threading import Lock
 from typing import TYPE_CHECKING, Any, Callable, Generic, Protocol, TypeVar
 
-CURRENT_BACKEND = None
-DEFAULT_BACKEND = "vispy"
+# Immutables
+
 SUPPORTED_BACKENDS = ("vispy", "matplotlib", "plotly")
+"""The list of supported backends."""
+
+BACKEND_LOCK = Lock()
+"""A Lock to avoid modifying backend (and defaults) in multiple threads at the same time (e.g., with Pytest."""
+
+# Mutables
+
+DEFAULT_BACKEND = "vispy"
+"""The default backend."""
+DEFAULT_KWARGS: MutableMapping[str, Any] = {}
+"""The default keyword arguments."""
 
 if TYPE_CHECKING:
     import sys
 
     from matplotlib.figure import Figure as MplFigure
     from mpl_toolkits.mplot3d import Axes3D
     from plotly.graph_objects import Figure
@@ -28,20 +41,27 @@
     P = ParamSpec("P")
     T = TypeVar("T", SceneCanvas, MplFigure, Figure)
 else:
     P = TypeVar("P")
     T = TypeVar("T")
 
 
-def use(backend: str) -> None:
+def set_defaults(backend: str | None = None, **kwargs: Any) -> str:
     """
-    Tell future plotting utilities to use this backend by default.
+    Set default keyword arguments for future plotting utilities.
 
     Args:
-        backend: The name of the backend to use.
+        backend: The name of the backend to use, or
+            :py:data:`None` to use the current default.
+        kwargs: Keyword arguments that will be passed to the
+            corresponding ``process_*_kwargs`` function, and
+            plot utilities.
+
+    Return:
+        The name of the (new) default backend.
 
     Raises:
         ValueError: If the backend is not supported.
         ImportError: If the backend is not installed.
 
     Examples:
         The following example shows how to set the default plotting backend.
@@ -62,60 +82,99 @@
         >>>
         >>> my_plot()  # When not specified, use default backend
         Using vispy backend
         >>>
         >>> my_plot(backend="matplotlib")  # We can force the backend
         Using matplotlib backend
         >>>
-        >>> dplt.use("matplotlib")  # Or change the default backend...
-        >>>
+        >>> dplt.set_defaults("matplotlib")  # Or change the default backend...
+        'matplotlib'
         >>> my_plot()  # So that now it defaults to 'matplotlib'
         Using matplotlib backend
         >>>
         >>> my_plot(backend="vispy")  # Of course, the 'vispy' backend is still available
         Using vispy backend
     """
+    global DEFAULT_BACKEND, DEFAULT_KWARGS
+
+    if backend is None:
+        backend = DEFAULT_BACKEND
     if backend not in SUPPORTED_BACKENDS:
         raise ValueError(
             f"The backend '{backend}' is not supported. "
             f"We currently support: {', '.join(SUPPORTED_BACKENDS)}."
         )
 
+    with BACKEND_LOCK:
+        try:
+            importlib.import_module(f"{backend}")
+            DEFAULT_BACKEND = backend
+            DEFAULT_KWARGS = kwargs
+            return backend
+        except ImportError:
+            raise ImportError(
+                f"Could not load backend '{backend}', did you install it?"
+            ) from None
+
+
+@contextmanager
+def use(*args: Any, **kwargs: Any) -> Iterator[str]:
+    """
+    Create a context manager that sets plotting defaults and returns the current default backend.
+
+    When exiting the context, the previous default backend
+    and default keyword arguments are set back.
+
+    Args:
+        args: Positional arguments passed to
+            :py:func:`set_defaults`.
+        kwargs: Keywords arguments passed to
+            :py:func:`set_defaults`.
+
+    Return:
+        The name of the default backend used in this context.
+    """
+    global DEFAULT_BACKEND, DEFAULT_KWARGS
+    default_backend = DEFAULT_BACKEND
+    default_kwargs = DEFAULT_KWARGS
+
     try:
-        importlib.import_module(f"{backend}")
-        global DEFAULT_BACKEND
-        DEFAULT_BACKEND = backend
-    except ImportError:
-        raise ImportError(
-            f"Could not load backend '{backend}', did you install it?"
-        ) from None
+        yield set_defaults(*args, **kwargs)
+    finally:
+        DEFAULT_BACKEND = default_backend
+        DEFAULT_KWARGS = default_kwargs
 
 
 class Dispatcher(Protocol, Generic[P, T]):  # pragma: no cover
     def __call__(
         self,
         *args: P.args,
         **kwargs: P.kwargs,
-    ) -> T:
-        ...
+    ) -> T: ...
 
     def register(
         self,
         backend: str,
-    ) -> Callable[[Callable[P, T]], Callable[P, T]]:
-        ...
+    ) -> Callable[[Callable[P, T]], Callable[P, T]]: ...
 
-    def dispatch(self, backend: str) -> Callable[P, T]:
-        ...
+    def dispatch(self, backend: str) -> Callable[P, T]: ...
 
 
 def dispatch(fun: Callable[P, T]) -> Dispatcher[P, T]:
     """
     Transform a function into a backend dispatcher for plot functions.
 
+    Args:
+        fun: The callable that will register future dispatch
+            functions for each backend implementation.
+
+    Return:
+        The same callable, wrapped in a :py:class:`Dispatcher`
+        class instance.
+
     Examples:
         The following example shows how one can implement plotting
         utilities on different backends for a given plot.
 
         >>> import differt.plotting as dplt
         >>>
         >>> @dplt.dispatch
@@ -164,31 +223,31 @@
         ValueError: Unsupported backend 'numpy', allowed values are: ...
     """
     registry = {}
 
     def register(
         backend: str,
     ) -> Callable[[Callable[P, T]], Callable[P, T]]:
-        """Register a new implemenation."""
+        """Register a new implementation."""
         if backend not in SUPPORTED_BACKENDS:
             raise ValueError(
                 f"Unsupported backend '{backend}', "
                 f"allowed values are: {', '.join(SUPPORTED_BACKENDS)}."
             )
 
         def wrapper(impl: Callable[P, T]) -> Callable[P, T]:
-            """Actually register the backend implemention."""
+            """Actually register the backend implementation."""
 
             @wraps(impl)
             def __wrapper__(*args: P.args, **kwargs: P.kwargs) -> T:  # noqa: N807
                 try:
                     return impl(*args, **kwargs)
                 except ImportError as e:
                     raise ImportError(
-                        "An import error occured when dispatching "
+                        "An import error occurred when dispatching "
                         f"plot utility to backend '{backend}'. "
                         "Did you correctly install it?"
                     ) from e
 
             registry[backend] = __wrapper__
 
             return __wrapper__
@@ -205,15 +264,15 @@
 
     @wraps(fun)
     def main_wrapper(
         *args: P.args,
         **kwargs: P.kwargs,
     ) -> T:
         # We cannot currently add keyword argument to the signature,
-        # at least Pyright we not allow that,
+        # at least Pyright will not allow that,
         # see: https://github.com/microsoft/pyright/issues/5844.
         #
         # The motivation is detailed in P612:
         # https://peps.python.org/pep-0612/#concatenating-keyword-parameters.
         backend: str = kwargs.pop("backend", DEFAULT_BACKEND)  # type: ignore
         return dispatch(backend)(*args, **kwargs)
 
@@ -288,14 +347,17 @@
         evaluates to :py:data:`True`.
 
     Return:
         The canvas and view used to display contents.
     """
     from vispy import scene
 
+    for key, value in DEFAULT_KWARGS.items():
+        kwargs.setdefault(key, value)
+
     maybe_view = kwargs.pop("view", None)
     canvas = (
         kwargs.pop("canvas", None)
         or (maybe_view.parent.canvas if maybe_view else None)
         or scene.SceneCanvas(keys="interactive", bgcolor="white")
     )
 
@@ -334,14 +396,17 @@
 
     Return:
         The figure and axes used to display contents.
     """
     import matplotlib.pyplot as plt
     from mpl_toolkits.mplot3d import Axes3D
 
+    for key, value in DEFAULT_KWARGS.items():
+        kwargs.setdefault(key, value)
+
     maybe_ax = kwargs.pop("ax", None)
     figure = (
         kwargs.pop("figure", None)
         or (maybe_ax.get_figure() if maybe_ax else None)
         or plt.figure()
     )
 
@@ -379,8 +444,45 @@
             The figure that draws contents of the scene.
 
     Return:
         The figure used to display contents.
     """
     import plotly.graph_objects as go
 
+    for key, value in DEFAULT_KWARGS.items():
+        kwargs.setdefault(key, value)
+
     return kwargs.pop("figure", None) or go.Figure()
+
+
+@contextmanager
+def reuse(**kwargs: Any) -> Iterator[SceneCanvas | MplFigure | Figure]:
+    """Create a context manager that will automatically reuse the current canvas / figure.
+
+    Args:
+        args: Positional arguments passed to
+            :py:func:`set_defaults`.
+        kwargs: Keywords arguments passed to
+            :py:func:`set_defaults`.
+
+    Return:
+        The canvas or figure that is reused for this context.
+    """
+    global DEFAULT_KWARGS
+    backend: str | None = kwargs.pop("backend", None)
+
+    with use(backend=backend) as b:
+        try:
+            if b == "vispy":
+                canvas, view = process_vispy_kwargs(kwargs)
+                DEFAULT_KWARGS = {"canvas": canvas, "view": view, **kwargs}
+                yield canvas
+            elif b == "matplotlib":
+                figure, ax = process_matplotlib_kwargs(kwargs)
+                DEFAULT_KWARGS = {"figure": figure, "ax": ax, **kwargs}
+                yield figure
+            else:
+                figure = process_plotly_kwargs(kwargs)
+                DEFAULT_KWARGS = {"figure": figure, **kwargs}
+                yield figure
+        finally:
+            pass  # No need to reset anything, use(...) will do this
```

### Comparing `DiffeRT-0.0.9/python/differt/rt/fermat.py` & `differt-0.15/differt/rt/fermat.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 Fermat's principle states that the path taken by a ray between two
 given points is the path that can be traveled in the least time
 :cite:`fermat-principle`. In a homogeneous medium,
 this means that the path of least time is also the path of last distance.
 
 As a result, this module offers minimization methods for finding ray paths.
 """
+
 from functools import partial
 from typing import Any
 
 import jax
 import jax.numpy as jnp
 from beartype import beartype as typechecker
 from jaxtyping import Array, Float, jaxtyped
 
 from ..geometry.utils import orthogonal_basis
 from ..utils import minimize
 
 
-@jaxtyped(typechecker=typechecker)
 @partial(jax.jit, static_argnames=("steps", "optimizer"))
+@jaxtyped(typechecker=typechecker)
 def fermat_path_on_planar_mirrors(
     from_vertices: Float[Array, "*batch 3"],
     to_vertices: Float[Array, "*batch 3"],
     mirror_vertices: Float[Array, "*batch num_mirrors 3"],
     mirror_normals: Float[Array, "*batch num_mirrors 3"],
     **kwargs: Any,
 ) -> Float[Array, "*batch num_mirrors 3"]:
```

### Comparing `DiffeRT-0.0.9/python/differt/rt/image_method.py` & `differt-0.15/differt/rt/image_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,43 @@
 The method assumes infinitely long mirrors, and will return invalid
 paths in some degenerated cases such as consecutive colinear mirrors,
 or impossible configurations. It is the user's responsibility to make
 sure that the returned path is correct.
 
 Otherwise, the returned path will, for each reflection, have equal angles
 of incidence and of reflection.
+
+Examples:
+    The following image shows how the Image Method (IM) can be applied
+    to find a path between two nodes (i.e., BS and UE).
+
+    .. figure:: ../_static/image-method.svg
+        :width: 70%
+        :align: center
+        :alt: Image Method example.
+
+        Example application of IM in RT. The method determines the only
+        valid path that can be taken to join BS and UE with, in between, reflection with
+        two mirrors (the interaction order is important). First, the consecutive images
+        of the BS are determined through each mirror, using line symmetry. Second,
+        intersections with mirrors are computed backward, `i.e.`, from last mirror to
+        first, by joining the UE, then the intersections points, with the images of the
+        BS. Finally, the valid path can be obtained by joining BS, the intermediary
+        intersection points, and the UE :cite:`mpt-eucap2023{fig. 5}`.
 """
+
 import chex
 import jax
 import jax.numpy as jnp
 from beartype import beartype as typechecker
 from jaxtyping import Array, Bool, Float, jaxtyped
 
 
-@jaxtyped(typechecker=typechecker)
 @jax.jit
+@jaxtyped(typechecker=typechecker)
 def image_of_vertices_with_respect_to_mirrors(
     vertices: Float[Array, "*batch 3"],
     mirror_vertices: Float[Array, "*batch 3"],
     mirror_normals: Float[Array, "*batch 3"],
 ) -> Float[Array, "*batch 3"]:
     """
     Return the image of vertices with respect to mirrors.
@@ -83,16 +102,16 @@
         vertices
         - 2.0
         * jnp.sum(incident * mirror_normals, axis=-1, keepdims=True)
         * mirror_normals
     )
 
 
-@jaxtyped(typechecker=typechecker)
 @jax.jit
+@jaxtyped(typechecker=typechecker)
 def intersection_of_line_segments_with_planes(
     segment_starts: Float[Array, "*batch 3"],
     segment_ends: Float[Array, "*batch 3"],
     plane_vertices: Float[Array, "*batch 3"],
     plane_normals: Float[Array, "*batch 3"],
 ) -> Float[Array, "*batch 3"]:
     """
@@ -121,16 +140,16 @@
     v = plane_vertices - segment_starts
     un = jnp.sum(u * plane_normals, axis=-1, keepdims=True)
     vn = jnp.sum(v * plane_normals, axis=-1, keepdims=True)
     offset = jnp.where(un == 0.0, 0.0, vn * u / un)
     return segment_starts + offset
 
 
-@jaxtyped(typechecker=typechecker)
 @jax.jit
+@jaxtyped(typechecker=typechecker)
 def image_method(
     from_vertices: Float[Array, "*batch 3"],
     to_vertices: Float[Array, "*batch 3"],
     mirror_vertices: Float[Array, "*batch num_mirrors 3"],
     mirror_normals: Float[Array, "*batch num_mirrors 3"],
 ) -> Float[Array, "*batch num_mirrors 3"]:
     """
@@ -216,23 +235,23 @@
         xs=(mirror_vertices, mirror_normals, images),
         reverse=True,
     )
 
     return jnp.moveaxis(paths, 0, -2)
 
 
-@jaxtyped(typechecker=typechecker)
 @jax.jit
+@jaxtyped(typechecker=typechecker)
 def consecutive_vertices_are_on_same_side_of_mirrors(
     vertices: Float[Array, "*batch num_vertices 3"],
     mirror_vertices: Float[Array, "*batch num_mirrors 3"],
     mirror_normals: Float[Array, "*batch num_mirrors 3"],
 ) -> Bool[Array, "*batch num_mirrors"]:
     """
-    Check if consecutive vertices, but skiping one every other vertex, are on the same side of a given mirror. The number of vertices ``num_vertices`` must be equal to ``num_mirrors + 2``.
+    Check if consecutive vertices, but skipping one every other vertex, are on the same side of a given mirror. The number of vertices ``num_vertices`` must be equal to ``num_mirrors + 2``.
 
     This check is needed after using :func:`image_method` because it can return
     vertices that are behind a mirror, which causes the path to go through this
     mirror, and is someone we want to avoid.
 
     Args:
         vertices: An array of vertices, usually describing ray paths.
```

### Comparing `DiffeRT-0.0.9/python/differt/utils.py` & `differt-0.15/differt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """General purpose utilities."""
+
 import sys
 from collections.abc import Iterable, Mapping
 from functools import partial
 from typing import Any, Callable, Optional, Union
 
-import chex
+import chex  # TODO: fixme, chex is not a dependency
 import jax
 import jax.numpy as jnp
 import optax
 from beartype import beartype as typechecker
 from jaxtyping import Array, Num, Shaped, jaxtyped
 
 if sys.version_info >= (3, 11):
     from typing import TypeVarTuple, Unpack
 else:
     from typing_extensions import TypeVarTuple, Unpack
 
 # Redefined here, because chex uses deprecated type hints
+# TODO: fixme
 OptState = Union[chex.Array, Iterable["OptState"], Mapping[Any, "OptState"]]
 Ts = TypeVarTuple("Ts")
 
 
-@jaxtyped(typechecker=typechecker)
 @jax.jit
+@jaxtyped(typechecker=typechecker)
 def sorted_array2(array: Shaped[Array, "m n"]) -> Shaped[Array, "m n"]:
     """
     Sort a 2D array by row and (then) by column.
 
     Args:
         array: The input array.
 
@@ -87,16 +89,16 @@
     if array.size == 0:
         return array
 
     return array[jnp.lexsort(array.T[::-1])]  # type: ignore
 
 
 # Beartype does not support TypeVarTuple at the moment
-@jaxtyped(typechecker=None)
 @partial(jax.jit, static_argnames=("fun", "steps", "optimizer"))
+@jaxtyped(typechecker=None)
 def minimize(
     fun: Callable[[Num[Array, "*batch n"], *Ts], Num[Array, " *batch"]],
     x0: Num[Array, "*batch n"],
     args: tuple[Unpack[Ts]] = (),
     steps: int = 1000,
     optimizer: Optional[optax.GradientTransformation] = None,
 ) -> tuple[Num[Array, "*batch n"], Num[Array, " *batch"]]:
```

### Comparing `DiffeRT-0.0.9/PKG-INFO` & `differt-0.15/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,99 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: DiffeRT
-Version: 0.0.9
+Version: 0.15
+Summary: Differentiable Ray Tracing Toolbox for Radio Propagation Simulations
+Project-URL: Changelog, https://github.com/jeertmans/DiffeRT/releases
+Project-URL: Documentation, https://eertmans.be/DiffeRT
+Project-URL: Founding, https://github.com/sponsors/jeertmans
+Project-URL: Homepage, https://github.com/jeertmans/DiffeRT
+Project-URL: Repository, https://github.com/jeertmans/DiffeRT
+Author-email: Jérome Eertmans <jeertmans@icloud.com>
+License-Expression: MIT
+License-File: LICENSE.md
+Keywords: differentiable,jax,propagation,radio,ray tracing
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: beartype >=0.17.2
-Requires-Dist: equinox >=0.11.2
-Requires-Dist: jax >=0.4.20
-Requires-Dist: jaxtyping >=0.2.24
-Requires-Dist: numpy >=1.26.1
-Requires-Dist: optax >=0.1.7
-Requires-Dist: typing-extensions >=4.9.0 ; python_version < '3.10'
-Requires-Dist: differt[jupyter,matplotlib,plotly,vispy,vispy-backend] ; extra == 'all'
-Requires-Dist: differt[all] ; extra == 'docs'
-Requires-Dist: myst-nb >=0.17.2 ; extra == 'docs'
-Requires-Dist: pillow >=10.1.0 ; extra == 'docs'
-Requires-Dist: sphinx >=6, <7 ; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints >=1.23 ; extra == 'docs'
-Requires-Dist: sphinx-book-theme >=1.0.1 ; extra == 'docs'
-Requires-Dist: sphinx-copybutton >=0.5.2 ; extra == 'docs'
-Requires-Dist: sphinx-design >=0.5.0 ; extra == 'docs'
-Requires-Dist: sphinx-remove-toctrees >=0.0.3 ; extra == 'docs'
-Requires-Dist: sphinxext-opengraph >=0.9.0 ; extra == 'docs'
-Requires-Dist: sphinxcontrib-apidoc >=0.4.0 ; extra == 'docs'
-Requires-Dist: sphinxcontrib-bibtex >=2.5.0 ; extra == 'docs'
-Requires-Dist: notebook >=7 ; extra == 'jupyter'
-Requires-Dist: jupyter-rfb >=0.4.2 ; extra == 'jupyter'
-Requires-Dist: ipympl ; extra == 'jupyter'
-Requires-Dist: matplotlib >=3.8.1 ; extra == 'maplotlib'
-Requires-Dist: plotly >=5.18.0 ; extra == 'plotly'
-Requires-Dist: vispy >=0.14.1 ; extra == 'vispy'
-Requires-Dist: PyQt6 >=6.6.1 ; extra == 'vispy-backend'
+Requires-Python: >=3.9
+Requires-Dist: beartype>=0.17.2
+Requires-Dist: differt-core==0.0.13
+Requires-Dist: equinox>=0.11.2
+Requires-Dist: jax>=0.4.20
+Requires-Dist: jaxtyping>=0.2.24
+Requires-Dist: numpy>=1.26.1
+Requires-Dist: optax>=0.1.7
+Requires-Dist: requests>=2.31.0
+Requires-Dist: tqdm>=4.66.2
+Requires-Dist: typing-extensions>=4.9.0; python_version < '3.11'
 Provides-Extra: all
-Provides-Extra: docs
+Requires-Dist: ipympl; extra == 'all'
+Requires-Dist: jupyter-rfb>=0.4.2; extra == 'all'
+Requires-Dist: matplotlib>=3.8.1; extra == 'all'
+Requires-Dist: notebook>=7; extra == 'all'
+Requires-Dist: plotly>=5.18.0; extra == 'all'
+Requires-Dist: pyqt6>=6.6.1; extra == 'all'
+Requires-Dist: vispy>=0.14.1; extra == 'all'
 Provides-Extra: jupyter
-Provides-Extra: maplotlib
+Requires-Dist: ipympl; extra == 'jupyter'
+Requires-Dist: jupyter-rfb>=0.4.2; extra == 'jupyter'
+Requires-Dist: notebook>=7; extra == 'jupyter'
+Provides-Extra: matplotlib
+Requires-Dist: matplotlib>=3.8.1; extra == 'matplotlib'
 Provides-Extra: plotly
+Requires-Dist: plotly>=5.18.0; extra == 'plotly'
 Provides-Extra: vispy
+Requires-Dist: vispy>=0.14.1; extra == 'vispy'
 Provides-Extra: vispy-backend
-License-File: LICENSE.md
-Summary: Differentiable Ray Tracing Toolbox for Radio Propagation Simulations
-Keywords: ray tracing,differentiable,propagation,radio,jax
-Author-email: Jérome Eertmans <jeertmans@icloud.com>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Changelog, https://github.com/jeertmans/DiffeRT/releases
-Project-URL: Documentation, https://eertmans.be/DiffeRT
-Project-URL: Founding, https://github.com/sponsors/jeertmans
-Project-URL: Homepage, https://github.com/jeertmans/DiffeRT
-Project-URL: Repository, https://github.com/jeertmans/DiffeRT
+Requires-Dist: pyqt6>=6.6.1; extra == 'vispy-backend'
+Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/jeertmans/DiffeRT/main/static/logo_250px.png" alt="DiffeRT logo"></img>
 </div>
 
 <div align="center">
 
 # DiffeRT
 
 [![Latest Release][pypi-version-badge]][pypi-version-url]
 [![Python version][pypi-python-version-badge]][pypi-version-url]
 [![Documentation][documentation-badge]][documentation-url]
 [![Codecov][codecov-badge]][codecov-url]
-[![PDM][pdm-badge]][pdm-url]
 
 </div>
 
 ## Usage
 
-> [!WARNING]
+> **WARNING:**
 > Until this package reaches version `0.1.x`, breaking changes
-> should be expected.
+> should be expected. Checkout the [ROADMAP](https://github.com/jeertmans/DiffeRT/blob/main/ROADMAP.md) for
+> future features.
 >
 > If you have any suggestion regarding the development of this package,
 > please open an [issue](https://github.com/jeertmans/DiffeRT/issues).
 
+The easiest way to install DiffeRT is through pip:
+
+```bash
+pip install differt
+```
+
+We provide pre-built binaries for most platforms. If you want (or need)
+to build the package from the source distribution, check out the
+requirements below.
+
 ## Contributing
 
-> [!IMPORTANT]
+> **IMPORTANT:**
 > The current documentation is very light and a more complete guide for
 > new contributors will be written in the near future.
 >
 > Until then, do not hesitate to reach me for help with
 > [GitHub issues](https://github.com/jeertmans/DiffeRT/issues)!
 
 This project is built using both Python and Rust code, to provide an easy-to-use
@@ -98,32 +102,41 @@
 
 ### Requirements
 
 To run build this package locally, you need:
 
 - [Python 3.9](https://www.python.org/) or above;
 - [Rust](https://www.rust-lang.org/) stable toolchain;
+- `make` (e.g., GNU Make or Make for Windows);
 - [Maturin](https://www.maturin.rs/) for building Python bindings from Rust code;
-- and [PDM](https://pdm-project.org) to manage all Python dependencies.
+- and [Rye](https://rye.astral.sh/) to manage this project.
+
+
+## Local development
 
-### Building locally
+The following commands assume that you installed
+the project locally with:
 
-You can build the project locally using:
+```bash
+rye sync
+```
+
+and that you activated the corresponding Python virtual environment:
 
 ```bash
-pdm install
+. .venv/bin/activate  # or .venv\Scripts\activate on Windows
 ```
 
 ### Documentation
 
 To generate the documentation, please run the following:
 
 ```bash
 cd docs
-pdm run make html
+make html
 ```
 
 Finally, you can open `build/html/index.html` to see the generated docs.
 
 ### Testing
 
 Both Rust and Python codebases have their own tests and benchmarks.
@@ -143,26 +156,23 @@
 ```
 
 #### Testing Python code
 
 in the same way, you can very test you code with Pytest:
 
 ```bash
-pdm run pytest
+pytest
 ```
 
 or benchmark it:
 
 ```bash
-pdm run pytest --benchmark-only
+pytest --benchmark-only
 ```
 
 [pypi-version-badge]: https://img.shields.io/pypi/v/DiffeRT?label=DiffeRT&color=blueviolet
 [pypi-version-url]: https://pypi.org/project/DiffeRT/
 [pypi-python-version-badge]: https://img.shields.io/pypi/pyversions/DiffeRT?color=orange
 [documentation-badge]: https://readthedocs.org/projects/differt/badge/?version=latest
 [documentation-url]: https://differt.readthedocs.io/latest/?badge=latest
-[codecov-badge]: https://codecov.io/gh/jeertmans/DiffeRT/branch/main/graph/badge.svg?token=8P4DY9JCE4
+[codecov-badge]: https://codecov.io/gh/jeertmans/DiffeRT/branch/main/graph/badge.svg?token=v63alnTWzu
 [codecov-url]: https://codecov.io/gh/jeertmans/DiffeRT
-[pdm-badge]: https://img.shields.io/badge/pdm-managed-blueviolet
-[pdm-url]: https://pdm-project.org
-
```

