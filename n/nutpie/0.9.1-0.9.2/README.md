# Comparing `tmp/nutpie-0.9.1.tar.gz` & `tmp/nutpie-0.9.2.tar.gz`

## Comparing `nutpie-0.9.1.tar` & `nutpie-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 nutpie-0.9.1/Cargo.toml
--rw-r--r--   0     1001      127     4882 2023-09-14 09:44:07.000000 nutpie-0.9.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      152 2023-09-14 09:44:07.000000 nutpie-0.9.1/.gitignore
--rw-r--r--   0     1001      127     1058 2023-09-14 09:44:07.000000 nutpie-0.9.1/CHANGELOG.md
--rw-r--r--   0     1001      127     1072 2023-09-14 09:44:07.000000 nutpie-0.9.1/LICENSE
--rw-r--r--   0     1001      127     3583 2023-09-14 09:44:07.000000 nutpie-0.9.1/README.md
--rw-r--r--   0     1001      127     5212 2023-09-14 09:44:07.000000 nutpie-0.9.1/benches/run_tvm_leapfrog.rs_old
--rw-r--r--   0     1001      127     2654 2023-09-14 09:44:07.000000 nutpie-0.9.1/cliff.toml
--rw-r--r--   0     1001      127       10 2023-09-14 09:44:18.000000 nutpie-0.9.1/dist/nutpie-0.9.1.tar.gz
--rw-r--r--   0     1001      127   251122 2023-09-14 09:44:07.000000 nutpie-0.9.1/notebooks/pytensor_logp.ipynb
--rw-r--r--   0     1001      127     7329 2023-09-14 09:44:07.000000 nutpie-0.9.1/notebooks/pytensor_logp.md
--rw-r--r--   0     1001      127      914 2023-09-14 09:44:07.000000 nutpie-0.9.1/pyproject.toml
--rw-r--r--   0     1001      127      567 2023-09-14 09:44:07.000000 nutpie-0.9.1/python/nutpie/__init__.py
--rw-r--r--   0     1001      127    15227 2023-09-14 09:44:07.000000 nutpie-0.9.1/python/nutpie/compile_pymc.py
--rw-r--r--   0     1001      127     4761 2023-09-14 09:44:07.000000 nutpie-0.9.1/python/nutpie/compile_stan.py
--rw-r--r--   0     1001      127     8687 2023-09-14 09:44:07.000000 nutpie-0.9.1/python/nutpie/sample.py
--rw-r--r--   0     1001      127       70 2023-09-14 09:44:07.000000 nutpie-0.9.1/src/lib.rs
--rw-r--r--   0     1001      127     7955 2023-09-14 09:44:07.000000 nutpie-0.9.1/src/pymc.rs
--rw-r--r--   0     1001      127     7127 2023-09-14 09:44:07.000000 nutpie-0.9.1/src/sampler.rs
--rw-r--r--   0     1001      127    13457 2023-09-14 09:44:07.000000 nutpie-0.9.1/src/stan.rs
--rw-r--r--   0     1001      127     8528 2023-09-14 09:44:07.000000 nutpie-0.9.1/src/wrapper.rs
--rw-r--r--   0     1001      127     1521 2023-09-14 09:44:07.000000 nutpie-0.9.1/tests/test_pymc.py
--rw-r--r--   0     1001      127      721 2023-09-14 09:44:07.000000 nutpie-0.9.1/tests/test_stan.py
--rw-r--r--   0     1001      127    34943 2023-09-14 09:44:07.000000 nutpie-0.9.1/Cargo.lock
--rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 nutpie-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 nutpie-0.9.2/Cargo.toml
+-rw-r--r--   0     1001      127      224 2024-02-19 19:13:09.000000 nutpie-0.9.2/.github/dependabot.yml
+-rw-r--r--   0     1001      127     5136 2024-02-19 19:13:09.000000 nutpie-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      152 2024-02-19 19:13:09.000000 nutpie-0.9.2/.gitignore
+-rw-r--r--   0     1001      127     1058 2024-02-19 19:13:09.000000 nutpie-0.9.2/CHANGELOG.md
+-rw-r--r--   0     1001      127     1072 2024-02-19 19:13:09.000000 nutpie-0.9.2/LICENSE
+-rw-r--r--   0     1001      127     3659 2024-02-19 19:13:09.000000 nutpie-0.9.2/README.md
+-rw-r--r--   0     1001      127     5212 2024-02-19 19:13:09.000000 nutpie-0.9.2/benches/run_tvm_leapfrog.rs_old
+-rw-r--r--   0     1001      127     2654 2024-02-19 19:13:09.000000 nutpie-0.9.2/cliff.toml
+-rw-r--r--   0     1001      127   251122 2024-02-19 19:13:09.000000 nutpie-0.9.2/notebooks/pytensor_logp.ipynb
+-rw-r--r--   0     1001      127     7329 2024-02-19 19:13:09.000000 nutpie-0.9.2/notebooks/pytensor_logp.md
+-rw-r--r--   0     1001      127      265 2024-02-19 19:13:09.000000 nutpie-0.9.2/python/nutpie/__init__.py
+-rw-r--r--   0     1001      127    16263 2024-02-19 19:13:09.000000 nutpie-0.9.2/python/nutpie/compile_pymc.py
+-rw-r--r--   0     1001      127     5040 2024-02-19 19:13:09.000000 nutpie-0.9.2/python/nutpie/compile_stan.py
+-rw-r--r--   0     1001      127     8687 2024-02-19 19:13:09.000000 nutpie-0.9.2/python/nutpie/sample.py
+-rw-r--r--   0     1001      127       70 2024-02-19 19:13:09.000000 nutpie-0.9.2/src/lib.rs
+-rw-r--r--   0     1001      127     7955 2024-02-19 19:13:09.000000 nutpie-0.9.2/src/pymc.rs
+-rw-r--r--   0     1001      127     7127 2024-02-19 19:13:09.000000 nutpie-0.9.2/src/sampler.rs
+-rw-r--r--   0     1001      127    13457 2024-02-19 19:13:09.000000 nutpie-0.9.2/src/stan.rs
+-rw-r--r--   0     1001      127     8528 2024-02-19 19:13:09.000000 nutpie-0.9.2/src/wrapper.rs
+-rw-r--r--   0     1001      127     1769 2024-02-19 19:13:09.000000 nutpie-0.9.2/tests/test_pymc.py
+-rw-r--r--   0     1001      127      721 2024-02-19 19:13:09.000000 nutpie-0.9.2/tests/test_stan.py
+-rw-r--r--   0     1001      127    34943 2024-02-19 19:13:09.000000 nutpie-0.9.2/Cargo.lock
+-rw-r--r--   0     1001      127      914 2024-02-19 19:13:09.000000 nutpie-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4797 1970-01-01 00:00:00.000000 nutpie-0.9.2/PKG-INFO
```

### Comparing `nutpie-0.9.1/Cargo.toml` & `nutpie-0.9.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nutpie"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
     "Adrian Seyboldt <adrian.seyboldt@gmail.com>",
     "PyMC Developers <pymc.devs@gmail.com>"
 ]
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/pymc-devs/nutpie"
```

### Comparing `nutpie-0.9.1/.github/workflows/ci.yml` & `nutpie-0.9.2/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -33,29 +33,30 @@
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
-          sccache: 'true'
           manylinux: 2_28
           before-script-linux: |
             dnf install -y clang-libs clang || apt install llvm-dev libclang-dev clang
