# Comparing `tmp/stellar_spice-0.3.tar.gz` & `tmp/stellar_spice-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellar_spice-0.3.tar", last modified: Thu May 16 01:23:49 2024, max compression
+gzip compressed data, was "stellar_spice-0.4.tar", last modified: Wed May 29 03:56:42 2024, max compression
```

## Comparing `stellar_spice-0.3.tar` & `stellar_spice-0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.145123 stellar_spice-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-16 01:23:49.145123 stellar_spice-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 01:23:41.000000 stellar_spice-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-16 01:23:41.000000 stellar_spice-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:23:49.145123 stellar_spice-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.137123 stellar_spice-0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.137123 stellar_spice-0.3/src/spice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.137123 stellar_spice-0.3/src/spice/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/geometry/sutherland_hodgman.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/geometry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/mesh_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/mesh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/mesh_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/mesh_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/orbit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/phoebe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/spots.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/phoebe_model/
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/phoebe_model/DI-Her-meshes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/plots/plot_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/spectrum/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/spectrum/filter_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/filter_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/planck_law.py
--rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/spectrum/spectrum_korg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/spectrum/spectrum_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/spectrum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.145123 stellar_spice-0.3/src/stellar_spice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.259790 stellar_spice-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-29 03:56:42.259790 stellar_spice-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-29 03:56:36.000000 stellar_spice-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-29 03:56:36.000000 stellar_spice-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:56:42.259790 stellar_spice-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.251790 stellar_spice-0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.251790 stellar_spice-0.4/src/spice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.251790 stellar_spice-0.4/src/spice/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/geometry/sutherland_hodgman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/geometry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.255790 stellar_spice-0.4/src/spice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/mesh_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/mesh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/mesh_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/mesh_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/orbit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/phoebe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/spots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.255790 stellar_spice-0.4/src/spice/phoebe_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-29 03:56:36.000000 stellar_spice-0.4/src/spice/phoebe_model/DI-Her-meshes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.255790 stellar_spice-0.4/src/spice/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/plots/plot_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.255790 stellar_spice-0.4/src/spice/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/spectrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/spectrum/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.255790 stellar_spice-0.4/src/spice/spectrum/filter_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/spectrum/filter_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/spectrum/planck_law.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/spectrum/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/spectrum/spectrum_korg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/spectrum/spectrum_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/spectrum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.255790 stellar_spice-0.4/src/spice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-29 03:56:37.000000 stellar_spice-0.4/src/spice/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:56:42.259790 stellar_spice-0.4/src/stellar_spice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-29 03:56:42.000000 stellar_spice-0.4/src/stellar_spice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-29 03:56:42.000000 stellar_spice-0.4/src/stellar_spice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:56:42.000000 stellar_spice-0.4/src/stellar_spice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-29 03:56:42.000000 stellar_spice-0.4/src/stellar_spice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 03:56:42.000000 stellar_spice-0.4/src/stellar_spice.egg-info/top_level.txt
```

### Comparing `stellar_spice-0.3/PKG-INFO` & `stellar_spice-0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellar-spice
-Version: 0.3
+Version: 0.4
 Description-Content-Type: text/markdown
 Requires-Dist: celluloid~=0.2.0
 Requires-Dist: jax~=0.4.24
 Requires-Dist: jaxlib~=0.4.24
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: flax~=0.8.1
 Requires-Dist: joblib~=1.3.2
@@ -12,26 +12,30 @@
 Provides-Extra: huggingface
 Requires-Dist: huggingface-hub~=0.21.3; extra == "huggingface"
 Provides-Extra: dev
 Requires-Dist: pytest~=8.0.0; extra == "dev"
 Requires-Dist: pytest-datadir~=1.5.0; extra == "dev"
 Requires-Dist: coverage~=7.4.3; extra == "dev"
 
