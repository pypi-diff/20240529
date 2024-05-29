# Comparing `tmp/gsw-xarray-0.3.0.tar.gz` & `tmp/gsw_xarray-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsw-xarray-0.3.0.tar", max compression
+gzip compressed data, was "gsw_xarray-0.4.0.tar", max compression
```

## Comparing `gsw-xarray-0.3.0.tar` & `gsw_xarray-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
--rw-r--r--   0        0        0     1473 2022-09-09 20:00:25.193880 gsw-xarray-0.3.0/LICENSE.rst
--rw-r--r--   0        0        0     7000 2022-09-09 20:00:25.193880 gsw-xarray-0.3.0/README.rst
--rw-r--r--   0        0        0      886 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/__init__.py
--rw-r--r--   0        0        0     1268 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/_arguments.py
--rw-r--r--   0        0        0    19497 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/_attributes.py
--rw-r--r--   0        0        0     2002 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/_check_funcs.py
--rw-r--r--   0        0        0     5822 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/_core.py
--rw-r--r--   0        0        0      279 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/_function_utils.py
--rw-r--r--   0        0        0     7534 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/_names.py
--rw-r--r--   0        0        0      818 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/_units.py
--rw-r--r--   0        0        0      891 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/_util.py
--rw-r--r--   0        0        0      241 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/conversions.py
--rw-r--r--   0        0        0      229 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/density.py
--rw-r--r--   0        0        0      226 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/energy.py
--rw-r--r--   0        0        0      232 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/freezing.py
--rw-r--r--   0        0        0      238 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/geostrophy.py
--rw-r--r--   0        0        0      217 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/ice.py
--rw-r--r--   0        0        0      235 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/stability.py
--rw-r--r--   0        0        0        0 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/tests/__init__.py
--rw-r--r--   0        0        0      973 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/tests/conftest.py
--rw-r--r--   0        0        0     1133 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/tests/test_attrs.py
--rw-r--r--   0        0        0     1886 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/tests/test_gsw_xarray.py
--rw-r--r--   0        0        0     5261 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/tests/test_imports.py
--rw-r--r--   0        0        0     6376 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/tests/test_units.py
--rw-r--r--   0        0        0      580 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/gsw_xarray/tests/test_utils.py
--rw-r--r--   0        0        0      946 2022-09-09 20:00:25.201880 gsw-xarray-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8207 1970-01-01 00:00:00.000000 gsw-xarray-0.3.0/setup.py
--rw-r--r--   0        0        0     8025 1970-01-01 00:00:00.000000 gsw-xarray-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1473 2024-05-29 08:46:22.185867 gsw_xarray-0.4.0/LICENSE.rst
+-rw-r--r--   0        0        0     9854 2024-05-29 08:46:22.185867 gsw_xarray-0.4.0/README.rst
+-rw-r--r--   0        0        0      707 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/__init__.py
+-rw-r--r--   0        0        0     8192 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_accessor.py
+-rw-r--r--   0        0        0     2481 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_arguments.py
+-rw-r--r--   0        0        0    19565 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_attributes.py
+-rw-r--r--   0        0        0     2002 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_check_funcs.py
+-rw-r--r--   0        0        0     5855 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_core.py
+-rw-r--r--   0        0        0     1390 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_function_utils.py
+-rw-r--r--   0        0        0     7542 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_names.py
+-rw-r--r--   0        0        0     2758 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_options.py
+-rw-r--r--   0        0        0      818 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_units.py
+-rw-r--r--   0        0        0      675 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_util.py
+-rw-r--r--   0        0        0      891 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/_util_module.py
+-rw-r--r--   0        0        0      265 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/conversions.py
+-rw-r--r--   0        0        0      253 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/density.py
+-rw-r--r--   0        0        0      250 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/energy.py
+-rw-r--r--   0        0        0      256 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/freezing.py
+-rw-r--r--   0        0        0      262 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/geostrophy.py
+-rw-r--r--   0        0        0      241 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/ice.py
+-rw-r--r--   0        0        0      259 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/stability.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/__init__.py
+-rw-r--r--   0        0        0      986 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/conftest.py
+-rw-r--r--   0        0        0     5184 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/test_accessor.py
+-rw-r--r--   0        0        0     1204 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/test_attrs.py
+-rw-r--r--   0        0        0     1796 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/test_gsw_xarray.py
+-rw-r--r--   0        0        0     5530 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/test_imports.py
+-rw-r--r--   0        0        0     6730 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/test_units.py
+-rw-r--r--   0        0        0      565 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/test_utils.py
+-rw-r--r--   0        0        0      469 2024-05-29 08:46:22.193867 gsw_xarray-0.4.0/gsw_xarray/tests/test_version.py
+-rw-r--r--   0        0        0     1888 2024-05-29 08:46:22.197867 gsw_xarray-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10851 1970-01-01 00:00:00.000000 gsw_xarray-0.4.0/PKG-INFO
```

### Comparing `gsw-xarray-0.3.0/LICENSE.rst` & `gsw_xarray-0.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gsw-xarray-0.3.0/gsw_xarray/_attributes.py` & `gsw_xarray-0.4.0/gsw_xarray/_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -304,26 +304,26 @@
         },
     ),
     "enthalpy_ice": {
         "units": "J/kg",
     },
     "enthalpy_second_derivatives": (
         {
-            "units": "(J/kg)(g/kg)^-2",
+            "units": "(J/kg)/((g/kg)^2)",
         },
         {
             "units": "J/(kg K(g/kg))",
         },
         {
             "units": "J/(kg K^2)",
         },
     ),
     "enthalpy_second_derivatives_CT_exact": (
         {
-            "units": "(J/kg)(g/kg)^-2",
+            "units": "(J/kg)/((g/kg)^2)",
         },
         {
             "units": "J/(kg K(g/kg))",
         },
         {
             "units": "J/(kg K^2)",
         },
@@ -644,60 +644,60 @@
         },
         {
             "units": "kg/g",
         },
     ),
     "rho_first_derivatives": (
         {
-            "units": "(kg/m^3)(g/kg)^-1",
+            "units": "(kg/m^3)/(g/kg)",
         },
         {
             "units": "kg/(m^3 K)",
         },
         {
             "units": "kg/(m^3 Pa)",
         },
     ),
     "rho_first_derivatives_wrt_enthalpy": (
         {
-            "units": "(kg/m^3)(g/kg)^-1",  # matlab doc is uncorrect
+            "units": "(kg/m^3)/(g/kg)",  # matlab doc is uncorrect
         },
         {
-            "units": "(kg/m^3)(J/kg)^-1",
+            "units": "(kg/m^3)/(J/kg)",
         },
     ),
     "rho_ice": {
         "units": "kg/m^3",
     },
     "rho_second_derivatives": (
         {
-            "units": "(kg/m^3)(g/kg)^-2",
+            "units": "(kg/m^3)/((g/kg)^2)",
         },
         {
-            "units": "(kg/m^3)(g/kg)^-1 K^-1",
+            "units": "(kg/m^3)/(g/kg) K^-1",
         },
         {
             "units": "(kg/m^3) K^-2",
         },
         {
-            "units": "(kg/m^3)(g/kg)^-1 Pa^-1",
+            "units": "(kg/m^3)/(g/kg) Pa^-1",
         },
         {
             "units": "(kg/m^3) K^-1 Pa^-1",
         },
     ),
     "rho_second_derivatives_wrt_enthalpy": (
         {
-            "units": "(kg/m^3)(g/kg)^-2",  # matlab doc is uncorrect
+            "units": "(kg/m^3)/((g/kg)^2)",  # matlab doc is uncorrect
         },
         {
-            "units": "(kg/m^3)(g/kg)^-1 J^-1/kg^-1",
+            "units": "(kg/m^3)/(g/kg) J^-1/kg^-1",
         },
         {
-            "units": "(kg/m^3)(J/kg)^-2",
+            "units": "(kg/m^3)/((J/kg)^2)",
         },
     ),
     "rho_t_exact": {
         "standard_name": "sea_water_density",
         "units": "kg/m^3",
     },
     "seaice_fraction_to_freeze_seawater": (
@@ -754,60 +754,60 @@
         },
     ),
     "specvol_anom_standard": {
         "units": "m^3/kg",
     },
     "specvol_first_derivatives": (
         {
-            "units": "(m^3/kg)(g/kg)^-1",
+            "units": "(m^3/kg)/(g/kg)",
         },
         {
             "units": "m^3/(kg K)",
         },
         {
             "units": "m^3/(kg Pa)",
         },
     ),
     "specvol_first_derivatives_wrt_enthalpy": (
         {
-            "units": "(m^3/kg)(g/kg)^-1",  # seems to be an error in the doc
+            "units": "(m^3/kg)/(g/kg)",  # seems to be an error in the doc
         },
         {
-            "units": "(m^3/kg)(J/kg)^-1",
+            "units": "(m^3/kg)/(J/kg)",
         },
     ),
     "specvol_ice": {
         "units": "m^3/kg",
     },
     "specvol_second_derivatives": (
         {
-            "units": "(m^3/kg)(g/kg)^-2",
+            "units": "(m^3/kg)/((g/kg)^2)",
         },
         {
-            "units": "(m^3/kg)(g/kg)^-1 K^-1",
+            "units": "(m^3/kg)/(g/kg) K^-1",
         },
         {
             "units": "(m^3/kg) K^-2",
         },
         {
-            "units": "(m^3/kg)(g/kg)^-1 Pa^-1",  # seems to be an error in the doc
+            "units": "(m^3/kg)/(g/kg) Pa^-1",  # seems to be an error in the doc
         },
         {
             "units": "(m^3/kg) K^-1 Pa^-1",
         },
     ),
     "specvol_second_derivatives_wrt_enthalpy": (
         {
-            "units": "(m^3/kg)(g/kg)^-2",  # error in doc?
+            "units": "(m^3/kg)/((g/kg)^2)",  # error in doc?
         },
         {
-            "units": "(m^3/kg)(g/kg)^-1 J^-1/kg^-1",
+            "units": "(m^3/kg)/(g/kg) J^-1/kg^-1",
         },
         {
-            "units": "(m^3/kg)(J/kg)^-2",
+            "units": "(m^3/kg)/((J/kg)^2)",
         },
     ),
     "specvol_t_exact": {
         "units": "kg/m^3",
     },
     "spiciness0": {
         "units": "kg/m^3",
@@ -815,14 +815,15 @@
     "spiciness1": {
         "units": "kg/m^3",
     },
     "spiciness2": {
         "units": "kg/m^3",
     },
     "t90_from_t68": {
+        "standard_name": "sea_water_temperature",
         "units": "degC",
         "reference_scale": "ITS-90",
     },
     "t_deriv_chem_potential_water_t_exact": {
         "units": "J/g/C",
     },
     "t_freezing": {
@@ -862,9 +863,10 @@
     },
     "thermobaric": {
         "units": "1/(K Pa)",
     },
     "z_from_p": {
         "standard_name": "height_above_mean_sea_level",
         "units": "m",
+        "positive": "up",
     },
 }
