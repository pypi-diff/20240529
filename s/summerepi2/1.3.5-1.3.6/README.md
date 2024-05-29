# Comparing `tmp/summerepi2-1.3.5.tar.gz` & `tmp/summerepi2-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summerepi2-1.3.5.tar", max compression
+gzip compressed data, was "summerepi2-1.3.6.tar", max compression
```

## Comparing `summerepi2-1.3.5.tar` & `summerepi2-1.3.6.tar`

### file list

```diff
@@ -1,34 +1,39 @@
--rw-r--r--   0        0        0     1512 2022-11-27 21:58:51.446839 summerepi2-1.3.5/LICENSE.txt
--rw-r--r--   0        0        0     1942 2024-03-25 23:34:31.579325 summerepi2-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     4871 2024-03-25 23:19:46.211672 summerepi2-1.3.5/README.md
--rw-r--r--   0        0        0      280 2022-11-27 21:58:51.470346 summerepi2-1.3.5/summer2/__init__.py
--rw-r--r--   0        0        0     4095 2022-11-27 21:58:51.471557 summerepi2-1.3.5/summer2/adjust.py
--rw-r--r--   0        0        0     4782 2022-11-27 21:58:51.471557 summerepi2-1.3.5/summer2/compartment.py
--rw-r--r--   0        0        0    11683 2022-11-27 21:58:51.475937 summerepi2-1.3.5/summer2/derived_outputs.py
--rw-r--r--   0        0        0    10490 2023-11-22 21:41:46.346511 summerepi2-1.3.5/summer2/experimental/model_builder.py
--rw-r--r--   0        0        0     2590 2023-11-22 21:41:46.352533 summerepi2-1.3.5/summer2/extras/test_models.py
--rw-r--r--   0        0        0    19461 2023-11-22 21:41:46.355984 summerepi2-1.3.5/summer2/flows.py
--rw-r--r--   0        0        0      209 2023-11-22 21:41:46.360978 summerepi2-1.3.5/summer2/functions/__init__.py
--rw-r--r--   0        0        0     2276 2023-11-22 21:41:46.363900 summerepi2-1.3.5/summer2/functions/derived.py
--rw-r--r--   0        0        0     4481 2023-11-22 21:41:46.369367 summerepi2-1.3.5/summer2/functions/interpolate.py
--rw-r--r--   0        0        0     4106 2023-11-22 21:41:46.372729 summerepi2-1.3.5/summer2/functions/time.py
--rw-r--r--   0        0        0     4033 2023-11-22 21:41:46.377509 summerepi2-1.3.5/summer2/functions/util.py
--rw-r--r--   0        0        0     8195 2023-11-22 21:41:46.381111 summerepi2-1.3.5/summer2/inspect.py
--rw-r--r--   0        0        0    55616 2023-11-22 21:41:46.386067 summerepi2-1.3.5/summer2/model.py
--rw-r--r--   0        0        0       22 2022-11-27 21:58:51.481744 summerepi2-1.3.5/summer2/parameters/__init__.py
--rw-r--r--   0        0        0    11253 2023-11-22 21:41:46.393065 summerepi2-1.3.5/summer2/parameters/param_impl.py
--rw-r--r--   0        0        0     4255 2023-11-22 21:41:46.397626 summerepi2-1.3.5/summer2/parameters/params.py
--rw-r--r--   0        0        0     4804 2022-11-27 21:58:51.484030 summerepi2-1.3.5/summer2/population.py
--rw-r--r--   0        0        0       40 2022-11-27 21:58:51.485116 summerepi2-1.3.5/summer2/runner/__init__.py
--rw-r--r--   0        0        0        0 2022-11-27 21:58:51.486457 summerepi2-1.3.5/summer2/runner/jax/__init__.py
--rw-r--r--   0        0        0     5240 2023-11-22 21:41:46.402360 summerepi2-1.3.5/summer2/runner/jax/derived_outputs.py
--rw-r--r--   0        0        0    28228 2023-11-22 21:41:46.408502 summerepi2-1.3.5/summer2/runner/jax/model_impl.py
--rw-r--r--   0        0        0    11659 2024-02-08 04:59:18.770793 summerepi2-1.3.5/summer2/runner/jax/ode.py
--rw-r--r--   0        0        0     2736 2023-11-22 21:41:46.419988 summerepi2-1.3.5/summer2/runner/jax/solvers.py
--rw-r--r--   0        0        0     5369 2023-11-22 21:41:46.423877 summerepi2-1.3.5/summer2/runner/jax/stratify.py
--rw-r--r--   0        0        0     8170 2023-11-22 21:41:46.428917 summerepi2-1.3.5/summer2/runner/model_runner.py
--rw-r--r--   0        0        0     6277 2022-11-27 21:58:51.493538 summerepi2-1.3.5/summer2/solver.py
--rw-r--r--   0        0        0    17065 2022-11-27 21:58:51.494698 summerepi2-1.3.5/summer2/stratification.py
--rw-r--r--   0        0        0      472 2022-11-27 21:58:51.494698 summerepi2-1.3.5/summer2/tracker.py
--rw-r--r--   0        0        0     3760 2023-11-22 21:41:46.433498 summerepi2-1.3.5/summer2/utils.py
--rw-r--r--   0        0        0     6344 1970-01-01 00:00:00.000000 summerepi2-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1512 2022-09-01 20:25:00.648111 summerepi2-1.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     1978 2024-05-29 04:15:25.821971 summerepi2-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3266 2024-04-23 00:32:16.967244 summerepi2-1.3.6/README.md
+-rw-r--r--   0        0        0      280 2022-09-01 05:32:07.966265 summerepi2-1.3.6/summer2/__init__.py
+-rw-r--r--   0        0        0     4095 2022-09-01 05:32:07.967266 summerepi2-1.3.6/summer2/adjust.py
+-rw-r--r--   0        0        0     4782 2022-09-01 05:32:07.967769 summerepi2-1.3.6/summer2/compartment.py
+-rw-r--r--   0        0        0      137 2022-08-26 06:17:31.101047 summerepi2-1.3.6/summer2/compute_bak/__init__.py
+-rw-r--r--   0        0        0     2151 2022-08-27 21:20:06.649159 summerepi2-1.3.6/summer2/compute_bak/compute_jax.py
+-rw-r--r--   0        0        0    11683 2022-09-01 05:32:07.968765 summerepi2-1.3.6/summer2/derived_outputs.py
+-rw-r--r--   0        0        0    10490 2023-04-05 00:33:04.716810 summerepi2-1.3.6/summer2/experimental/model_builder.py
+-rw-r--r--   0        0        0     2590 2023-11-14 00:54:52.318965 summerepi2-1.3.6/summer2/extras/test_models.py
+-rw-r--r--   0        0        0    19461 2023-11-14 00:54:52.319936 summerepi2-1.3.6/summer2/flows.py
+-rw-r--r--   0        0        0      209 2023-07-31 01:18:46.918141 summerepi2-1.3.6/summer2/functions/__init__.py
+-rw-r--r--   0        0        0     2350 2023-08-14 02:57:47.751138 summerepi2-1.3.6/summer2/functions/derived.py
+-rw-r--r--   0        0        0     4481 2024-04-23 00:28:13.386989 summerepi2-1.3.6/summer2/functions/interpolate.py
+-rw-r--r--   0        0        0     4620 2023-01-17 01:08:37.545738 summerepi2-1.3.6/summer2/functions/interpolate_old.py
+-rw-r--r--   0        0        0     4106 2023-07-18 01:31:47.511898 summerepi2-1.3.6/summer2/functions/time.py
+-rw-r--r--   0        0        0     4033 2023-11-14 00:54:52.321434 summerepi2-1.3.6/summer2/functions/util.py
+-rw-r--r--   0        0        0     8195 2023-11-14 00:54:52.322435 summerepi2-1.3.6/summer2/inspect.py
+-rw-r--r--   0        0        0    55654 2024-04-23 01:05:26.061935 summerepi2-1.3.6/summer2/model.py
+-rw-r--r--   0        0        0       22 2022-10-11 01:49:59.803947 summerepi2-1.3.6/summer2/parameters/__init__.py
+-rw-r--r--   0        0        0    11253 2023-09-27 22:59:53.735298 summerepi2-1.3.6/summer2/parameters/param_impl.py
+-rw-r--r--   0        0        0     4255 2023-04-05 00:33:04.747809 summerepi2-1.3.6/summer2/parameters/params.py
+-rw-r--r--   0        0        0     1642 2023-09-05 02:52:23.354619 summerepi2-1.3.6/summer2/parameters/support.py
+-rw-r--r--   0        0        0     4804 2022-09-01 05:32:07.974766 summerepi2-1.3.6/summer2/population.py
+-rw-r--r--   0        0        0       40 2022-09-01 05:32:07.975265 summerepi2-1.3.6/summer2/runner/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-01 05:32:07.975767 summerepi2-1.3.6/summer2/runner/jax/__init__.py
+-rw-r--r--   0        0        0     5240 2023-05-02 00:15:48.813286 summerepi2-1.3.6/summer2/runner/jax/derived_outputs.py
+-rw-r--r--   0        0        0    28228 2024-04-23 00:28:13.388989 summerepi2-1.3.6/summer2/runner/jax/model_impl.py
+-rw-r--r--   0        0        0    11659 2024-02-12 22:04:51.906575 summerepi2-1.3.6/summer2/runner/jax/ode.py
+-rw-r--r--   0        0        0    11222 2022-10-12 17:29:54.983503 summerepi2-1.3.6/summer2/runner/jax/ode2.py
+-rw-r--r--   0        0        0     2736 2022-11-30 22:02:39.159369 summerepi2-1.3.6/summer2/runner/jax/solvers.py
+-rw-r--r--   0        0        0     5369 2023-09-27 22:25:22.310714 summerepi2-1.3.6/summer2/runner/jax/stratify.py
+-rw-r--r--   0        0        0     8170 2022-12-02 02:13:10.114800 summerepi2-1.3.6/summer2/runner/model_runner.py
+-rw-r--r--   0        0        0     6277 2022-10-11 01:50:00.034457 summerepi2-1.3.6/summer2/solver.py
+-rw-r--r--   0        0        0    17065 2023-04-18 23:09:58.702374 summerepi2-1.3.6/summer2/stratification.py
+-rw-r--r--   0        0        0      472 2022-09-01 05:32:08.049501 summerepi2-1.3.6/summer2/tracker.py
+-rw-r--r--   0        0        0     3760 2023-05-11 02:02:50.793367 summerepi2-1.3.6/summer2/utils.py
+-rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 summerepi2-1.3.6/PKG-INFO
```

### Comparing `summerepi2-1.3.5/LICENSE.txt` & `summerepi2-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/pyproject.toml` & `summerepi2-1.3.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "summerepi2"
-version = "1.3.5"
+version = "1.3.6"
 readme = "README.md"
 license = "BSD-2-Clause"