-![spice logo](docs/img/spice.svg)
+![spice logo](https://raw.githubusercontent.com/maja-jablonska/spice/main/docs/img/spice.svg)
 
 A stellar spectra integration library.
 
 The package can be installed using PyPI:
 
 ```bash
 pip install stellar-spice
 ```
 
 Paper is currently in prep.
 
+# Documentation
+
+Read the [docs](https://spice.readthedocs.io) here.
+
 # Features implemented
 
 - [x] Rotation
 - [x] Spots
 - [ ] Pulsations
 - [ ] PHOEBE integration
```

### Comparing `stellar_spice-0.3/pyproject.toml` & `stellar_spice-0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stellar-spice"
-version = "0.3"
+version = "0.4"
 readme = "README.md"
 dependencies = [
     "celluloid~=0.2.0",
     "jax~=0.4.24",
     "jaxlib~=0.4.24",
     "numpy~=1.26.4",
     "flax~=0.8.1",
```

### Comparing `stellar_spice-0.3/src/spice/geometry/sutherland_hodgman.py` & `stellar_spice-0.4/src/spice/geometry/sutherland_hodgman.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/geometry/utils.py` & `stellar_spice-0.4/src/spice/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/models/binary.py` & `stellar_spice-0.4/src/spice/models/binary.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/models/mesh_generation.py` & `stellar_spice-0.4/src/spice/models/mesh_generation.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/models/mesh_model.py` & `stellar_spice-0.4/src/spice/models/mesh_model.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/models/mesh_transform.py` & `stellar_spice-0.4/src/spice/models/mesh_transform.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/models/mesh_view.py` & `stellar_spice-0.4/src/spice/models/mesh_view.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/models/orbit_utils.py` & `stellar_spice-0.4/src/spice/models/orbit_utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/models/phoebe_utils.py` & `stellar_spice-0.4/src/spice/models/phoebe_utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/models/spots.py` & `stellar_spice-0.4/src/spice/models/spots.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import jax
 import jax.numpy as jnp
 from jax.typing import ArrayLike
 from .mesh_model import MeshModel
-from .utils import vertex_to_polar
+from .utils import mesh_polar_vertices, spherical_harmonic, vertex_to_polar
 
 
 def __cos_law(lat1, lon1, lat2, lon2):
     """
     Calculate the great circle angular distance between two points
     on the sphere (specified in radians)
 
@@ -27,61 +27,55 @@
     abuns = jnp.array([abun, abun, abun_bg, abun_bg])
     y = jnp.interp(dist_rad, angles, abuns, abun, abun_bg)
     return y
 
 
 v_spot = jax.vmap(__overabundance_spot_params, in_axes=(None, None, None, None, None, None, 0))
 
-
+    
 @jax.jit
-def add_spot(mesh: MeshModel,
-             theta: float,
-             phi: float,
-             param_delta: float,
-             radius: float,
-             radius_factor: float,
-             param_index: int) -> MeshModel:
-    """Add a spot to the mesh model.
+def add_spherical_harmonic_spot(mesh: MeshModel,
+                                m: int, n: int,
+                                param_delta: float,
+                                param_index: int) -> MeshModel:
+    """Add a spot/parameter variation as a spherical harmonic to the mesh model.
 
     Args:
         mesh (MeshModel): mesh model
-        theta (float): theta coordinate of the spot center
-        phi (float): phi coordinate of the spot center
+        m (int): m index of the spherical harmonic
+        n (int): n index of the spherical harmonic
         param_delta (float): difference in the parameter value between the spot and the background
-        radius (float): spot radius in radians
-        radius_factor (float): factor of the difference gradient on the spot edge
         param_index (int): index of the parameter in the parameters array
 
     Returns:
         MeshModel: mesh with the spot added
     """
-    spot_parameters = v_spot(theta, phi, param_delta, 0., radius, radius_factor, mesh.centers)
+    center_polar_coords = mesh_polar_vertices(mesh.centers)
+    spot_parameters = spherical_harmonic(m, n, center_polar_coords) * param_delta
     return mesh._replace(parameters = mesh.parameters.at[:, param_index].set(
-        mesh.parameters[:, param_index]+spot_parameters))
+        mesh.parameters[:, param_index]+spot_parameters.reshape((-1, 1))))
 
 
-def add_spots(mesh: MeshModel,
-              thetas: ArrayLike,
-              phis: ArrayLike,
-              param_deltas: ArrayLike,
-              radii: ArrayLike,
-              radius_factors: ArrayLike,
-              param_indices: ArrayLike) -> MeshModel:
-    """Add multiple spots to the mesh model
+# @jax.jit
+def add_spherical_harmonic_spots(mesh: MeshModel,
+                                 m: ArrayLike, n: ArrayLike,
+                                 param_deltas: ArrayLike,
+                                 param_indices: ArrayLike) -> MeshModel:
+    """Add a spot/parameter variation as a spherical harmonic to the mesh model.
 
     Args:
         mesh (MeshModel): mesh model
-        thetas (ArrayLike): theta coordinates of the spots centers
-        phis (ArrayLike): phi coordinates of the spots centers
-        param_deltas (ArrayLike): difference in the parameter valuea between the spota and the background
-        radii (ArrayLike): spot radii in radians
-        radius_factors (ArrayLike): factors of the difference gradients on the spot edges
-        param_indices (ArrayLike): indices of the parameters in the parameters array
+        m (ArrayLike): m indices of the spherical harmonic
+        n (ArrayLike): n indices of the spherical harmonic
+        param_deltas (ArrayLike): difference in the parameter values between the spot and the background
+        param_indices (ArrayLike): indices of the parameter in the parameters array
 
     Returns:
         MeshModel: mesh with the spots added
     """
     def scan(carry, params):
-        return add_spot(carry, *params[:-1], params[-1].astype(int)), params
-    
-    updated_mesh, _ = jax.lax.scan(scan, mesh, jnp.vstack([thetas, phis, param_deltas, radii, radius_factors, param_indices]).T)
+        return add_spherical_harmonic_spot(
+            carry, m=params[0].astype(int), n=params[1].astype(int), param_delta=params[2], param_index=jnp.atleast_1d(params[3].astype(int))
+            ), params
+        
+    updated_mesh, _ = jax.lax.scan(scan, mesh, jnp.vstack([m, n, param_deltas, param_indices]).T)
     return updated_mesh
```

### Comparing `stellar_spice-0.3/src/spice/models/utils.py` & `stellar_spice-0.4/src/spice/models/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,44 +4,66 @@
 from jax.typing import ArrayLike
 from typing import Tuple
 import warnings
 
 from .mesh_generation import face_center
 from spice.utils import ExperimentalWarning
 
-@jax.jit
-def apply_pulsation(verts: ArrayLike,
-                    faces: ArrayLike,
-                    magnitude: float) -> Tuple[ArrayLike, ArrayLike, ArrayLike, ArrayLike]:
-    """Apply the pulsation 
-
-    Args:
-        verts (ArrayLike): _description_
-        faces (ArrayLike): _description_
-        magnitude (float): _description_
-
-    Returns:
-        Tuple[ArrayLike, ArrayLike, ArrayLike, ArrayLike]: _description_
-    """
-    warnings.warn("This feature is experimental - use with caution.", ExperimentalWarning)
-    direction_vectors = verts/jnp.linalg.norm(verts, axis=1).reshape((-1, 1))
-    verts = verts + magnitude*direction_vectors
-    areas, centers = jax.jit(jax.vmap(face_center, in_axes=(None, 0)))(verts, faces.astype(jnp.int32))
-    mus = jnp.dot(centers/jnp.linalg.norm(centers, axis=1).reshape((-1, 1)), jnp.array([0, 0, 1]))
-    return verts, faces, areas, centers, mus
-
 def vertex_to_polar(v: ArrayLike) -> ArrayLike:
     v += 1e-5
     r = jnp.sqrt(v[0]**2+v[1]**2+v[2]**2)+1e-5
     return jnp.nan_to_num(
         jnp.array([
             jnp.arctan2(v[2], r),
             jnp.arctan2(v[1], v[0])
         ])
     )
+    
+@jax.jit
+def spherical_harmonic(m, n, polar_coordinates):
+    m_array = (m*jnp.ones_like(polar_coordinates[:, 0])).astype(int)
+    n_array = (n*jnp.ones_like(polar_coordinates[:, 1])).astype(int)
+    return jax.scipy.special.sph_harm(m_array,
+                                      n_array,
+                                      polar_coordinates[:, 0],
+                                      polar_coordinates[:, 1],
+                                      n_max=10).real
+    
+def evaluate_fourier_for_value(d0: float, P: float, d: ArrayLike, phi: ArrayLike, timestamp: float) -> ArrayLike:
+    """
+    Args:
+        d0 (float): amplitude D_0
+        P (float): period P
+        d (ArrayLike): amplitudes [1, n]
+        phi (ArrayLike): phases [1, n]
+        timestamp (float): timestamps
+
+    Returns:
+        ArrayLike: values
+    """
+    n = jnp.arange(1, d.shape[0]+1)
+    return d0 + jnp.sum(d*jnp.cos(n/P*timestamp-phi))
+
+def evaluate_fourier_prim_for_value(d0: float, P: float, d: ArrayLike, phi: ArrayLike, timestamp: float) -> ArrayLike:
+    """
+    Args:
+        d0 (float): amplitude D_0
+        P (float): period P
+        d (ArrayLike): amplitudes [1, n]
+        phi (ArrayLike): phases [1, n]
+        timestamp (float): timestamps
+
+    Returns:
+        ArrayLike: values
+    """
+    n = jnp.arange(1, d.shape[0]+1)
+    return jnp.sum(-d*n/P*jnp.sin(n/P*timestamp-phi))
+
+evaluate_many_fouriers_for_value = jax.jit(jax.vmap(evaluate_fourier_for_value, in_axes=(0, 0, 0, 0, None)))
+evaluate_many_fouriers_prim_for_value = jax.jit(jax.vmap(evaluate_fourier_prim_for_value, in_axes=(0, 0, 0, 0, None)))
 
 @jax.jit
 def mesh_polar_vertices(vertices: ArrayLike) -> ArrayLike:
     return (jax.vmap(vertex_to_polar, in_axes=0)(vertices))
 
 
 @jax.jit
```

### Comparing `stellar_spice-0.3/src/spice/phoebe_model/DI-Her-meshes.py` & `stellar_spice-0.4/src/spice/phoebe_model/DI-Her-meshes.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/plots/plot_mesh.py` & `stellar_spice-0.4/src/spice/plots/plot_mesh.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/spectrum/filter.py` & `stellar_spice-0.4/src/spice/spectrum/filter.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/spectrum/planck_law.py` & `stellar_spice-0.4/src/spice/spectrum/planck_law.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/spectrum/spectrum.py` & `stellar_spice-0.4/src/spice/spectrum/spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 def simulate_spectrum(intensity_fn: Callable[[ArrayLike, float, ArrayLike], ArrayLike],
                       m: MeshModel,
                       log_wavelengths: ArrayLike,
                       chunk_size: int = DEFAULT_CHUNK_SIZE):
     
     return __spectrum_flash_sum(intensity_fn,
                                 log_wavelengths,
-                                _adjust_dim(m.areas, chunk_size),
+                                _adjust_dim(jnp.where(m.mus>0, m.areas, 0.), chunk_size),
                                 _adjust_dim(jnp.where(m.mus>0, m.mus, 0.), chunk_size),
                                 _adjust_dim(m.los_velocities, chunk_size),
                                 _adjust_dim(m.parameters, chunk_size),
                                 chunk_size)
     
 
 @partial(jax.jit, static_argnums=(0, 5))
```

### Comparing `stellar_spice-0.3/src/spice/spectrum/spectrum_korg.py` & `stellar_spice-0.4/src/spice/spectrum/spectrum_korg.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/spectrum/spectrum_transformer.py` & `stellar_spice-0.4/src/spice/spectrum/spectrum_transformer.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/spice/spectrum/utils.py` & `stellar_spice-0.4/src/spice/spectrum/utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.3/src/stellar_spice.egg-info/PKG-INFO` & `stellar_spice-0.4/src/stellar_spice.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellar-spice
-Version: 0.3
+Version: 0.4
 Description-Content-Type: text/markdown
 Requires-Dist: celluloid~=0.2.0
 Requires-Dist: jax~=0.4.24
 Requires-Dist: jaxlib~=0.4.24
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: flax~=0.8.1
 Requires-Dist: joblib~=1.3.2
@@ -12,26 +12,30 @@
 Provides-Extra: huggingface
 Requires-Dist: huggingface-hub~=0.21.3; extra == "huggingface"
 Provides-Extra: dev
 Requires-Dist: pytest~=8.0.0; extra == "dev"
 Requires-Dist: pytest-datadir~=1.5.0; extra == "dev"
 Requires-Dist: coverage~=7.4.3; extra == "dev"
 
-![spice logo](docs/img/spice.svg)
+![spice logo](https://raw.githubusercontent.com/maja-jablonska/spice/main/docs/img/spice.svg)
 
 A stellar spectra integration library.
 
 The package can be installed using PyPI:
 
 ```bash
 pip install stellar-spice
 ```
 
 Paper is currently in prep.
 
+# Documentation
+
+Read the [docs](https://spice.readthedocs.io) here.
+
 # Features implemented
 
 - [x] Rotation
 - [x] Spots
 - [ ] Pulsations
 - [ ] PHOEBE integration
```

### Comparing `stellar_spice-0.3/src/stellar_spice.egg-info/SOURCES.txt` & `stellar_spice-0.4/src/stellar_spice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

