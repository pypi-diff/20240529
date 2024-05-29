# Comparing `tmp/invert4geom-0.5.0.tar.gz` & `tmp/invert4geom-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invert4geom-0.5.0.tar", last modified: Tue May  7 16:35:17 2024, max compression
+gzip compressed data, was "invert4geom-0.6.0.tar", last modified: Wed May 29 16:46:55 2024, max compression
```

## Comparing `invert4geom-0.5.0.tar` & `invert4geom-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.067020 invert4geom-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 16:35:10.000000 invert4geom-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-07 16:35:17.067020 invert4geom-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-07 16:35:10.000000 invert4geom-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-07 16:35:10.000000 invert4geom-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:35:17.067020 invert4geom-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.059020 invert4geom-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.059020 invert4geom-0.5.0/src/invert4geom/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    36264 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/regional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-07 16:35:10.000000 invert4geom-0.5.0/src/invert4geom/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.063020 invert4geom-0.5.0/src/invert4geom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 16:35:17.000000 invert4geom-0.5.0/src/invert4geom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:17.063020 invert4geom-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25647 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_regional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    25696 2024-05-07 16:35:10.000000 invert4geom-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:46:55.218475 invert4geom-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-29 16:46:50.000000 invert4geom-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-29 16:46:55.218475 invert4geom-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-29 16:46:50.000000 invert4geom-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-29 16:46:50.000000 invert4geom-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:46:55.218475 invert4geom-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:46:55.210475 invert4geom-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:46:55.210475 invert4geom-0.6.0/src/invert4geom/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 16:46:50.000000 invert4geom-0.6.0/src/invert4geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24988 2024-05-29 16:46:50.000000 invert4geom-0.6.0/src/invert4geom/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49495 2024-05-29 16:46:50.000000 invert4geom-0.6.0/src/invert4geom/inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-05-29 16:46:50.000000 invert4geom-0.6.0/src/invert4geom/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39378 2024-05-29 16:46:50.000000 invert4geom-0.6.0/src/invert4geom/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-29 16:46:50.000000 invert4geom-0.6.0/src/invert4geom/regional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-29 16:46:50.000000 invert4geom-0.6.0/src/invert4geom/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31943 2024-05-29 16:46:50.000000 invert4geom-0.6.0/src/invert4geom/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:46:55.214475 invert4geom-0.6.0/src/invert4geom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-29 16:46:55.000000 invert4geom-0.6.0/src/invert4geom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-29 16:46:55.000000 invert4geom-0.6.0/src/invert4geom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:46:55.000000 invert4geom-0.6.0/src/invert4geom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-29 16:46:55.000000 invert4geom-0.6.0/src/invert4geom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 16:46:55.000000 invert4geom-0.6.0/src/invert4geom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:46:55.214475 invert4geom-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:46:50.000000 invert4geom-0.6.0/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25709 2024-05-29 16:46:50.000000 invert4geom-0.6.0/tests/test_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-29 16:46:50.000000 invert4geom-0.6.0/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-29 16:46:50.000000 invert4geom-0.6.0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:46:50.000000 invert4geom-0.6.0/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-05-29 16:46:50.000000 invert4geom-0.6.0/tests/test_regional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:46:50.000000 invert4geom-0.6.0/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26241 2024-05-29 16:46:50.000000 invert4geom-0.6.0/tests/test_utils.py
```

### Comparing `invert4geom-0.5.0/LICENSE` & `invert4geom-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invert4geom-0.5.0/PKG-INFO` & `invert4geom-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invert4geom
-Version: 0.5.0
+Version: 0.6.0
 Summary: Constrained gravity inversion to recover the geometry of a density contrast.
 Author-email: Matt Tankersley <matt.d.tankersley@gmail.com>
 License: Copyright 2023 Matt Tankersley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -72,14 +72,15 @@
 Provides-Extra: viz
 Requires-Dist: pyvista; extra == "viz"
 Requires-Dist: trame; extra == "viz"
 Requires-Dist: ipywidgets; extra == "viz"
 Requires-Dist: matplotlib; extra == "viz"
 Requires-Dist: seaborn; extra == "viz"
 Requires-Dist: ipython; extra == "viz"
+Requires-Dist: plotly; extra == "viz"
 Provides-Extra: test
 Requires-Dist: pytest>=6; extra == "test"
 Requires-Dist: pytest-cov>=3; extra == "test"
 Requires-Dist: invert4geom[opti]; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=4.0; extra == "docs"
 Requires-Dist: myst_parser; extra == "docs"
@@ -172,26 +173,41 @@
 
 <!-- <p align="center">
 <img src="docs/figures/cover_fig.png" width="400"/>
 </p> -->
 
 <!-- SPHINX-START2 -->
 
-**Invert4geom** is a Python library for performing 3D geometric gravity
-inversions, where the aim is to recover the geometry of a density contrast.
+**Invert4geom** is a Python library for performing 3D geometric gravity inversions, where the aim is to recover the geometry of a density contrast.
 