```

### Comparing `gsw-xarray-0.3.0/gsw_xarray/_check_funcs.py` & `gsw_xarray-0.4.0/gsw_xarray/_check_funcs.py`

 * *Files identical despite different names*

### Comparing `gsw-xarray-0.3.0/gsw_xarray/_core.py` & `gsw_xarray-0.4.0/gsw_xarray/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from functools import wraps, singledispatch
+from functools import singledispatch, wraps
 
 import gsw
 import xarray as xr
 
+from ._arguments import input_properties
 from ._attributes import _func_attrs
-from ._arguments import input_units
-from ._names import _names
 from ._check_funcs import _check_funcs
 from ._function_utils import args_and_kwargs_to_kwargs
+from ._names import _names
 from ._units import safe_unit
 
 try:
-    import pint_xarray
     import pint
+    import pint_xarray
 
 except ImportError:
     pint_xarray = None
 
 
 def add_attrs(rv, attrs, name):
     if isinstance(rv, xr.DataArray):
@@ -47,15 +47,15 @@
 
 @convert_and_dequantify_reg.register
 def _cd_xr(arg: xr.DataArray, kw):
     if arg.pint.units is not None:
         # pint-xarray raises ValueError if conversion does not work
         # so we split the choice of unit and conversion
         try:
-            input_unit = input_units[kw]
+            input_unit = input_properties[kw]["units"]
         except KeyError:
             input_unit = arg.pint.units
         input_unit = safe_unit(input_unit, arg.pint.registry)
         _arg = arg.pint.to({arg.name: input_unit})
         _arg = _arg.pint.dequantify()
         _reg = arg.pint.registry
     else:
@@ -65,15 +65,15 @@
 
 
 if pint_xarray is not None:
 
     @convert_and_dequantify_reg.register
     def _cd_pint(arg: pint.Quantity, kw):
         try:
-            input_unit = input_units[kw]
+            input_unit = input_properties[kw]["units"]
         except KeyError:
             input_unit = arg.unit
         input_unit = safe_unit(input_unit, arg._REGISTRY)
         _arg = arg.to(input_unit)
         _arg = _arg.magnitude
         _reg = arg._REGISTRY
         return _arg, _reg
@@ -95,15 +95,15 @@
 
     for kw, arg in kwargs.items():
         # convert and dequantify
         # we can safely always call this due to the pint_xarray check above (and the base case of the single dispatch)
         _arg, _reg = convert_and_dequantify_reg(arg, kw)
         new_kwargs[kw] = _arg
         # We append registry only if kw has a unit, e.g. we skip it if kw is 'axis' or 'interp_method'
-        if input_units[kw] is not None and _arg is not None:
+        if input_properties[kw]["units"] is not None and _arg is not None:
             registries.append(_reg)
 
     registries = set(registries)
     # If there is a None in registries, but len > 1 => error
     if (len(registries) > 1) and (None in registries):
         raise ValueError("Mixed usage of Quantity and non Quantity is forbidden.")
 
@@ -123,15 +123,15 @@
     return new_kwargs, registries
 
 
 def cf_attrs(fname, attrs, name, check_func):
     def cf_attrs_decorator(func):
         @wraps(func)
         def cf_attrs_wrapper(*args, **kwargs):
-            # We start by transforming all args to kwargs,
+            # We transform all args to kwargs,
             # Except the default ones
             kwargs = args_and_kwargs_to_kwargs(func, args, kwargs, add_defaults=False)
             kwargs, unit_registry = pint_compat(fname, kwargs)
             # We add the default arguments
             # It is necessary to not add defaults before pint compat
             # Otherwise, defaults are never Quantities
             kwargs = args_and_kwargs_to_kwargs(func, [], kwargs, add_defaults=True)
@@ -139,15 +139,15 @@
             # back the original args
             o_args = list(kwargs.values())[: len(args)]
             o_kwargs = {i: kwargs[i] for i in list(kwargs)[len(args) :]}
             rv = func(*o_args, **o_kwargs)
             attrs_checked = check_func(attrs, kwargs)
             if isinstance(rv, tuple):
                 rv_updated = []