-homepage = "http://summerepi.com/"
-documentation = "http://summerepi.com/"
+homepage = "https://github.com/monash-emu/summer2"
+documentation = "https://summer2.readthedocs.io/en/latest/"
 repository = "https://github.com/monash-emu/summer2"
 keywords = [
     "epidemiology",
     "disease",
     "compartmental",
     "infectious",
 ]
@@ -20,17 +20,17 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10.0"
 numpy = ">=1.20.3"
 networkx = ">=2.6.2"
 pandas = ">=1.3.2"
 plotly = ">=5.5.0"
-computegraph = "==0.4.4"
-jax = "==0.4.24"
-jaxlib = "==0.4.24"
+computegraph = "==0.4.5"
+jax = ">=0.4.24"
+jaxlib = ">=0.4.24"
 
 sphinx-rtd-theme = {version = "^0.5.1", optional = true}
 recommonmark = {version = "^0.7.1", optional = true}
 nbsphinx = {version = "^0.8.2", optional = true}
 sphinxcontrib-napoleon = {version = "^0.7", optional = true}
 ipykernel  = {version = "^6.15.1", optional = true}
 matplotlib = {version = ">=3.4.3", optional = true}
```

### Comparing `summerepi2-1.3.5/README.md` & `summerepi2-1.3.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: summerepi2
+Version: 1.3.6
+Summary: Summer is a compartmental disease modelling framework, written in Python. It provides a high-level API to build and run models.
+Home-page: https://github.com/monash-emu/summer2
+License: BSD-2-Clause
+Keywords: epidemiology,disease,compartmental,infectious
+Author: David Shipman
+Author-email: dshipman@gmail.com
+Requires-Python: >=3.10.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: docs
+Requires-Dist: computegraph (==0.4.5)
+Requires-Dist: ipykernel (>=6.15.1,<7.0.0) ; extra == "docs"
+Requires-Dist: jax (>=0.4.24)
+Requires-Dist: jaxlib (>=0.4.24)
+Requires-Dist: matplotlib (>=3.4.3) ; extra == "docs"
+Requires-Dist: nbsphinx (>=0.8.2,<0.9.0) ; extra == "docs"
+Requires-Dist: networkx (>=2.6.2)
+Requires-Dist: numpy (>=1.20.3)
+Requires-Dist: pandas (>=1.3.2)
+Requires-Dist: plotly (>=5.5.0)
+Requires-Dist: pygraphviz (>=1.10,<2.0) ; extra == "docs"
+Requires-Dist: recommonmark (>=0.7.1,<0.8.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=0.5.1,<0.6.0) ; extra == "docs"
+Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8) ; extra == "docs"
+Project-URL: Documentation, https://summer2.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/monash-emu/summer2
+Description-Content-Type: text/markdown
+
 # summer2: compartmental disease modelling in Python
 
 [![Automated Tests](https://github.com/monash-emu/summer2/actions/workflows/tests.yml/badge.svg)](https://github.com/monash-emu/summer2/actions/workflows/tests.yml)
 
 summer2 is a Python-based framework for the creation and execution of [compartmental](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology) (or "state-based") epidemiological models of infectious disease transmission.
 
 It provides a range of structures for easily implementing compartmental models, including structure for some of the most common features added to basic compartmental frameworks, including:
@@ -18,33 +51,23 @@
 Some helpful links to learn more:
 
 - **[Documentation](https://summer2.readthedocs.io/)** with [code examples](https://summer2.readthedocs.io/en/latest/examples/index.html)
 - [Available on PyPi](https://pypi.org/project/summerepi2/) as `summerepi2`.
 
 ## Installation and Quickstart
 
-This project requires at least Python 3.8
+This project requires at least Python 3.10
 
 Set up and activate an appropriate virtual environment, then install the `summerepi2` package from PyPI
 
 ```bash
 pip install summerepi2
 ```
 
-Important note for Windows users:
-summerepi2 relies on the Jax framework for fast retargetable computing.  This is automatically
-installed under Linux, OSX, and WSL environments. 
-It is strongly recommended that you use WSL, but in instances were you are unable to do so,
-an unofficial build of jax can be installed by running the following command
-
-```bash
-pip install jax[cpu]==0.3.24 -f https://whls.blob.core.windows.net/unstable/index.html
-```
-
-Then you can now use the library to build and run models. See [here](https://summer2.readthedocs.io/en/latest/examples/index.html) for some code examples.
+You can now use the library to build and run models. See [here](https://summer2.readthedocs.io/en/latest/examples/index.html) for some code examples.
 
 ## Optional (recommended) extras
 
 Summer has advanced interactive plotting tools built in - but they are greatly improved with the
 addition of the pygraphviz library.
 
 If you are using conda, the simplest method of installation is as follows:
@@ -56,39 +79,14 @@
 For other install methods, see
 https://pygraphviz.github.io/documentation/stable/install.html
 
 ## Development
 
 [Poetry](https://python-poetry.org/) is used for packaging and dependency management.
 
-Initial project setup is documented [here](./docs/dev-setup.md) and should work for Windows or Ubuntu, maybe for MacOS.
-
-Some common things to do as a developer working on this codebase:
-
-```bash
-# Activate summer conda environment prior to doing other stuff (see setup docs)
-conda activate summer
-
-# Install latest requirements
-poetry install
-
-# Publish to PyPI - use your PyPI credentials
-poetry publish --build
-
-# Add a new package
-poetry add
-
-# Run tests
-pytest -vv
-
-# Format Python code
-black .
-isort . --profile black
-```
-
 ## Releases
 
 Releases are numbered using [Semantic Versioning](https://semver.org/)
 
 - 1.0.0/1:
   - Initial release
 - 1.2.1
@@ -115,23 +113,7 @@
 - 1.3.3
   - Fix issue with binary search for piecewise functions
 - 1.3.4
   - Update import in ode.py for changed jax API
 - 1.3.5
   - Force specific jax (0.4.24) to stop breaking changes
 
-## Release process
-
-To do a release:
-
-- Commit any code changes and push them to GitHub
-- Choose a new release number accoridng to [Semantic Versioning](https://semver.org/)
-- Add a release note above
-- Edit the `version` key in `pyproject.toml` to reflect the release number
-- Publish the package to [PyPI](https://pypi.org/project/summerepi/) using Poetry, you will need a PyPI login and access to the project
-- Commit the release changes and push them to GitHub (Use a commit message like "Release 1.1.0")
-- Update `requirements.txt` in Autumn to use the new version of Summer
-
-```bash
-poetry build
-poetry publish
-```
```

### Comparing `summerepi2-1.3.5/summer2/adjust.py` & `summerepi2-1.3.6/summer2/adjust.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/compartment.py` & `summerepi2-1.3.6/summer2/compartment.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/derived_outputs.py` & `summerepi2-1.3.6/summer2/derived_outputs.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/experimental/model_builder.py` & `summerepi2-1.3.6/summer2/experimental/model_builder.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/extras/test_models.py` & `summerepi2-1.3.6/summer2/extras/test_models.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/flows.py` & `summerepi2-1.3.6/summer2/flows.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/functions/derived.py` & `summerepi2-1.3.6/summer2/functions/derived.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""
-Functions operating over arrays
-
-These are designed for use on derived outputs; ie it is expected that data
-will be a time series whose length is equal to model.times, and that these
-functions will operate over the whole array, and return an array of the same
-shape as the input
-
-Where possible, these functions will mimic (or at least be similar to) their
-pandas.Series counterparts
-
-"""
-
-from typing import Callable
-
-from jax import numpy as jnp
-from jax import Array
-
-
-def get_rolling_diff(periods: int = 1) -> Callable[[Array], Array]:
-    """Build a function that returns the difference of each value at index i,
-    to the value at index i-periods ala pandas.Series.diff
-
-    Args:
-        periods: The index distance to diff
-
-    Returns:
-        A function over a 1d array that returns an array of the same shape,
-        whose values are the diffs
-    """
-
-    def rolling_diff(x):
-        out_arr = jnp.empty_like(x)
-        out_arr = out_arr.at[periods:].set(x[periods:] - x[:-periods])
-        out_arr = out_arr.at[:periods].set(jnp.nan)
-        return out_arr
-
-    return rolling_diff
-
-
-def _rolling_index(a: jnp.ndarray, window: int):
-    idx = jnp.arange(len(a) - window + 1)[:, None] + jnp.arange(window)[None, :]
-    return a[idx]
-
-
-def get_rolling_reduction(func: callable, window: int) -> Callable[[Array], Array]:
-    """Build a function that comptues a reduction function 'func' over each
-    rolling window of length 'window'
-
-    Reduction functions are those that take an array as input and return a scalar,
-    (or in general reduce array axes to scalar values), such as jnp.mean, jnp.max etc
-
-    This is designed to operate like pandas.Series.rolling (with its default
-    window parameters)
-
-    Args:
-        func: The reduction function to call; must be jax jittable
-        window: The window length
-
-    Returns:
-        A function over a 1d array that returns an array of the same shape, but with
-        the rolling reduction applied
-
-    """
-
-    def rolling_func(x):
-        out_arr = jnp.empty_like(x)
-        windowed = _rolling_index(x, window)
-        agg = func(windowed, axis=1)
-        out_arr = out_arr.at[:window].set(jnp.nan)
-        out_arr = out_arr.at[window - 1 :].set(agg)
-        return out_arr
-
-    return rolling_func
+"""
+Functions operating over arrays
+
+These are designed for use on derived outputs; ie it is expected that data
+will be a time series whose length is equal to model.times, and that these
+functions will operate over the whole array, and return an array of the same
+shape as the input
+
+Where possible, these functions will mimic (or at least be similar to) their
+pandas.Series counterparts
+
+"""
+
+from typing import Callable
+
+from jax import numpy as jnp
+from jax import Array
+
+
+def get_rolling_diff(periods: int = 1) -> Callable[[Array], Array]:
+    """Build a function that returns the difference of each value at index i,
+    to the value at index i-periods ala pandas.Series.diff
+
+    Args:
+        periods: The index distance to diff
+
+    Returns:
+        A function over a 1d array that returns an array of the same shape,
+        whose values are the diffs
+    """
+
+    def rolling_diff(x):
+        out_arr = jnp.empty_like(x)
+        out_arr = out_arr.at[periods:].set(x[periods:] - x[:-periods])
+        out_arr = out_arr.at[:periods].set(jnp.nan)
+        return out_arr
+
+    return rolling_diff
+
+
+def _rolling_index(a: jnp.ndarray, window: int):
+    idx = jnp.arange(len(a) - window + 1)[:, None] + jnp.arange(window)[None, :]
+    return a[idx]
+
+
+def get_rolling_reduction(func: callable, window: int) -> Callable[[Array], Array]:
+    """Build a function that comptues a reduction function 'func' over each
+    rolling window of length 'window'
+
+    Reduction functions are those that take an array as input and return a scalar,
+    (or in general reduce array axes to scalar values), such as jnp.mean, jnp.max etc
+
+    This is designed to operate like pandas.Series.rolling (with its default
+    window parameters)
+
+    Args:
+        func: The reduction function to call; must be jax jittable
+        window: The window length
+
+    Returns:
+        A function over a 1d array that returns an array of the same shape, but with
+        the rolling reduction applied
+
+    """
+
+    def rolling_func(x):
+        out_arr = jnp.empty_like(x)
+        windowed = _rolling_index(x, window)
+        agg = func(windowed, axis=1)
+        out_arr = out_arr.at[:window].set(jnp.nan)
+        out_arr = out_arr.at[window - 1 :].set(agg)
+        return out_arr
+
+    return rolling_func
```

### Comparing `summerepi2-1.3.5/summer2/functions/interpolate.py` & `summerepi2-1.3.6/summer2/functions/interpolate.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/functions/time.py` & `summerepi2-1.3.6/summer2/functions/time.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/functions/util.py` & `summerepi2-1.3.6/summer2/functions/util.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/inspect.py` & `summerepi2-1.3.6/summer2/inspect.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/model.py` & `summerepi2-1.3.6/summer2/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module contains the main disease modelling class.
 """
+
 import copy
 import logging
 from datetime import datetime
 from collections import OrderedDict
 from typing import Callable, Dict, List, Optional, Tuple, Union
 from warnings import warn
 import itertools
@@ -198,14 +199,15 @@
         """Set the initial population with a graphobject (Function, Data or array)
         The output of this object must be an array matching the model's final compartments,
         and therefore no further stratification is possible after this function is called
 
         Args:
             init_pop: GraphObject or array type
         """
+        self._assert_not_finalized()
         self._init_pop_dist = {}
         self._array_population = init_pop
 
     def set_initial_population(self, distribution: Dict[str, float], force=False):
         """
         Sets the initial population of the model, which is zero by default.
         Use this method before strafication to determine population by stratification
```

### Comparing `summerepi2-1.3.5/summer2/parameters/param_impl.py` & `summerepi2-1.3.6/summer2/parameters/param_impl.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/parameters/params.py` & `summerepi2-1.3.6/summer2/parameters/params.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/population.py` & `summerepi2-1.3.6/summer2/population.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/runner/jax/derived_outputs.py` & `summerepi2-1.3.6/summer2/runner/jax/derived_outputs.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/runner/jax/model_impl.py` & `summerepi2-1.3.6/summer2/runner/jax/model_impl.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/runner/jax/ode.py` & `summerepi2-1.3.6/summer2/runner/jax/ode.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/runner/jax/solvers.py` & `summerepi2-1.3.6/summer2/runner/jax/solvers.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/runner/jax/stratify.py` & `summerepi2-1.3.6/summer2/runner/jax/stratify.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/runner/model_runner.py` & `summerepi2-1.3.6/summer2/runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/solver.py` & `summerepi2-1.3.6/summer2/solver.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/stratification.py` & `summerepi2-1.3.6/summer2/stratification.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.3.5/summer2/utils.py` & `summerepi2-1.3.6/summer2/utils.py`

 * *Files identical despite different names*