+
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
       - name: pytest
         if: ${{ startsWith(matrix.target, 'x86_64') }}
         shell: bash
         run: |
           set -e
-          pip install 'nutpie[all]' --find-links dist --force-reinstall
+          pip install --find-links dist --force-reinstall 'nutpie[all]'
+          pip install --find-links dist --force-reinstall --no-deps --no-index 'nutpie[all]'
           pip install pytest
           pytest
       - name: pytest
         if: ${{ !startsWith(matrix.target, 'x86') && matrix.target != 'ppc64' }}
         uses: uraimo/run-on-arch-action@v2.5.0
         with:
           arch: ${{ matrix.target }}
@@ -106,14 +107,15 @@
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.target, 'aarch64') }}
         shell: bash
         run: |
           set -e
           pip install "nutpie[all]" --find-links dist --force-reinstall
+          pip install --find-links dist --force-reinstall --no-deps --no-index 'nutpie[all]'
           pip install pytest
           pytest
 
   macos:
     runs-on: macos-latest
     strategy:
       fail-fast: false
@@ -140,14 +142,15 @@
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.target, 'aarch64') }}
         shell: bash
         run: |
           set -e
           pip install 'nutpie[all]' --find-links dist --force-reinstall
+          pip install --find-links dist --force-reinstall --no-deps --no-index 'nutpie[all]'
           pip install pytest
           pytest
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
```

### Comparing `nutpie-0.9.1/CHANGELOG.md` & `nutpie-0.9.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/LICENSE` & `nutpie-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/README.md` & `nutpie-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# nutpie: A fast sampler for bayesian posteriors
+# nutpie: A fast sampler for Bayesian posteriors
 
 ## Installation
 