-                for (i, da) in enumerate(rv):
+                for i, da in enumerate(rv):
                     # Verify the unit
                     attrs_checked[i]["units"] = safe_unit(
                         attrs_checked[i]["units"], unit_registry
                     )
                     add_attrs(da, attrs_checked[i], name[i])
                     rv_updated.append(
                         quantify(da, attrs_checked[i], unit_registry=unit_registry)
```

### Comparing `gsw-xarray-0.3.0/gsw_xarray/_names.py` & `gsw_xarray-0.4.0/gsw_xarray/_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "SR_from_SP": "SR",
     "Sstar_from_SA": "Sstar",
     "Sstar_from_SP": "Sstar",
     "Turner_Rsubrho": ("Tu", "Rsubrho", "p_mid"),
     "adiabatic_lapse_rate_from_CT": "adiabatic",
     "adiabatic_lapse_rate_ice": "adiabatic",
     "alpha": "alpha",
-    "alpha_on_beta": "alpha",
+    "alpha_on_beta": "alpha_on_beta",
     "alpha_wrt_t_exact": "alpha",
     "alpha_wrt_t_ice": "alpha",
     "beta": "beta",
     "beta_const_t_exact": "beta",
     "cabbeling": "cabbeling",
     "chem_potential_water_ice": "chem",
     "chem_potential_water_t_exact": "chem",
```

### Comparing `gsw-xarray-0.3.0/gsw_xarray/_units.py` & `gsw_xarray-0.4.0/gsw_xarray/_units.py`

 * *Files identical despite different names*

### Comparing `gsw-xarray-0.3.0/gsw_xarray/_util.py` & `gsw_xarray-0.4.0/gsw_xarray/_util_module.py`

 * *Files identical despite different names*

### Comparing `gsw-xarray-0.3.0/gsw_xarray/tests/conftest.py` & `gsw_xarray-0.4.0/gsw_xarray/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+import numpy as np
 import pytest
-
 import xarray as xr
-import numpy as np
 
 
 @pytest.fixture
 def ds():
     ds = xr.Dataset()
     id = np.arange(3)
     ds["id"] = xr.DataArray(id, coords={"id": id})
@@ -19,15 +18,15 @@
     ds["p"] = ds["id"] * 10
     ds["p"].attrs = {"standard_name": "sea_water_pressure", "units": "dbar"}
     return ds
 
 
 @pytest.fixture(scope="session")
 def ureg():
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
     from pint_xarray import unit_registry as ureg
 
     return ureg
 
 
 @pytest.fixture
 def ds_pint(ds, ureg):
```

### Comparing `gsw-xarray-0.3.0/gsw_xarray/tests/test_attrs.py` & `gsw_xarray-0.4.0/gsw_xarray/tests/test_attrs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """
 Functions that return tuples must have tuples
 (with the same length) as attributes and names
 """
-import pytest
-from inspect import signature, _empty
 
-from .test_imports import gsw_base
+from inspect import _empty, signature
 
-from gsw_xarray._names import _names
-from gsw_xarray._attributes import _func_attrs
 import gsw
+import pytest
+
+from gsw_xarray._attributes import _func_attrs
+from gsw_xarray._names import _names
+
+from .test_imports import gsw_base
 
 
 @pytest.mark.parametrize("func_name", gsw_base)
 def test_(func_name):
-    if func_name in ["indexer", "match_args_return", "pchip_interp"]:
+    if func_name in [
+        "indexer",
+        "match_args_return",
+        "pchip_interp",
+        "gibbs",
+        "gibbs_ice",
+    ]:
         # Internal gsw cookery or non wrapped functions
         return
     f = getattr(gsw, func_name)
     n_args = len(signature(f).parameters)
     p = signature(f).parameters
     n_args = len([i for i in p.keys() if p[i].default is _empty])
     if "axis" in p.keys():
```

### Comparing `gsw-xarray-0.3.0/gsw_xarray/tests/test_gsw_xarray.py` & `gsw_xarray-0.4.0/gsw_xarray/tests/test_gsw_xarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from gsw_xarray import __version__
-import gsw_xarray as gsw
-import xarray as xr
 import numpy as np
 import pytest
+import xarray as xr
 
-
-def test_version():
-    assert __version__ == "0.2.1"
+import gsw_xarray as gsw
 
 
 def test_func_standard(ds):
     """Basic test"""
     sigma0 = gsw.sigma0(SA=ds.SA, CT=ds.CT)
     assert sigma0.attrs["standard_name"] == "sea_water_sigma_t"
     assert sigma0.name == "sigma0"
```

### Comparing `gsw-xarray-0.3.0/gsw_xarray/tests/test_imports.py` & `gsw_xarray-0.4.0/gsw_xarray/tests/test_imports.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from types import ModuleType
-import numpy as np
 
+import gsw
+import numpy as np
 import pytest
 
+import gsw_xarray
+
 """
 Here all import machinery is tested (dir, getattr, ...),
 for functions and modules.
 
 The import gsw_xarray is kept in every function to not interfere
 between them with a global import.
 """
 
-import gsw_xarray
-import gsw
-
 
 def get_module_names(module):
     mod_names = dir(module)
 
     # filter out all the "private" names
     public_names = list(filter(lambda name: not name.startswith("_"), mod_names))
 
@@ -27,14 +27,15 @@
             lambda name: not isinstance(getattr(module, name), ModuleType), public_names
         )
     )
 
 
 gsw_base = get_module_names(gsw)
 wrapped_funcs = gsw_xarray._core._wrapped_funcs
+del gsw_xarray
 
 submodules = [
     "conversions",
     "density",
     "energy",
     "freezing",
     "geostrophy",
@@ -42,27 +43,33 @@
     "stability",
 ]
 
 
 @pytest.mark.parametrize("upstream_func", gsw_base)
 def test_wrapped_interface(upstream_func):
     """Tests the complete gsw function namespace against ours"""
+    import gsw_xarray
+
     assert hasattr(gsw_xarray, upstream_func)
 
 
 @pytest.mark.parametrize("upstream_func", gsw_base)
 def test_wrapped_return(upstream_func):
+    import gsw_xarray
+
     if upstream_func in wrapped_funcs:
         assert getattr(gsw_xarray, upstream_func) is wrapped_funcs[upstream_func]
     else:
         assert getattr(gsw_xarray, upstream_func) is getattr(gsw, upstream_func)
 
 
 @pytest.mark.parametrize("submodule", submodules)
 def test_wrapped_interface_submodules(submodule):
+    import gsw_xarray
+
     upstream_submodule = getattr(gsw, submodule)
     wrapped_submodule = getattr(gsw_xarray, submodule)
 
     upstream_funcs = get_module_names(upstream_submodule)
     for name in upstream_funcs:
         if name in wrapped_funcs:
             assert getattr(wrapped_submodule, name) is wrapped_funcs[name]
@@ -75,14 +82,16 @@
     """This tests the interface in the form of:
     > from gsw_xarray import func
     where func is any function on the upstream gsw
 
     It does this by creating an empty "locals" dict and calling an exec on the way the code
     would be written, it then checks the idenity of that returned result
     """
+    import gsw_xarray  # noqa: F401
+
     result = {}
     # the empty dict is for the "globals" that we don't care about (exec would populate it with builtins)
     exec(f"from gsw_xarray import {upstream_func}", {}, result)
     func = result[upstream_func]
     if upstream_func in wrapped_funcs:
         assert func is wrapped_funcs[upstream_func]
     else:
@@ -93,14 +102,16 @@
 @pytest.mark.parametrize("submodule", submodules)
 def test_import_interface_submodule(submodule, upstream_func):
     """This tests the interface in the form of:
     > from gsw_xarray.submod import func
     where submod is one of the submodule groupings in the upstream
 
     """