-Typical use cases include modeling the topography of the Moho, the
-sediment-basement contact, or bathymetry. These density contrasts are
-represented by a layer of vertical right-rectangular prisms. Since we use
-vertical prisms, they don't take the curvature of the Earth into account. For
-large-scale applications, such as continental studies, it would be better to use
-tesseroids instead of prisms.
-
-See the [overview](overview.md) for further description of this package and what
-it can be used for.
+Typical use cases include modeling the topography of the Moho, the sediment-basement contact, or bathymetry.
+These density contrasts are represented by a layer of vertical right-rectangular prisms.
+Since we use vertical prisms, they don't take the curvature of the Earth into account.
+For large-scale applications, such as continental studies, it would be better to use tesseroids instead of prisms.
+
+See the [overview](overview.md) for further description of this package and what it can be used for.
+
+#### What _Invert4Geom_ is for:
+
+- invert **gravity** data to recover the topography of a density contrast
+- use with **gridded** gravity data
+- discretization using _vertical right-rectangular prisms_
+- performing regional-residual separation
+- stochastic uncertainty analysis of inversion results
+- basic visualization tools
+
+#### What _Invert4Geom_ is **NOT** for:
+
+- performing parameter-estimation inversions (i.e. recovering density values) -> see [SimPEG](https://simpeg.xyz/) or [pyGIMLi](https://www.pygimli.org/index.html)
+- a point-and-click GUI -> see [Geosoft/Seequent Oasis Montaj](https://www.seequent.com/products-solutions/ geosoft-oasis-montaj/) or [MiraGeoscience VPmg](https://www.mirageoscience.com/mining-industry-software/geoscience-analyst-pro-geophysics/)
+- a ready-to-use inversion with minimal user input
+- use with discrete (un-gridded) gravity data -> see [Harmonica](https://www.fatiando.org/harmonica/latest/index.html) for gridding your data
+- for processing gravity data -> see [Harmonica](https://www.fatiando.org/harmonica/latest/index.html) for gravity processing tools
+- for use with tesseroids, or non-regular grids (raise an issue request if you want this implemented!)
+- publication-quality visualization -> see [PyGMT](https://www.pygmt.org/dev/index.html) for plotting tools
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/mdtanker/invert4geom/workflows/CI/badge.svg
 [actions-link]:             https://github.com/mdtanker/invert4geom/actions
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/invert4geom
 [conda-link]:               https://github.com/conda-forge/invert4geom-feedstock
 [codecov-badge]:            https://codecov.io/github/mdtanker/invert4geom/badge.svg?
```

### Comparing `invert4geom-0.5.0/pyproject.toml` & `invert4geom-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 readme = "README.md"
-version = "0.5.0"
+version = "0.6.0"
 license = {file = "LICENSE"}
 
 keywords = ["inversion", "gravity", "geometry", "density", "Moho", "sediment", "geophysics", "geology", "geoscience"]
 
 dependencies = [
   "numpy",
   "pandas",
@@ -62,14 +62,15 @@
 viz = [
   "pyvista",
   "trame",
   "ipywidgets",
   "matplotlib",
   "seaborn",
   "ipython",
+  "plotly",
 ]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
   "invert4geom[opti]",
 ]
 docs = [
@@ -178,21 +179,22 @@
   "T20",         # flake8-print
   "UP",          # pyupgrade
   "YTT",         # flake8-2020
   "EXE",         # flake8-executable
   "NPY",         # NumPy specific rules
   "PD",          # pandas-vet
 ]
-lint.extend-ignore = [
+lint.ignore = [
   "PLR",    # Design related pylint codes
   "G004",   # Logging with f-strings
   "PD901",  # Bad variable name warning
   "PD003", # Changes .isna to .isnull
   "PD004", # Changes .notna to .notnull
   "PD011", # Changes .values() to .to_numpy()
+  "ISC001", # Implicit string concatenation
 ]
 src = ["src"]
 lint.unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
   "PD003", # Changes .isna to .isnull
   "PD004", # Changes .notna to .notnull
@@ -209,24 +211,25 @@
 "tests/**" = ["T20"]
 "noxfile.py" = ["T20"]
 "*.ipynb" = ["E402", "B018", "T201"]
 
 
 [tool.pylint]
 py-version = "3.9"
-ignore-paths = ["CHANGELOG.md"]
+# ignore-patterns = [".*.md",]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 similarities.min-similarity-lines = 5
 messages_control.disable = [
   "design",
   "fixme",
   "line-too-long",
   "missing-module-docstring",
   "wrong-import-position",
+  "cyclic-import",
 ]
 
 [tool.semantic_release]
 version_variables = ["src/invert4geom/__init__.py:__version__"]
 version_toml = ["pyproject.toml:project.version"]
 major_on_zero = false
 build_command = """
```

### Comparing `invert4geom-0.5.0/src/invert4geom/inversion.py` & `invert4geom-0.6.0/src/invert4geom/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1075 +1,1045 @@
 from __future__ import annotations  # pylint: disable=too-many-lines
 
 import copy
-import itertools
 import logging
-import time
 import typing
+import warnings
 
+import dask
 import harmonica as hm
-import numba
 import numpy as np
 import pandas as pd
-import scipy as sp
+import pygmt
 import verde as vd
 import xarray as xr
+import xrft
 from nptyping import NDArray
-from tqdm.autonotebook import tqdm
+from pykdtree.kdtree import KDTree  # pylint: disable=no-name-in-module
 
-from invert4geom import plotting, utils
 
-
-@numba.jit(cache=True, nopython=True)  # type: ignore[misc]
-def grav_column_der(
-    grav_easting: NDArray,
-    grav_northing: NDArray,
-    grav_upward: NDArray,
-    prism_easting: NDArray,
-    prism_northing: NDArray,
-    prism_top: NDArray,
-    prism_spacing: float,
-    prism_density: NDArray,
-) -> NDArray:
-    """
-        Function to calculate the vertical derivate of the gravitational acceleration at
-        an observation point caused by a right, rectangular prism. Approximated with
-        Hammer's annulus approximation :footcite:p:`mccubbineairborne2016`.
+def rmse(data: NDArray, as_median: bool = False) -> float:
+    """
+    function to give the root mean/median squared error (RMSE) of data
 
     Parameters
     ----------
-    grav_easting, grav_northing, grav_upward : NDArray
-        coordinates of gravity observation points.
-    prism_easting, prism_northing, prism_top : NDArray
-        coordinates of prism's center in northing, easting, and upward directions,
-        respectively
-    prism_spacing : float
-        resolution of prism layer in meters
-    prism_density : NDArray
-        density of prisms, in kg/m^3
+    data : NDArray
+        input data
+    as_median : bool, optional
+        choose to give root median squared error instead, by default False
 
     Returns
     -------
-    NDArray
-        array of vertical derivative of gravity at observation point for series of
-        prisms
-
-    References
-    ----------
-    .. footbibliography::
+    float
+        RMSE value
     """
+    if as_median:
+        value: float = np.sqrt(np.nanmedian(data**2).item())
+    else:
+        value = np.sqrt(np.nanmean(data**2).item())
 
-    r = np.sqrt(
-        np.square(grav_northing - prism_northing)
-        + np.square(grav_easting - prism_easting)
-    )
-    r1 = r - 0.5 * prism_spacing
-    r2 = r + 0.5 * prism_spacing
-
-    # gravity observation point can't be within prism
-    # if it is, instead calculate gravity on prism edge
-    r1[r1 < 0] = 0
-    r2[r2 < prism_spacing] = prism_spacing
-
-    f = np.square(prism_spacing) / (
-        np.pi * (np.square(r2) - np.square(r1))
-    )  # eq 2.19 in McCubbine 2016 Thesis
-    # 2*pi*G = 0.0000419
-    return (
-        0.0000419
-        * f
-        * prism_density
-        * (prism_top - grav_upward)
-        * (
-            1 / np.sqrt(np.square(r2) + np.square(prism_top - grav_upward))
-            - 1 / np.sqrt(np.square(r1) + np.square(prism_top - grav_upward))
-        )
-    )
+    return value
 
 
-@numba.njit(parallel=True)  # type: ignore[misc]
-def jacobian_annular(
-    grav_easting: NDArray,
-    grav_northing: NDArray,
-    grav_upward: NDArray,
-    prism_easting: NDArray,
-    prism_northing: NDArray,
-    prism_top: NDArray,
-    prism_density: NDArray,
-    prism_spacing: float,
-    jac: NDArray,
-) -> NDArray:
-    """
-    Function to calculate the Jacobian matrix using the annular cylinder
-    approximation. The resulting Jacobian is a matrix (numpy array) with a row per
-    gravity observation and a column per prism. This approximates the prisms as an
-    annulus :footcite:p:`mccubbineairborne2016`, and calculates it's vertical gravity
-    derivative. Takes arrays from `jacobian`, feeds them into `grav_column_der`, and
-    returns the jacobian.
+def nearest_grid_fill(
+    grid: xr.DataArray,
+    method: str = "verde",
+) -> xr.DataArray:
+    """
+    fill missing values in a grid with the nearest value.
 
     Parameters
     ----------
-    grav_easting, grav_northing, grav_upward : NDArray
-        coordinates of gravity observation points
-    prism_easting, prism_northing, prism_top : NDArray
-        coordinates of prism's center in northing, easting, and upward directions,
-        respectively
-    prism_density : NDArray
-        density of prisms, in kg/m^3
-    prism_spacing : float
-        resolution of prism layer in meters
-    jac : NDArray
-        empty jacobian matrix with a row per gravity observation and a column per prism
+    grid : xr.DataArray
+        grid with missing values
+    method : str, optional
+        choose method of filling, by default "verde"
 
     Returns
     -------
-    NDArray
-        returns a jacobian matrix of shape (number of gravity points, number of prisms)
-
-    References
-    ----------
-    .. footbibliography::
+    xr.DataArray
+        filled grid
     """
 
-    for i in numba.prange(len(grav_easting)):  # pylint: disable=not-an-iterable
-        jac[i, :] = grav_column_der(
-            grav_easting[i],
-            grav_northing[i],
-            grav_upward[i],
-            prism_easting,
-            prism_northing,
-            prism_top,
-            prism_spacing,
-            prism_density,
+    # get coordinate names
+    original_dims = list(grid.sizes.keys())
+
+    # get original grid name
+    original_name = grid.name
+
+    if method == "rioxarray":
+        filled: xr.DataArray = (
+            grid.rio.write_crs("epsg:3031")
+            .rio.set_spatial_dims(original_dims[1], original_dims[0])
+            .rio.write_nodata(np.nan)
+            .rio.interpolate_na(method="nearest")
+            .rename(original_name)
+        )
+    elif method == "verde":
+        df = vd.grid_to_table(grid)
+        df_dropped = df[df[grid.name].notnull()]
+        coords = (df_dropped[grid.dims[1]], df_dropped[grid.dims[0]])
+        region = vd.get_region((df[grid.dims[1]], df[grid.dims[0]]))
+        filled = (
+            vd.KNeighbors()
+            .fit(coords, df_dropped[grid.name])
+            .grid(region=region, shape=grid.shape, data_names=original_name)[
+                original_name
+            ]
         )
+    # elif method == "pygmt":
+    #     filled = pygmt.grdfill(grid, mode="n", verbose="q").rename(original_name)
+    else:
+        msg = "method must be 'rioxarray', or 'verde'"
+        raise ValueError(msg)
 
-    return jac
+    # reset coordinate names if changed
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="rename '")
+        return filled.rename(
+            {
+                next(iter(filled.dims)): original_dims[0],
+                list(filled.dims)[1]: original_dims[1],
+            }
+        )
 
 
-def prism_properties(
-    prisms_layer: xr.Dataset,
-    method: str = "itertools",
-) -> NDArray:
+def filter_grid(
+    grid: xr.DataArray,
+    filter_width: float | None = None,
+    filt_type: str = "lowpass",
+) -> xr.DataArray:
     """
-    extract prism properties from prism layer
+    _summary_
 
     Parameters
     ----------
-    prisms_layer : xr.Dataset
-       harmonica prism layer
-    method : str, optional
-        choice of method to extract properties, by default "itertools"
+    grid : xr.DataArray
+        grid to filter the values of
+    filter_width : float, optional
+        width of the filter in meters, by default None
+    filt_type : str, optional
+        type of filter to use, by default "lowpass"
+    change_spacing : bool, optional
+        if True, will filter the grid and resample the grid to be at the same spacing
+        of the filter width, by default False
 
     Returns
     -------
-    NDArray
-        array of prism properties
+    xr.DataArray
+        a filtered grid
+
     """
+    # get coordinate names
+    original_dims = list(grid.sizes.keys())
 
-    if method == "itertools":
-        prisms_properties: NDArray = []
-        for (
-            y,
-            x,
-        ) in itertools.product(
-            range(prisms_layer.northing.size), range(prisms_layer.easting.size)
-        ):
-            prisms_properties.append(
-                [
-                    *list(prisms_layer.prism_layer.get_prism((y, x))),
-                    prisms_layer.density.values[y, x],
-                ]
-            )
-        prisms_properties = np.array(prisms_properties)
-    elif method == "forloops":
-        prisms_properties = []
-        for y in range(prisms_layer.northing.size):
-            for x in range(prisms_layer.easting.size):
-                prisms_properties.append(
-                    [
-                        *list(prisms_layer.prism_layer.get_prism((y, x))),
-                        prisms_layer.density.values[y, x],
-                    ]
-                )
-        np.asarray(prisms_properties)
-    elif method == "generator":
-        # slower, but doesn't allocate memory
-        prisms_properties = [
-            list(prisms_layer.prism_layer.get_prism((y, x)))  # noqa: RUF005
-            + [prisms_layer.density.values[y, x]]
-            for y in range(prisms_layer.northing.size)
-            for x in range(prisms_layer.easting.size)
-        ]
+    # get original grid name
+    original_name = grid.name
+
+    # if there are nan's, fill them with nearest neighbor
+    if grid.isnull().any():
+        filled = nearest_grid_fill(grid, method="verde")
+        # print("filling NaN's with nearest neighbor")
+    else:
+        filled = grid.copy()
+
+    # reset coordinate names if changed
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="rename '")
+        filled = filled.rename(
+            {
+                next(iter(filled.dims)): original_dims[0],
+                list(filled.dims)[1]: original_dims[1],
+            }
+        )
+
+    # define width of padding in each direction
+    pad_width = {
+        original_dims[1]: grid[original_dims[1]].size // 3,
+        original_dims[0]: grid[original_dims[0]].size // 3,
+    }
+
+    # apply padding
+    padded = xrft.pad(filled, pad_width)
+
+    if filt_type == "lowpass":
+        filt = hm.gaussian_lowpass(padded, wavelength=filter_width).rename("filt")
+    elif filt_type == "highpass":
+        filt = hm.gaussian_highpass(padded, wavelength=filter_width).rename("filt")
+    elif filt_type == "up_deriv":
+        filt = hm.derivative_upward(padded).rename("filt")
+    elif filt_type == "easting_deriv":
+        filt = hm.derivative_easting(padded).rename("filt")
+    elif filt_type == "northing_deriv":
+        filt = hm.derivative_northing(padded).rename("filt")
     else:
-        msg = "method must be one of 'itertools', 'forloops', or 'generator'"
+        msg = "filt_type must be 'lowpass' or 'highpass'"
         raise ValueError(msg)
 
-    return prisms_properties
+    unpadded = xrft.unpad(filt, pad_width)
+
+    # reset coordinate values to original (avoid rounding errors)
+    unpadded = unpadded.assign_coords(
+        {
+            original_dims[0]: grid[original_dims[0]].to_numpy(),
+            original_dims[1]: grid[original_dims[1]].to_numpy(),
+        }
+    )
+
+    if grid.isnull().any():
+        result: xr.DataArray = xr.where(grid.notnull(), unpadded, grid)
+    else:
+        result = unpadded.copy()
+
+    # reset coordinate names if changed
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="rename '")
+        result = result.rename(
+            {
+                next(iter(result.dims)): original_dims[0],
+                # list(result.dims)[0]: original_dims[0],
+                list(result.dims)[1]: original_dims[1],
+            }
+        )
+
+    return result.rename(original_name)
+
+
+def dist_nearest_points(
+    targets: pd.DataFrame,
+    data: pd.DataFrame | xr.DataArray | xr.Dataset,
+    coord_names: tuple[str, str] | None = None,
+) -> typing.Any:
+    """
+    for all gridcells calculate to the distance to the nearest target.
 
+    Parameters
+    ----------
+    targets : pd.DataFrame
+        contains the coordinates of the targets
+    data : pd.DataFrame | xr.DataArray | xr.Dataset
+        the grid data, in either gridded or tabular form
+    coord_names : tuple[str, str] | None, optional
+        the names of the coordinates for both the targets and the data, by default None
 
-@numba.jit(forceobj=True, parallel=True)  # type: ignore[misc]
-def jacobian_prism(
-    prisms_properties: NDArray,
-    grav_easting: NDArray,
-    grav_northing: NDArray,
-    grav_upward: NDArray,
-    delta: float,
-    jac: NDArray,
-) -> NDArray:
+    Returns
+    -------
+    typing.Any
+        the distance to the nearest target for each gridcell, in the same format as the
+        input for `data`.
     """
-    Function to calculate the Jacobian matrix with the vertical gravity derivative
-    as a numerical approximation with small prisms
 
-    Takes arrays from `jacobian` and calculates the jacobian.
+    if coord_names is None:
+        coord_names = ("easting", "northing")
+
+    df_targets = targets[[coord_names[0], coord_names[1]]].copy()
+
+    df_data: pd.DataFrame | xr.DataArray | xr.Dataset
+    if isinstance(data, pd.DataFrame):
+        df_data = data[list(coord_names)].copy()
+    elif isinstance(data, xr.DataArray):
+        df_grid = vd.grid_to_table(data).dropna()
+        df_data = df_grid[[coord_names[0], coord_names[1]]].copy()  # pylint: disable=unsubscriptable-object
+    elif isinstance(data, xr.Dataset):
+        try:
+            df_grid = vd.grid_to_table(data[next(iter(data.variables))]).dropna()
+            # df_grid = vd.grid_to_table(data[list(data.variables)[0]]).dropna()
+        except IndexError:
+            df_grid = vd.grid_to_table(data).dropna()
+        df_data = df_grid[[coord_names[0], coord_names[1]]].copy()  # pylint: disable=unsubscriptable-object
+
+    min_dist, _ = KDTree(df_targets.values).query(df_data.values, 1)
+
+    df_data["min_dist"] = min_dist
+
+    if isinstance(data, pd.DataFrame):
+        return df_data
+    return df_data.set_index([coord_names[0], coord_names[1]][::-1]).to_xarray()
+
+
+def normalize_xarray(
+    da: xr.DataArray,
+    low: float = 0,
+    high: float = 1,
+) -> xr.DataArray:
+    """
+    Normalize a grid between provided values
 
     Parameters
     ----------
-    prisms_properties : NDArray
-        array of prism properties of shape (number of prisms, 7) with the 7 entries for
-        each prism being: west, east, south, north, bottom, top, density
-    grav_easting, grav_northing,grav_upward : NDArray
-        coordinates of gravity observation points.
-    delta : float
-        thickness in meters of small prisms used to calculate vertical derivative
-    jac : NDArray
-        empty jacobian matrix with a row per gravity observation and a column per prism
+    da : xr.DataArray
+        grid to normalize
+    low : float, optional
+        lower value for normalization, by default 0
+    high : float, optional
+        higher value for normalization, by default 1
 
     Returns
     -------
-    NDArray
-        returns a NDArray of shape (number of gravity points, number of prisms)
+    xr.DataArray
+        a normalized grid
     """
+    # min_val = da.values.min()
+    # max_val = da.values.max()
 
-    # Build a small prism on top of existing prism (thickness equal to delta)
-    for i in numba.prange(len(prisms_properties)):  # pylint: disable=not-an-iterable
-        prism = prisms_properties[i]
-        density = prism[6]
-        bottom = prism[5]
-        top = prism[5] + delta
-        delta_prism = (prism[0], prism[1], prism[2], prism[3], bottom, top)
-
-        jac[:, i] = (
-            hm.prism_gravity(
-                coordinates=(grav_easting, grav_northing, grav_upward),
-                prisms=delta_prism,
-                density=density,
-                field="g_z",
-                parallel=True,
-            )
-            / delta
-        )
+    da = da.copy()
+
+    min_val = da.quantile(0)
+    max_val = da.quantile(1)
+
+    da2: xr.DataArray = (high - low) * (
+        ((da - min_val) / (max_val - min_val)).clip(0, 1)
+    ) + low
 
-    return jac
+    return da2.drop("quantile")
 
 
-def jacobian(
-    deriv_type: str,
-    coordinates: pd.DataFrame,
-    empty_jac: NDArray | None = None,
-    prisms_layer: xr.Dataset | None = None,
-    prism_spacing: float | None = None,
-    prism_size: float | None = None,
-    prisms_properties_method: str = "itertools",
-) -> NDArray:
+def normalized_mindist(
+    points: pd.DataFrame,
+    grid: xr.DataArray,
+    low: float | None = None,
+    high: float | None = None,
+    mindist: float | None = None,
+    region: list[float] | None = None,
+) -> xr.DataArray:
     """
-    dispatcher for creating the jacobian matrix with 2 method options
+    Find the minimum distance between each grid cell and the nearest point. If low and
+    high are provided, normalize the min dists grid between these values. If region is
+    provided, all grid cells outside region are set to a distance of 0.
 
     Parameters
     ----------
-    deriv_type : str
-        choose between "annulus" and "prisms" methods of calculating the vertical
-        derivative of gravity of a prism
-    coordinates : pd.DataFrame
-        coordinate dataframe of gravity observation points with columns "easting",
-        "northing", "upward"
-    empty_jac : NDArray, optional
-        optionally provide an empty jacobian matrix of shape (number of gravity
-        observations x number of prisms), by default None
-    prisms_layer : xr.Dataset, optional
-        harmonica prism layer, by default None
-    prism_spacing : float, optional
-        resolution of prism layer, by default None
-    prism_size : float, optional
-        height of prisms for small prism vertical derivative method, by default None
-    prisms_properties_method : str, optional
-        method for extracting prism properties, by default "itertools"
+    points : pd.DataFrame
+        coordinates of the points
+    grid : xr.DataArray
+        gridded data to find min dists for each grid cell
+    low : float | None, optional
+        lower value for normalization, by default None
+    high : float | None, optional
+        higher value for normalization, by default None
+    mindist : float | None, optional
+        the minimum allowed distance, all values below are set equal to, by default None
+    region : list[float] | None, optional
+        bounding region for which all grid cells outside will be set to low, by default
+        None
 
     Returns
     -------
-    NDArray
-        a filled out jacobian matrix
+    xr.DataArray
+        grid of normalized minimum distances
     """
 
-    # convert dataframes to numpy arrays
-    coordinates_array = coordinates.to_numpy()
+    grid = copy.deepcopy(grid)
 
-    # get various arrays based on gravity column names
-    grav_easting = coordinates_array[:, coordinates.columns.get_loc("easting")]
-    grav_northing = coordinates_array[:, coordinates.columns.get_loc("northing")]
-    grav_upward = coordinates_array[:, coordinates.columns.get_loc("upward")]
+    # get coordinate names
+    original_dims = list(grid.sizes.keys())
 
-    assert len(grav_easting) == len(grav_northing) == len(grav_upward)
+    constraints_df = points.copy()
 
-    if empty_jac is None:
-        empty_jac = np.empty(
-            (len(grav_easting), prisms_layer.top.size),  # type: ignore[union-attr]
-            dtype=np.float64,
-        )
-        logging.warning("no empty jacobian supplied")
-
-    jac = empty_jac.copy()
+    min_dist: xr.DataArray = dist_nearest_points(
+        targets=constraints_df,
+        data=grid,
+        coord_names=(str(original_dims[1]), str(original_dims[0])),
+    ).min_dist
 
-    if deriv_type == "annulus":
-        # convert dataframe to arrays
-        # arrays = {
-        #   k:prisms_layer[k].to_numpy().ravel() for k in list(prisms_layer.variables)}
-        df = prisms_layer.to_dataframe().reset_index().dropna().astype(float)  # type: ignore[union-attr]
-        prism_easting = df.easting.to_numpy()
-        prism_northing = df.northing.to_numpy()
-        prism_top = df.top.to_numpy()
-        prism_density = df.density.to_numpy()
-
-        if np.all((prism_top - grav_upward.mean()) == 0):
-            msg = (
-                "All prism tops coincides exactly with the elevation of the gravity "
-                "observation points, leading to issues with calculating the vertical "
-                "derivative of gravity with the annulus technique. Either slightly "
-                "change the prism tops or gravity elevations, or use the small-prisms "
-                "vertical derivative technique."
-            )
-            logging.warning(msg)
+    # set points < mindist to low
+    if mindist is not None:
+        min_dist = xr.where(min_dist < mindist, 0, min_dist)
 
-        jac = jacobian_annular(
-            grav_easting,
-            grav_northing,
-            grav_upward,
-            prism_easting,
-            prism_northing,
-            prism_top,
-            prism_density,
-            prism_spacing,
-            jac,
+    # set points outside of region to low
+    if region is not None:
+        df = vd.grid_to_table(min_dist)
+        df["are_inside"] = vd.inside(
+            (df[original_dims[1]], df[original_dims[0]]),
+            region=region,
         )
+        new_min_dist = df.set_index([original_dims[0], original_dims[1]]).to_xarray()
+        new_min_dist = xr.where(new_min_dist.are_inside, new_min_dist, 0)
 
-    elif deriv_type == "prisms":
-        # get prisms info in following format, 3 methods:
-        # ((west, east, south, north, bottom, top), density)
-        assert prisms_layer is not None
-        prisms_properties = prism_properties(
-            prisms_layer,
-            method=prisms_properties_method,
-        )
-        if prism_size is None:
-            msg = "need to set small prism height"
-            raise ValueError(msg)
+        # add nans back
+        new_min_dist = xr.where(min_dist.isnull(), np.nan, new_min_dist)
 
-        jac = jacobian_prism(
-            prisms_properties,
-            grav_easting,
-            grav_northing,
-            grav_upward,
-            prism_size,
-            jac,
-        )
+        min_dist = new_min_dist.min_dist
 
+    # normalize from low to high
+    if (low is None) & (high is None):
+        pass
     else:
-        msg = "invalid string for deriv_type"
-        raise ValueError(msg)
+        assert low is not None
+        assert high is not None
+        min_dist = normalize_xarray(min_dist, low=low, high=high)
+
+    return min_dist
 
-    return jac
 
+def sample_grids(
+    df: pd.DataFrame,
+    grid: str | xr.DataArray,
+    sampled_name: str,
+    **kwargs: typing.Any,
+) -> pd.DataFrame:
+    """
+    Sample data at every point along a line
 
-def solver(
-    jac: NDArray,
-    residuals: NDArray,
-    damping: float | None = None,
-    solver_type: str = "scipy least squares",
-    # bounds =None,
-    # surface=None,
-) -> NDArray:
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe containing columns 'x', 'y', or columns with names defined by kwarg
+        "coor_names".
+    grid : str or xr.DataArray
+        Grid to sample, either file name or xr.DataArray
+    sampled_name : str,
+        Name for sampled column
+
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe with new column (sampled_name) of sample values from (grid)
+    """
+
+    # drop name column if it already exists
+    try:
+        df1 = df.drop(columns=sampled_name)
+    except KeyError:
+        df1 = df.copy()
+
+    df2 = df1.copy()
+
+    # reset the index
+    df3 = df2.reset_index()
+
+    x, y = kwargs.get("coord_names", ("easting", "northing"))
+    # get points to sample at
+    points = df3[[x, y]].copy()
+
+    # sample the grid at all x,y points
+    sampled = pygmt.grdtrack(
+        points=points,
+        grid=grid,
+        newcolname=sampled_name,
+        # radius=kwargs.get("radius", None),
+        no_skip=True,  # if false causes issues
+        verbose=kwargs.get("verbose", "w"),
+        interpolation=kwargs.get("interpolation", "c"),
+    )
+
+    df3[sampled_name] = sampled[sampled_name]
+
+    # reset index to previous
+    df4 = df3.set_index("index")
+
+    # reset index name to be same as originals
+    df4.index.name = df1.index.name
+
+    # check that dataframe is identical to original except for new column
+    pd.testing.assert_frame_equal(df4.drop(columns=sampled_name), df1)
+
+    return df4
+
+
+def extract_prism_data(
+    prism_layer: xr.Dataset,
+) -> tuple[
+    pd.DataFrame,
+    xr.Dataset,
+    float,
+    xr.DataArray,
+]:
     """
-    Calculate shift to add to prism's for each iteration of the inversion. Finds
-    the least-squares solution to the Jacobian and the gravity residual
+    extract necessary info from starting prism layer, adds variables 'topo' and
+    'starting_topo' to prism layer dataset (prisms_ds), converts it into dataframe
+    (prisms_df), gets the prism spacing (spacing) from prisms_ds, and creates a grid of
+    the starting topography (topo_grid) from the tops and bottoms of the prism layer.
 
     Parameters
     ----------
-    jac : NDArray
-        input jacobian matrix with a row per gravity observation, and a column per
-        prisms.
-    residuals : NDArray
-        array of gravity residuals
-    damping : float | None, optional
-        positive damping (Tikhonov 0th order) regularization
-    solver_type : {
-        'verde least squares',
-        'scipy least squares',
-        'scipy conjugate',
-        'numpy least squares',
-        'steepest descent',
-        'gauss newton',
-        } optional
-        choose which solving method to use, by default "scipy least squares"
+    prism_layer : xr.Dataset
+       starting model prism layer
 
     Returns
     -------
-    NDArray
-        array of correction values to apply to each prism.
+    tuple[pd.DataFrame, pd.Dataset, float, xr.DataArray]
+        prisms_df, prisms_ds, spacing, topo_grid
     """
 
-    if solver_type == "scipy least squares":
-        # https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.lsqr.html
+    prisms_ds = copy.deepcopy(prism_layer.load())
 
-        if damping is None:
-            damping = 0
-        results = sp.sparse.linalg.lsqr(
-            A=jac,
-            b=residuals,
-            show=False,
-            damp=damping,  # float, typically 0-1
-            # atol= ,
-            # btol=1e-4, # if 1e-6, residuals should be accurate to ~6 digits
-            iter_lim=5000,  # limit of iterations, just in case of issues
-        )
-        # print(f"number of solver iters:{results[2]}")
-        step = results[0]
+    # add starting topo to dataset
+    topo_grid = xr.where(prisms_ds.density > 0, prisms_ds.top, prisms_ds.bottom)
+    prisms_ds["topo"] = topo_grid
+    prisms_ds["starting_topo"] = topo_grid
 
-    # elif solver_type == "verde least squares":
-    #     """
-    #     if damping not None, uses sklearn.linear_model.Ridge(alpha=damping)
-    #     alpha: 0 to +inf. multiplies the L2 term, can also pass an array
-    #     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html # noqa: E501
-    #     """
-    #     step = vd.base.least_squares(
-    #         jacobian=jac,
-    #         data=residuals,
-    #         weights=weights,
-    #         damping=damping,  # float, typically 100-10,000
-    #         copy_jacobian=False,
-    #     )
-
-    # elif solver_type == "scipy constrained":
-    #     """
-    #     https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.lsq_linear.html#scipy.optimize.lsq_linear # noqa: E501
-    #     """
-    #     if bounds is None:
-    #         step = sp.optimize.lsq_linear(
-    #             A=jac,
-    #             b=residuals,
-    #             method="trf",
-    #             max_iter=5,
-    #         )["x"]
-    #     else:
-    #         step = sp.optimize.lsq_linear(
-    #             A=jac,
-    #             b=residuals,
-    #             bounds=bounds,
-    #             method="trf",
-    #             max_iter=5,
-    #         )["x"]
-    # # elif solver_type == "scipy nonlinear lsqr":
-    # #     """
-    # #     https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.least_squares.html#scipy.optimize.least_squares # noqa: E501
-    # #     """
-    # #     if bounds is None:
-    # #         bounds = [-np.inf, np.inf]
-
-    # elif solver_type == "CLR":
-    #     """
-    #     https://github.com/avidale/constrained-linear-regression
-    #     """
-    #     model = ConstrainedLinearRegression(
-    #         # max_iter=2,
-    #         ridge=damping,
-    #         # fit_intercept=False,
-    #     )
-    #     if bounds is None:
-    #         step = model.fit(
-    #             X=jac,
-    #             y=residuals,
-    #         ).coef_
-    #     else:
-    #         step = model.fit(
-    #             X=jac,
-    #             y=residuals,
-    #             min_coef=bounds[0],
-    #             max_coef=bounds[1],
-    #         ).coef_
-
-    # elif solver_type == "scipy conjugate":
-    #     step = sp.sparse.linalg.cg(
-    #         jac,
-    #         residuals,
-    #     )[0]
-
-    # elif solver_type == "numpy least squares":
-    #     step = np.linalg.lstsq(
-    #         jac,
-    #         residuals,
-    #     )[0]
-
-    # elif solver_type == "steepest descent":
-    #     """Jacobian transpose algorithm"""
-    #     residuals = residuals
-    #     step = jac.T @ residuals
-
-    # elif solver_type == "gauss newton":
-    #     """
-    #     Gauss Newton w/ 1st order Tikhonov regularization
-    #     from https://nbviewer.org/github/compgeolab/2020-aachen-inverse-problems/blob/main/gravity-inversion.ipynb # noqa: E501
-    #     """
-    #     if damping in [None, 0]:
-    #         hessian = jac.T @ jac
-    #         gradient = jac.T @ residuals
-    #     else:
-    #         fdmatrix = finite_difference_matrix(jac[0].size)
-    #         hessian = jac.T @ jac + damping * fdmatrix.T @ fdmatrix
-    #         gradient = (
-    #             jac.T @ residuals - damping * fdmatrix.T @ fdmatrix @ surface
-    #         )
-
-    #     # scipy solver appears to be slightly faster
-    #     # step = np.linalg.solve(hessian, gradient)
-    #     step = sp.linalg.solve(hessian, gradient)
+    # turn dataset into dataframe
+    prisms_df = prisms_ds.to_dataframe().reset_index().dropna().astype(float)
 
-    else:
-        msg = "invalid string for solver_type"
-        raise ValueError(msg)
+    spacing = get_spacing(prisms_df)
 
-    return step
+    return prisms_df, prisms_ds, spacing, topo_grid
 
 
-# def finite_difference_matrix(nparams):
-#     """
-#     Create the finite difference matrix for regularization.
-#     """
-#     fdmatrix = np.zeros((nparams - 1, nparams))
-#     for i in range(fdmatrix.shape[0]):
-#         fdmatrix[i, i] = -1
-#         fdmatrix[i, i + 1] = 1
-#     return fdmatrix
-
-
-def update_l2_norms(
-    rmse: float,
-    l2_norm: float,
-) -> tuple[float, float]:
+def get_spacing(prisms_df: pd.DataFrame) -> float:
     """
-    update the l2 norm and delta l2 norm of the misfit
+    Extract spacing of harmonica prism layer using a dataframe representation.
 
     Parameters
     ----------
-    rmse : float
-        root mean square error of the residual gravity misfit
-    l2_norm : float
-        l2 norm of the residual gravity misfit
+    prisms_df : pd.DataFrame
+        dataframe of harmonica prism layer
+
     Returns
     -------
-    tuple[float, float]
-        updated l2 norm and delta l2 norm
+    float
+        spacing of prisms
     """
+    return float(abs(prisms_df.northing.unique()[1] - prisms_df.northing.unique()[0]))
 
-    # square-root of RMSE is the l-2 norm
-    updated_l2_norm = np.sqrt(rmse)
 
-    updated_delta_l2_norm = l2_norm / updated_l2_norm
+def sample_bounding_surfaces(
+    prisms_df: pd.DataFrame,
+    upper_confining_layer: xr.DataArray | None = None,
+    lower_confining_layer: xr.DataArray | None = None,
+) -> pd.DataFrame:
+    """
+    sample upper and/or lower confining layers into prisms dataframe
 
-    # we want the misfit (L2-norm) to be steadily decreasing with each iteration.
-    # If it increases, something is wrong, stop inversion
-    # If it doesn't decrease enough, inversion has finished and can be stopped
-    # delta L2 norm starts at +inf, and should decreases with each iteration.
-    # if it gets close to 1, the iterations aren't making progress and can be stopped.
-    # a value of 1.001 means the L2 norm has only decrease by 0.1% between iterations.
-    # and RMSE has only decreased by 0.05%.
+    Parameters
+    ----------
+    prisms_df : pd.DataFrame
+        dataframe of prism properties
+    upper_confining_layer : xr.DataArray | None, optional
+        layer which the inverted topography should always be below, by default None
+    lower_confining_layer : xr.DataArray | None, optional
+        layer which the inverted topography should always be above, by default None
 
-    # update the l2_norm
-    l2_norm = updated_l2_norm
+    Returns
+    -------
+    pd.DataFrame
+        a dataframe with added columns 'upper_bounds' and 'lower_bounds', which are the
+        sampled values of the supplied confining grids.
+    """
+    df = prisms_df.copy()
 
-    # updated the delta l2_norm
-    delta_l2_norm = updated_delta_l2_norm
+    if upper_confining_layer is not None:
+        df = sample_grids(
+            df=df,
+            grid=upper_confining_layer,
+            sampled_name="upper_bounds",
+            coord_names=["easting", "northing"],
+        )
+        assert len(df.upper_bounds) != 0
+    if lower_confining_layer is not None:
+        df = sample_grids(
+            df=df,
+            grid=lower_confining_layer,
+            sampled_name="lower_bounds",
+            coord_names=["easting", "northing"],
+        )
+        assert len(df.lower_bounds) != 0
+    return df
 
-    return (
-        l2_norm,
-        delta_l2_norm,
-    )
 
+def enforce_confining_surface(
+    prisms_df: pd.DataFrame,
+    iteration_number: int,
+) -> pd.DataFrame:
+    """
+    alter the surface correction values to ensure when added to the current iteration's
+    topography it doesn't intersect optional confining layers.
 
-def end_inversion(
+    Parameters
+    ----------
+    prisms_df : pd.DataFrame
+        prism layer dataframe with optional 'upper_bounds' or 'lower_bounds' columns,
+        and current iteration's topography.
+    iteration_number : int
+        number of the current iteration, starting at 1 not 0
+
+    Returns
+    -------
+    pd.DataFrame
+        a dataframe with added column 'iter_{iteration_number}_correction
+    """
+
+    df = prisms_df.copy()
+
+    if "upper_bounds" in df:
+        # get max upward change allowed for each prism
+        # positive values indicate max allowed upward change
+        # negative values indicate topography is already too far above upper bound
+        df["max_change_above"] = df.upper_bounds - df.topo
+        number_enforced = 0
+        for i, j in enumerate(df[f"iter_{iteration_number}_correction"]):
+            if j > df.max_change_above[i]:
+                number_enforced += 1
+                df.loc[i, f"iter_{iteration_number}_correction"] = df.max_change_above[
+                    i
+                ]
+        logging.info("enforced upper confining surface at %s prisms", number_enforced)
+    if "lower_bounds" in df:
+        # get max downward change allowed for each prism
+        # negative values indicate max allowed downward change
+        # positive values indicate topography is already too far below lower bound
+        df["max_change_below"] = df.lower_bounds - df.topo
+        number_enforced = 0
+        for i, j in enumerate(df[f"iter_{iteration_number}_correction"]):
+            if j < df.max_change_below[i]:
+                number_enforced += 1
+                df.loc[i, f"iter_{iteration_number}_correction"] = df.max_change_below[
+                    i
+                ]
+
+        logging.info("enforced lower confining surface at %s prisms", number_enforced)
+
+    # check that when constrained correction is added to topo it doesn't intersect
+    # either bounding layer
+    updated_topo: pd.Series[float] = df[f"iter_{iteration_number}_correction"] + df.topo
+    if "upper_bounds" in df and np.any((df.upper_bounds - updated_topo) < -0.001):
+        msg = (
+            "Constraining didn't work and updated topography intersects upper "
+            "constraining surface"
+        )
+        raise ValueError(msg)
+    if "lower_bounds" in df and np.any((updated_topo - df.lower_bounds) < -0.001):
+        msg = (
+            "Constraining didn't work and updated topography intersects lower "
+            "constraining surface"
+        )
+        raise ValueError(msg)
+    return df
+
+
+def apply_surface_correction(
+    prisms_df: pd.DataFrame,
     iteration_number: int,
-    max_iterations: int,
-    l2_norm: float,
-    starting_l2_norm: float,
-    l2_norm_tolerance: float,
-    delta_l2_norm: float,
-    previous_delta_l2_norm: float,
-    delta_l2_norm_tolerance: float,
-    perc_increase_limit: float = 0.20,
-) -> tuple[bool, list[str]]:
+) -> tuple[pd.DataFrame, xr.DataArray]:
     """
-    check if the inversion should be terminated
+    update the prisms dataframe and dataset with the surface correction. Ensure that
+    the updated surface doesn't intersect the optional confining surfaces.
 
     Parameters
     ----------
+    prisms_df : pd.DataFrame
+        dataframe of prism properties
     iteration_number : int
         the iteration number, starting at 1 not 0
-    max_iterations : int
-        the maximum allowed iterations, inclusive and starting at 1
-    l2_norm : float
-        the current iteration's l2 norm
-    starting_l2_norm : float
-        the l2 norm of iteration 1
-    l2_norm_tolerance : float
-        the l2 norm value to end the inversion at
-    delta_l2_norm : float
-        the current iteration's delta l2 norm
-    previous_delta_l2_norm : float
-        the delta l2 norm of the previous iteration
-    delta_l2_norm_tolerance : float
-        the delta l2 norm value to end the inversion at
-    perc_increase_limit : float, optional
-        the set tolerance for decimal percentage increase relative to the starting l2
-        norm, by default 0.20
 
     Returns
     -------
-    tuple[bool, list[str]]
-        first term is a boolean of whether or not to end the inversion, second term is a
-        list of termination reasons.
+    tuple[pd.DataFrame, xr.DataArray]
+        updated prisms dataframe and correction grid
     """
-    end = False
-    termination_reason = []
 
-    # ignore for first iteration
-    if iteration_number == 1:
-        pass
-    else:
-        if l2_norm > starting_l2_norm * (1 + perc_increase_limit):
-            logging.info(
-                "\nInversion terminated after %s iterations because L2 norm (%s) \n"
-                "was over %s%% greater than starting L2 norm (%s) \n"
-                "Change parameter 'perc_increase_limit' if desired.",
-                iteration_number,
-                l2_norm,
-                perc_increase_limit * 100,
-                starting_l2_norm,
-            )
-            end = True
-            termination_reason.append("l2-norm increasing")
+    df = prisms_df.copy()
 
-        if (delta_l2_norm <= delta_l2_norm_tolerance) & (
-            previous_delta_l2_norm <= delta_l2_norm_tolerance
-        ):
-            logging.info(
-                "\nInversion terminated after %s iterations because there was no "
-                "significant variation in the L2-norm over 2 iterations \n"
-                "Change parameter 'delta_l2_norm_tolerance' if desired.",
-                iteration_number,
-            )
+    # for negative densities, negate the correction
+    df.loc[df.density < 0, f"iter_{iteration_number}_correction"] *= -1
 
-            end = True
-            termination_reason.append("delta l2-norm tolerance")
+    # optionally constrain the surface correction with bounding surfaces
+    df = enforce_confining_surface(df, iteration_number)
 
-        if l2_norm < l2_norm_tolerance:
-            logging.info(
-                "\nInversion terminated after %s iterations because L2-norm (%s) was "
-                "less then set tolerance: %s \nChange parameter "
-                "'l2_norm_tolerance' if desired.",
-                iteration_number,
-                l2_norm,
-                l2_norm_tolerance,
-            )
+    # grid the corrections
+    correction_grid = (
+        df.rename(columns={f"iter_{iteration_number}_correction": "z"})
+        .set_index(["northing", "easting"])
+        .to_xarray()
+        .z
+    )
 
-            end = True
-            termination_reason.append("l2-norm tolerance")
+    return df, correction_grid
 
-    if iteration_number >= max_iterations:
-        logging.info(
-            "\nInversion terminated after %s iterations with L2-norm=%s because "
-            "maximum number of iterations (%s) reached.",
-            iteration_number,
-            round(l2_norm, 2),
-            max_iterations,
-        )
 
-        end = True
-        termination_reason.append("max iterations")
+def update_prisms_ds(
+    prisms_ds: xr.Dataset,
+    correction_grid: xr.DataArray,
+    zref: float,
+) -> xr.Dataset:
+    """
+    apply the corrections grid and update the prism tops, bottoms, topo, and
+    densities.
+
+    Parameters
+    ----------
+    prisms_ds : xr.Dataset
+        harmonica prism layer
+    correction_grid : xr.DataArray
+        grid of corrections to apply to the prism layer
+    zref : float
+        reference level for the prism layer
+
+    Returns
+    -------
+    xr.Dataset
+        updated prism layer with new tops, bottoms, topo, and densities
+    """
+
+    ds = prisms_ds.copy()
+
+    density_contrast = ds.density.values.max()
+
+    # create topo from top and bottom
+    topo_grid = xr.where(ds.density > 0, ds.top, ds.bottom)
+
+    # apply correction to topo
+    topo_grid += correction_grid
 
-    return end, termination_reason
+    # update the prism layer
+    ds.prism_layer.update_top_bottom(surface=topo_grid, reference=zref)
 
+    # update the density
+    ds["density"] = xr.where(ds.top > zref, density_contrast, -density_contrast)
 
-def update_gravity_and_misfit(
-    gravity_df: pd.DataFrame,
+    # update the topo
+    ds["topo"] = topo_grid
+
+    return ds
+
+
+def add_updated_prism_properties(
+    prisms_df: pd.DataFrame,
     prisms_ds: xr.Dataset,
-    input_grav_column: str,
     iteration_number: int,
 ) -> pd.DataFrame:
     """
-    calculate the forward gravity of the supplied prism layer, add the results to a
-    new dataframe column, and update the residual misfit. The supplied gravity dataframe
-    needs a 'reg' column, which describes the regional component and can be 0.
+    update the prisms dataframe the the new prism tops, bottoms, topo, and densities
+    the iteration number, starting at 1 not 0
 
     Parameters
     ----------
-    gravity_df : pd.DataFrame
-        gravity dataframe with gravity observation coordinate columns ('easting',
-        'northing', 'upwards'), a gravity data column, set by `input_grav_column`,
-        and a regional gravity column ('reg').
-
+    prisms_df : pd.DataFrame
+        dataframe of prism properties
     prisms_ds : xr.Dataset
-        harmonica prism layer
-    input_grav_column : str
-        name of gravity data column
+        dataset of prism properties
     iteration_number : int
-        iteration number to use in updated column names
+        the iteration number, starting at 1 not 0
 
     Returns
     -------
     pd.DataFrame
-        a gravity dataframe with 2 new columns, one for the iterations forward gravity
-        and one for the iterations residual misfit.
+        updated prism dataframe with new tops, bottoms, topo, and densities
     """
-    gravity = gravity_df.copy()
 
-    # update the forward gravity
-    gravity[f"iter_{iteration_number}_forward_grav"] = prisms_ds.prism_layer.gravity(
-        coordinates=(gravity.easting, gravity.northing, gravity.upward),
-        field="g_z",
-    )
+    df = prisms_df.copy()
+    ds = prisms_ds.copy()
 
-    # each iteration updates the topography of the layer to minimize the residual
-    # portion of the misfit. We then want to recalculate the forward gravity of the
-    # new layer, use the same original regional misfit, and re-calculate the residual
-    # Gmisfit  = Gobs_corr - Gforward
-    # Gres = Gmisfit - Greg
-    # Gres = Gobs_corr_shift - Gforward - Greg
-    # update the residual misfit with the new forward gravity and the same regional
-    gravity[f"iter_{iteration_number}_final_misfit"] = (
-        gravity[input_grav_column]
-        - gravity[f"iter_{iteration_number}_forward_grav"]
-        - gravity.reg
-    )
+    # turn back into dataframe
+    prisms_iter = ds.to_dataframe().reset_index().dropna().astype(float)
 
-    return gravity
+    # add new cols to dict
+    dict_of_cols = {
+        f"iter_{iteration_number}_top": prisms_iter.top,
+        f"iter_{iteration_number}_bottom": prisms_iter.bottom,
+        f"iter_{iteration_number}_density": prisms_iter.density,
+        f"iter_{iteration_number}_layer": prisms_iter.topo,
+    }
 
+    df = pd.concat([df, pd.DataFrame(dict_of_cols)], axis=1)
+    df["topo"] = prisms_iter.topo
+
+    return df
 
-def run_inversion(
-    input_grav: pd.DataFrame,
-    input_grav_column: str,
-    prism_layer: xr.Dataset,
-    density_contrast: float,
-    zref: float,
-    max_iterations: int,
-    l2_norm_tolerance: float = 0.2,
-    delta_l2_norm_tolerance: float = 1.001,
-    perc_increase_limit: float = 0.10,
-    deriv_type: str = "annulus",
-    jacobian_prism_size: float = 1,
-    solver_type: str = "scipy least squares",
-    solver_damping: float | None = None,
-    upper_confining_layer: xr.DataArray | None = None,
-    lower_confining_layer: xr.DataArray | None = None,
-    weights_after_solving: bool = False,
-    inversion_region: tuple[float, float, float, float] | None = None,
-    plot_convergence: bool = False,
-    plot_dynamic_convergence: bool = False,
-) -> tuple[pd.DataFrame, pd.DataFrame, dict[str, typing.Any], float]:
-    """
-    perform a geometric inversion, where the topography is updated to minimize the
-    residual misfit between the forward gravity of the layer, and the observed gravity.
-    To aid in regularizing an ill-posed problem choose any of the following options:
-    * add damping to the solver, with `solver_damping`
-    * weight the surface correction values with a weighting grid with
-    `weights_after_solving` and the `weights` variable of the prisms dataset
-    * bound the topography of the layer, with `upper_confining_layer` and
-    `lower_confining_layer`
+
+def create_topography(
+    method: str,
+    region: tuple[float, float, float, float],
+    spacing: float,
+    registration: str = "g",
+    upwards: float | None = None,
+    constraints_df: pd.DataFrame | None = None,
+    dampings: list[float] | None = None,
+) -> xr.DataArray:
+    """
+    Create a grid of topography data from either the interpolation of point data or
+    creating a grid of constant value.
 
     Parameters
     ----------
-    input_grav : pd.DataFrame
-        dataframe with gravity data and coordinates, must have columns "res" and "reg"
-        for residual and regional gravity, and coordinate columns "easting", "northing",
-        and "upward".
-    input_grav_column : str
-        column name containing the gravity data *before* regional separation
-    prism_layer : xr.Dataset
-        starting prism layer
-    density_contrast : float
-        density contrast of the prisms layer, should be same value used to create the
-        starting model
-    zref : float
-        reference height of the prisms layer, should be same value used to create the
-        starting model
-    max_iterations : int
-        the maximum allowed iterations, inclusive and starting at 1
-    l2_norm_tolerance : float, optional
-        _the l2 norm value to end the inversion at, by default 0.2
-    delta_l2_norm_tolerance : float, optional
-        the delta l2 norm value to end the inversion at, by default 1.001
-    perc_increase_limit : float, optional
-        the set tolerance for decimal percentage increase relative to the starting l2
-        norm, by default 0.10
-    deriv_type : str, optional
-        either "annulus" or "prism" to determine method of calculating the vertical
-        derivate of gravity of a prism, by default "annulus"
-    jacobian_prism_size : float, optional
-        height of prisms in meters for vertical derivative, by default 1
-    solver_type : str, optional
-        solver type to use, by default "scipy least squares"
-    solver_damping : float | None, optional
-        damping parameter for regularization of the solver, by default None
-    upper_confining_layer : xr.DataArray | None, optional
-        topographic layer to use as upper limit for inverted topography, by default None
-    lower_confining_layer : xr.DataArray | None, optional
-        topographic layer to use as lower limit for inverted topography, by default None
-    weights_after_solving : bool, optional
-        use "weights" variable of prisms dataset to scale surface corrections grid, by
-        default False, by default False
-    inversion_region : tuple[float, float, float, float]
-        inside region to calculated residual RMSE within, in the form (min_easting,
-        max_easting, min_northing, max_northing)
-    plot_convergence : bool, optional
-        plot the misfit convergence, by default False
-    plot_dynamic_convergence : bool, optional
-        plot the misfit convergence dynamically, by default False
+    method : str
+        method to use, either 'flat' or 'splines'
+    region : tuple[float, float, float, float]
+        region of the grid
+    spacing : float
+        spacing of the grid
+    registration : str, optional
+        choose between gridline "g" or pixel "p" registration, by default "g"
+    upwards : float | None, optional
+        constant value to use for method "flat", by default None
+    constraints_df : pd.DataFrame | None, optional
+        dataframe with column 'upwards' to use for method "splines", by default None
+    dampings : list[float] | None, optional
+        damping values to use in spline cross validation for method "spline", by
+        default None
 
     Returns
     -------
-    tuple[pd.DataFrame, pd.DataFrame, dict[str, typing.Any], float]
-        prisms_df: pd.DataFrame, prism properties for each iteration,
-        gravity: pd.DataFrame, gravity anomalies for each iteration,
-        params: dict, Properties of the inversion such as kwarg values,
-        elapsed_time: float, time in seconds for the inversion to run
+    xr.DataArray
+        a topography grid
     """
+    if dampings is None:
+        dampings = np.logspace(-10, 0, 20)
 
-    logging.info("starting inversion")
-
-    time_start = time.perf_counter()
+    if method == "flat":
+        if registration == "g":
+            pixel_register = False
+        elif registration == "p":
+            pixel_register = True
+        else:
+            msg = "registration must be 'g' or 'p'"
+            raise ValueError(msg)
 
-    gravity = copy.deepcopy(input_grav)
+        if upwards is None:
+            msg = "upwards must be provided if method is `flat`"
+            raise ValueError(msg)
 
-    # if inversion region provided, create column of booleans defining inside/outside
-    if inversion_region is not None:
-        gravity["inside"] = vd.inside(
-            (gravity.easting, gravity.northing),
-            region=inversion_region,
-        )
+        # create grid of coordinates
+        (x, y) = vd.grid_coordinates(  # pylint: disable=unbalanced-tuple-unpacking
+            region=region,
+            spacing=spacing,
+            pixel_register=pixel_register,
+        )
+        # make flat topography of value = upwards
+        return vd.make_xarray_grid(
+            (x, y),
+            np.ones_like(x) * upwards,
+            data_names="upward",
+            dims=("northing", "easting"),
+        ).upward
+
+    if method == "splines":
+        # get coordinates of the constraint points
+        if constraints_df is None:
+            msg = "constraints_df must be provided if method is `splines`"
+            raise ValueError(msg)
+        coords = (constraints_df.easting, constraints_df.northing)
 
-    # extract variables from starting prism layer
-    (
-        prisms_df,
-        prisms_ds,
-        prism_spacing,
-        _,
-    ) = utils.extract_prism_data(prism_layer)
-
-    logging.info("extracted prism spacing is %s", prism_spacing)
-
-    # create empty jacobian matrix
-    empty_jac: NDArray = np.empty(
-        (len(gravity[input_grav_column]), prisms_ds.top.size),
-        dtype=np.float64,
-    )
+        # create a cross validated spline with default values
+        spline = vd.SplineCV(dampings=dampings)
 
-    # if there is a confining surface (above or below), which the inverted layer
-    # shouldn't intersect, then sample those layers into the df
-    prisms_df = utils.sample_bounding_surfaces(
-        prisms_df,
-        upper_confining_layer,
-        lower_confining_layer,
-    )
+        # fit the spline to the constraint points
+        try:
+            spline.fit(
+                coordinates=coords,
+                data=constraints_df.upward,
+            )
+        except ValueError as e:
+            logging.warning(e)
+            spline = vd.Spline()
+            spline.fit(
+                coordinates=coords,
+                data=constraints_df.upward,
+            )
+            return spline.grid(
+                region=region,
+                spacing=spacing,
+            ).scalars
+
+        try:
+            if spline.damping_ in [np.min(dampings), np.max(dampings)]:
+                logging.warning(
+                    "Warning: best damping parameter (%s) for verde.SplineCV() is at "
+                    "the limit of provided values (%s, %s) and thus is likely not a "
+                    "global minimum, expand the range of values with 'dampings' to "
+                    "ensure the best damping value is found.",
+                    spline.damping_,
+                    np.nanmin(dampings),
+                    np.nanmax(dampings),
+                )
+        except TypeError:
+            pass
 
-    # set starting delta L2 norm to positive infinity
-    delta_l2_norm = np.inf
+        # grid the fitted spline at desired spacing and region
+        return spline.grid(
+            region=region,
+            spacing=spacing,
+        ).scalars
+
+    msg = "method must be 'flat' or 'splines'"
+    raise ValueError(msg)
+
+
+def grids_to_prisms(
+    surface: xr.DataArray,
+    reference: float | xr.DataArray,
+    density: float | int | xr.DataArray,
+    input_coord_names: tuple[str, str] = ("easting", "northing"),
+) -> xr.Dataset:
+    """
+    create a Harmonica layer of prisms with assigned densities.
 
-    # iteration times
-    iter_times = []
+    Parameters
+    ----------
+    surface : xr.DataArray
+        data to use for prism surface
+    reference : float | xr.DataArray
+        data or constant to use for prism reference, if value is below surface, prism
+        will be inverted
+    density : float | int | xr.DataArray
+        data or constant to use for prism densities.
+    input_coord_names : tuple[str, str], optional
+        names of the coordinates in the input dataarray, by default
+        ["easting", "northing"]
+    Returns
+    -------
+    xr.Dataset
+       a prisms layer with assigned densities
+    """
 
-    pbar = tqdm(range(max_iterations), desc="Iteration")
-    for iteration, _ in enumerate(pbar, start=1):
-        logging.info(
-            "\n #################################### \n iteration %s", iteration
-        )
-        # start iteration timer
-        iter_time_start = time.perf_counter()
+    # if density provided as a single number, use it for all prisms
+    if isinstance(density, (float, int)):
+        dens = density * np.ones_like(surface)
+    # if density provided as a dataarray, map each density to the correct prisms
+    elif isinstance(density, xr.DataArray):
+        dens = density
+    else:
+        msg = "invalid density type, should be a number or DataArray"
+        raise ValueError(msg)
 
-        # after first iteration reset residual with previous iteration's results
-        if iteration == 1:
-            pass
-        else:
-            gravity["res"] = gravity[f"iter_{iteration-1}_final_misfit"]
-            prisms_df["density"] = prisms_df[f"iter_{iteration-1}_density"]
+    # create layer of prisms based off input dataarrays
+    prisms = hm.prism_layer(
+        coordinates=(
+            surface[input_coord_names[0]].values,
+            surface[input_coord_names[1]].values,
+        ),
+        surface=surface,
+        reference=reference,
+        properties={
+            "density": dens,
+        },
+    )
 
-        # add starting residual to df
-        gravity[f"iter_{iteration}_initial_misfit"] = gravity.res
+    prisms["thickness"] = prisms.top - prisms.bottom
 
-        # set iteration stats
-        if inversion_region is not None:
-            # if inversion region is supplied, calculate RMSE only within that region
-            initial_rmse = utils.rmse(
-                gravity[gravity.inside][f"iter_{iteration}_initial_misfit"]
-            )
-        else:
-            initial_rmse = utils.rmse(gravity[f"iter_{iteration}_initial_misfit"])
-        l2_norm = np.sqrt(initial_rmse)
+    return prisms
 
-        if iteration == 1:
-            starting_misfit = initial_rmse
-            starting_l2_norm = l2_norm
-
-        # calculate jacobian sensitivity matrix
-        jac = jacobian(
-            deriv_type,
-            gravity.select_dtypes(include=["number"]),
-            empty_jac,
-            prisms_layer=prisms_ds,
-            prism_spacing=prism_spacing,
-            prism_size=jacobian_prism_size,
-        )
 
-        # calculate correction for each prism
-        surface_correction = solver(
-            jac=jac,
-            residuals=gravity.res.values,
-            damping=solver_damping,
-            solver_type=solver_type,
-        )
+def best_spline_cv(
+    coordinates: tuple[pd.Series | NDArray, pd.Series | NDArray],
+    data: pd.Series | NDArray,
+    weights: pd.Series | NDArray | None = None,
+    dampings: typing.Any | None = None,
+    delayed: bool = False,
+    force_coords: tuple[pd.Series | NDArray, pd.Series | NDArray] | None = None,
+) -> vd.Spline:
+    """
+    find the best damping parameter for a verde.SplineCV() fit
 
-        # print correction values
-        logging.info(
-            "Layer correction median: %s m, RMSE:%s m",
-            round(np.median(surface_correction), 4),
-            round(utils.rmse(surface_correction), 4),
-        )
+    Parameters
+    ----------
+    coordinates : tuple[pd.Series  |  NDArray, pd.Series  |  NDArray]
+        easting and northing coordinates of the data
+    data : pd.Series | NDArray
+        data for fitting the spline to
+    weights : pd.Series | NDArray | None, optional
+        if not None, then the weights assigned to each data point. Typically, this
+        should be 1 over the data uncertainty squared, by default None
+    dampings : typing.Any | None, optional
+        the positive damping regularization parameter. Controls how much smoothness is
+        imposed on the estimated forces. If None, no regularization is used, by default
+        None
+    delayed : bool, optional
+        if True, will use dask.delayed to dispatch computations and allow mod:dask to
+        execute the grid search in parallel, by default False
+    force_coords : tuple[pd.Series  |  NDArray, pd.Series  |  NDArray] | None, optional
+        the easting and northing coordinates of the point forces. Same as force_coords
+        if it is not None. Otherwise, same as the data locations used to fit the spline,
+        by default None
 
-        # add corrections to prisms_df
-        prisms_df = pd.concat(
-            [
-                prisms_df,
-                pd.DataFrame({f"iter_{iteration}_correction": surface_correction}),
-            ],
-            axis=1,
-        )
-        # apply the surface correction to the prisms dataframe and enforce confining
-        # layer if supplied
-        prisms_df, correction_grid = utils.apply_surface_correction(
-            prisms_df, iteration
-        )
+    Returns
+    -------
+    vd.Spline
+        the spline which best fits the data
+    """
+    if isinstance(dampings, (float, int)):
+        dampings = [dampings]
 
-        # instead of applying weights to the Jacobian, apply them to the topo
-        # correction grid
-        if weights_after_solving is True:
-            correction_grid = correction_grid * prisms_ds.weights
-
-        # add the corrections to the topo and update the prisms dataset
-        prisms_ds = utils.update_prisms_ds(prisms_ds, correction_grid, zref)
-
-        # add updated properties to prisms dataframe
-        prisms_df = utils.add_updated_prism_properties(
-            prisms_df,
-            prisms_ds,
-            iteration,
-        )
+    # if dampings is None:
+    #     dampings = list(np.logspace(-10, -2, num=9))
+    #     dampings.append(None)
+    spline = vd.SplineCV(
+        dampings=dampings,
+        delayed=delayed,
+        force_coords=force_coords,
+    )
+    # with warnings.catch_warnings():
+    # warnings.simplefilter("ignore", sp.linalg.LinAlgWarning)
+    # with HiddenPrints():
+    spline.fit(
+        coordinates,
+        data,
+        weights=weights,
+    )
 
-        if upper_confining_layer is not None:
-            assert np.all(prisms_df.upper_bounds - prisms_df.topo) >= 0
+    try:
+        logging.info("Highest score: %s", spline.scores_.max())
+    except AttributeError:
+        logging.info("Highest score: %s", max(dask.compute(spline.scores_)[0]))
+
+    logging.info("Best damping: %s", spline.damping_)
+
+    try:
+        if len(dampings) > 2 and spline.damping_ in [  # type: ignore [arg-type]
+            np.min(dampings),
+            np.max(dampings),
+        ]:
+            logging.warning(
+                "Warning: best damping parameter (%s) for verde.SplineCV() is at the "
+                "limit of provided values (%s, %s) and thus is likely not a global "
+                "minimum, expand the range of values with 'dampings' to ensure the best"
+                " damping value is found.",
+                spline.damping_,
+                np.nanmin(dampings),
+                np.nanmax(dampings),
+            )
 
-        # update the forward gravity and the misfit
-        gravity = update_gravity_and_misfit(
-            gravity,
-            prisms_ds,
-            input_grav_column,
-            iteration,
-        )
+    except TypeError:
+        pass
 
-        # update the misfit RMSE
-        if inversion_region is not None:
-            # if inversion region is supplied, calculate RMSE only within that region
-            updated_rmse = utils.rmse(
-                gravity[gravity.inside][f"iter_{iteration}_final_misfit"]
-            )
-        else:
-            updated_rmse = utils.rmse(gravity[f"iter_{iteration}_final_misfit"])
-        logging.info("updated misfit RMSE: %s", round(updated_rmse, 4))
-        final_rmse = updated_rmse
-
-        # update the l2 and delta l2 norms
-        previous_delta_l2_norm = copy.copy(delta_l2_norm)
-        l2_norm, delta_l2_norm = update_l2_norms(updated_rmse, l2_norm)
-        final_l2_norm = l2_norm
-        logging.info(
-            "updated L2-norm: %s, tolerance: %s", round(l2_norm, 4), l2_norm_tolerance
-        )
-        logging.info(
-            "updated delta L2-norm : %s, tolerance: %s",
-            round(delta_l2_norm, 4),
-            delta_l2_norm_tolerance,
-        )
+    return spline
 
-        # end iteration timer
-        iter_time_end = time.perf_counter()
-        iter_times.append(iter_time_end - iter_time_start)
-
-        # decide if to end the inversion
-        end, termination_reason = end_inversion(
-            iteration,
-            max_iterations,
-            l2_norm,
-            starting_l2_norm,
-            l2_norm_tolerance,
-            delta_l2_norm,
-            previous_delta_l2_norm,
-            delta_l2_norm_tolerance,
-            perc_increase_limit=perc_increase_limit,
-        )
 
-        if plot_dynamic_convergence is True:
-            plotting.plot_dynamic_convergence(
-                gravity,
-                l2_norm_tolerance,
-                starting_misfit,
-                inversion_region=inversion_region,
-            )
+def eq_sources_score(
+    params: dict[str, float],
+    coordinates: tuple[pd.Series | NDArray, pd.Series | NDArray, pd.Series | NDArray],
+    data: pd.Series | NDArray,
+    delayed: bool = False,
+    **kwargs: typing.Any,
+) -> float:
+    """
+    _summary_
 
-        if end is True:
-            pbar.set_description(f"Inversion ended due to {termination_reason}")
-            break
-        # end of inversion loop
-
-    time_end = time.perf_counter()
-
-    elapsed_time = time_end - time_start
-
-    # collect input parameters into a dictionary
-    params = {
-        # first column
-        "density_contrast": f"{density_contrast} kg/m3",
-        "reference level": f"{zref} m",
-        "max_iterations": max_iterations,
-        "l2_norm_tolerance": f"{l2_norm_tolerance}",
-        "delta_l2_norm_tolerance": f"{delta_l2_norm_tolerance}",
-        # second column
-        "deriv_type": deriv_type,
-        "solver_type": solver_type,
-        "solver_damping": solver_damping,
-        "upper_confining_layer": "Not enabled"
-        if upper_confining_layer is None
-        else "Enabled",
-        "lower_confining_layer": "Not enabled"
-        if lower_confining_layer is None
-        else "Enabled",
-        # third column
-        "time_elapsed": f"{int(elapsed_time)} seconds",
-        "average_iteration_time": f"{round(np.mean(iter_times), 2)} seconds",
-        "Final misfit RMSE / L2-norm": (
-            f"{round(final_rmse,4)} /{round(final_l2_norm,4)} mGal"
-        ),
-        "Termination reason": termination_reason,
-        "iter_times": iter_times,
-    }
+    Parameters
+    ----------
+    params : dict[str, float]
+        dictionary with damping and depth parameters for the equivalent sources fit
+    coordinates : tuple[pd.Series  |  NDArray, pd.Series  |
+        NDArray, pd.Series  |  NDArray]
+        easting, northing, and upwards coordinates of the gravity data
+    data : pd.Series | NDArray
+        gravity data values
+    delayed : bool, optional
+        If True, will use dask.delayed to dispatch computations without actually
+        executing them. The returned scores will be a list of delayed objects, by
+        default False
 
-    if plot_convergence is True:
-        plotting.plot_convergence(
-            gravity,
-            iter_times=iter_times,
-            inversion_region=inversion_region,
+    Returns
+    -------
+    float
+        the mean score of the equivalent sources fit
+    """
+    eqs = hm.EquivalentSources(
+        damping=params.get("damping"),
+        depth=params.get("depth"),
+        **kwargs,
+    )
+    return float(
+        np.mean(
+            vd.cross_val_score(
+                eqs,
+                coordinates,
+                data,
+                delayed=delayed,
+                weights=kwargs.get("weights", None),
+            )
         )
-
-    return prisms_df, gravity, params, elapsed_time
+    )
+    # eqs.fit(coordinates, data, weights=kwargs.get("weights", None))
+    # score = eqs.score(coordinates, data, weights=kwargs.get("weights", None))
```

### Comparing `invert4geom-0.5.0/src/invert4geom/optimization.py` & `invert4geom-0.6.0/src/invert4geom/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 import logging
 import math
 import multiprocessing
 import os
 import pathlib
+import random
 import re
 import subprocess
 import typing
 import warnings
 
 import harmonica as hm
 import pandas as pd
 from nptyping import NDArray
 
-from invert4geom import utils
+from invert4geom import plotting, utils
 
 try:
     import optuna
 except ImportError:
     optuna = None
 
 try:
@@ -403,17 +404,17 @@
     coordinates: tuple[pd.Series | NDArray, pd.Series | NDArray, pd.Series | NDArray],
     data: pd.Series | NDArray,
     n_trials: int = 0,
     damping_limits: tuple[float, float] = (0, 10**3),
     depth_limits: tuple[float, float] = (0, 10e6),
     sampler: optuna.samplers.BaseSampler | None = None,
     parallel: bool = False,
-    fname: str = "tmp",
+    fname: str | None = None,
     use_existing: bool = False,
-    # plot:bool=False,
+    plot: bool = False,
     **eq_kwargs: typing.Any,
 ) -> tuple[pd.DataFrame, hm.EquivalentSources]:
     """
     find the best parameter values for fitting equivalent sources to a set of gravity
     data.
 
     Parameters
@@ -430,28 +431,33 @@
     depth_limits : tuple[float, float], optional
         lower and upper bounds of depth parameter, by default (0, 10e6)
     sampler : optuna.samplers.BaseSampler | None, optional
         type of sampler to use, by default None
     parallel : bool, optional
         if True, will run the trials in parallel, by default False
     fname : str, optional
-        path and filename to save the study results, by default "tmp"
+        path and filename to save the study results, by default "tmp" with a random
+        number attached
     use_existing : bool, optional
         if True, will continue a previously starting optimization, by default False
 
     Returns
     -------
     tuple[pd.DataFrame, hm.EquivalentSources]
         gives a dataframe of the tested parameter sets and associated scores, and the
         best resulting fitted equivalent sources.
     """
     if optuna is None:
         msg = "Missing optional dependency 'optuna' required for optimization."
         raise ImportError(msg)
 
+    # set file name for saving results with random number between 0 and 999
+    if fname is None:
+        fname = f"tmp_{random.randint(0,999)}"
+
     # set name and storage for the optimization
     study_name = fname
     fname = f"{study_name}.log"
 
     # remove if exists
     if use_existing is True:
         pass
@@ -518,21 +524,34 @@
                 parallel=parallel,
             )
 
     logging.info("Best params: %s", study.best_params)
     logging.info("Best trial: %s", study.best_trial.number)
     logging.info("Best score: %s", study.best_trial.value)
 
+    if study.best_params.get("damping") in [damping_limits[0], damping_limits[1]]:
+        logging.warning(
+            "Best damping value (%s) is at the limit of provided "
+            "values (%s, %s) and thus is likely not a global minimum, expand the "
+            "range "
+            "of values tested to ensure the best parameter value is found.",
+            study.best_params.get("damping"),
+            damping_limits[0],
+            damping_limits[1],
+        )
+
     eqs = hm.EquivalentSources(
         damping=study.best_params.get("damping"),
         depth=study.best_params.get("depth"),
         **eq_kwargs,
     ).fit(coordinates, data, weights=eq_kwargs.get("weights"))
 
-    # if plot is True:
-    #     plotting.plot_optuna_inversion_figures(
-    #         study,
-    #         target_names=["score"],
-    #         # include_duration=True,
-    #     )
+    if plot is True:
+        plotting.plot_optuna_inversion_figures(
+            study,
+            target_names=["score"],
+            plot_history=False,
+            plot_slice=True,
+            # include_duration=True,
+        )
 
     return study_df.sort_values("value", ascending=False), eqs
```

### Comparing `invert4geom-0.5.0/src/invert4geom/plotting.py` & `invert4geom-0.6.0/src/invert4geom/plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 import typing
 
 import numpy as np
 import pandas as pd
 
 try:
+    import optuna
+except ImportError:
+    optuna = None
+
+try:
+    import plotly
+except ImportError:
+    plotly = None
+
+try:
     from IPython.display import clear_output
 except ImportError:
     clear_output = None
 
 try:
     import matplotlib.pyplot as plt
     from matplotlib.ticker import MaxNLocator
@@ -32,32 +42,28 @@
 
 from invert4geom import utils
 
 
 def plot_2_parameter_cv_scores(
     scores: list[float],
     parameter_pairs: list[tuple[float, float]],
-    logx: bool = False,
-    logy: bool = False,
     param_names: tuple[str, str] = ("Hyperparameter 1", "Hyperparameter 2"),
     figsize: tuple[float, float] = (5, 3.5),
-    cmap: str = "viridis",
+    cmap: str | None = None,
 ) -> None:
     """
     plot a scatter plot graph with x axis equal to parameter 1, y axis equal to
     parameter 2, and points colored by cross-validation scores.
 
     Parameters
     ----------
     scores : list[float]
         score values
     parameter_pairs : list[float]
         parameter values
-    logx, logy : bool, optional
-        make the x or y axes log scale, by default False
     param_names : tuple[str, str], optional
         name to give for the parameters, by default "Hyperparameter"
     figsize : tuple[float, float], optional
         size of the figure, by default (5, 3.5)
     cmap : str, optional
         matplotlib colormap for scores, by default "viridis"
     """
@@ -67,14 +73,17 @@
         raise ImportError(msg)
     sns.set_theme()
     # Check if matplotlib is installed
     if plt is None:
         msg = "Missing optional dependency 'matplotlib' required for plotting."
         raise ImportError(msg)
 
+    if cmap is None:
+        cmap = sns.color_palette("mako", as_cmap=True)
+
     df = pd.DataFrame(
         {
             "scores": scores,
             param_names[0]: [
                 parameter_pairs[i][0] for i in list(range(len(parameter_pairs)))
             ],
             param_names[1]: [
@@ -86,15 +95,18 @@
 
     best = df.iloc[0]
 
     plt.figure(figsize=figsize)
     plt.title("Two parameter cross-validation")
 
     grid = df.set_index([param_names[1], param_names[0]]).to_xarray().scores
-    grid.plot(cmap=cmap)
+    grid.plot(
+        cmap=cmap,
+        # norm=plt.Normalize(df.scores.min(), df.scores.max()),
+    )
     # plt.contourf(
     #     df[param_names[0]],
     #     df[param_names[1]],
     #     Z = grid,
     #     cmap = cmap,
     # )
     plt.scatter(
@@ -114,18 +126,14 @@
         color=sns.color_palette()[3],
         label="Minimum",
     )
     plt.legend(
         loc="upper right",
     )
 
-    if logx:
-        plt.xscale("log")
-    if logy:
-        plt.yscale("log")
     plt.xlabel(param_names[0])
     plt.ylabel(param_names[1])
     # plt.colorbar()
     plt.tight_layout()
 
 
 def plot_cv_scores(
@@ -247,17 +255,18 @@
     ax1.set_xlabel("Iteration")
     if logy:
         ax1.set_yscale("log")
     ax1.set_ylabel("RMS (mGal)", color="b")
     ax1.tick_params(axis="y", colors="b", which="both")
 
     if iter_times is not None:
-        iter_times.insert(0, 0)
+        iteration_times = iter_times.copy()
+        iteration_times.insert(0, 0)
         ax2 = ax1.twinx()
-        ax2.plot(range(iters + 1), np.cumsum(iter_times), "g-")
+        ax2.plot(range(iters + 1), np.cumsum(iteration_times), "g-")
         ax2.set_ylabel("Cumulative time (s)", color="g")
         ax2.tick_params(axis="y", colors="g")
         ax2.grid(False)
 
     plt.tight_layout()
 
 
@@ -672,19 +681,19 @@
                 cmap = "RdBu_r"
                 lims = (-corrections_lim, corrections_lim)
                 robust = True
                 norm = None
             # plot grids
             j[row].plot(
                 ax=axes,
-                cmap=cmap,
-                norm=norm,
-                robust=robust,
-                vmin=lims[0],
-                vmax=lims[1],
+                cmap=cmap,  # pylint: disable=possibly-used-before-assignment
+                norm=norm,  # pylint: disable=possibly-used-before-assignment
+                robust=robust,  # pylint: disable=possibly-used-before-assignment
+                vmin=lims[0],  # pylint: disable=possibly-used-before-assignment
+                vmax=lims[1],  # pylint: disable=possibly-used-before-assignment
                 cbar_kwargs={
                     "orientation": "horizontal",
                     "anchor": (1, 1),
                     "fraction": 0.05,
                     "pad": 0.04,
                 },
             )
@@ -706,19 +715,19 @@
             axes.set_yticklabels([])
             axes.set_xlabel("")
             axes.set_ylabel("")
             axes.set_aspect("equal")
 
     # add text with inversion parameter info
     text1, text2, text3 = [], [], []
-    params.pop("iter_times")
+    params.pop("Iteration times")
     for i, (k, v) in enumerate(params.items(), start=1):
         if i <= 5:
             text1.append(f"{k}: {v}\n")
-        elif i <= 9:
+        elif i <= 11:
             text2.append(f"{k}: {v}\n")
         else:
             text3.append(f"{k}: {v}\n")
 
     text1 = "".join(text1)  # type: ignore[assignment]
     text2 = "".join(text2)  # type: ignore[assignment]
     text3 = "".join(text3)  # type: ignore[assignment]
@@ -1003,7 +1012,230 @@
     # Add a ceiling light
     add_light(plotter, prisms[i])  # pylint: disable=undefined-loop-variable
 
     if kwargs.get("show_axes", True):
         plotter.show_axes()
 
     plotter.show(jupyter_backend=kwargs.get("backend", "client"))
+
+
+def combined_history(
+    study: typing.Any,
+    target_names: list[str],
+    include_duration: bool = False,
+) -> typing.Any:
+    """
+    plot combined optimization history for multiobjective optimizations.
+
+    Parameters
+    ----------
+    study : typing.Any
+        the optuna study object
+    target_names : list[str]
+        list of names for parameters in the study
+    include_duration : bool, optional
+        whether to add the duration to the plot, by default False
+
+    Returns
+    -------
+    typing.Any
+        a plotly figure
+    """
+    # Check if optuna is installed
+    if optuna is None:
+        msg = "Missing optional dependency 'optuna' required for optimization."
+        raise ImportError(msg)
+
+    # Check if plotly is installed
+    if plotly is None:
+        msg = "Missing optional dependency 'plotly' required for plotting."
+        raise ImportError(msg)
+
+    target_names = target_names.copy()
+    figs = []
+    for i, j in enumerate(target_names):
+        f = optuna.visualization.plot_optimization_history(
+            study,
+            target=lambda t: t.values[i],  # noqa: B023 # pylint: disable=cell-var-from-loop
+            target_name=j,
+        )
+        figs.append(f)
+
+    if include_duration is True and "duration" not in target_names:
+        f = optuna.visualization.plot_optimization_history(
+            study, target=lambda t: t.duration.total_seconds(), target_name="duration"
+        )
+        figs.append(f)
+        target_names.append("duration")
+
+    if len(target_names) < 2:
+        layout = plotly.graph_objects.Layout(
+            title="Optimization History Plot",
+            yaxis=plotly.graph_objs.layout.YAxis(
+                title=target_names[0],
+            ),
+            xaxis={"title": "Trial"},
+        )
+    elif len(target_names) >= 2:
+        yaxes = {}
+        for i, j in enumerate(target_names, start=1):
+            if i == 1:
+                pass
+            else:
+                yax = plotly.graph_objs.layout.YAxis(
+                    title=j,
+                    overlaying="y",
+                    side="left",
+                    anchor="free",
+                    autoshift=True,
+                )
+                yaxes[f"yaxis{i}"] = yax
+        layout = plotly.graph_objects.Layout(
+            title="Optimization History Plot",
+            yaxis1=plotly.graph_objs.layout.YAxis(
+                title=target_names[0],
+                side="right",
+            ),
+            xaxis={"title": "Trial"},
+            **yaxes,
+        )
+
+    # Create figure with secondary x-axis
+    fig = plotly.graph_objects.Figure(layout=layout)  # pylint: disable=possibly-used-before-assignment
+
+    # Add traces
+    for i, j in enumerate(target_names):
+        fig.add_trace(
+            plotly.graph_objects.Scatter(
+                x=figs[i].data[0]["x"],
+                y=figs[i].data[0]["y"],
+                name=j,
+                mode="markers",
+                yaxis=f"y{i+1}",
+            )
+        )
+
+    fig.update_layout(xaxis_title="Trial", title="Optimization History Plot")
+
+    return fig
+
+
+def plot_optuna_inversion_figures(
+    study: typing.Any,
+    target_names: list[str],
+    include_duration: bool = False,
+    # params=None,
+    # seperate_param_importances=False,
+    plot_history: bool = True,
+    plot_slice: bool = True,
+    # plot_importance=True,
+    # plot_edf=True,
+    # plot_pareto=True,
+) -> None:
+    """
+    plot the results of an optuna optimization
+
+    Parameters
+    ----------
+    study : typing.Any
+        the optuna study object
+    target_names : list[str]
+        list of names for parameters in the study
+    include_duration : bool, optional
+        whether to add the duration to the plot, by default False
+    plot_history : bool, optional
+        choose to plot the optimization history, by default True
+    plot_slice : bool, optional
+        choose to plot the parameter values vs. score for each parameter, by default
+        True
+    """
+    # Check if optuna is installed
+    if optuna is None:
+        msg = "Missing optional dependency 'optuna' required for optimization."
+        raise ImportError(msg)
+
+    if plot_history:
+        combined_history(
+            study,
+            target_names,
+            include_duration=include_duration,
+        ).show()
+
+    # if params is None:
+    #     params = [k for k, v in study.get_trials()[0].params.items()]
+
+    if plot_slice:
+        for i, j in enumerate(target_names):
+            optuna.visualization.plot_slice(
+                study,
+                target=lambda t: t.values[i],  # noqa: B023 # pylint: disable=cell-var-from-loop
+                target_name=j,
+            ).show()
+
+        if include_duration is True and "duration" not in target_names:
+            optuna.visualization.plot_slice(
+                study,
+                target=lambda t: t.duration.total_seconds(),
+                target_name="Execution time",
+            ).show()
+
+    # if plot_importance:
+    #     if len(params) <= 1:
+    #         pass
+    #     else:
+    #         try:
+    #             if seperate_param_importances is True:
+    #                 combined_importance(
+    #                     study,
+    #                     target_names,
+    #                     params=[
+    #                         "deriv_type",
+    #                         "verde_damping",
+    #                     ],
+    #                     include_duration=include_duration,
+    #                 ).show()
+
+    #                 combined_importance(
+    #                     study,
+    #                     target_names,
+    #                     params=["deriv_type", "scipy_damping"],
+    #                     include_duration=include_duration,
+    #                 ).show()
+    #             else:
+    #                 combined_importance(
+    #                     study,
+    #                     target_names,
+    #                     params=params,
+    #                     include_duration=include_duration,
+    #                 ).show()
+    #         except AttributeError:
+    #             print("issue with showing importance figure")
+
+    # if plot_edf:
+    #     combined_edf(study, target_names, include_duration=include_duration).show()
+
+    # if plot_pareto:
+    #     if len(target_names) == 1:
+    #         if "duration" not in target_names:
+    #             if include_duration is True:
+    #                 optuna.visualization.plot_pareto_front(
+    #                     study,
+    #                     targets=lambda t: (t.values[0], t.duration.total_seconds()),
+    #                     target_names=target_names + ["duration"],
+    #                 ).show()
+
+    #     elif len(target_names) > 1:
+    #         if "duration" not in target_names:
+    #             if include_duration is True:
+    #                 optuna.visualization.plot_pareto_front(
+    #                     study,
+    #                     targets=lambda t: (t.values, t.duration.total_seconds()),
+    #                     target_names=target_names + ["duration"],
+    #                 ).show()
+    #             elif include_duration is False:
+    #                 optuna.visualization.plot_pareto_front(
+    #                     study, target_names=target_names
+    #                 ).show()
+    #         elif "duration" in target_names:
+    #             optuna.visualization.plot_pareto_front(
+    #                 study, target_names=target_names
+    #             ).show()
```

### Comparing `invert4geom-0.5.0/src/invert4geom/synthetic.py` & `invert4geom-0.6.0/src/invert4geom/synthetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,17 @@
     xr.Dataset
         synthetic topography dataset
     """
     if registration == "g":
         pixel_register = False
     elif registration == "p":
         pixel_register = True
+    else:
+        msg = "registration must be either 'g' or 'p'"
+        raise ValueError(msg)
 
     # create grid of coordinates
     (x, y) = vd.grid_coordinates(  # pylint: disable=unbalanced-tuple-unpacking
         region=region,
         spacing=spacing,
         pixel_register=pixel_register,
     )
@@ -219,14 +222,17 @@
         synthetic topography dataset
     """
 
     if registration == "g":
         pixel_register = False
     elif registration == "p":
         pixel_register = True
+    else:
+        msg = "registration must be either 'g' or 'p'"
+        raise ValueError(msg)
 
     # create grid of coordinates
     (x, y) = vd.grid_coordinates(  # pylint: disable=unbalanced-tuple-unpacking
         region=region,
         spacing=spacing,
         pixel_register=pixel_register,
     )
```

### Comparing `invert4geom-0.5.0/src/invert4geom/utils.py` & `invert4geom-0.6.0/src/invert4geom/cross_validation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,921 +1,741 @@
-from __future__ import annotations  # pylint: disable=too-many-lines
+from __future__ import annotations
 
-import copy
+import itertools
 import logging
+import pathlib
+import pickle
+import random
 import typing
-import warnings
 
-import dask
-import harmonica as hm
 import numpy as np
 import pandas as pd
-import pygmt
 import verde as vd
 import xarray as xr
-import xrft
-from nptyping import NDArray
-from pykdtree.kdtree import KDTree  # pylint: disable=no-name-in-module
+from polartoolkit import utils as polar_utils
+from tqdm.autonotebook import tqdm
 
+from invert4geom import inversion, plotting, regional, utils
 
-def rmse(data: NDArray, as_median: bool = False) -> float:
-    """
-    function to give the root mean/median squared error (RMSE) of data
-
-    Parameters
-    ----------
-    data : NDArray
-        input data
-    as_median : bool, optional
-        choose to give root median squared error instead, by default False
 
-    Returns
-    -------
-    float
-        RMSE value
-    """
-    if as_median:
-        value: float = np.sqrt(np.nanmedian(data**2).item())
-    else:
-        value = np.sqrt(np.nanmean(data**2).item())
-
-    return value
-
-
-def nearest_grid_fill(
-    grid: xr.DataArray,
-    method: str = "verde",
-) -> xr.DataArray:
-    """
-    fill missing values in a grid with the nearest value.
-
-    Parameters
-    ----------
-    grid : xr.DataArray
-        grid with missing values
-    method : str, optional
-        choose method of filling, by default "verde"
-
-    Returns
-    -------
-    xr.DataArray
-        filled grid
-    """
-
-    # get coordinate names
-    original_dims = list(grid.sizes.keys())
-
-    # get original grid name
-    original_name = grid.name
-
-    if method == "rioxarray":
-        filled: xr.DataArray = (
-            grid.rio.write_crs("epsg:3031")
-            .rio.set_spatial_dims(original_dims[1], original_dims[0])
-            .rio.write_nodata(np.nan)
-            .rio.interpolate_na(method="nearest")
-            .rename(original_name)
-        )
-    elif method == "verde":
-        df = vd.grid_to_table(grid)
-        df_dropped = df[df[grid.name].notnull()]
-        coords = (df_dropped[grid.dims[1]], df_dropped[grid.dims[0]])
-        region = vd.get_region((df[grid.dims[1]], df[grid.dims[0]]))
-        filled = (
-            vd.KNeighbors()
-            .fit(coords, df_dropped[grid.name])
-            .grid(region=region, shape=grid.shape, data_names=original_name)[
-                original_name
-            ]
-        )
-    # elif method == "pygmt":
-    #     filled = pygmt.grdfill(grid, mode="n", verbose="q").rename(original_name)
-
-    # reset coordinate names if changed
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message="rename '")
-        return filled.rename(
-            {
-                next(iter(filled.dims)): original_dims[0],
-                list(filled.dims)[1]: original_dims[1],
-            }
-        )
-
-
-def filter_grid(
-    grid: xr.DataArray,
-    filter_width: float | None = None,
-    filt_type: str = "lowpass",
-) -> xr.DataArray:
+def resample_with_test_points(
+    data_spacing: float,
+    data: pd.DataFrame,
+    region: tuple[float, float, float, float],
+) -> pd.DataFrame:
     """
-    _summary_
+    take a dataframe of coordinates and make all rows that fall on the data_spacing
+    grid training points. Add rows at each point which falls on the grid points of
+    half the data_spacing, assign these with label "test". If other data is present
+    in dataframe, will sample at each new location.
 
     Parameters
     ----------
-    grid : xr.DataArray
-        grid to filter the values of
-    filter_width : float, optional
-        width of the filter in meters, by default None
-    filt_type : str, optional
-        type of filter to use, by default "lowpass"
-    change_spacing : bool, optional
-        if True, will filter the grid and resample the grid to be at the same spacing
-        of the filter width, by default False
+    data_spacing : float
+        full spacing size which will be halved
+    data : pd.DataFrame
+        dataframe with coordinate columns "easting" and "northing", all other columns
+        will be sampled at new grid spacing
+    region : tuple[float, float, float, float]
+        region to create grid over, in the form (min_easting, max_easting, min_northing,
+        max_northing)
 
     Returns
     -------
-    xr.DataArray
-        a filtered grid
-
+    pd.DataFrame
+        a new dataframe with new column "test" of booleans which shows whether each row
+        is a testing or training point.
     """
-    # get coordinate names
-    original_dims = list(grid.sizes.keys())
 
-    # get original grid name
-    original_name = grid.name
-
-    # if there are nan's, fill them with nearest neighbor
-    if grid.isnull().any():
-        filled = nearest_grid_fill(grid, method="verde")
-        # print("filling NaN's with nearest neighbor")
-    else:
-        filled = grid.copy()
-
-    # reset coordinate names if changed
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message="rename '")
-        filled = filled.rename(
-            {
-                next(iter(filled.dims)): original_dims[0],
-                list(filled.dims)[1]: original_dims[1],
-            }
-        )
-
-    # define width of padding in each direction
-    pad_width = {
-        original_dims[1]: grid[original_dims[1]].size // 3,
-        original_dims[0]: grid[original_dims[0]].size // 3,
-    }
-
-    # apply padding
-    padded = xrft.pad(filled, pad_width)
-
-    if filt_type == "lowpass":
-        filt = hm.gaussian_lowpass(padded, wavelength=filter_width).rename("filt")
-    elif filt_type == "highpass":
-        filt = hm.gaussian_highpass(padded, wavelength=filter_width).rename("filt")
-    elif filt_type == "up_deriv":
-        filt = hm.derivative_upward(padded).rename("filt")
-    elif filt_type == "easting_deriv":
-        filt = hm.derivative_easting(padded).rename("filt")
-    elif filt_type == "northing_deriv":
-        filt = hm.derivative_northing(padded).rename("filt")
-    else:
-        msg = "filt_type must be 'lowpass' or 'highpass'"
-        raise ValueError(msg)
-
-    unpadded = xrft.unpad(filt, pad_width)
-
-    # reset coordinate values to original (avoid rounding errors)
-    unpadded = unpadded.assign_coords(
-        {
-            original_dims[0]: grid[original_dims[0]].to_numpy(),
-            original_dims[1]: grid[original_dims[1]].to_numpy(),
-        }
+    # create coords for full data
+    coords = vd.grid_coordinates(
+        region=region,
+        spacing=data_spacing / 2,
+        pixel_register=False,
     )
 
-    if grid.isnull().any():
-        result: xr.DataArray = xr.where(grid.notnull(), unpadded, grid)
-    else:
-        result = unpadded.copy()
-
-    # reset coordinate names if changed
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message="rename '")
-        result = result.rename(
-            {
-                next(iter(result.dims)): original_dims[0],
-                # list(result.dims)[0]: original_dims[0],
-                list(result.dims)[1]: original_dims[1],
-            }
-        )
-
-    return result.rename(original_name)
-
-
-def dist_nearest_points(
-    targets: pd.DataFrame,
-    data: pd.DataFrame | xr.DataArray | xr.Dataset,
-    coord_names: tuple[str, str] | None = None,
-) -> typing.Any:
-    """
-    for all gridcells calculate to the distance to the nearest target.
-
-    Parameters
-    ----------
-    targets : pd.DataFrame
-        contains the coordinates of the targets
-    data : pd.DataFrame | xr.DataArray | xr.Dataset
-        the grid data, in either gridded or tabular form
-    coord_names : tuple[str, str] | None, optional
-        the names of the coordinates for both the targets and the data, by default None
-
-    Returns
-    -------
-    typing.Any
-        the distance to the nearest target for each gridcell, in the same format as the
-        input for `data`.
-    """
-
-    if coord_names is None:
-        coord_names = ("easting", "northing")
-
-    df_targets = targets[[coord_names[0], coord_names[1]]].copy()
-
-    df_data: pd.DataFrame | xr.DataArray | xr.Dataset
-    if isinstance(data, pd.DataFrame):
-        df_data = data[list(coord_names)].copy()
-    elif isinstance(data, xr.DataArray):
-        df_grid = vd.grid_to_table(data).dropna()
-        df_data = df_grid[[coord_names[0], coord_names[1]]].copy()  # pylint: disable=unsubscriptable-object
-    elif isinstance(data, xr.Dataset):
-        try:
-            df_grid = vd.grid_to_table(data[next(iter(data.variables))]).dropna()
-            # df_grid = vd.grid_to_table(data[list(data.variables)[0]]).dropna()
-        except IndexError:
-            df_grid = vd.grid_to_table(data).dropna()
-        df_data = df_grid[[coord_names[0], coord_names[1]]].copy()  # pylint: disable=unsubscriptable-object
-
-    min_dist, _ = KDTree(df_targets.values).query(df_data.values, 1)
-
-    df_data["min_dist"] = min_dist
-
-    if isinstance(data, pd.DataFrame):
-        return df_data
-    return df_data.set_index([coord_names[0], coord_names[1]][::-1]).to_xarray()
-
-
-def normalize_xarray(
-    da: xr.DataArray,
-    low: float = 0,
-    high: float = 1,
-) -> xr.DataArray:
-    """
-    Normalize a grid between provided values
-
-    Parameters
-    ----------
-    da : xr.DataArray
-        grid to normalize
-    low : float, optional
-        lower value for normalization, by default 0
-    high : float, optional
-        higher value for normalization, by default 1
-
-    Returns
-    -------
-    xr.DataArray
-        a normalized grid
-    """
-    # min_val = da.values.min()
-    # max_val = da.values.max()
-
-    da = da.copy()
-
-    min_val = da.quantile(0)
-    max_val = da.quantile(1)
-
-    da2: xr.DataArray = (high - low) * (
-        ((da - min_val) / (max_val - min_val)).clip(0, 1)
-    ) + low
-
-    return da2.drop("quantile")
-
-
-def normalized_mindist(
-    points: pd.DataFrame,
-    grid: xr.DataArray,
-    low: float | None = None,
-    high: float | None = None,
-    mindist: float | None = None,
-    region: list[float] | None = None,
-) -> xr.DataArray:
+    # turn coordinates into dataarray
+    full_points = vd.make_xarray_grid(
+        (coords[0], coords[1]),
+        data=np.ones_like(coords[0]),
+        data_names="tmp",
+        dims=("northing", "easting"),
+    )
+    # turn dataarray in dataframe
+    full_df = vd.grid_to_table(full_points).drop(columns="tmp")
+    # set all points to test
+    full_df["test"] = True  # pylint: disable=unsupported-assignment-operation
+
+    # subset training points, every other value
+    train_df = full_df[  # pylint: disable=unsubscriptable-object
+        (full_df.easting.isin(full_points.easting.values[::2]))
+        & (full_df.northing.isin(full_points.northing.values[::2]))
+    ].copy()
+    # set training points to not be test points
+    train_df["test"] = False
+
+    # merge training and testing dfs
+    df = full_df.set_index(["northing", "easting"])
+    df.update(train_df.set_index(["northing", "easting"]))
+    df2 = df.reset_index()
+
+    df2["test"] = df2.test.astype(bool)
+
+    grid = data.set_index(["northing", "easting"]).to_xarray()
+    for i in list(grid):
+        if i == "test":
+            pass
+        else:
+            df2[i] = utils.sample_grids(
+                df2,
+                grid[i],
+                i,
+                coord_names=("easting", "northing"),
+            )[i].astype(data[i].dtype)
+
+    # test with this, using same input spacing as original
+    # pd.testing.assert_frame_equal(df2, full_res_grav, check_like=True,)
+
+    return df2
+
+
+def grav_cv_score(
+    training_data: pd.DataFrame,
+    testing_data: pd.DataFrame,
+    progressbar: bool = True,
+    rmse_as_median: bool = False,
+    plot: bool = False,
+    **kwargs: typing.Any,
+) -> float:
     """
-    Find the minimum distance between each grid cell and the nearest point. If low and
-    high are provided, normalize the min dists grid between these values. If region is
-    provided, all grid cells outside region are set to a distance of 0.
+    Find the score, represented by the root mean squared error (RMSE), between the
+    testing gravity data, and the predict gravity data after and
+    inversion. Follows methods of :footcite:t:`uiedafast2017`.
 
     Parameters
     ----------
-    points : pd.DataFrame
-        coordinates of the points
-    grid : xr.DataArray
-        gridded data to find min dists for each grid cell
-    low : float | None, optional
-        lower value for normalization, by default None
-    high : float | None, optional
-        higher value for normalization, by default None
-    mindist : float | None, optional
-        the minimum allowed distance, all values below are set equal to, by default None
-    region : list[float] | None, optional
-        bounding region for which all grid cells outside will be set to low, by default
-        None
+    training_data : pd.DataFrame
+       rows of the data frame which are just the training data
+    testing_data : pd.DataFrame
+        rows of the data frame which are just the testing data
+    rmse_as_median : bool, optional
+        calculate the RMSE as the median as opposed to the mean, by default False
+    progressbar : bool, optional
+        choose to show the progress bar for the forward gravity calculation, by default
+        True
+    plot : bool, optional
+        choose to plot the observed and predicted data grids, and their difference,
+        located at the testing points, by default False
 
     Returns
     -------
-    xr.DataArray
-        grid of normalized minimum distances
-    """
-
-    grid = copy.deepcopy(grid)
-
-    # get coordinate names
-    original_dims = list(grid.sizes.keys())
-
-    constraint_points = points.copy()
-
-    min_dist: xr.DataArray = dist_nearest_points(
-        targets=constraint_points,
-        data=grid,
-        coord_names=(str(original_dims[1]), str(original_dims[0])),
-    ).min_dist
-
-    # set points < mindist to low
-    if mindist is not None:
-        min_dist = xr.where(min_dist < mindist, 0, min_dist)
-
-    # set points outside of region to low
-    if region is not None:
-        df = vd.grid_to_table(min_dist)
-        df["are_inside"] = vd.inside(
-            (df[original_dims[1]], df[original_dims[0]]),
-            region=region,
-        )
-        new_min_dist = df.set_index([original_dims[0], original_dims[1]]).to_xarray()
-        new_min_dist = xr.where(new_min_dist.are_inside, new_min_dist, 0)
-
-        # add nans back
-        new_min_dist = xr.where(min_dist.isnull(), np.nan, new_min_dist)
-
-        min_dist = new_min_dist.min_dist
-
-    # normalize from low to high
-    if (low is None) & (high is None):
-        pass
-    else:
-        assert low is not None
-        assert high is not None
-        min_dist = normalize_xarray(min_dist, low=low, high=high)
-
-    return min_dist
-
-
-def sample_grids(
-    df: pd.DataFrame,
-    grid: str | xr.DataArray,
-    sampled_name: str,
-    **kwargs: typing.Any,
-) -> pd.DataFrame:
-    """
-    Sample data at every point along a line
+    float
+        a score, represented by the root mean squared error, between the testing gravity
+        data and the predicted gravity data.
 
-    Parameters
+    References
     ----------
-    df : pd.DataFrame
-        Dataframe containing columns 'x', 'y', or columns with names defined by kwarg
-        "coor_names".
-    grid : str or xr.DataArray
-        Grid to sample, either file name or xr.DataArray
-    sampled_name : str,
-        Name for sampled column
-
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe with new column (sampled_name) of sample values from (grid)
+    :footcite:t:`uiedafast2017`
     """
 
-    # drop name column if it already exists
-    try:
-        df1 = df.drop(columns=sampled_name)
-    except KeyError:
-        df1 = df.copy()
+    train = training_data.copy()
+    test = testing_data.copy()
 
-    df2 = df1.copy()
+    zref: float = kwargs.get("zref")  # type: ignore[assignment]
+    density_contrast: float = kwargs.get("density_contrast")  # type: ignore[assignment]
 
-    # reset the index
-    df3 = df2.reset_index()
-
-    x, y = kwargs.get("coord_names", ("x", "y"))
-    # get points to sample at
-    points = df3[[x, y]].copy()
+    new_kwargs = {
+        key: value
+        for key, value in kwargs.items()
+        if key
+        not in [
+            "zref",
+            "density_contrast",
+        ]
+    }
 
-    # sample the grid at all x,y points
-    sampled = pygmt.grdtrack(
-        points=points,
-        grid=grid,
-        newcolname=sampled_name,
-        # radius=kwargs.get("radius", None),
-        no_skip=True,  # if false causes issues
-        verbose=kwargs.get("verbose", "w"),
-        interpolation=kwargs.get("interpolation", "c"),
+    # run inversion
+    results = inversion.run_inversion(
+        grav_df=train,
+        zref=zref,
+        density_contrast=density_contrast,
+        **new_kwargs,
     )
+    prism_results, _, _, _ = results
 
-    df3[sampled_name] = sampled[sampled_name]
-
-    # reset index to previous
-    df4 = df3.set_index("index")
-
-    # reset index name to be same as originals
-    df4.index.name = df1.index.name
+    # get last iteration's layer result
+    final_topography = prism_results.set_index(["northing", "easting"]).to_xarray().topo
 
-    # check that dataframe is identical to original except for new column
-    pd.testing.assert_frame_equal(df4.drop(columns=sampled_name), df1)
+    density_grid = xr.where(
+        final_topography >= zref,
+        density_contrast,
+        -density_contrast,
+    )
 
-    return df4
+    # create new prism layer
+    prism_layer = utils.grids_to_prisms(
+        final_topography,
+        reference=zref,
+        density=density_grid,
+    )
 
+    # calculate forward gravity of starting prism layer
+    test["test_point_grav"] = prism_layer.prism_layer.gravity(
+        coordinates=(
+            test.easting,
+            test.northing,
+            test.upward,
+        ),
+        field="g_z",
+        progressbar=progressbar,
+    )
 
-def extract_prism_data(
-    prism_layer: xr.Dataset,
+    # compare forward of inverted layer with observed
+    observed = test[kwargs.get("grav_data_column")] - test.reg
+    predicted = test.test_point_grav
+
+    dif = predicted - observed
+
+    score = utils.rmse(dif, as_median=rmse_as_median)
+
+    if plot:
+        test_grid = test.set_index(["northing", "easting"]).to_xarray()
+        obs = test_grid[kwargs.get("grav_data_column")] - test_grid.reg
+        pred = test_grid.test_point_grav.rename("")
+
+        polar_utils.grd_compare(
+            pred,
+            obs,
+            grid1_name="Predicted gravity",
+            grid2_name="Observed gravity",
+            plot=True,
+            plot_type="xarray",
+            robust=True,
+            title=f"Score={score}",
+            rmse_in_title=False,
+        )
+
+    return score
+
+
+def grav_optimal_parameter(
+    training_data: pd.DataFrame,
+    testing_data: pd.DataFrame,
+    param_to_test: tuple[str, list[float]],
+    rmse_as_median: bool = False,
+    progressbar: bool = True,
+    plot_grids: bool = False,
+    plot_cv: bool = False,
+    verbose: bool = False,
+    results_fname: str | None = None,
+    **kwargs: typing.Any,
 ) -> tuple[
-    pd.DataFrame,
-    xr.Dataset,
+    tuple[pd.DataFrame, pd.DataFrame, dict[str, typing.Any], float],
+    float,
     float,
-    xr.DataArray,
+    list[float],
+    list[float],
 ]:
     """
-    extract necessary info from starting prism layer, adds variables 'topo' and
-    'starting_topo' to prism layer dataset (prisms_ds), converts it into dataframe
-    (prisms_df), gets the prism spacing (spacing) from prisms_ds, and creates a grid of
-    the starting topography (topo_grid) from the tops and bottoms of the prism layer.
+    Calculate the cross validation scores for a set of parameter values and return the
+    best score and value.
 
     Parameters
     ----------
-    prism_layer : xr.Dataset
-       starting model prism layer
+    training_data : pd.DataFrame
+        just the training data rows
+    testing_data : pd.DataFrame
+        just the testing data rows
+    param_to_test : tuple[str, list[float]]
+        first value is a string of the parameter that is being tested, and the second
+        value is a list of the values to test
+    rmse_as_median : bool, optional
+        calculate the RMSE as the median as opposed to the mean, by default False
+    progressbar : bool, optional
+        display a progress bar for the number of tested values, by default True
+    plot_grids : bool, optional
+        plot all the grids of observed and predicted data for each parameter value, by
+        default False
+    plot_cv : bool, optional
+       plot a graph of scores vs parameter values, by default False
+    verbose : bool, optional
+       log the results, by default False
+    results_fname : str, optional
+        file name to save results to, by default "tmp" with an attached random number
 
     Returns
     -------
-    tuple[pd.DataFrame, pd.Dataset, float, xr.DataArray]
-        prisms_df, prisms_ds, spacing, topo_grid
-    """
-
-    prisms_ds = copy.deepcopy(prism_layer.load())
-
-    # add starting topo to dataset
-    topo_grid = xr.where(prisms_ds.density > 0, prisms_ds.top, prisms_ds.bottom)
-    prisms_ds["topo"] = topo_grid
-    prisms_ds["starting_topo"] = topo_grid
-
-    # turn dataset into dataframe
-    prisms_df = prisms_ds.to_dataframe().reset_index().dropna().astype(float)
-
-    spacing = get_spacing(prisms_df)
-
-    return prisms_df, prisms_ds, spacing, topo_grid
+    tuple[ tuple[pd.DataFrame, pd.DataFrame, dict[str, typing.Any], float],
+        float, float, list[float], list[float], ]
+        the inversion results, the optimal parameter value, the score associated with
+        it, the parameter values and the scores for each parameter value
+    """
+
+    train = training_data.copy()
+    test = testing_data.copy()
+
+    # pull parameter out of kwargs
+    param_name = param_to_test[0]
+    param_values = param_to_test[1]
+
+    # set file name for saving results with random number between 0 and 999
+    if results_fname is None:
+        results_fname = f"tmp_{random.randint(0,999)}"
+
+    # run inversions and collect scores
+    scores = []
+    pbar = tqdm(
+        param_values,
+        desc=f"{param_name} values",
+        disable=not progressbar,
+    )
+    for i, value in enumerate(pbar):
+        # update parameter value in kwargs
+        kwargs[param_name] = value
+        # run cross validation
+        score = grav_cv_score(
+            training_data=train,
+            testing_data=test,
+            rmse_as_median=rmse_as_median,
+            plot=plot_grids,
+            results_fname=f"{results_fname}_trial_{i}",
+            progressbar=False,
+            **kwargs,
+        )
+        scores.append(score)
+        if (i == 1) and (score > scores[0]):
+            msg = (
+                "first score was lower than second, consider changing the lower"
+                " parameter value range"
+            )
+            logging.warning(msg)
+    if verbose:
+        # set Python's logging level to get information about the inversion\s progress
+        logger = logging.getLogger()
+        logger.setLevel(logging.INFO)
+
+    # print value and score pairs
+    for value, score in zip(param_values, scores):
+        logging.info("%s value: %s -> Score: %s", param_name, value, score)
+
+    best_idx = np.argmin(scores)
+    best_score = scores[best_idx]
+    best_param_value = param_values[best_idx]
+    logging.info(
+        "Best score of %s with %s=%s", best_score, param_name, best_param_value
+    )
 
+    # get best inversion result of each set
+    with pathlib.Path(f"{results_fname}_trial_{best_idx}.pickle").open("rb") as f:
+        inv_results = pickle.load(f)
+
+    # delete other inversion results
+    for i in range(len(scores)):
+        if i == best_idx:
+            pass
+        else:
+            pathlib.Path(f"{results_fname}_trial_{i}.pickle").unlink(missing_ok=True)
+
+    # put scores and parameter values into dict
+    results = {
+        "scores": scores,
+        "param_values": param_values,
+    }
 
-def get_spacing(prisms_df: pd.DataFrame) -> float:
+    if best_param_value in [np.min(param_values), np.max(param_values)]:
+        logging.warning(
+            "Best parameter value (%s) for %s CV is at the limit of provided "
+            "values (%s, %s) and thus is likely not a global minimum, expand the range "
+            "of values tested to ensure the best parameter value is found.",
+            best_param_value,
+            param_name,
+            np.nanmin(param_values),
+            np.nanmax(param_values),
+        )
+
+    # remove if exists
+    pathlib.Path(results_fname).unlink(missing_ok=True)
+
+    # save scores and dampings to pickle
+    with pathlib.Path(f"{results_fname}.pickle").open("wb") as f:
+        pickle.dump(results, f)
+
+    if plot_cv:
+        # plot scores
+        plotting.plot_cv_scores(
+            scores,
+            param_values,
+            param_name=param_name,
+            # logx=True,
+            # logy=True,
+        )
+
+    return inv_results, best_param_value, best_score, param_values, scores
+
+
+def constraints_cv_score(
+    grav_df: pd.DataFrame,
+    constraints_df: pd.DataFrame,
+    rmse_as_median: bool = False,
+    **kwargs: typing.Any,
+) -> float:
     """
-    Extract spacing of harmonica prism layer using a dataframe representation.
+    Find the score, represented by the root mean squared error (RMSE), between the
+    constraint point elevation, and the inverted topography at the constraint points.
+    Follows methods of :footcite:t:`uiedafast2017`.
 
     Parameters
     ----------
-    prisms_df : pd.DataFrame
-        dataframe of harmonica prism layer
-
+    grav_df : pd.DataFrame
+       gravity dataframe with columns "res", "reg", and column set by kwarg
+       grav_data_column
+    constraints_df : pd.DataFrame
+        constraints dataframe with columns "easting", "northing", and "upward"
+    rmse_as_median : bool, optional
+        calculate the RMSE as the median of the , as opposed to the mean, by default
+        False
     Returns
     -------
     float
-        spacing of prisms
-    """
-    return float(abs(prisms_df.northing.unique()[1] - prisms_df.northing.unique()[0]))
-
+        a score, represented by the root mean squared error, between the testing gravity
+        data and the predicted gravity data.
 
-def sample_bounding_surfaces(
-    prisms_df: pd.DataFrame,
-    upper_confining_layer: xr.DataArray | None = None,
-    lower_confining_layer: xr.DataArray | None = None,
-) -> pd.DataFrame:
-    """
-    sample upper and/or lower confining layers into prisms dataframe
-
-    Parameters
+    References
     ----------
-    prisms_df : pd.DataFrame
-        dataframe of prism properties
-    upper_confining_layer : xr.DataArray | None, optional
-        layer which the inverted topography should always be below, by default None
-    lower_confining_layer : xr.DataArray | None, optional
-        layer which the inverted topography should always be above, by default None
-
-    Returns
-    -------
-    pd.DataFrame
-        a dataframe with added columns 'upper_bounds' and 'lower_bounds', which are the
-        sampled values of the supplied confining grids.
+    .. footbibliography::
     """
-    df = prisms_df.copy()
 
-    if upper_confining_layer is not None:
-        df = sample_grids(
-            df=df,
-            grid=upper_confining_layer,
-            sampled_name="upper_bounds",
-            coord_names=["easting", "northing"],
-        )
-        assert len(df.upper_bounds) != 0
-    if lower_confining_layer is not None:
-        df = sample_grids(
-            df=df,
-            grid=lower_confining_layer,
-            sampled_name="lower_bounds",
-            coord_names=["easting", "northing"],
-        )
-        assert len(df.lower_bounds) != 0
-    return df
-
-
-def enforce_confining_surface(
-    prisms_df: pd.DataFrame,
-    iteration_number: int,
-) -> pd.DataFrame:
-    """
-    alter the surface correction values to ensure when added to the current iteration's
-    topography it doesn't intersect optional confining layers.
-
-    Parameters
-    ----------
-    prisms_df : pd.DataFrame
-        prism layer dataframe with optional 'upper_bounds' or 'lower_bounds' columns,
-        and current iteration's topography.
-    iteration_number : int
-        number of the current iteration, starting at 1 not 0
-
-    Returns
-    -------
-    pd.DataFrame
-        a dataframe with added column 'iter_{iteration_number}_correction
-    """
+    constraints_df = constraints_df.copy()
 
-    df = prisms_df.copy()
+    zref: float = kwargs.get("zref")  # type: ignore[assignment]
+    density_contrast: float = kwargs.get("density_contrast")  # type: ignore[assignment]
 
-    if "upper_bounds" in df:
-        # get max upward change allowed for each prism
-        # positive values indicate max allowed upward change
-        # negative values indicate topography is already too far above upper bound
-        df["max_change_above"] = df.upper_bounds - df.topo
-        number_enforced = 0
-        for i, j in enumerate(df[f"iter_{iteration_number}_correction"]):
-            if j > df.max_change_above[i]:
-                number_enforced += 1
-                df.loc[i, f"iter_{iteration_number}_correction"] = df.max_change_above[
-                    i
-                ]
-        logging.info("enforced upper confining surface at %s prisms", number_enforced)
-    if "lower_bounds" in df:
-        # get max downward change allowed for each prism
-        # negative values indicate max allowed downward change
-        # positive values indicate topography is already too far below lower bound
-        df["max_change_below"] = df.lower_bounds - df.topo
-        number_enforced = 0
-        for i, j in enumerate(df[f"iter_{iteration_number}_correction"]):
-            if j < df.max_change_below[i]:
-                number_enforced += 1
-                df.loc[i, f"iter_{iteration_number}_correction"] = df.max_change_below[
-                    i
-                ]
-
-        logging.info("enforced lower confining surface at %s prisms", number_enforced)
-
-    # check that when constrained correction is added to topo it doesn't intersect
-    # either bounding layer
-    updated_topo: pd.Series[float] = df[f"iter_{iteration_number}_correction"] + df.topo
-    if "upper_bounds" in df and np.any((df.upper_bounds - updated_topo) < -0.001):
-        msg = (
-            "Constraining didn't work and updated topography intersects upper "
-            "constraining surface"
-        )
-        raise ValueError(msg)
-    if "lower_bounds" in df and np.any((updated_topo - df.lower_bounds) < -0.001):
-        msg = (
-            "Constraining didn't work and updated topography intersects lower "
-            "constraining surface"
-        )
-        raise ValueError(msg)
-    return df
-
-
-def apply_surface_correction(
-    prisms_df: pd.DataFrame,
-    iteration_number: int,
-) -> tuple[pd.DataFrame, xr.DataArray]:
-    """
-    update the prisms dataframe and dataset with the surface correction. Ensure that
-    the updated surface doesn't intersect the optional confining surfaces.
-
-    Parameters
-    ----------
-    prisms_df : pd.DataFrame
-        dataframe of prism properties
-    iteration_number : int
-        the iteration number, starting at 1 not 0
-
-    Returns
-    -------
-    tuple[pd.DataFrame, xr.DataArray]
-        updated prisms dataframe and correction grid
-    """
-
-    df = prisms_df.copy()
-
-    # for negative densities, negate the correction
-    df.loc[df.density < 0, f"iter_{iteration_number}_correction"] *= -1
-
-    # optionally constrain the surface correction with bounding surfaces
-    df = enforce_confining_surface(df, iteration_number)
+    new_kwargs = {
+        key: value
+        for key, value in kwargs.items()
+        if key
+        not in [
+            "zref",
+            "density_contrast",
+        ]
+    }
 
-    # grid the corrections
-    correction_grid = (
-        df.rename(columns={f"iter_{iteration_number}_correction": "z"})
-        .set_index(["northing", "easting"])
-        .to_xarray()
-        .z
+    # run inversion
+    results = inversion.run_inversion(
+        grav_df=grav_df,
+        zref=zref,
+        density_contrast=density_contrast,
+        **new_kwargs,
     )
+    prism_results, _, _, _ = results
 
-    return df, correction_grid
-
-
-def update_prisms_ds(
-    prisms_ds: xr.Dataset,
-    correction_grid: xr.DataArray,
-    zref: float,
-) -> xr.Dataset:
-    """
-    apply the corrections grid and update the prism tops, bottoms, topo, and
-    densities.
-
-    Parameters
-    ----------
-    prisms_ds : xr.Dataset
-        harmonica prism layer
-    correction_grid : xr.DataArray
-        grid of corrections to apply to the prism layer
-    zref : float
-        reference level for the prism layer
-
-    Returns
-    -------
-    xr.Dataset
-        updated prism layer with new tops, bottoms, topo, and densities
-    """
-
-    ds = prisms_ds.copy()
-
-    density_contrast = ds.density.values.max()
-
-    # create topo from top and bottom
-    topo_grid = xr.where(ds.density > 0, ds.top, ds.bottom)
+    # get last iteration's layer result
+    final_topography = prism_results.set_index(["northing", "easting"]).to_xarray().topo
 
-    # apply correction to topo
-    topo_grid += correction_grid
-
-    # update the prism layer
-    ds.prism_layer.update_top_bottom(surface=topo_grid, reference=zref)
-
-    # update the density
-    ds["density"] = xr.where(ds.top > zref, density_contrast, -density_contrast)
+    # sample the inverted topography at the constraint points
+    constraints_df = utils.sample_grids(
+        constraints_df,
+        final_topography,
+        "inverted_topo",
+        coord_names=("easting", "northing"),
+    )
 
-    # update the topo
-    ds["topo"] = topo_grid
+    dif = constraints_df.upward - constraints_df.inverted_topo
 
-    return ds
+    return utils.rmse(dif, as_median=rmse_as_median)
 
 
-def add_updated_prism_properties(
-    prisms_df: pd.DataFrame,
-    prisms_ds: xr.Dataset,
-    iteration_number: int,
-) -> pd.DataFrame:
+def zref_density_optimal_parameter(
+    grav_df: pd.DataFrame,
+    constraints_df: pd.DataFrame,
+    starting_topography: xr.DataArray | None = None,
+    zref_values: list[float] | None = None,
+    density_contrast_values: list[float] | None = None,
+    starting_topography_kwargs: dict[str, typing.Any] | None = None,
+    regional_grav_kwargs: dict[str, typing.Any] | None = None,
+    rmse_as_median: bool = False,
+    progressbar: bool = True,
+    plot_cv: bool = False,
+    verbose: bool = False,
+    results_fname: str | None = None,
+    **kwargs: typing.Any,
+) -> tuple[
+    tuple[pd.DataFrame, pd.DataFrame, dict[str, typing.Any], float],
+    float,
+    float,
+    float,
+    list[typing.Any],
+    list[float],
+]:
     """
-    update the prisms dataframe the the new prism tops, bottoms, topo, and densities
-    the iteration number, starting at 1 not 0
+    Calculate the cross validation scores for a set of zref and density values and
+    return the best score and values. If only 1 parameter is needed to be test, can pass
+    a single value of the other parameter. This uses constraint points, where the target
+    topography is known. The inverted topography at each of these points is compared to
+    the known value and used to calculate the score.
 
     Parameters
     ----------
-    prisms_df : pd.DataFrame
-        dataframe of prism properties
-    prisms_ds : xr.Dataset
-        dataset of prism properties
-    iteration_number : int
-        the iteration number, starting at 1 not 0
+    grav_df : pd.DataFrame
+        dataframe with gravity data and coordinates, must have coordinate columns
+        "easting", "northing", and "upward", and gravity data column defined by kwarg
+        "grav_data_column".
+    constraints_df : pd.DataFrame
+        dataframe with points where the topography of interest has been previously
+        measured, must have coordinate columns "easting", "northing", and "upward".
+    starting_topography : xr.DataArray,optional
+        starting topography to use to create the starting prism model. If not supplied,
+        starting_topography_kwargs must be provided to create the starting topography.
+        By default None.
+    zref_values : list[float] | None, optional
+        Reference level values to test, by default None
+    density_contrast_values : list[float] | None, optional
+        Density contrast values to test, by default None
+    starting_topography_kwargs : dict[str, typing.Any] | None, optional
+        Keywords used to create the starting topography, by default None
+    regional_grav_kwargs : dict[str, typing.Any] | None, optional
+        Keywords used to calculate the regional field, by default None
+    rmse_as_median : bool, optional
+        Use the median instead of the root mean square as the scoring metric, by default
+        False
+    progressbar : bool, optional
+        display a progress bar for the number of tested values, by default True
+    plot_cv : bool, optional
+        plot a graph of scores vs parameter values, by default False
+    verbose : bool, optional
+        log the results, by default False
+    results_fname : str, optional
+        file name to save results to, by default "tmp" with an attached random number
 
     Returns
     -------
-    pd.DataFrame
-        updated prism dataframe with new tops, bottoms, topo, and densities
-    """
-
-    df = prisms_df.copy()
-    ds = prisms_ds.copy()
-
-    # turn back into dataframe
-    prisms_iter = ds.to_dataframe().reset_index().dropna().astype(float)
-
-    # add new cols to dict
-    dict_of_cols = {
-        f"iter_{iteration_number}_top": prisms_iter.top,
-        f"iter_{iteration_number}_bottom": prisms_iter.bottom,
-        f"iter_{iteration_number}_density": prisms_iter.density,
-        f"iter_{iteration_number}_layer": prisms_iter.topo,
-    }
-
-    df = pd.concat([df, pd.DataFrame(dict_of_cols)], axis=1)
-    df["topo"] = prisms_iter.topo
-
-    return df
-
-
-def grids_to_prisms(
-    surface: xr.DataArray,
-    reference: float | xr.DataArray,
-    density: float | int | xr.DataArray,
-    input_coord_names: tuple[str, str] = ("easting", "northing"),
-) -> xr.Dataset:
-    """
-    create a Harmonica layer of prisms with assigned densities.
+    tuple[ tuple[pd.DataFrame, pd.DataFrame, dict[str, typing.Any], float],
+        float, float, float, list[typing.Any], list[float], ]
+        the inversion results, the optimal parameter value, the score associated with
+        it, the parameter values and the scores for each parameter value
+    """
+
+    if verbose:
+        # set Python's logging level to get information about the inversion\s progress
+        logger = logging.getLogger()
+        logger.setLevel(logging.INFO)
+    else:
+        logger = logging.getLogger()
+        logger.setLevel(logging.WARNING)
 
-    Parameters
-    ----------
-    surface : xr.DataArray
-        data to use for prism surface
-    reference : float | xr.DataArray
-        data or constant to use for prism reference, if value is below surface, prism
-        will be inverted
-    density : float | int | xr.DataArray
-        data or constant to use for prism densities.
-    input_coord_names : tuple[str, str], optional
-        names of the coordinates in the input dataarray, by default
-        ["easting", "northing"]
-    Returns
-    -------
-    xr.Dataset
-       a prisms layer with assigned densities
-    """
+    # set file name for saving results with random number between 0 and 999
+    if results_fname is None:
+        results_fname = f"tmp_{random.randint(0,999)}"
 
-    # if density provided as a single number, use it for all prisms
-    if isinstance(density, (float, int)):
-        dens = density * np.ones_like(surface)
-    # if density provided as a dataarray, map each density to the correct prisms
-    elif isinstance(density, xr.DataArray):
-        dens = density
-    else:
-        msg = "invalid density type, should be a number or DataArray"
+    if constraints_df is None:
+        msg = "must provide constraints_df"
         raise ValueError(msg)
 
-    # create layer of prisms based off input dataarrays
-    prisms = hm.prism_layer(
-        coordinates=(
-            surface[input_coord_names[0]].values,
-            surface[input_coord_names[1]].values,
-        ),
-        surface=surface,
-        reference=reference,
-        properties={
-            "density": dens,
-        },
-    )
-
-    prisms["thickness"] = prisms.top - prisms.bottom
-
-    return prisms
-
-
-def best_spline_cv(
-    coordinates: tuple[pd.Series | NDArray, pd.Series | NDArray],
-    data: pd.Series | NDArray,
-    weights: pd.Series | NDArray | None = None,
-    dampings: typing.Any | None = None,
-    delayed: bool = False,
-    force_coords: tuple[pd.Series | NDArray, pd.Series | NDArray] | None = None,
-) -> vd.Spline:
-    """
-    find the best damping parameter for a verde.SplineCV() fit
+    if (zref_values is None) & (density_contrast_values is None):
+        msg = "must provide either or both zref_values and density_contrast_values"
+        raise ValueError(msg)
 
-    Parameters
-    ----------
-    coordinates : tuple[pd.Series  |  NDArray, pd.Series  |  NDArray]
-        easting and northing coordinates of the data
-    data : pd.Series | NDArray
-        data for fitting the spline to
-    weights : pd.Series | NDArray | None, optional
-        if not None, then the weights assigned to each data point. Typically, this
-        should be 1 over the data uncertainty squared, by default None
-    dampings : typing.Any | None, optional
-        the positive damping regularization parameter. Controls how much smoothness is
-        imposed on the estimated forces. If None, no regularization is used, by default
-        None
-    delayed : bool, optional
-        if True, will use dask.delayed to dispatch computations and allow mod:dask to
-        execute the grid search in parallel, by default False
-    force_coords : tuple[pd.Series  |  NDArray, pd.Series  |  NDArray] | None, optional
-        the easting and northing coordinates of the point forces. Same as force_coords
-        if it is not None. Otherwise, same as the data locations used to fit the spline,
-        by default None
+    if zref_values is None:
+        zref = kwargs.get("zref", None)
+        if zref is None:
+            msg = "must provide zref_values or zref in kwargs"
+            raise ValueError(msg)
+        zref_values = [zref]
+    elif density_contrast_values is None:
+        density_contrast = kwargs.get("density_contrast", None)
+        if density_contrast is None:
+            msg = "must provide density_contrast_values or density_contrast in kwargs"
+            raise ValueError(msg)
+        density_contrast_values = [density_contrast]
+
+    # raise warning about using constraint point minimization for regional estimation
+    if (regional_grav_kwargs is not None) and (
+        regional_grav_kwargs.get("regional_method") == "constraints"
+    ):
+        msg = (
+            "Using constraint points for regional field estimation. This is not "
+            "recommended as the constraint points are used for the cross-validation, "
+            "making the scoring metric meaningless. Consider using a different method "
+            "for regional field estimation."
+        )
+        logging.warning(msg)
+
+    # create all possible combinations of zref and density contrast
+    parameter_pairs = list(itertools.product(zref_values, density_contrast_values))  # type: ignore[arg-type]
+
+    if "test" in grav_df.columns:
+        assert (
+            grav_df.test.any()
+        ), "test column contains True value, not needed except for during damping CV"
+
+    # run inversions and collect scores
+    scores = []
+    pbar = tqdm(
+        parameter_pairs,
+        desc="Zref/Density pairs",
+        disable=not progressbar,
+    )
 
-    Returns
-    -------
-    vd.Spline
-        the spline which best fits the data
-    """
-    if isinstance(dampings, (float, int)):
-        dampings = [dampings]
-    assert isinstance(dampings, list)
-    # if dampings is None:
-    #     dampings = list(np.logspace(-10, -2, num=9))
-    #     dampings.append(None)
-    spline = vd.SplineCV(
-        dampings=dampings,
-        delayed=delayed,
-        force_coords=force_coords,
-    )
-    # with warnings.catch_warnings():
-    # warnings.simplefilter("ignore", sp.linalg.LinAlgWarning)
-    # with HiddenPrints():
-    spline.fit(
-        coordinates,
-        data,
-        weights=weights,
-    )
-
-    try:
-        logging.info("Highest score: %s", spline.scores_.max())
-    except AttributeError:
-        logging.info("Highest score: %s", max(dask.compute(spline.scores_)[0]))
-
-    logging.info("Best damping: %s", spline.damping_)
-
-    try:
-        if len(dampings) > 2 and spline.damping_ in [
-            np.min(dampings),
-            np.max(dampings),
-        ]:
-            warnings.warn(
-                f"Warning: best damping parameter ({spline.damping_}) for "
-                "verde.SplineCV() is at the limit of provided values "
-                f"({np.nanmin(dampings), np.nanmax(dampings)}) and thus is likely "
-                f"not a global minimum, expand the range of values with 'dampings'",
-                stacklevel=2,
+    for i, (zref, density_contrast) in enumerate(pbar):
+        # create starting topography
+        if starting_topography is None:
+            if starting_topography_kwargs is None:
+                msg = (
+                    "starting_topography_kwargs must be provided if "
+                    "starting_topography is not provided"
+                )
+                raise ValueError(msg)
+            method = starting_topography_kwargs.get("method")
+            upwards = starting_topography_kwargs.get("upwards", None)
+            if (method == "flat") & (upwards is None):
+                upwards = zref
+
+            created_starting_topography = utils.create_topography(
+                method=method,  # type: ignore [arg-type]
+                region=starting_topography_kwargs.get("region", None),
+                spacing=starting_topography_kwargs.get("spacing", None),
+                upwards=upwards,
+                constraints_df=constraints_df,
+                dampings=starting_topography_kwargs.get(
+                    "dampings", np.logspace(-10, 0, 100)
+                ),
             )
-    except TypeError:
-        pass
-
-    return spline
+        else:
+            created_starting_topography = starting_topography.copy()
 
+        # re-calculate density grid with new density contrast
+        density_grid = xr.where(
+            created_starting_topography >= zref, density_contrast, -density_contrast
+        )
+
+        # create layer of prisms
+        starting_prisms = utils.grids_to_prisms(
+            created_starting_topography,
+            reference=zref,
+            density=density_grid,
+        )
+
+        # calculate forward gravity of starting prism layer
+        grav_df["starting_grav"] = starting_prisms.prism_layer.gravity(
+            coordinates=(
+                grav_df.easting,
+                grav_df.northing,
+                grav_df.upward,
+            ),
+            field="g_z",
+            progressbar=False,
+        )
+
+        # calculate misfit as observed - starting
+        grav_data_column = kwargs.get("grav_data_column")
+        grav_df["misfit"] = grav_df[grav_data_column] - grav_df.starting_grav
+
+        # calculate regional field
+        reg_kwargs = regional_grav_kwargs.copy()  # type: ignore[union-attr]
+
+        grav_df = regional.regional_separation(
+            method=reg_kwargs.pop("regional_method", None),
+            grav_df=grav_df,
+            regional_column="reg",
+            grav_data_column="misfit",
+            **reg_kwargs,
+        )
+
+        # remove the regional from the misfit to get the residual
+        grav_df["res"] = grav_df.misfit - grav_df.reg
+
+        # update zref value in kwargs
+        kwargs["zref"] = zref
+
+        # update density contrast value in kwargs
+        kwargs["density_contrast"] = density_contrast
+
+        # update starting model in kwargs
+        kwargs["prism_layer"] = starting_prisms
+
+        # run cross validation
+        score = constraints_cv_score(
+            grav_df=grav_df,
+            constraints_df=constraints_df,
+            results_fname=f"{results_fname}_trial_{i}",
+            rmse_as_median=rmse_as_median,
+            **kwargs,
+        )
+        scores.append(score)
+
+    logger = logging.getLogger()
+    logger.setLevel(logging.INFO)
+
+    # print parameter and score pairs
+    for (zref, density_contrast), score in zip(parameter_pairs, scores):
+        logging.info(
+            "Reference level: %s, Density contrast: %s -> Score: %s",
+            zref,
+            density_contrast,
+            score,
+        )
+
+    best_idx = np.argmin(scores)
+    best_score = scores[best_idx]
+    best_zref = parameter_pairs[best_idx][0]
+    best_density = parameter_pairs[best_idx][1]
+    logging.info(
+        "Best score of %s with reference level=%s and density contrast=%s",
+        best_score,
+        best_zref,
+        best_density,
+    )
 
-def eq_sources_score(
-    params: dict[str, float],
-    coordinates: tuple[pd.Series | NDArray, pd.Series | NDArray, pd.Series | NDArray],
-    data: pd.Series | NDArray,
-    delayed: bool = False,
-    **kwargs: typing.Any,
-) -> float:
-    """
-    _summary_
+    # get best inversion result of each set
+    with pathlib.Path(f"{results_fname}_trial_{best_idx}.pickle").open("rb") as f:
+        inv_results = pickle.load(f)
+
+    # delete other inversion results
+    for i in range(len(scores)):
+        if i == best_idx:
+            pass
+        else:
+            pathlib.Path(f"{results_fname}_trial_{i}.pickle").unlink(missing_ok=True)
+
+    # put scores and parameter pairs into dict
+    results = {
+        "scores": scores,
+        "zref_values": parameter_pairs[0],
+        "density_contrast_values": parameter_pairs[1],
+    }
 
-    Parameters
-    ----------
-    params : dict[str, float]
-        dictionary with damping and depth parameters for the equivalent sources fit
-    coordinates : tuple[pd.Series  |  NDArray, pd.Series  |
-        NDArray, pd.Series  |  NDArray]
-        easting, northing, and upwards coordinates of the gravity data
-    data : pd.Series | NDArray
-        gravity data values
-    delayed : bool, optional
-        If True, will use dask.delayed to dispatch computations without actually
-        executing them. The returned scores will be a list of delayed objects, by
-        default False
+    # remove if exists
+    pathlib.Path(results_fname).unlink(missing_ok=True)
 
-    Returns
-    -------
-    float
-        the mean score of the equivalent sources fit
-    """
-    eqs = hm.EquivalentSources(
-        damping=params.get("damping"),
-        depth=params.get("depth"),
-        **kwargs,
-    )
-    return float(
-        np.mean(
-            vd.cross_val_score(
-                eqs,
-                coordinates,
-                data,
-                delayed=delayed,
-                weights=kwargs.get("weights", None),
+    # save scores and parameter pairs to pickle
+    with pathlib.Path(f"{results_fname}.pickle").open("wb") as f:
+        pickle.dump(results, f)
+
+    if plot_cv:
+        if len(zref_values) == 1:
+            plotting.plot_cv_scores(
+                scores,
+                density_contrast_values,  # type: ignore[arg-type]
+                param_name="Density contrast (kg/m$^3$)",
+                plot_title="Density contrast Cross-validation",
+                # logx=True,
+                # logy=True,
             )
-        )
-    )
-    # eqs.fit(coordinates, data, weights=kwargs.get("weights", None))
-    # score = eqs.score(coordinates, data, weights=kwargs.get("weights", None))
+        elif len(density_contrast_values) == 1:  # type: ignore[arg-type]
+            plotting.plot_cv_scores(
+                scores,
+                zref_values,
+                param_name="Reference level (m)",
+                plot_title="Reference level Cross-validation",
+                # logx=True,
+                # logy=True,
+            )
+        else:
+            plotting.plot_2_parameter_cv_scores(
+                scores,
+                parameter_pairs,
+                param_names=("Reference level (m)", "Density contrast (kg/m$^3$)"),
+                # logx=True,
+                # logy=True,
+            )
+
+    return inv_results, best_zref, best_density, best_score, parameter_pairs, scores
```

### Comparing `invert4geom-0.5.0/src/invert4geom.egg-info/PKG-INFO` & `invert4geom-0.6.0/src/invert4geom.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invert4geom
-Version: 0.5.0
+Version: 0.6.0
 Summary: Constrained gravity inversion to recover the geometry of a density contrast.
 Author-email: Matt Tankersley <matt.d.tankersley@gmail.com>
 License: Copyright 2023 Matt Tankersley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -72,14 +72,15 @@
 Provides-Extra: viz
 Requires-Dist: pyvista; extra == "viz"
 Requires-Dist: trame; extra == "viz"
 Requires-Dist: ipywidgets; extra == "viz"
 Requires-Dist: matplotlib; extra == "viz"
 Requires-Dist: seaborn; extra == "viz"
 Requires-Dist: ipython; extra == "viz"
+Requires-Dist: plotly; extra == "viz"
 Provides-Extra: test
 Requires-Dist: pytest>=6; extra == "test"
 Requires-Dist: pytest-cov>=3; extra == "test"
 Requires-Dist: invert4geom[opti]; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=4.0; extra == "docs"
 Requires-Dist: myst_parser; extra == "docs"
@@ -172,26 +173,41 @@
 
 <!-- <p align="center">
 <img src="docs/figures/cover_fig.png" width="400"/>
 </p> -->
 
 <!-- SPHINX-START2 -->
 
-**Invert4geom** is a Python library for performing 3D geometric gravity
-inversions, where the aim is to recover the geometry of a density contrast.
+**Invert4geom** is a Python library for performing 3D geometric gravity inversions, where the aim is to recover the geometry of a density contrast.
 
-Typical use cases include modeling the topography of the Moho, the
-sediment-basement contact, or bathymetry. These density contrasts are
-represented by a layer of vertical right-rectangular prisms. Since we use
-vertical prisms, they don't take the curvature of the Earth into account. For
-large-scale applications, such as continental studies, it would be better to use
-tesseroids instead of prisms.
-
-See the [overview](overview.md) for further description of this package and what
-it can be used for.
+Typical use cases include modeling the topography of the Moho, the sediment-basement contact, or bathymetry.
+These density contrasts are represented by a layer of vertical right-rectangular prisms.
+Since we use vertical prisms, they don't take the curvature of the Earth into account.
+For large-scale applications, such as continental studies, it would be better to use tesseroids instead of prisms.
+
+See the [overview](overview.md) for further description of this package and what it can be used for.
+
+#### What _Invert4Geom_ is for:
+
+- invert **gravity** data to recover the topography of a density contrast
+- use with **gridded** gravity data
+- discretization using _vertical right-rectangular prisms_
+- performing regional-residual separation
+- stochastic uncertainty analysis of inversion results
+- basic visualization tools
+
+#### What _Invert4Geom_ is **NOT** for:
+
+- performing parameter-estimation inversions (i.e. recovering density values) -> see [SimPEG](https://simpeg.xyz/) or [pyGIMLi](https://www.pygimli.org/index.html)
+- a point-and-click GUI -> see [Geosoft/Seequent Oasis Montaj](https://www.seequent.com/products-solutions/ geosoft-oasis-montaj/) or [MiraGeoscience VPmg](https://www.mirageoscience.com/mining-industry-software/geoscience-analyst-pro-geophysics/)
+- a ready-to-use inversion with minimal user input
+- use with discrete (un-gridded) gravity data -> see [Harmonica](https://www.fatiando.org/harmonica/latest/index.html) for gridding your data
+- for processing gravity data -> see [Harmonica](https://www.fatiando.org/harmonica/latest/index.html) for gravity processing tools
+- for use with tesseroids, or non-regular grids (raise an issue request if you want this implemented!)
+- publication-quality visualization -> see [PyGMT](https://www.pygmt.org/dev/index.html) for plotting tools
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/mdtanker/invert4geom/workflows/CI/badge.svg
 [actions-link]:             https://github.com/mdtanker/invert4geom/actions
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/invert4geom
 [conda-link]:               https://github.com/conda-forge/invert4geom-feedstock
 [codecov-badge]:            https://codecov.io/github/mdtanker/invert4geom/badge.svg?
```

### Comparing `invert4geom-0.5.0/src/invert4geom.egg-info/SOURCES.txt` & `invert4geom-0.6.0/src/invert4geom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invert4geom-0.5.0/src/invert4geom.egg-info/requires.txt` & `invert4geom-0.6.0/src/invert4geom.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,7 +57,8 @@
 [viz]
 pyvista
 trame
 ipywidgets
 matplotlib
 seaborn
 ipython
+plotly
```

### Comparing `invert4geom-0.5.0/tests/test_inversion.py` & `invert4geom-0.6.0/tests/test_inversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -545,56 +545,55 @@
     assert updated_delta_l2_norm == pytest.approx(
         expected_updated_delta_l2_norm, rel=1e-6
     )
 
 
 def test_end_inversion_first_iteration():
     """
-    Test that the inversion is not terminated in the first iteration.
+    Test that the inversion is not terminated in the first iteration even if the L2 norm
+    is below the tolerance.
     """
     iteration_number = 1
     max_iterations = 100
-    l2_norm = 1.0
-    starting_l2_norm = 1.0
-    l2_norm_tolerance = 0.1
+    l2_norms = [1.0]
+    l2_norm_tolerance = 2.0
     delta_l2_norm = 0.01
     previous_delta_l2_norm = 0.01
     delta_l2_norm_tolerance = 0.01
+    perc_increase_limit = 0.20
     end, termination_reason = inversion.end_inversion(
         iteration_number,
         max_iterations,
-        l2_norm,
-        starting_l2_norm,
+        l2_norms,
         l2_norm_tolerance,
         delta_l2_norm,
         previous_delta_l2_norm,
         delta_l2_norm_tolerance,
+        perc_increase_limit,
     )
     assert not end
     assert termination_reason == []
 
 
 def test_end_inversion_l2_norm_increasing():
     """
     Test that the inversion is terminated when L2 norm increases beyond a limit.
     """
-    iteration_number = 2
+    iteration_number = 3
     max_iterations = 100
-    l2_norm = 1.3
-    starting_l2_norm = 1.0
+    l2_norms = [1.0, 1.15, 1.21]
     l2_norm_tolerance = 0.1
     delta_l2_norm = 0.01
     previous_delta_l2_norm = 0.01
     delta_l2_norm_tolerance = 0.01
     perc_increase_limit = 0.20
     end, termination_reason = inversion.end_inversion(
         iteration_number,
         max_iterations,
-        l2_norm,
-        starting_l2_norm,
+        l2_norms,
         l2_norm_tolerance,
         delta_l2_norm,
         previous_delta_l2_norm,
         delta_l2_norm_tolerance,
         perc_increase_limit,
     )
     assert end
@@ -603,82 +602,82 @@
 
 def test_end_inversion_delta_l2_norm_tolerance():
     """
     Test that the inversion is terminated when delta L2 norm is below a tolerance.
     """
     iteration_number = 2
     max_iterations = 100
-    l2_norm = 1.0
-    starting_l2_norm = 1.0
+    l2_norms = [1.0, 1.0]
     l2_norm_tolerance = 0.1
     delta_l2_norm = 0.01
     previous_delta_l2_norm = 0.01
     delta_l2_norm_tolerance = 0.01
+    perc_increase_limit = 0.20
     end, termination_reason = inversion.end_inversion(
         iteration_number,
         max_iterations,
-        l2_norm,
-        starting_l2_norm,
+        l2_norms,
         l2_norm_tolerance,
         delta_l2_norm,
         previous_delta_l2_norm,
         delta_l2_norm_tolerance,
+        perc_increase_limit,
     )
     assert end
     assert "delta l2-norm tolerance" in termination_reason
 
 
 def test_end_inversion_l2_norm_tolerance():
     """
     Test that the inversion is terminated when L2 norm is below a tolerance.
     """
     iteration_number = 2
     max_iterations = 100
-    l2_norm = 0.05
-    starting_l2_norm = 1.0
+    l2_norms = [1.0, 0.05]
     l2_norm_tolerance = 0.1
     delta_l2_norm = 0.01
     previous_delta_l2_norm = 0.01
     delta_l2_norm_tolerance = 0.01
+    perc_increase_limit = 0.20
     end, termination_reason = inversion.end_inversion(
         iteration_number,
         max_iterations,
-        l2_norm,
-        starting_l2_norm,
+        l2_norms,
         l2_norm_tolerance,
         delta_l2_norm,
         previous_delta_l2_norm,
         delta_l2_norm_tolerance,
+        perc_increase_limit,
     )
     assert end
     assert "l2-norm tolerance" in termination_reason
 
 
 def test_end_inversion_max_iterations():
     """
     Test that the inversion is terminated when the maximum number of iterations is
     reached.
     """
     iteration_number = 101
     max_iterations = 100
-    l2_norm = 0.5
-    starting_l2_norm = 1.0
+    l2_norms = [1.0, 0.5]
     l2_norm_tolerance = 0.1
     delta_l2_norm = 0.01
     previous_delta_l2_norm = 0.01
     delta_l2_norm_tolerance = 0.01
+    perc_increase_limit = 0.20
     end, termination_reason = inversion.end_inversion(
         iteration_number,
         max_iterations,
-        l2_norm,
-        starting_l2_norm,
+        l2_norms,
         l2_norm_tolerance,
         delta_l2_norm,
         previous_delta_l2_norm,
         delta_l2_norm_tolerance,
+        perc_increase_limit,
     )
     assert end
     assert "max iterations" in termination_reason
 
 
 def test_update_gravity_and_misfit_forward_gravity():
     """
@@ -691,15 +690,15 @@
     # 1       200      100      20            6.8           7.0    -0.2    0 -0.2
     # 2       400     -100      20            7.2           7.0     0.2    0  0.2
     # 3       400      100      20            8.0           7.0     1.0    0  1.0
 
     updated_gravity_df = inversion.update_gravity_and_misfit(
         gravity_df=gravity_df_copy,
         prisms_ds=dummy_prism_layer(),
-        input_grav_column="observed_grav",
+        grav_data_column="observed_grav",
         iteration_number=1,
     )
     # Check that 'iter_1_forward_grav' column is created
     assert "iter_1_forward_grav" in updated_gravity_df.columns
     # Ensure that the 'iter_1_forward_grav' values are as expected
     expected_forward_grav = [7.18, 7.18, 7.70, 7.70]
     assert updated_gravity_df.iter_1_forward_grav.tolist() == pytest.approx(
@@ -725,15 +724,15 @@
     # 0       200     -100      20            6.5           7.0    -0.5    3 -3.5
     # 1       200      100      20            6.8           7.0    -0.2    2 -2.2
     # 2       400     -100      20            7.2           7.0     0.2    1 -0.8
     # 3       400      100      20            8.0           7.0     1.0    0  1.0
     updated_gravity_df = inversion.update_gravity_and_misfit(
         gravity_df=gravity_df_copy,
         prisms_ds=dummy_prism_layer(),
-        input_grav_column="observed_grav",
+        grav_data_column="observed_grav",
         iteration_number=1,
     )
     # expected_forward_grav = [7.18, 7.18, 7.70, 7.70]
     # Ensure that the 'iter_1_final_misfit' values are as expected
     # new misfit should be observed grav - iter_5_forward_grav - regional
     expected_misfit = [-3.68, -2.38, -1.5, 0.30]
     assert updated_gravity_df.iter_1_final_misfit.tolist() == pytest.approx(
@@ -747,16 +746,16 @@
 #     Test the inversions returned values.
 #     """
 #     gravity_df = dummy_misfit_df(regional=False)
 #     prisms_ds = dummy_prism_layer()
 #     print(gravity_df)
 #     print(prisms_ds)
 #     results = inversion.run_inversion(
-#         input_grav=gravity_df,
-#         input_grav_column="observed_grav",
+#         grav_df=gravity_df,
+#         grav_data_column="observed_grav",
 #         prism_layer=prisms_ds,
 #         max_iterations=3,
 #     )
 #     prisms_df, gravity, params, elapsed_time = results
 #     # print(prisms_df)
 #     # print(gravity)
 #     # print(params)
@@ -782,15 +781,15 @@
 #     # calculate misfit -> [-0.4, -0.1, 0.1, 0.6]
 #     gravity_df_copy["iter_4_final_misfit"] = gravity_df_copy.observed_grav -
 # gravity_df_copy.iter_4_forward_grav
 #     # print(gravity_df_copy)
 #     updated_gravity_df = inversion.update_gravity_and_misfit(
 #         gravity_df=gravity_df_copy,
 #         prisms_ds=dummy_prism_layer(),
-#         input_grav_column="observed_grav",
+#         grav_data_column="observed_grav",
 #         iteration_number=5,
 #     )
 #     # Check that 'iter_5_forward_grav' column is created
 #     assert 'iter_5_forward_grav' in updated_gravity_df.columns
 #     # Ensure that the 'iter_5_forward_grav' values are as expected
 #     expected_forward_grav = [7.18, 7.18, 7.70, 7.70]
 #     assert updated_gravity_df.iter_5_forward_grav.tolist() == pytest.approx(
```

### Comparing `invert4geom-0.5.0/tests/test_optimization.py` & `invert4geom-0.6.0/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `invert4geom-0.5.0/tests/test_regional.py` & `invert4geom-0.6.0/tests/test_regional.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     coords = vd.scatter_points(region=region, size=num_constraints, random_state=0)
     points = pd.DataFrame(data={"easting": coords[0], "northing": coords[1]})
 
     # print(grav_df.describe())
 
     df = regional.regional_dc_shift(
         grav_df=grav_df,
-        grav_grid=dummy_grid().misfit,
-        constraint_points=points,
-        regional_col_name="reg",
+        grav_data_column="misfit",
+        constraints_df=points,
+        regional_column="reg",
     )
 
     # print(df.describe())
 
     # test whether regional field has been removed correctly
     # by whether the means of the reg and misfit are similar
     # print(np.mean(df.reg), np.mean(df.misfit))
@@ -74,35 +74,34 @@
     test the regional_dc_shift function with a supplied DC shift
     """
 
     grav_df = dummy_grid().to_dataframe().reset_index()
 
     df = regional.regional_dc_shift(
         grav_df=grav_df,
+        grav_data_column="misfit",
         dc_shift=-200,
-        regional_col_name="reg",
+        regional_column="reg",
     )
 
     assert df.reg.mean() == -200
 
 
-@pytest.mark.parametrize("fill_method", ["rioxarray", "verde"])
 @pytest.mark.parametrize("trend", [0, 2])
-def test_regional_trend(fill_method, trend):
+def test_regional_trend(trend):
     """
     test the regional_trend function
     """
     anomalies = dummy_df()
     # print(fill_method, trend)
 
     df = regional.regional_trend(
         trend=trend,
-        grav_grid=dummy_grid().misfit,
         grav_df=anomalies,
-        fill_method=fill_method,
+        grav_data_column="misfit",
     )
 
     # grid = df.set_index(["northing", "easting"]).to_xarray()
     # polar_utils.grd_compare(grid.reg, grid.misfit, plot=True, plot_type="xarray")
 
     assert len(df.misfit) == len(df.reg)
 
@@ -134,16 +133,16 @@
     """
     test the regional_filter function
     """
     grav_df = dummy_df()
 
     df = regional.regional_filter(
         filter_width=300e3,
-        grav_grid=dummy_grid().misfit,
         grav_df=grav_df,
+        grav_data_column="misfit",
         # registration="g",
     )
 
     # grid = df.set_index(["northing", "easting"]).to_xarray()
     # polar_utils.grd_compare(grid.reg, grid.misfit, plot=True, plot_type="xarray")
 
     assert len(df.misfit) == len(df.reg)
@@ -175,15 +174,15 @@
         percent=True,
         seed=0,
     )
 
     df = regional.regional_eq_sources(
         source_depth=100e3,
         grav_df=grav_df,
-        input_grav_name="misfit",
+        grav_data_column="misfit",
     )
     # print(df)
     reg_range = np.max(df.reg) - np.min(df.reg)
     misfit_range = np.max(df.misfit) - np.min(df.misfit)
     # print(reg_range, misfit_range)
     # test  whether regional field has been remove correctly
     # by whether the range of regional values are lower than the range of misfit values
@@ -214,21 +213,20 @@
     # )
     # create 10 random point within the region
     num_constraints = 10
     coords = vd.scatter_points(region=region, size=num_constraints, random_state=0)
     points = pd.DataFrame(data={"easting": coords[0], "northing": coords[1]})
 
     df = regional.regional_constraints(
-        constraint_points=points,
-        grav_grid=dummy_grid().misfit,
+        constraints_df=points,
         grav_df=anomalies,
-        region=region,
-        spacing=50,
+        grav_data_column="misfit",
         grid_method=test_input,
         eqs_gridding_trials=2,
+        grav_obs_height=1e3,
     )
 
     # grid = df.set_index(["northing", "easting"]).to_xarray()
     # polar_utils.grd_compare(
     #     grid.reg, grid.misfit, plot=True, plot_type="xarray",
     #     points=points.rename(columns={"easting":"x", "northing":"y"}),
     #     )
```

### Comparing `invert4geom-0.5.0/tests/test_utils.py` & `invert4geom-0.6.0/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,64 +259,68 @@
 
 
 def test_normalize_xarray_range():
     """
     Ensure the output is within the [low, high] range.
     """
     data = np.array([1, 2, 3, 4, 5])
-    da = xr.DataArray(data, dims="x")
+    da = xr.DataArray(data, dims="easting")
     da_normalized = utils.normalize_xarray(da, low=2, high=5)
     assert da_normalized.min() >= 2
     assert da_normalized.max() <= 5
 
 
 def test_normalize_xarray_values():
     """
     Ensure the normalized data matches the expected values.
     """
     data = np.array([1, 2, 3, 4, 5])
-    da = xr.DataArray(data, dims="x")
+    da = xr.DataArray(data, dims="easting")
     da_normalized = utils.normalize_xarray(da, low=0, high=1)
     expected_values = np.array([0.0, 0.25, 0.5, 0.75, 1.0])
     npt.assert_array_almost_equal(da_normalized.values, expected_values, decimal=6)
 
 
 def test_normalize_xarray_negative_values():
     """
     Ensure the function handles negative values correctly.
     """
     data = np.array([-5, 0, 5])
-    da = xr.DataArray(data, dims="x")
+    da = xr.DataArray(data, dims="easting")
     da_normalized = utils.normalize_xarray(da, low=0, high=1)
     expected_values = np.array([0.0, 0.5, 1.0])
     npt.assert_array_almost_equal(da_normalized.values, expected_values, decimal=6)
 
 
 def test_normalize_xarray_custom_range():
     """
     Ensure the function handles a custom low and high range correctly.
     """
     data = np.array([10, 20, 30])
-    da = xr.DataArray(data, dims="x")
+    da = xr.DataArray(data, dims="easting")
     da_normalized = utils.normalize_xarray(da, low=-1, high=1)
     expected_values = np.array([-1.0, 0.0, 1.0])
     npt.assert_array_almost_equal(da_normalized.values, expected_values, decimal=6)
 
 
 def test_normalized_mindist_defaults():
     """
     test the normalized_mindist function
     """
     # create 2 constraint points
-    points = pd.DataFrame({"x": [0, 2], "y": [0, -1]})
+    points = pd.DataFrame({"easting": [0, 2], "northing": [0, -1]})
     # create dataarray
     df = pd.DataFrame(
-        {"x": [-4, 4, 0, 4, -4], "y": [-4, 4, 0, -4, 4], "z": [0, 1, 2, 3, 4]}
+        {
+            "easting": [-4, 4, 0, 4, -4],
+            "northing": [-4, 4, 0, -4, 4],
+            "z": [0, 1, 2, 3, 4],
+        }
     )
-    da = df.set_index(["y", "x"]).to_xarray().z
+    da = df.set_index(["northing", "easting"]).to_xarray().z
     # calculate the min distance with defaults
     min_dist = utils.normalized_mindist(
         points=points,
         grid=da,
     )
     # test the grid is correct
     expected = np.array(
@@ -331,20 +335,24 @@
 
 def test_normalized_mindist_mindist():
     """
     test the normalized_mindist function with any values lower than 4 set to 0 with
     parameter `mindist`.
     """
     # create 2 constraint points
-    points = pd.DataFrame({"x": [0, 2], "y": [0, -1]})
+    points = pd.DataFrame({"easting": [0, 2], "northing": [0, -1]})
     # create dataarray
     df = pd.DataFrame(
-        {"x": [-4, 4, 0, 4, -4], "y": [-4, 4, 0, -4, 4], "z": [0, 1, 2, 3, 4]}
+        {
+            "easting": [-4, 4, 0, 4, -4],
+            "northing": [-4, 4, 0, -4, 4],
+            "z": [0, 1, 2, 3, 4],
+        }
     )
-    da = df.set_index(["y", "x"]).to_xarray().z
+    da = df.set_index(["northing", "easting"]).to_xarray().z
 
     # calculate the min distance with mindist value of 4
     min_dist = utils.normalized_mindist(
         points=points,
         grid=da,
         mindist=4,
     )
@@ -359,20 +367,24 @@
 
 
 def test_normalized_mindist_region():
     """
     test the normalized_mindist function with region parameter
     """
     # create 2 constraint points
-    points = pd.DataFrame({"x": [0, 2], "y": [0, -1]})
+    points = pd.DataFrame({"easting": [0, 2], "northing": [0, -1]})
     # create dataarray
     df = pd.DataFrame(
-        {"x": [-4, 4, 0, 4, -4], "y": [-4, 4, 0, -4, 4], "z": [0, 1, 2, 3, 4]}
+        {
+            "easting": [-4, 4, 0, 4, -4],
+            "northing": [-4, 4, 0, -4, 4],
+            "z": [0, 1, 2, 3, 4],
+        }
     )
-    da = df.set_index(["y", "x"]).to_xarray().z
+    da = df.set_index(["northing", "easting"]).to_xarray().z
     # calculate the min distance and points outside region set to 0
     min_dist = utils.normalized_mindist(
         points=points,
         grid=da,
         region=[-4.0, -3.0, -4.0, 0],
     )
     # test the grid is correct
@@ -383,20 +395,24 @@
 
 
 def test_normalized_mindist_high_low():
     """
     test the normalized_mindist function with set high and low values
     """
     # create 2 constraint points
-    points = pd.DataFrame({"x": [0, 2], "y": [0, -1]})
+    points = pd.DataFrame({"easting": [0, 2], "northing": [0, -1]})
     # create dataarray
     df = pd.DataFrame(
-        {"x": [-4, 4, 0, 4, -4], "y": [-4, 4, 0, -4, 4], "z": [0, 1, 2, 3, 4]}
+        {
+            "easting": [-4, 4, 0, 4, -4],
+            "northing": [-4, 4, 0, -4, 4],
+            "z": [0, 1, 2, 3, 4],
+        }
     )
-    da = df.set_index(["y", "x"]).to_xarray().z
+    da = df.set_index(["northing", "easting"]).to_xarray().z
     # calculate the min distance with normalizing limits
     min_dist = utils.normalized_mindist(
         points=points,
         grid=da,
         low=0.2,
         high=5,
     )
@@ -407,20 +423,20 @@
 
 def test_sample_grids_on_nodes():
     """
     Test if the sampled column contains valid values at grid nodes.
     """
     grid = dummy_grid().scalars
     name = "sampled_data"
-    df = pd.DataFrame({"x": [0, 100, 200], "y": [200, 300, 400]})
+    df = pd.DataFrame({"easting": [0, 100, 200], "northing": [200, 300, 400]})
     result_df = utils.sample_grids(df, grid, sampled_name=name)
     expected = pd.DataFrame(
         {
-            "x": [0, 100, 200],
-            "y": [200, 300, 400],
+            "easting": [0, 100, 200],
+            "northing": [200, 300, 400],
             name: [40000, 100000, 200000],
         },
     )
     pdt.assert_frame_equal(
         result_df,
         expected,
         check_dtype=False,
@@ -429,18 +445,18 @@
 
 def test_sample_grids_off_nodes():
     """
     Test if the sampled column contains valid values not on grid nodes.
     """
     grid = dummy_grid().scalars
     name = "sampled_data"
-    df = pd.DataFrame({"x": [50, 101], "y": [280, 355]})
+    df = pd.DataFrame({"easting": [50, 101], "northing": [280, 355]})
     result_df = utils.sample_grids(df, grid, sampled_name=name)
     expected = pd.DataFrame(
-        {"x": [50, 101], "y": [280, 355], name: [83790.0, 138949.640109]}
+        {"easting": [50, 101], "northing": [280, 355], name: [83790.0, 138949.640109]}
     )
     pdt.assert_frame_equal(
         result_df,
         expected,
         check_dtype=False,
     )
 
@@ -473,51 +489,51 @@
 def test_sample_grids_one_out_of_grid_coordinates():
     """
     Test if the function handles out-of-grid coordinates gracefully by setting NaN
     values.
     """
     grid = dummy_grid().scalars
     name = "sampled_data"
-    df = pd.DataFrame({"x": [0, -1000, 200], "y": [200, -1000, 400]})
+    df = pd.DataFrame({"easting": [0, -1000, 200], "northing": [200, -1000, 400]})
     result_df = utils.sample_grids(df, grid, sampled_name=name)
     assert np.isnan(result_df[name].iloc[1])
 
 
 def test_sample_grids_first_out_of_grid_coordinates():
     """
     Test if the function handles out-of-grid coordinates gracefully by setting NaN
     values.
     """
     grid = dummy_grid().scalars
     name = "sampled_data"
-    df = pd.DataFrame({"x": [-50, 150, 200], "y": [500, 350, 400]})
+    df = pd.DataFrame({"easting": [-50, 150, 200], "northing": [500, 350, 400]})
     result_df = utils.sample_grids(df, grid, sampled_name=name)
     assert np.isnan(result_df[name].iloc[0])
 
 
 def test_sample_grids_last_out_of_grid_coordinates():
     """
     Test if the function handles out-of-grid coordinates gracefully by setting NaN
     values.
     """
     grid = dummy_grid().scalars
     name = "sampled_data"
-    df = pd.DataFrame({"x": [200, 150, 0], "y": [200, 350, 0]})
+    df = pd.DataFrame({"easting": [200, 150, 0], "northing": [200, 350, 0]})
     result_df = utils.sample_grids(df, grid, sampled_name=name)
     assert np.isnan(result_df[name].iloc[2])
 
 
 def test_sample_grids_all_out_of_grid_coordinates_all():
     """
     Test if the function handles out-of-grid coordinates gracefully by setting NaN
     values.
     """
     grid = dummy_grid().scalars
     name = "sampled_data"
-    points = pd.DataFrame({"x": [-100, -200, -300], "y": [500, 1000, 600]})
+    points = pd.DataFrame({"easting": [-100, -200, -300], "northing": [500, 1000, 600]})
     result_df = utils.sample_grids(points, grid, sampled_name=name)
     assert result_df[name].isnull().all()  # All values should be NaN
 
 
 def test_extract_prism_data():
     """
     Test if function for checking prisms and extract data works properly
@@ -541,22 +557,26 @@
 
 
 def test_sample_bounding_surfaces_valid_values():
     """
     Ensure that correct values are sampled, including a NaN
     """
     lower_confining_layer = dummy_grid().scalars
-    points = pd.DataFrame({"x": [0, -100, 200], "y": [200, -300, 400]})
+    points = pd.DataFrame({"easting": [0, -100, 200], "northing": [200, -300, 400]})
     result_df = utils.sample_grids(
         points,
         lower_confining_layer,
         sampled_name="sampled",
     )
     expected = pd.DataFrame(
-        {"x": [0, -100, 200], "y": [200, -300, 400], "sampled": [40000, np.nan, 200000]}
+        {
+            "easting": [0, -100, 200],
+            "northing": [200, -300, 400],
+            "sampled": [40000, np.nan, 200000],
+        }
     )
     pdt.assert_frame_equal(result_df, expected)
 
 
 def test_sample_bounding_surfaces_upper_and_lower():
     """
     Ensure that when both upper and lower layers are provided, both are sampled.
```