-nutpie can be installed using conda or mamba from conda-forge with
+nutpie can be installed using Conda or Mamba from conda-forge with
 
-```
-mamba install -c conda-forge nutpie pymc
+```bash
+mamba install -c conda-forge nutpie
 ```
 
 Or using pip:
 
-```
+```bash
 pip install nutpie
 ```
 
-To install it from source, install a rust compiler and maturin and then
+To install it from source, install a Rust compiler and maturin and then
 
-```
+```bash
 maturin develop --release
 ```
 
-If you want to use the nightly simd implementation for some of the math functions,
-switch to rust nightly and then install with the `simd_support` feature in then
+If you want to use the nightly SIMD implementation for some of the math functions,
+switch to Rust nightly and then install with the `simd_support` feature in then
 nutpie directory:
 
-```
+```bash
 rustup override set nightly
 maturin develop --release --features=simd_support
 ```
 
 ## Usage with PyMC
 
-First, PyMC and numba need to be installed, for example using
+First, PyMC and Numba need to be installed, for example using
 
-```
-mamba install pymc numba
+```bash
+mamba install -c conda-forge pymc numba
 ```
 
 We need to create a model:
 
 ```python
 import pymc as pm
 import numpy as np
@@ -87,39 +87,39 @@
 We then compile this model and sample form the posterior:
 
 ```python
 compiled_model = nutpie.compile_pymc_model(pymc_model)
 trace_pymc = nutpie.sample(compiled_model)
 ```
 
-`trace_pymc` now contains an arviz `InferenceData` object, including sampling
+`trace_pymc` now contains an ArviZ `InferenceData` object, including sampling
 statistics and the posterior of the variables defined above.
 
 ## Usage with Stan
 
-In order to sample from stan model, `bridgestan` needs to be installed.
-A pip package is available, but right now this can not be installed using conda.
+In order to sample from Stan model, `bridgestan` needs to be installed.
+A pip package is available, but right now this can not be installed using Conda.
 
-```
+```bash
 pip install bridgestan
 ```
 
 When we install nutpie with pip, we can also specify that we want optional
 dependencies for Stan models using
 
 ```
-pip install 'bridgestan[stan]'
+pip install 'nutpie[stan]'
 ```
 
 In addition, a C++ compiler needs to be available. For details see
-[the stan docs](https://mc-stan.org/docs/cmdstan-guide/cmdstan-installation.html#cpp-toolchain).
+[the Stan docs](https://mc-stan.org/docs/cmdstan-guide/cmdstan-installation.html#cpp-toolchain).
 
 We can then compile a Stan model, and sample using nutpie:
 
-```
+```python
 import nutpie
 
 code = """
 data {
     real mu;
 }
 parameters {
@@ -134,11 +134,11 @@
 # Provide data
 compiled = compiled.with_data(mu=3.)
 trace = nutpie.sample(compiled)
 ```
 
 ## Advantages
 