+    import gsw_xarray  # noqa: F401
+
     result = {}
     upstream_interface = get_module_names(getattr(gsw, submodule))
 
     expected_func = getattr(gsw, upstream_func)
 
     if upstream_func not in upstream_interface:
         with pytest.raises(ImportError):
@@ -119,14 +130,16 @@
             assert func is expected_func
 
 
 @pytest.mark.parametrize("upstream_func", gsw_base)
 @pytest.mark.parametrize("submodule", submodules)
 def test_attr_method(submodule, upstream_func):
     """tests the identities of funcs in the form of gsw_xarray.submodule.func"""
+    import gsw_xarray  # noqa: F401
+
     upstream_interface = get_module_names(getattr(gsw, submodule))
 
     expected_func = getattr(gsw, upstream_func)
 
     if upstream_func not in upstream_interface:
         with pytest.raises(AttributeError):
             eval(f"gsw_xarray.{submodule}.{upstream_func}")
@@ -139,26 +152,30 @@
         if upstream_func in wrapped_funcs:
             assert func is wrapped_funcs[upstream_func]
         else:
             assert func is expected_func
 
 
 def test_wildcard_top_level():
+    import gsw_xarray  # noqa: F401
+
     upstream_interface = {}
     exec("from gsw import *", {}, upstream_interface)
 
     wrapped_interface = {}
     exec("from gsw_xarray import *", {}, wrapped_interface)
 
     assert wrapped_interface.keys() == upstream_interface.keys()
 
 
 @pytest.mark.parametrize("submodule", submodules)
 def test_wildcard_submodule(submodule):
     """tests the identities of funcs in the form of gsw_xarray.submodule.func"""
+    import gsw_xarray  # noqa: F401
+
     upstream_interface = {}
     exec(f"from gsw.{submodule} import *", {}, upstream_interface)
 
     wrapped_interface = {}
     exec(f"from gsw_xarray.{submodule} import *", {}, wrapped_interface)
 
     assert wrapped_interface.keys() == upstream_interface.keys()
```

### Comparing `gsw-xarray-0.3.0/gsw_xarray/tests/test_units.py` & `gsw_xarray-0.4.0/gsw_xarray/tests/test_units.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 """
 Testing units with pint and cf_units
 """
-import pytest
+
+from inspect import signature
+
+import gsw
 import numpy as np
+import pytest
 import xarray as xr
-import gsw
+
 import gsw_xarray
+from gsw_xarray._arguments import input_properties
+from gsw_xarray._attributes import _func_attrs
 
 from .test_imports import gsw_base
-from gsw_xarray._attributes import _func_attrs
-from gsw_xarray._arguments import input_units
-from inspect import signature
 
 ##########
 # Outputs
 ##########
 
 
 @pytest.mark.parametrize("func_name", gsw_base)
 def test_unit_pint(func_name, ureg):
-
-    if func_name in ["indexer", "match_args_return", "pchip_interp"]:
+    if func_name in [
+        "indexer",
+        "match_args_return",
+        "pchip_interp",
+        "gibbs",
+        "gibbs_ice",
+    ]:
         # Internal gsw cookery or non wrapped functions
         return
     if func_name == "geostrophic_velocity":
         pytest.xfail(
             'geostrophic_velocity outputs "degree_north" and "degree_east" that are not compatible with pint'
         )
     attrs = _func_attrs[func_name]
@@ -36,15 +44,21 @@
         print(a["units"])
         ureg.Unit(a["units"])
 
 
 @pytest.mark.parametrize("func_name", gsw_base)
 def test_unit_cf_units(func_name):
     cf_units = pytest.importorskip("cf_units")
-    if func_name in ["indexer", "match_args_return", "pchip_interp"]:
+    if func_name in [
+        "indexer",
+        "match_args_return",
+        "pchip_interp",
+        "gibbs",
+        "gibbs_ice",
+    ]:
         # Internal gsw cookery or non wrapped functions
         return
     attrs = _func_attrs[func_name]
     if isinstance(attrs, dict):
         attrs = [
             attrs,
         ]
@@ -86,115 +100,120 @@
 ##########
 # Input
 ##########
 
 
 @pytest.mark.parametrize("func_name", gsw_base)
 def test_unit_of_arg(func_name, ureg):
-
-    if func_name in ["indexer", "match_args_return", "pchip_interp"]:
+    if func_name in [
+        "indexer",
+        "match_args_return",
+        "pchip_interp",
+        "gibbs",
+        "gibbs_ice",
+    ]:
         # Internal gsw cookery or non wrapped functions
         return
     func = getattr(gsw, func_name)
     s = signature(func)
     p = s.parameters
     for i in p:
-        assert i in input_units.keys()
+        assert i in input_properties.keys()
 
 
 def test_ds_mixed_quantity_non_quantity(ds, ds_pint):
     """If at least 1 of the inputs is quantity, all inputs should be quantity"""
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
 
     with pytest.raises(ValueError):
-        sigma0 = gsw_xarray.sigma0(SA=ds.SA, CT=ds_pint.CT)
+        gsw_xarray.sigma0(SA=ds.SA, CT=ds_pint.CT)
 
 
 def test_ds_mixed_quantity_non_quantity_axis_arg_None_arg(ds_pint):
     """Should not use dimension for None args, nor for the axis arg"""
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
 
     gsw_xarray.Nsquared(SA=ds_pint.SA, CT=ds_pint.CT, p=ds_pint.p, axis=0, lat=None)
 
 
 def test_pint_mixed_quantity_non_quantity(T):
     """If at least 1 of the inputs is quantity, all inputs should be quantity"""
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
 
     with pytest.raises(ValueError):
-        sigma0 = gsw_xarray.sigma0(SA=35, CT=T)
+        gsw_xarray.sigma0(SA=35, CT=T)
 
 
 def test_pint_quantity_xarray(ds_pint, T):
     """If input is mixed between pint-xarray and pint quantity it should return pint-xarray wrapped quantity"""
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
 
     sigma0 = gsw_xarray.sigma0(SA=ds_pint.SA, CT=T)
     assert sigma0.pint.units == pint_xarray.unit_registry("kg / m^3")
 
 
 def test_pint_quantity(S, T):
     """If input is pint quantity should return a quantity"""
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
     pint = pytest.importorskip("pint")
 
     CT = gsw_xarray.CT_from_pt(SA=S, pt=T)
     assert isinstance(CT, pint.Quantity)
 
 
 def test_pint_quantity_tuple(S, T):
     """If input is pint quantity should return a quantity"""
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
     import pint
 
     (a, b) = gsw_xarray.CT_first_derivatives(S, pt=T)
     assert isinstance(a, pint.Quantity)
     assert isinstance(b, pint.Quantity)
 
 
 def test_mixed_unit_registries():
     """If input quantities are from different registries, it should fail"""
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
     import pint
 
     ureg_a = pint.UnitRegistry()
     ureg_b = pint.UnitRegistry()
     with pytest.raises(ValueError):
         gsw_xarray.CT_first_derivatives(
             35 * ureg_a("g / kg"), pt=ureg_b.Quantity(1, ureg_b.degC)
         )
 
 
 def test_pint_quantity_convert_kwargs(ds_pint):
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
 
     sigma0_good_units = gsw_xarray.sigma0(SA=ds_pint.SA, CT=ds_pint.CT)
     sigma0_bad_units = gsw_xarray.sigma0(
         SA=ds_pint.SA.pint.to("mg / kg"), CT=ds_pint.CT.pint.to("kelvin")
     )
     xr.testing.assert_equal(sigma0_good_units, sigma0_bad_units)
 
 
 def test_pint_quantity_convert_args(ds_pint):
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
 
     sigma0_good_units = gsw_xarray.sigma0(ds_pint.SA, ds_pint.CT)
     sigma0_bad_units = gsw_xarray.sigma0(
         ds_pint.SA.pint.to("mg / kg"), ds_pint.CT.pint.to("kelvin")
     )
     xr.testing.assert_equal(sigma0_good_units, sigma0_bad_units)
 
 
 def test_pint_quantity_convert_kwargs_pint(S, T):
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
 
     sigma0_good_units = gsw_xarray.sigma0(SA=S, CT=T)
     sigma0_bad_units = gsw_xarray.sigma0(SA=S.to("mg / kg"), CT=T.to("kelvin"))
     assert np.allclose(sigma0_good_units, sigma0_bad_units)
 
 
 def test_pint_quantity_convert_args_pint(S, T):
-    pint_xarray = pytest.importorskip("pint_xarray")
+    pint_xarray = pytest.importorskip("pint_xarray")  # noqa: F841
 
     sigma0_good_units = gsw_xarray.sigma0(S, T)
     sigma0_bad_units = gsw_xarray.sigma0(S.to("mg / kg"), T.to("kelvin"))
     assert np.allclose(sigma0_good_units, sigma0_bad_units)
```

### Comparing `gsw-xarray-0.3.0/gsw_xarray/tests/test_utils.py` & `gsw_xarray-0.4.0/gsw_xarray/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pytest
-
 from .._function_utils import args_and_kwargs_to_kwargs
 
 
 def func(a, b, c=2, d=3):
     return
```

### Comparing `gsw-xarray-0.3.0/setup.py` & `gsw_xarray-0.4.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,297 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+.. |CI Status| image:: https://github.com/docotak/gsw-xarray/actions/workflows/ci.yml/badge.svg
+  :target: https://github.com/DocOtak/gsw-xarray/actions/workflows/ci.yml
+  :alt: CI Status
+.. |Documentation Status| image:: https://readthedocs.org/projects/gsw-xarray/badge/?version=latest
+  :target: https://gsw-xarray.readthedocs.io/en/latest/?badge=latest
+  :alt: Documentation Status
+.. |pypi| image:: https://badge.fury.io/py/gsw-xarray.svg
+   :target: https://badge.fury.io/py/gsw-xarray
+   :alt: pypi package
+.. |conda forge| image:: https://img.shields.io/conda/vn/conda-forge/gsw-xarray
+   :target: https://anaconda.org/conda-forge/gsw-xarray
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8297618.svg
+   :target: https://doi.org/10.5281/zenodo.8297618
+   :alt: zenodo DOI
 
-packages = \
-['gsw_xarray', 'gsw_xarray.tests']
+gsw-xarray: Wrapper for gsw that adds CF attributes
+===================================================
+|CI Status| |Documentation Status| |pypi| |conda forge| |zenodo|
 
-package_data = \
-{'': ['*']}
+gsw-xarray is a wrapper for `gsw python <https://github.com/TEOS-10/GSW-python>`_
+that will add CF attributes to xarray.DataArray outputs.
+It is meant to be a drop in wrapper for the upstream GSW-Python library and will only add these attributes if one argument to a function is an xarray.DataArray.
 