-nutpie uses `nuts-rs`, a library written in rust, that implements NUTS as in
-pymc and stan, but with a slightly different mass matrix tuning method as
+nutpie uses [`nuts-rs`](https://github.com/pymc-devs/nuts-rs), a library written in Rust, that implements NUTS as in
+PyMC and Stan, but with a slightly different mass matrix tuning method as
 those. It often produces a higher effective sample size per gradient
 evaluation, and tends to converge faster and with fewer gradient evaluation.
```

### Comparing `nutpie-0.9.1/benches/run_tvm_leapfrog.rs_old` & `nutpie-0.9.2/benches/run_tvm_leapfrog.rs_old`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/cliff.toml` & `nutpie-0.9.2/cliff.toml`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/notebooks/pytensor_logp.ipynb` & `nutpie-0.9.2/notebooks/pytensor_logp.ipynb`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/notebooks/pytensor_logp.md` & `nutpie-0.9.2/notebooks/pytensor_logp.md`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/pyproject.toml` & `nutpie-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/python/nutpie/compile_pymc.py` & `nutpie-0.9.2/python/nutpie/compile_pymc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import dataclasses
 import itertools
 from dataclasses import dataclass
+from importlib.util import find_spec
 from math import prod
-from typing import Any, Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple
 
-import numba
-import numba.core.ccallback
 import numpy as np
 import pandas as pd
-import pymc as pm
-import pytensor
-import pytensor.link.numba.dispatch
-import pytensor.tensor as pt
-from numba import literal_unroll
-from numba.cpython.unsafe.tuple import alloca_once, tuple_setitem
 from numpy.typing import NDArray
-from pymc.initial_point import make_initial_point_fn
 
 from nutpie import _lib
 from nutpie.sample import CompiledModel
 
+try:
+    from numba.extending import intrinsic
+except ImportError:
 
-@numba.extending.intrinsic
+    def intrinsic(f):
+        return f
+
+
+if TYPE_CHECKING:
+    import numba.core.ccallback
+    import pymc as pm
+
+
+@intrinsic
 def address_as_void_pointer(typingctx, src):
     """returns a void pointer from a given memory address"""
     from numba.core import cgutils, types
 
     sig = types.voidptr(src)
 
     def codegen(cgctx, builder, sig, args):
         return builder.inttoptr(args[0], cgutils.voidptr_t)
 
     return sig, codegen
 
 
 @dataclass(frozen=True)
 class CompiledPyMCModel(CompiledModel):
-    compiled_logp_func: numba.core.ccallback.CFunc
-    compiled_expand_func: numba.core.ccallback.CFunc
+    compiled_logp_func: "numba.core.ccallback.CFunc"
+    compiled_expand_func: "numba.core.ccallback.CFunc"
     shared_data: Dict[str, NDArray]
     user_data: NDArray
     n_expanded: int
     shape_info: Any
     logp_func: Any
     expand_func: Any
     _n_dim: int
@@ -140,28 +144,43 @@
         ],
     )
     user_data = np.zeros((), dtype=record_dtype)
     update_user_data(user_data, shared_data)
     return user_data
 
 
-def compile_pymc_model(model: pm.Model, **kwargs) -> CompiledPyMCModel:
+def compile_pymc_model(model: "pm.Model", **kwargs) -> CompiledPyMCModel:
     """Compile necessary functions for sampling a pymc model.
 
     Parameters
     ----------
     model : pymc.Model
         The model to compile.
 
     Returns
     -------
     compiled_model : CompiledPyMCModel
         A compiled model object.
 
     """