-install_requires = \
-['gsw>=3.4.0', 'xarray>=0.20.2']
-
-extras_require = \
-{'docs': ['Sphinx>=4.4.0', 'furo>=2022.1.2'],
- 'pint': ['pint-xarray>=0.2.1,<0.3.0', 'Pint>=0.18']}
-
-setup_kwargs = {
-    'name': 'gsw-xarray',
-    'version': '0.3.0',
-    'description': 'Drop in wrapper for gsw which adds CF standard name and units attributes to xarray results',
-    'long_description': '.. |CI Status| image:: https://github.com/docotak/gsw-xarray/actions/workflows/ci.yml/badge.svg\n  :target: https://github.com/DocOtak/gsw-xarray/actions/workflows/ci.yml\n  :alt: CI Status\n.. |Documentation Status| image:: https://readthedocs.org/projects/gsw-xarray/badge/?version=latest\n  :target: https://gsw-xarray.readthedocs.io/en/latest/?badge=latest\n  :alt: Documentation Status\n.. |pypi| image:: https://badge.fury.io/py/gsw-xarray.svg\n   :target: https://badge.fury.io/py/gsw-xarray\n   :alt: pypi package\n.. |conda forge| image:: https://img.shields.io/conda/vn/conda-forge/gsw-xarray\n   :target: https://anaconda.org/conda-forge/gsw-xarray\n\ngsw-xarray: Wrapper for gsw that adds CF attributes\n===================================================\n|CI Status| |Documentation Status| |pypi| |conda forge|\n\ngsw-xarray is a wrapper for `gsw python <https://github.com/TEOS-10/GSW-python>`_\nthat will add CF attributes to xarray.DataArray outputs.\nIt is meant to be a drop in wrapper for the upstream GSW-Python library and will only add these attributes if one argument to a function is an xarray.DataArray.\n\nYou can find the documentation on `gsw-xarray.readthedocs.io <https://gsw-xarray.readthedocs.io/>`_.\n\nUsage\n-----\n\n.. code:: python\n\n   import gsw_xarray as gsw\n\n   # Create a xarray.Dataset\n   import numpy as np\n   import xarray as xr\n   ds = xr.Dataset()\n   id = np.arange(3)\n   ds[\'id\'] = xr.DataArray(id, coords={\'id\':id})\n   ds[\'CT\'] = ds[\'id\'] * 10\n   ds[\'CT\'].attrs = {\'standard_name\':\'sea_water_conservative_temperature\'}\n   ds[\'SA\'] = ds[\'id\'] * 0.1 + 34\n   ds[\'SA\'].attrs = {\'standard_name\':\'sea_water_absolute_salinity\'}\n\n   # Apply gsw functions\n   sigma0 = gsw.sigma0(SA=ds[\'SA\'], CT=ds[\'CT\'])\n   print(sigma0.attrs)\n\nOutputs\n\n::\n\n   {\'standard_name\': \'sea_water_sigma_t\', \'units\': \'kg/m^3\'}\n\nDon\'t worry about usage with non xarray array objects, just use in all places you would the upstream library:\n\n.. code:: python\n\n   sigma0 = gsw.sigma0(id * 10, id * 0.1 + 34)\n   print(type(sigma0), sigma0)\n\nOutputs\n\n::\n\n   <class \'numpy.ndarray\'> [-5.08964499  2.1101098   9.28348219]\n\n\nWe support (and convert the unit if necessary) the usage of pint.Quantities and the usage of xarray wrapped Quantities.\nSupport for pint requires the installation of two optional dependencies: ``pint`` and ``pint-xarray``.\nIf all the inputs to a gsw function are Quantities, the returned object will also be a Quantity belonging to the same UnitRegistry.\n\n.. warning::\n\n   Quantities must all belong to the same pint.UnitRegistry, a ValueError will be thrown if there are mixed registries.\n\n.. warning::\n\n   If one input is a Quantity, all inputs must be Quantities (and/or xarray wrapped Quantities), except for the `axis` and `interp_method` arguments.\n   For mixed usage of Quantities and non Quantities, a ValueError will be thrown.\n\n.. code:: python\n\n   import pint_xarray\n   import gsw_xarray as gsw\n\n   # Create a xarray.Dataset\n   import numpy as np\n   import xarray as xr\n   ds = xr.Dataset()\n   id = np.arange(3)\n   ds[\'id\'] = xr.DataArray(id, coords={\'id\':id})\n   ds[\'CT\'] = ds[\'id\'] * 10\n   # make sure there are unit attrs this time\n   ds[\'CT\'].attrs = {\'standard_name\':\'sea_water_conservative_temperature\', \'units\': \'degC\'}\n   ds[\'SA\'] = ds[\'id\'] * 0.1 + 34\n   ds[\'SA\'].attrs = {\'standard_name\':\'sea_water_absolute_salinity\', \'units\': \'g/kg\'}\n\n   # use the pint accessor to quantify things\n   ds = ds.pint.quantify()\n\n   # Apply gsw functions\n   sigma0 = gsw.sigma0(SA=ds[\'SA\'], CT=ds[\'CT\'])\n   # outputs are now quantities!\n   print(sigma0)\n\nOutputs\n\n::\n\n   <xarray.DataArray \'sigma0\' (id: 3)>\n   <Quantity([27.17191038 26.12820162 24.03930887], \'kilogram / meter ** 3\')>\n   Coordinates:\n     * id       (id) int64 0 1 2\n   Attributes:\n       standard_name:  sea_water_sigma_t\n\nThe usage of xarray wrapped Quantities is not required, you can use pint directly (though the ``pint-xarray`` dep still needs to be installed).\n\n.. code:: python\n\n   import gsw_xarray as gsw\n   import pint\n   ureg = pint.UnitRegistry()\n   SA = ureg.Quantity(35, ureg("g/kg"))\n   CT = ureg.Quantity(10, ureg.degC)\n   sigma0 = gsw.sigma0(SA=SA, CT=CT)\n   print(sigma0)\n\nOutputs\n\n::\n\n   26.824644457868317 kilogram / meter ** 3\n\nAs gsw-xarray converts arguments to the proper unit when Quantities are used, we can e.g. use the temperature in Kelvin:\n\n.. code:: python\n\n   CT = ureg.Quantity(10, ureg.degC).to(\'kelvin\')\n   sigma0 = gsw.sigma0(SA=SA, CT=CT)\n   print(sigma0)\n\nOutputs\n\n::\n\n   26.824644457868317 kilogram / meter ** 3\n\n.. note::\n   If you do not wish to use the unit conversion ability, you need to pass dequantified Quantities\n   (e.g. `da.pint.dequantify()` for pint-xarray or `arg.magnitude` for pint.Quantity).\n\n.. warning::\n   On the opposite, gsw-xarray will not check the units if non Quantity arguments are used.\n   If you wish to use unit conversion, please pass quantified arguments (if your xarray.Dataset /\n   xarray.DataArray has the \'units\' attribute, you can use `da.pint.quantify()`)\n\n.. note::\n   We recommend that you use the `cf-xarray <https://cf-xarray.readthedocs.io/en/latest/units.html>`_ registry for units,\n   as it implements geophysical units as `degree_north`, `degrees_north`, etc.\n   gsw-xarray internally uses `degree_north` and `degree_east` for latitude and longitude unit names.\n   If they are not found in the unit registry, they will be replaced by `degree`.\n\n   The function `gsw.SP_from_SK` uses part per thousand for SK. \'ppt\' is already used for picopint,\n   so the expected unit is replaced by \'1\'.\n\n\nInstallation\n------------\nPip\n...\n\n.. code:: bash\n\n    pip install gsw-xarray\n\n\nConda\n.....\n\nInside a conda environment:  ``conda install -c conda-forge gsw-xarray``.\n\nPipenv\n......\n\nInside a pipenv environment: ``pipenv install gsw-xarray``.\n\n\nContributor guide\n-----------------\n\nAll contributions, bug reports, bug fixes, documentation improvements,\nenhancements, and ideas are welcome.\nIf you notice a bug or are missing a feature, fell free\nto open an issue in the `GitHub issues page <https://github.com/DocOtak/gsw-xarray/issues>`_.\n\nIn order to contribute to gsw-xarray, please fork the repository and\nsubmit a pull request. A good step by step tutorial for starting with git can be found in the\n`xarray contributor guide <https://xarray.pydata.org/en/stable/contributing.html#working-with-the-code>`_.\nA main difference is that we do not use conda as python environment, but poetry.\n\nSet up the environment\n......................\n\nYou will first need to `install poetry <https://python-poetry.org/docs/#installation>`_.\nThen go to your local clone of gsw-xarray and launch installation:\n\n.. code:: bash\n\n   cd /path/to/your/gsw-xarray\n   poetry install\n\nYou can then activate the environment by launching a shell\nwithin the virtual environment:\n\n.. code:: bash\n\n   poetry shell\n\nYou can check that the tests pass locally:\n\n.. code:: bash\n\n   pytest gsw_xarray/tests\n\nRelease (for maintainers only)\n..............................\n\nTODO...\n',
-    'author': 'Andrew Barna',
-    'author_email': 'abarna@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DocOtak/gsw-xarray',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8',
-}
+You can find the documentation on `gsw-xarray.readthedocs.io <https://gsw-xarray.readthedocs.io/>`_.
 
+Usage
+-----
+Simple usage
+............
 
-setup(**setup_kwargs)
+.. code:: python
+
+   import gsw_xarray as gsw
+
+   # Create a xarray.Dataset
+   import numpy as np
+   import xarray as xr
+   ds = xr.Dataset()
+   id = np.arange(3)
+   ds['id'] = xr.DataArray(id, coords={'id':id})
+   ds['CT'] = ds['id'] * 10
+   ds['CT'].attrs = {'standard_name':'sea_water_conservative_temperature'}
+   ds['SA'] = ds['id'] * 0.1 + 34
+   ds['SA'].attrs = {'standard_name':'sea_water_absolute_salinity'}
+
+   # Apply gsw functions
+   sigma0 = gsw.sigma0(SA=ds['SA'], CT=ds['CT'])
+   print(sigma0.attrs)
+
+Outputs
+
+::
+
+   {'standard_name': 'sea_water_sigma_t', 'units': 'kg/m^3'}
+
+Don't worry about usage with non xarray array objects, just use in all places you would the upstream library:
+
+.. code:: python
+
+   sigma0 = gsw.sigma0(id * 10, id * 0.1 + 34)
+   print(type(sigma0), sigma0)
+
+Outputs
+
+::
+
+   <class 'numpy.ndarray'> [-5.08964499  2.1101098   9.28348219]
+
+Using Pint
+..........
+   
+We support (and convert the unit if necessary) the usage of pint.Quantities and the usage of xarray wrapped Quantities.
+Support for pint requires the installation of two optional dependencies: ``pint`` and ``pint-xarray``.
+If all the inputs to a gsw function are Quantities, the returned object will also be a Quantity belonging to the same UnitRegistry.
+
+.. warning::
+
+   Quantities must all belong to the same pint.UnitRegistry, a ValueError will be thrown if there are mixed registries.
+
+.. warning::
+
+   If one input is a Quantity, all inputs must be Quantities (and/or xarray wrapped Quantities), except for the `axis` and `interp_method` arguments.
+   For mixed usage of Quantities and non Quantities, a ValueError will be thrown.
+
+.. code:: python
+
+   import pint_xarray
+   import gsw_xarray as gsw
+
+   # Create a xarray.Dataset
+   import numpy as np
+   import xarray as xr
+   ds = xr.Dataset()
+   id = np.arange(3)
+   ds['id'] = xr.DataArray(id, coords={'id':id})
+   ds['CT'] = ds['id'] * 10
+   # make sure there are unit attrs this time
+   ds['CT'].attrs = {'standard_name':'sea_water_conservative_temperature', 'units': 'degC'}
+   ds['SA'] = ds['id'] * 0.1 + 34
+   ds['SA'].attrs = {'standard_name':'sea_water_absolute_salinity', 'units': 'g/kg'}
+
+   # use the pint accessor to quantify things
+   ds = ds.pint.quantify()
+
+   # Apply gsw functions
+   sigma0 = gsw.sigma0(SA=ds['SA'], CT=ds['CT'])
+   # outputs are now quantities!
+   print(sigma0)
+
+Outputs
+
+::
+
+   <xarray.DataArray 'sigma0' (id: 3)>
+   <Quantity([27.17191038 26.12820162 24.03930887], 'kilogram / meter ** 3')>
+   Coordinates:
+     * id       (id) int64 0 1 2
+   Attributes:
+       standard_name:  sea_water_sigma_t
+
+The usage of xarray wrapped Quantities is not required, you can use pint directly (though the ``pint-xarray`` dep still needs to be installed).
+
+.. code:: python
+
+   import gsw_xarray as gsw
+   import pint
+   ureg = pint.UnitRegistry()
+   SA = ureg.Quantity(35, ureg("g/kg"))
+   CT = ureg.Quantity(10, ureg.degC)
+   sigma0 = gsw.sigma0(SA=SA, CT=CT)
+   print(sigma0)
+
+Outputs
+
+::
+
+   26.824644457868317 kilogram / meter ** 3
+
+As gsw-xarray converts arguments to the proper unit when Quantities are used, we can e.g. use the temperature in Kelvin:
+
+.. code:: python
+
+   CT = ureg.Quantity(10, ureg.degC).to('kelvin')
+   sigma0 = gsw.sigma0(SA=SA, CT=CT)
+   print(sigma0)
+
+Outputs
+
+::
+
+   26.824644457868317 kilogram / meter ** 3
+
+.. note::
+   If you do not wish to use the unit conversion ability, you need to pass dequantified Quantities
+   (e.g. `da.pint.dequantify()` for pint-xarray or `arg.magnitude` for pint.Quantity).
+
+.. warning::
+   On the opposite, gsw-xarray will not check the units if non Quantity arguments are used.
+   If you wish to use unit conversion, please pass quantified arguments (if your xarray.Dataset /
+   xarray.DataArray has the 'units' attribute, you can use `da.pint.quantify()`)
+
+.. note::
+   We recommend that you use the `cf-xarray <https://cf-xarray.readthedocs.io/en/latest/units.html>`_ registry for units,
+   as it implements geophysical units as `degree_north`, `degrees_north`, etc.
+   gsw-xarray internally uses `degree_north` and `degree_east` for latitude and longitude unit names.
+   If they are not found in the unit registry, they will be replaced by `degree`.
+
+   The function `gsw.SP_from_SK` uses part per thousand for SK. 'ppt' is already used for picopint,
+   so the expected unit is replaced by '1'.
+
+
+Xarray accessor
+...............
+
+gsw-xarray provides a new accessor for xarray, that allows to call the gsw **functions** directly on a dataset:
+
+.. code:: python
+
+   ds.gsw.sigma0(CT="CT", SA="SA")
+   # or
+   ds.gsw.sigma0(CT=ds.CT, SA=ds.SA)
+   # or even, if CT and SA have the proper standard names
+   ds.gsw.sigma0()
+
+Any type of mixte usage with dataArrays, numbers, strings, or autoparse with standard names is possible.
+
+If all arguments are present in the dataset with the proper standard name, it is possible to use the accessor with brackets, as if it was a dictionary
+
+.. code:: python
+
+   ds.gsw["sigma0"]
+   # Or if you want to get a list of multiple variables
+   ds.gsw[["sigma0", "alpha"]]
+
+If the dataset contains multiple variables with same standard name (e.g. practical salinity from bottle or CTD), you can set an option to tell gsw_xarray which variable to get:
+
+.. code:: python
+
+   # Globally
+   gsw_xarray.set_cf_name_preference(standard_name="variable_in_dataset")
+   # Or in a context, e.g.
+   with gsw_xarray.set_non_cf_name(sea_water_pressure="pres_adjusted"):
+       # write code here
+       pass
+   
+If you wish to use the accessor with automatic detection of arguments, but for a function whose arguments do not have a standard name, it is possible. You need to set an option in gsw-xarray, either in a context or globally
+
+.. code:: python
+
+   # Globally
+   gsw_xarray.set_non_cf_name(argument="argument_name_in_dataset")
+   # Or in a context, e.g.
+   with gsw_xarray.set_non_cf_name(Rt="Rt_in_ds"):
+       ds.gsw.SP_salinometer(t=0)
+
+In this 2nd case, the function ``gsw.SP_salinometer`` take the argument ``Rt`` which has no standard name.
+
+When using user set options, the order of priority to automatically get variables is: 1) variables set by ``gsw_xarray.set_cf_name_preference``, 2) variables with standard name (internal mapping), and 3) variables set by ``gsw_xarray.set_non_cf_name``.
+   
+Installation
+------------
+Pip
+...
+
+.. code:: bash
+
+    pip install gsw-xarray
+
+
+Conda
+.....
+
+Inside a conda environment:  ``conda install -c conda-forge gsw-xarray``.
+
+
+Citation
+--------
+
+If you use gsw-xarray, please cite the reference paper for the upstream gsw library:  McDougall, T.J. and P.M. Barker, 2011: Getting started with TEOS-10 and the Gibbs Seawater (GSW) Oceanographic Toolbox, 28pp., SCOR/IAPSO WG127, ISBN 978-0-646-55621-5
+
+.. code-block:: bibtex
+
+    @book{mcdougall2011getting,
+      author = {McDougall, T. J. and Barker, P. M.},
+      title = {Getting Started with TEOS-10 and the Gibbs Seawater (GSW) Oceanographic Toolbox},
+      year = {2011},
+      pages = {28},
+      publisher = {SCOR/IAPSO WG127},
+      isbn = {978-0-646-55621-5}
+    }
+
+You can also cite gsw-xarray by using the zenodo DOI |zenodo|.
+
+Contributor guide
+-----------------
+
+All contributions, bug reports, bug fixes, documentation improvements,
+enhancements, and ideas are welcome.
+If you notice a bug or are missing a feature, fell free
+to open an issue in the `GitHub issues page <https://github.com/DocOtak/gsw-xarray/issues>`_.
+
+In order to contribute to gsw-xarray, please fork the repository and
+submit a pull request. A good step by step tutorial for starting with git can be found in the
+`xarray contributor guide <https://xarray.pydata.org/en/stable/contributing.html#working-with-the-code>`_.
+A main difference is that we do not use conda as python environment, but poetry.
+
+Set up the environment
+......................
+
+You will first need to `install poetry <https://python-poetry.org/docs/#installation>`_.
+Then go to your local clone of gsw-xarray and launch installation:
+
+.. code:: bash
+
+   cd /path/to/your/gsw-xarray
+   poetry install --with dev
+
+You can then activate the environment by launching a shell
+within the virtual environment:
+
+.. code:: bash
+
+   poetry shell
+
+You can check that the tests pass locally:
+
+.. code:: bash
+
+   pytest gsw_xarray/tests
+
+You can install `pre-commit <https://pre-commit.com/#install>`_ to run the linting
+automatically at each commit.
+   
+Release (for maintainers only)
+..............................
+
+TODO...
```

### Comparing `gsw-xarray-0.3.0/PKG-INFO` & `gsw_xarray-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: gsw-xarray
-Version: 0.3.0
+Version: 0.4.0
 Summary: Drop in wrapper for gsw which adds CF standard name and units attributes to xarray results
 Home-page: https://github.com/DocOtak/gsw-xarray
 License: BSD-3-Clause
 Author: Andrew Barna
 Author-email: abarna@gmail.com
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: docs
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: pint
-Requires-Dist: Pint (>=0.18); extra == "pint"
-Requires-Dist: Sphinx (>=4.4.0); extra == "docs"
-Requires-Dist: furo (>=2022.1.2); extra == "docs"
+Requires-Dist: Pint (>=0.20) ; extra == "pint"
+Requires-Dist: cf-xarray (>=0.7.4,<0.8.0)
 Requires-Dist: gsw (>=3.4.0)