+    if find_spec("pymc") is None:
+        raise ImportError(
+            "PyMC is not installed in the current environment. "
+            "Please install it with something like "
+            "'mamba install -c conda-forge pymc numba' "
+            "and restart your kernel in case you are in an interactive session."
+        )
+    if find_spec("numba") is None:
+        raise ImportError(
+            "Numba is not installed in the current environment. "
+            "Please install it with something like "
+            "'mamba install -c conda-forge numba' "
+            "and restart your kernel in case you are in an interactive session."
+        )
+    import numba
 
     (
         n_dim,
         n_expanded,
         logp_fn_pt,
         logp_fn,
         expand_fn_pt,
@@ -184,15 +203,20 @@
     logp_numba = numba.cfunc(c_sig, **kwargs)(logp_numba_raw)
 
     expand_numba_raw, c_sig_expand = _make_c_expand_func(
         n_dim, n_expanded, expand_fn, user_data, shared_expand, shared_data
     )
     expand_numba = numba.cfunc(c_sig_expand, **kwargs)(expand_numba_raw)
 
-    coords = {name: pd.Index(vals) for name, vals in model.coords.items()}
+    coords = {}
+    for name, vals in model.coords.items():
+        if vals is None:
+            vals = pd.RangeIndex(int(model.dim_lengths[name].eval()))
+        coords[name] = pd.Index(vals)
+
     if "unconstrained_parameter" in coords:
         raise ValueError("Model contains invalid name 'unconstrained_parameter'.")
 
     names = []
     for base, _, shape in zip(*shape_info):
         if base not in [var.name for var in model.value_vars]:
             continue
@@ -216,14 +240,17 @@
         shape_info=shape_info,
         logp_func=logp_fn_pt,
         expand_func=expand_fn_pt,
     )
 
 
 def _compute_shapes(model):
+    import pytensor
+    from pymc.initial_point import make_initial_point_fn
+
     point = make_initial_point_fn(model=model, return_transformed=True)(0)
 
     trace_vars = {
         var.name: var
         for var in model.value_vars + model.free_RVs + model.deterministics
         if var not in model.observed_RVs + model.potentials
     }
@@ -242,14 +269,18 @@
         mode=pytensor.compile.mode.FAST_COMPILE,
         on_unused_input="ignore",
     )
     return {name: shape for name, shape in zip(trace_vars.keys(), shape_func())}
 
 
 def _make_functions(model):
+    import pytensor
+    import pytensor.link.numba.dispatch
+    import pytensor.tensor as pt
+
     shapes = _compute_shapes(model)
 
     # Make logp_dlogp_function
     joined = pt.dvector("__joined_variables")
 
     value_vars = [model.rvs_to_values[var] for var in model.free_RVs]
 
@@ -354,14 +385,18 @@
         expand_fn,
         [var.name for var in expand_fn_pt.get_shared()],
         (all_names, all_slices, all_shapes),
     )
 
 
 def make_extraction_fn(inner, shared_data, shared_vars, record_dtype):
+    import numba
+    from numba import literal_unroll
+    from numba.cpython.unsafe.tuple import alloca_once, tuple_setitem
+
     if not shared_vars:
 
         @numba.njit(inline="always")
         def extract_shared(x, user_data_):
             return inner(x)
 
         return extract_shared
@@ -376,15 +411,15 @@
         for name in shared_vars
     )
 
     names = shared_vars
     indices = tuple(range(len(names)))
     shared_tuple = tuple(shared_data[name] for name in shared_vars)
 
-    @numba.extending.intrinsic
+    @intrinsic
     def tuple_setitem_literal(typingctx, tup, idx, val):
         """Return a copy of the tuple with item at *idx* replaced with *val*."""
         if not isinstance(idx, numba.types.IntegerLiteral):
             return
 
         idx_val = idx.literal_value
         assert idx_val >= 0