-Requires-Dist: pint-xarray (>=0.2.1,<0.3.0); extra == "pint"
+Requires-Dist: pint-xarray (>=0.3,<0.4) ; extra == "pint"
 Requires-Dist: xarray (>=0.20.2)
 Project-URL: Documentation, https://gsw-xarray.readthedocs.io/
 Project-URL: Repository, https://github.com/DocOtak/gsw-xarray
 Description-Content-Type: text/x-rst
 
 .. |CI Status| image:: https://github.com/docotak/gsw-xarray/actions/workflows/ci.yml/badge.svg
   :target: https://github.com/DocOtak/gsw-xarray/actions/workflows/ci.yml
@@ -31,27 +30,32 @@
   :target: https://gsw-xarray.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 .. |pypi| image:: https://badge.fury.io/py/gsw-xarray.svg
    :target: https://badge.fury.io/py/gsw-xarray
    :alt: pypi package
 .. |conda forge| image:: https://img.shields.io/conda/vn/conda-forge/gsw-xarray
    :target: https://anaconda.org/conda-forge/gsw-xarray
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8297618.svg
+   :target: https://doi.org/10.5281/zenodo.8297618
+   :alt: zenodo DOI
 
 gsw-xarray: Wrapper for gsw that adds CF attributes
 ===================================================
-|CI Status| |Documentation Status| |pypi| |conda forge|
+|CI Status| |Documentation Status| |pypi| |conda forge| |zenodo|
 
 gsw-xarray is a wrapper for `gsw python <https://github.com/TEOS-10/GSW-python>`_
 that will add CF attributes to xarray.DataArray outputs.
 It is meant to be a drop in wrapper for the upstream GSW-Python library and will only add these attributes if one argument to a function is an xarray.DataArray.
 
 You can find the documentation on `gsw-xarray.readthedocs.io <https://gsw-xarray.readthedocs.io/>`_.
 
 Usage
 -----
+Simple usage
+............
 
 .. code:: python
 
    import gsw_xarray as gsw
 
    # Create a xarray.Dataset
    import numpy as np
@@ -83,15 +87,17 @@
 
 Outputs
 
 ::
 
    <class 'numpy.ndarray'> [-5.08964499  2.1101098   9.28348219]
 
-
+Using Pint
+..........
+   
 We support (and convert the unit if necessary) the usage of pint.Quantities and the usage of xarray wrapped Quantities.
 Support for pint requires the installation of two optional dependencies: ``pint`` and ``pint-xarray``.
 If all the inputs to a gsw function are Quantities, the returned object will also be a Quantity belonging to the same UnitRegistry.
 
 .. warning::
 
    Quantities must all belong to the same pint.UnitRegistry, a ValueError will be thrown if there are mixed registries.
@@ -184,14 +190,62 @@
    gsw-xarray internally uses `degree_north` and `degree_east` for latitude and longitude unit names.
    If they are not found in the unit registry, they will be replaced by `degree`.
 
    The function `gsw.SP_from_SK` uses part per thousand for SK. 'ppt' is already used for picopint,
    so the expected unit is replaced by '1'.
 
 
+Xarray accessor
+...............
+
+gsw-xarray provides a new accessor for xarray, that allows to call the gsw **functions** directly on a dataset:
+
+.. code:: python
+
+   ds.gsw.sigma0(CT="CT", SA="SA")
+   # or
+   ds.gsw.sigma0(CT=ds.CT, SA=ds.SA)
+   # or even, if CT and SA have the proper standard names
+   ds.gsw.sigma0()
+
+Any type of mixte usage with dataArrays, numbers, strings, or autoparse with standard names is possible.
+
+If all arguments are present in the dataset with the proper standard name, it is possible to use the accessor with brackets, as if it was a dictionary
+
+.. code:: python
+
+   ds.gsw["sigma0"]
+   # Or if you want to get a list of multiple variables
+   ds.gsw[["sigma0", "alpha"]]
+
+If the dataset contains multiple variables with same standard name (e.g. practical salinity from bottle or CTD), you can set an option to tell gsw_xarray which variable to get:
+
+.. code:: python
+
+   # Globally
+   gsw_xarray.set_cf_name_preference(standard_name="variable_in_dataset")
+   # Or in a context, e.g.
+   with gsw_xarray.set_non_cf_name(sea_water_pressure="pres_adjusted"):
+       # write code here
+       pass
+   
+If you wish to use the accessor with automatic detection of arguments, but for a function whose arguments do not have a standard name, it is possible. You need to set an option in gsw-xarray, either in a context or globally
+
+.. code:: python
+
+   # Globally
+   gsw_xarray.set_non_cf_name(argument="argument_name_in_dataset")
+   # Or in a context, e.g.
+   with gsw_xarray.set_non_cf_name(Rt="Rt_in_ds"):
+       ds.gsw.SP_salinometer(t=0)
+
+In this 2nd case, the function ``gsw.SP_salinometer`` take the argument ``Rt`` which has no standard name.
+
+When using user set options, the order of priority to automatically get variables is: 1) variables set by ``gsw_xarray.set_cf_name_preference``, 2) variables with standard name (internal mapping), and 3) variables set by ``gsw_xarray.set_non_cf_name``.
+   
 Installation
 ------------
 Pip
 ...
 
 .. code:: bash
 
@@ -199,19 +253,32 @@
 
 
 Conda
 .....
 
 Inside a conda environment:  ``conda install -c conda-forge gsw-xarray``.
 
-Pipenv
-......
 
-Inside a pipenv environment: ``pipenv install gsw-xarray``.
+Citation
+--------
+
+If you use gsw-xarray, please cite the reference paper for the upstream gsw library:  McDougall, T.J. and P.M. Barker, 2011: Getting started with TEOS-10 and the Gibbs Seawater (GSW) Oceanographic Toolbox, 28pp., SCOR/IAPSO WG127, ISBN 978-0-646-55621-5
+
+.. code-block:: bibtex
+
+    @book{mcdougall2011getting,
+      author = {McDougall, T. J. and Barker, P. M.},
+      title = {Getting Started with TEOS-10 and the Gibbs Seawater (GSW) Oceanographic Toolbox},
+      year = {2011},
+      pages = {28},
+      publisher = {SCOR/IAPSO WG127},
+      isbn = {978-0-646-55621-5}
+    }
 
+You can also cite gsw-xarray by using the zenodo DOI |zenodo|.
 
 Contributor guide
 -----------------
 
 All contributions, bug reports, bug fixes, documentation improvements,
 enhancements, and ideas are welcome.
 If you notice a bug or are missing a feature, fell free
@@ -227,27 +294,30 @@
 
 You will first need to `install poetry <https://python-poetry.org/docs/#installation>`_.
 Then go to your local clone of gsw-xarray and launch installation:
 
 .. code:: bash
 
    cd /path/to/your/gsw-xarray
-   poetry install
+   poetry install --with dev
 
 You can then activate the environment by launching a shell
 within the virtual environment:
 
 .. code:: bash
 
    poetry shell
 
 You can check that the tests pass locally:
 
 .. code:: bash
 
    pytest gsw_xarray/tests
 
+You can install `pre-commit <https://pre-commit.com/#install>`_ to run the linting
+automatically at each commit.
+   
 Release (for maintainers only)
 ..............................
 
 TODO...
```