@@ -447,14 +482,16 @@
 
         return inner(x, *_shared_tuple)
 
     return extract_shared
 
 
 def _make_c_logp_func(n_dim, logp_fn, user_data, shared_logp, shared_data):
+    import numba
+
     extract = make_extraction_fn(logp_fn, shared_data, shared_logp, user_data.dtype)
 
     c_sig = numba.types.int64(
         numba.types.uint64,
         numba.types.CPointer(numba.types.double),
         numba.types.CPointer(numba.types.double),
         numba.types.CPointer(numba.types.double),
@@ -486,14 +523,16 @@
 
     return logp_numba, c_sig
 
 
 def _make_c_expand_func(
     n_dim, n_expanded, expand_fn, user_data, shared_vars, shared_data
 ):
+    import numba
+
     extract = make_extraction_fn(expand_fn, shared_data, shared_vars, user_data.dtype)
 
     c_sig = numba.types.int64(
         numba.types.uint64,
         numba.types.uint64,
         numba.types.CPointer(numba.types.double),
         numba.types.CPointer(numba.types.double),
```

### Comparing `nutpie-0.9.1/python/nutpie/compile_stan.py` & `nutpie-0.9.2/python/nutpie/compile_stan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import pathlib
 import tempfile
 from dataclasses import dataclass, replace
+from importlib.util import find_spec
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
 
 from nutpie import _lib
@@ -109,14 +110,21 @@
     extra_compile_args: Optional[List[str]] = None,
     extra_stanc_args: Optional[List[str]] = None,
     dims: Optional[Dict[str, int]] = None,
     coords: Optional[Dict[str, Any]] = None,
     model_name: Optional[str] = None,
     cleanup: bool = True,
 ) -> CompiledStanModel:
+    if find_spec("bridgestan") is None:
+        raise ImportError(
+            "BridgeStan is not installed in the current environment. "
+            "Please install it with something like "
+            "'pip install bridgestan'."
+        )
+
     import bridgestan
 
     if dims is None:
         dims = {}
     if coords is None:
         coords = {}
```

### Comparing `nutpie-0.9.1/python/nutpie/sample.py` & `nutpie-0.9.2/python/nutpie/sample.py`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/src/pymc.rs` & `nutpie-0.9.2/src/pymc.rs`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/src/sampler.rs` & `nutpie-0.9.2/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/src/stan.rs` & `nutpie-0.9.2/src/stan.rs`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/src/wrapper.rs` & `nutpie-0.9.2/src/wrapper.rs`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/tests/test_pymc.py` & `nutpie-0.9.2/tests/test_pymc.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,24 @@
         pm.Normal("a")
 
     compiled = nutpie.compile_pymc_model(model)
     trace = nutpie.sample(compiled, chains=1)
     trace.posterior.a
 
 
+def test_pymc_model():
+    with pm.Model() as model:
+        model.add_coord("foo", length=5)
+        pm.Normal("a", dims="foo")
+
+    compiled = nutpie.compile_pymc_model(model)
+    trace = nutpie.sample(compiled, chains=1)
+    trace.posterior.a
+
+
 def test_trafo():
     with pm.Model() as model:
         pm.Uniform("a")
 
     compiled = nutpie.compile_pymc_model(model)
     trace = nutpie.sample(compiled, chains=1)
     trace.posterior.a
```

### Comparing `nutpie-0.9.1/tests/test_stan.py` & `nutpie-0.9.2/tests/test_stan.py`

 * *Files identical despite different names*

### Comparing `nutpie-0.9.1/Cargo.lock` & `nutpie-0.9.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -677,15 +677,15 @@
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
 name = "nutpie"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "anyhow",
  "arrow2",
  "bridgestan",
  "criterion",
  "itertools 0.11.0",
  "ndarray",
```

### Comparing `nutpie-0.9.1/PKG-INFO` & `nutpie-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutpie
-Version: 0.9.1
+Version: 0.9.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=12.0.0
 Requires-Dist: pandas >=2.0
 Requires-Dist: xarray >=2023.6.0
 Requires-Dist: arviz >=0.15.0
@@ -24,51 +24,51 @@
 Author: Adrian Seyboldt <adrian.seyboldt@gmail.com>, PyMC Developers <pymc.devs@gmail.com>
 Author-email: PyMC Developers <pymc.devs@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/pymc-devs/nutpie
 
-# nutpie: A fast sampler for bayesian posteriors
+# nutpie: A fast sampler for Bayesian posteriors
 
 ## Installation
 
-nutpie can be installed using conda or mamba from conda-forge with
+nutpie can be installed using Conda or Mamba from conda-forge with
 
-```
-mamba install -c conda-forge nutpie pymc
+```bash
+mamba install -c conda-forge nutpie
 ```
 
 Or using pip:
 
-```
+```bash
 pip install nutpie
 ```
 
-To install it from source, install a rust compiler and maturin and then
+To install it from source, install a Rust compiler and maturin and then
 
-```
+```bash
 maturin develop --release
 ```
 
-If you want to use the nightly simd implementation for some of the math functions,
-switch to rust nightly and then install with the `simd_support` feature in then
+If you want to use the nightly SIMD implementation for some of the math functions,
+switch to Rust nightly and then install with the `simd_support` feature in then
 nutpie directory:
 
-```
+```bash
 rustup override set nightly
 maturin develop --release --features=simd_support
 ```
 
 ## Usage with PyMC
 
-First, PyMC and numba need to be installed, for example using
+First, PyMC and Numba need to be installed, for example using
 
-```
-mamba install pymc numba
+```bash
+mamba install -c conda-forge pymc numba
 ```
 
 We need to create a model:
 
 ```python
 import pymc as pm
 import numpy as np
@@ -117,39 +117,39 @@
 We then compile this model and sample form the posterior:
 
 ```python
 compiled_model = nutpie.compile_pymc_model(pymc_model)
 trace_pymc = nutpie.sample(compiled_model)
 ```
 
-`trace_pymc` now contains an arviz `InferenceData` object, including sampling
+`trace_pymc` now contains an ArviZ `InferenceData` object, including sampling
 statistics and the posterior of the variables defined above.
 
 ## Usage with Stan
 
-In order to sample from stan model, `bridgestan` needs to be installed.
-A pip package is available, but right now this can not be installed using conda.
+In order to sample from Stan model, `bridgestan` needs to be installed.
+A pip package is available, but right now this can not be installed using Conda.
 
-```
+```bash
 pip install bridgestan
 ```
 
 When we install nutpie with pip, we can also specify that we want optional
 dependencies for Stan models using
 
 ```
-pip install 'bridgestan[stan]'
+pip install 'nutpie[stan]'
 ```
 
 In addition, a C++ compiler needs to be available. For details see
-[the stan docs](https://mc-stan.org/docs/cmdstan-guide/cmdstan-installation.html#cpp-toolchain).
+[the Stan docs](https://mc-stan.org/docs/cmdstan-guide/cmdstan-installation.html#cpp-toolchain).
 
 We can then compile a Stan model, and sample using nutpie:
 
-```
+```python
 import nutpie
 
 code = """
 data {
     real mu;
 }
 parameters {
@@ -164,12 +164,12 @@
 # Provide data
 compiled = compiled.with_data(mu=3.)
 trace = nutpie.sample(compiled)
 ```
 
 ## Advantages
 
-nutpie uses `nuts-rs`, a library written in rust, that implements NUTS as in
-pymc and stan, but with a slightly different mass matrix tuning method as
+nutpie uses [`nuts-rs`](https://github.com/pymc-devs/nuts-rs), a library written in Rust, that implements NUTS as in
+PyMC and Stan, but with a slightly different mass matrix tuning method as
 those. It often produces a higher effective sample size per gradient
 evaluation, and tends to converge faster and with fewer gradient evaluation.
```

