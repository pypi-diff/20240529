# Comparing `tmp/rms_solar-1.0.2.tar.gz` & `tmp/rms_solar-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms_solar-1.0.2.tar", last modified: Tue May 14 19:18:42 2024, max compression
+gzip compressed data, was "rms_solar-2.0.0.tar", last modified: Wed May 29 18:25:37 2024, max compression
```

## Comparing `rms_solar-1.0.2.tar` & `rms_solar-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:42.002262 rms_solar-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:41.998263 rms_solar-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:41.998263 rms_solar-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:18:23.000000 rms_solar-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:18:23.000000 rms_solar-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-14 19:18:23.000000 rms_solar-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:18:23.000000 rms_solar-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-14 19:18:42.002262 rms_solar-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-14 19:18:23.000000 rms_solar-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-14 19:18:23.000000 rms_solar-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 19:18:23.000000 rms_solar-1.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:42.002262 rms_solar-1.0.2/rms_solar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:18:41.000000 rms_solar-1.0.2/rms_solar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 19:18:42.006262 rms_solar-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:42.002262 rms_solar-1.0.2/solar/
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:18:41.000000 rms_solar-1.0.2/solar/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    36381 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/colina.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:42.002262 rms_solar-1.0.2/solar/data_files/
--rw-r--r--   0 runner    (1001) docker     (127)  1155314 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/data_files/kurucz-fsunallp.2000resam125.txt
--rw-r--r--   0 runner    (1001) docker     (127)   118080 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/data_files/rieke-solar_spec.fits
--rw-r--r--   0 runner    (1001) docker     (127)    37440 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/data_files/stis-sun_reference_stis_002.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/kurucz.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/rieke.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/stis.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/stis_rieke.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-14 19:18:23.000000 rms_solar-1.0.2/solar/test_solar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:25:37.395779 rms_solar-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 18:25:08.000000 rms_solar-2.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-29 18:25:08.000000 rms_solar-2.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:25:37.391779 rms_solar-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-29 18:25:08.000000 rms_solar-2.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:25:37.391779 rms_solar-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-29 18:25:08.000000 rms_solar-2.0.0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-29 18:25:08.000000 rms_solar-2.0.0/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-29 18:25:08.000000 rms_solar-2.0.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-29 18:25:08.000000 rms_solar-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 18:25:08.000000 rms_solar-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-29 18:25:08.000000 rms_solar-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-29 18:25:08.000000 rms_solar-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 18:25:08.000000 rms_solar-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-29 18:25:37.395779 rms_solar-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-29 18:25:08.000000 rms_solar-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:25:37.391779 rms_solar-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 18:25:08.000000 rms_solar-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 18:25:08.000000 rms_solar-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-29 18:25:08.000000 rms_solar-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-29 18:25:08.000000 rms_solar-2.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 18:25:08.000000 rms_solar-2.0.0/docs/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-29 18:25:08.000000 rms_solar-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 18:25:08.000000 rms_solar-2.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:25:37.395779 rms_solar-2.0.0/rms_solar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-29 18:25:37.000000 rms_solar-2.0.0/rms_solar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-29 18:25:37.000000 rms_solar-2.0.0/rms_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:25:37.000000 rms_solar-2.0.0/rms_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-29 18:25:37.000000 rms_solar-2.0.0/rms_solar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 18:25:37.000000 rms_solar-2.0.0/rms_solar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 18:25:37.395779 rms_solar-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:25:37.395779 rms_solar-2.0.0/solar/
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/_fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 18:25:37.000000 rms_solar-2.0.0/solar/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39278 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/colina.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:25:37.395779 rms_solar-2.0.0/solar/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)  1155314 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/data_files/kurucz-fsunallp.2000resam125.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   118080 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/data_files/rieke-solar_spec.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    37440 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/data_files/stis-sun_reference_stis_002.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/kurucz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/rieke.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/stis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-29 18:25:08.000000 rms_solar-2.0.0/solar/stis_rieke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:25:37.395779 rms_solar-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-05-29 18:25:08.000000 rms_solar-2.0.0/tests/test_solar.py
```

### Comparing `rms_solar-1.0.2/.github/workflows/publish_to_pypi.yml` & `rms_solar-2.0.0/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/.github/workflows/publish_to_test_pypi.yml` & `rms_solar-2.0.0/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/.github/workflows/run-tests.yml` & `rms_solar-2.0.0/.github/workflows/run-tests.yml`

 * *Files 21% similar despite different names*

```diff
@@ -7,21 +7,35 @@
     branches: [ main ]
   push:
     branches: [ main ]
   schedule:
     - cron: "21 11 * * 0"
 
 jobs:
+  flake8:
+    name: Flake8 solar
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+        with:
+          ref: ${{ github.event.pull_request.head.sha }}
+
+      - name: Flake8
+        run: |
+          pip install flake8
+          flake8 solar tests
+
   test:
     name: Test solar
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
       fail-fast: false
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
```

### Comparing `rms_solar-1.0.2/.gitignore` & `rms_solar-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/CODE_OF_CONDUCT.md` & `rms_solar-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/CONTRIBUTING.md` & `rms_solar-2.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/LICENSE` & `rms_solar-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/pyproject.toml` & `rms_solar-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Microsoft :: Windows"
 ]
 
 [project.urls]
 Homepage = "https://github.com/SETI/rms-solar"
+Documentation = "https://rms-solar.readthedocs.io/en/latest"
 Repository = "https://github.com/SETI/rms-solar"
 Source = "https://github.com/SETI/rms-solar"
 Issues = "https://github.com/SETI/rms-solar/issues"
 
 [tool.setuptools]
 packages = ["solar"]
```

### Comparing `rms_solar-1.0.2/rms_solar.egg-info/SOURCES.txt` & `rms_solar-2.0.0/rms_solar.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 .coveragerc
+.flake8
 .gitignore
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
+.github/pull_request_template.md
 .github/workflows/publish_to_pypi.yml
 .github/workflows/publish_to_test_pypi.yml
 .github/workflows/run-tests.yml
+docs/Makefile
+docs/conf.py
+docs/index.rst
+docs/make.bat
+docs/module.rst
 rms_solar.egg-info/PKG-INFO
 rms_solar.egg-info/SOURCES.txt
 rms_solar.egg-info/dependency_links.txt
 rms_solar.egg-info/requires.txt
 rms_solar.egg-info/top_level.txt
 solar/__init__.py
+solar/_fake.py
 solar/_version.py
 solar/colina.py
 solar/kurucz.py
 solar/rieke.py
 solar/stis.py
 solar/stis_rieke.py
-solar/test_solar.py
 solar/data_files/kurucz-fsunallp.2000resam125.txt
 solar/data_files/rieke-solar_spec.fits
-solar/data_files/stis-sun_reference_stis_002.fits
+solar/data_files/stis-sun_reference_stis_002.fits
+tests/test_solar.py
```

### Comparing `rms_solar-1.0.2/solar/__init__.py` & `rms_solar-2.0.0/solar/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,49 @@
-################################################################################
-# solar/__init__.py: Models for the solar flux density at 1 AU.
-#
-# Models currently supported are:
-#   Colina      0.1195 to 2.5 micron
-#   Kurucz      0.15   to 300 micron
-#   Rieke       0.2    to 30  micron
-#   STIS        0.1195 to 2.7 micron
-#   STIS_Rieke  0.1195 to 30  micron
-################################################################################
+"""
+Models for solar flux density at a given distance from the Sun.
+
+This module provides access to various models of solar flux density. Models
+currently supported are:
 
-__all__ = []    # don't import any solar models by default, only as requested.
+- Colina      (0.1195 to 2.5 micron)
+- Kurucz      (0.15   to 300 micron)
+- Rieke       (0.2    to 30  micron)
+- STIS        (0.1195 to 2.7 micron)
+- STIS_Rieke  (0.1195 to 30  micron)
+
+The solar flux density can be returned directly in the form of a Tabulation
+object (see the package `rms-tabulation <https://pypi.org/project/rms-tabulation>`_
+or the mean flux density can be returned over a particular filter bandwith. In
+each case you can specify the model to use, the units for wavelength and flux
+density, the distance from the Sun, and whether or not to return just F instead
+of flux density.
+"""
+
+# When a user does a wildcard import (from solar import *), don't import any
+# solar models by default; but DO export the public interface functions and
+# variables.
+__all__ = ['flux_density', 'bandpass_flux_density', 'mean_flux_density',
+           'bandpass_f', 'mean_f', 'AU', 'C', 'TO_CGS', 'TO_PER_ANGSTROM',
+           'TO_PER_NM']
 
 import functools
 import importlib
 import numpy as np
 import tabulation as tab
 
 try:
     from ._version import __version__
-except ImportError as err:
+except ImportError:
     __version__ = 'Version unspecified'
 
 
 # Class constants to be used externally as needed
-AU = 149597870.7    # km
-C = 299792.458      # km/sec
+AU = 149597870.7       # km
+C = 299792.458         # km/sec
+C_IN_UM_HZ = C * 1.e9  # um/sec
 
 # Converts from W/m^2 to erg/s/cm^2
 TO_CGS = 1.e7 / 1.e4
 
 # Converts from flux per micron to flux per Angstrom
 TO_PER_ANGSTROM = 1.e-4
 
@@ -56,54 +71,58 @@
 XUNIT_DICT = {
     'um': (1.  , True),
     'nm': (1.e3, True),
     'A' : (1.e4, True),
     'Hz': (1.  , False),
 }
 
-C_IN_UM_HZ = C * 1.e9
 
 #===============================================================================
 @functools.lru_cache(maxsize=4)
-def flux_density(model='STIS_Rieke', units='W/m^2/um', xunits='um',
+def flux_density(model='STIS_Rieke', *, units='W/m^2/um', xunits='um',
                  sun_range=1., solar_f=False):
-    """A Tabulation of solar flux density at 1 AU in the specified units.
-
-    Note that the tabulation is always returned in units of microns.
+    """
+    Compute the flux density of a solar model in the specified units.
 
-    Input:
-        model           name of the model, default "STIS_Rieke".
-        units           units to provide, default "W/m^2/um". Options are:
-                        "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
-                        "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz",
-                        "erg/s/cm^2/Hz", "Jy", "uJy".
-        xunits          units for the x-axis, default "um" (for microns).
-                        Options are: "um", "nm", "A", or "Hz".
-        sun_range       optional distance from Sun to target in AU.
-        solar_f         True to divide by pi, providing solar F instead of
-                        solar flux density.
+    Args:
+        model (str, optional): Name of the model.
+        units (str, optional): Units for the flux.
+            Options are: "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
+            "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz", "erg/s/cm^2/Hz", "Jy",
+            or "uJy". "u" represents "mu" meaning micro.
+        xunits (str, optional): Units for the x-axis.
+            Options are: "um", "nm", "A", or "Hz". "u" represents "mu"
+            meaning micro.
+        sun_range (float, optional): Distance from Sun to target in AU.
+        solar_f (bool, optional): True to divide by pi, providing solar F
+            instead of solar flux density.
 
-    Return:             a Tabulation of the model solar flux density in the
-                        specified units.
+    Returns:
+        Tabulation: The model solar flux density in the specified units.
     """
 
     # Each reference to a named model triggers the import of its associated
     # Python file hosts/solar/<name>.py, referenced as "solar.<name>"
     # here. Note that modules are imported only if requested, not by default.
     try:
-        module = importlib.import_module('solar.' + model.lower())
+        module = importlib.import_module(f'solar.{model.lower()}')
     except ImportError:
-        raise ValueError('undefined solar model: ' + model)
+        raise ValueError(f'undefined solar model: {model} (valid models are: '
+                         'colina, kurucz, rieke, stis_rieke, stis)')
 
     # Check units
     if units not in UNIT_DICT:
-        raise ValueError('invalid units: ' + units)
+        valid_units = ', '.join(UNIT_DICT.keys())
+        raise ValueError(f'invalid units: {units} (valid units are: '
+                         f'{valid_units})')
 
     if xunits not in XUNIT_DICT:
-        raise ValueError('invalid units: ' + xunits)
+        valid_xunits = ', '.join(XUNIT_DICT.keys())
+        raise ValueError(f'invalid units: {xunits} (valid units are: '
+                         f'{valid_xunits})')
 
     # Get the tabulation
     tabulation = module.FLUX_DENSITY
 
     # If we have the desired units, return
     if units == module.UNITS and xunits == module.XUNITS:
         return tabulation * ((1./np.pi if solar_f else 1.) / sun_range**2)
@@ -145,166 +164,188 @@
         # or
         #   |dw/df| = C/f^2 = w^2/C
 
         if per_wavelength:  # we need df/dw
             if model_x_is_wavelength:  # pragma: no cover
                 new_y = ((factor * C_IN_UM_HZ * model_xscale**2) *
                          tabulation.y / tabulation.x**2)
-            else:  # pragma: no cover
-                # There are currently no models in Hz
+            else:  # pragma: no cover - There are currently no models in Hz
                 new_y = ((factor / C_IN_UM_HZ / model_xscale**2) *
                          tabulation.y * tabulation.x**2)
 
         else:               # we need dw/df
             if model_x_is_wavelength:  # pragma: no cover
                 new_y = ((factor / C_IN_UM_HZ / model_xscale**2) *
                          tabulation.y * tabulation.x**2)
-            else:  # pragma: no cover
-                # There are currently no models in Hz
+            else:  # pragma: no cover - There are currently no models in Hz
                 new_y = ((factor * C_IN_UM_HZ * model_xscale**2) *
                          tabulation.y / tabulation.x**2)
 
     return tab.Tabulation(new_x, new_y)
 
 #===============================================================================
-def bandpass_flux_density(bandpass, model='STIS_Rieke', units='W/m^2/um',
-                                    xunits='um', sun_range=1., solar_f=False):
-    """The solar flux density averaged over a filter bandpass.
-
-    Input:
-        bandpass        the Tabulation of the filter bandpass, with wavelength
-                        in microns. Alternatively, a tuple of two arrays
-                        (wavelength, flux), each of the same size.
-        model           name of the model, default "STIS_Rieke". Alternatively,
-                        a Tabulation of the solar flux density, in which case it
-                        must be in the desired units already, and must be
-                        tabulated in the same units as the bandpass.
-        units           units to provide, default "W/m^2/um". Options are:
-                        "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
-                        "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz",
-                        "erg/s/cm^2/Hz", "Jy", "uJy". Ignored if the solar model
-                        is a Tabulation.
-        xunits          units for the x-axis of the bandpass, default "um" (for
-                        microns). Options are: "um", "nm", "A", or "Hz".
-        sun_range       optional distance from Sun to target in AU.
-        solar_f         True to divide by pi, providing solar F instead of
-                        solar flux density.
+def bandpass_flux_density(bandpass, model='STIS_Rieke', *, units='W/m^2/um',
+                          xunits='um', sun_range=1., solar_f=False):
+    """
+    Compute the average solar flux density over a filter bandpass.
 
-    Return:             the mean solar flux density or solar F within the filter
-                        bandpass.
+    Args:
+        bandpass (Tabulation or tuple): The Tabulation of the filter bandpass,
+            with wavelength in units specified by `xunits` (if `model` is a
+            string) or in the same units as `model` (if `model` is a
+            Tabulation). Alternatively, a tuple of two arrays (wavelength,
+            fraction), each of the same size.
+        model (str or Tabulation, optional): Name of the model. Alternatively, a
+            Tabulation of the solar flux density, already in the desired units.
+        units (str, optional): Units for the flux.
+            Options are: "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
+            "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz", "erg/s/cm^2/Hz", "Jy",
+            or "uJy". "u" represents "mu" meaning micro. Ignored if `model` is a
+            Tabulation.
+        xunits (str, optional): Units for the x-axis.
+            Options are: "um", "nm", "A", or "Hz". "u" represents "mu" meaning
+            micro. Ignored if `model` is a Tabulation.
+        sun_range (float, optional): Distance from Sun to target in AU.
+        solar_f (bool, optional): True to divide by pi, providing solar F
+            instead of solar flux density.
+
+    Returns:
+        float: The mean solar flux density or solar F within the filter
+        bandpass.
+
+    Note:
+        If the bandpass of the filter is wider than the wavelength coverage of
+        the selected solar model, the computation will be restricted to the
+        wavelength range that is in common between the filter and the model.
     """
 
     if not isinstance(bandpass, tab.Tabulation):
         bandpass = tab.Tabulation(*bandpass)
 
     if isinstance(model, tab.Tabulation):
         flux = model * (1./np.pi if solar_f else 1.) / sun_range**2
     else:
         flux = flux_density(model, units=units, xunits=xunits,
-                                   sun_range=sun_range, solar_f=solar_f)
+                            sun_range=sun_range, solar_f=solar_f)
 
     # Multiply together the bandpass and the solar spectrum Tabulations
     product = bandpass * flux
 
     # Resample the bandpass at the same wavelengths for a more reliable
     # normalization
     bandpass = bandpass.resample(product.x)
 
     # Return the ratio of integrals
     return product.integral() / bandpass.integral()
 
 #===============================================================================
-def mean_flux_density(center, width, model='STIS_Rieke', units='W/m^2/um',
-                                     xunits='um', sun_range=1., solar_f=False):
-    """The solar flux density averaged over the bandpass of a "boxcar" filter,
-    given its center and full width.
-
-    Input:
-        center          the center of the bandpass.
-        width           the full width of the bandpass.
-        model           name of the model, default "STIS_Rieke". Alternatively,
-                        a Tabulation of the solar flux density, in which case it
-                        must be in the desired units already, and must be
-                        tabulated in the same units as the bandpass.
-        units           units to provide, default "W/m^2/um". Options are:
-                        "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
-                        "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz",
-                        "erg/s/cm^2/Hz", "Jy", "microJy", "uJy". Ignored if the
-                        solar model is a Tabulation.
-        xunits          units for bandpass center and width. Options are: "um"
-                        (for microns), "nm", "A", or "Hz". Default is "um".
-        sun_range       optional distance from Sun to target in AU.
-        solar_f         True to divide by pi, providing solar F instead of
-                        solar flux density.
+def mean_flux_density(center, width, model='STIS_Rieke', *, units='W/m^2/um',
+                      xunits='um', sun_range=1., solar_f=False):
+    """
+    Compute average solar flux density over the bandpass of a "boxcar" filter.
 
-    Return:             the mean solar flux density or solar F within the filter
-                        bandpass.
+    Args:
+        center (float): The center of the bandpass (microns).
+        width (float): The full width of the bandpass (microns).
+        model (str or Tabulation, optional): Name of the model. Alternatively, a
+            Tabulation of the solar flux density, already in the desired units.
+        units (str, optional): Units for the flux.
+            Options are: "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
+            "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz", "erg/s/cm^2/Hz", "Jy",
+            or "uJy". "u" represents "mu" meaning micro. Ignored if `model` is a
+            Tabulation.
+        xunits (str, optional): Units for the x-axis.
+            Options are: "um", "nm", "A", or "Hz". "u" represents "mu" meaning
+            micro. Ignored if `model` is a Tabulation.
+        sun_range (float, optional): Distance from Sun to target in AU.
+        solar_f (bool, optional): True to divide by pi, providing solar F
+            instead of solar flux density.
+
+    Returns:
+        float: The mean solar flux density or solar F within the filter bandpass.
+
+    Note:
+        If the bandpass of the filter is wider than the wavelength coverage
+        of the selected solar model, the computation will be restricted to the
+        wavelength range that is in common between the filter and the model.
     """
 
     # Create a boxcar filter Tabulation
-    bandpass = tab.Tabulation((center - width/2., center + width/2.), (1.,1.))
+    bandpass = tab.Tabulation((center - width/2., center + width/2.), (1., 1.))
 
     # Return the mean over the filter
     return bandpass_flux_density(bandpass, model=model, units=units,
-                                           xunits=xunits, sun_range=sun_range,
-                                           solar_f=solar_f)
+                                 xunits=xunits, sun_range=sun_range,
+                                 solar_f=solar_f)
 
 #===============================================================================
-def bandpass_f(bandpass, model='STIS_Rieke', units='W/m^2/um', xunits='um',
-                         sun_range=1.):
-    """Solar F averaged over a filter bandpass.
-
-    F is defined such that pi*F is the solar flux density.
-
-    Input:
-        bandpass        the Tabulation of the filter bandpass, with wavelength
-                        in microns. Alternatively, a tuple of two arrays
-                        (wavelength, flux), each of the same size.
-        model           name of the model, default "STIS_Rieke". Alternatively,
-                        a Tabulation of the solar flux density, in which case it
-                        must be in the desired units already, and must be
-                        tabulated in the same units as the bandpass.
-        units           units to provide, default "W/m^2/um". Options are:
-                        "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
-                        "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz",
-                        "erg/s/cm^2/Hz", "Jy", "uJy". Ignored if the solar model
-                        is a Tabulation.
-        xunits          units for the x-axis of the bandpass, default "um" (for
-                        microns). Options are: "um", "nm", "A", or "Hz".
-        sun_range       optional distance from Sun to target in AU.
+def bandpass_f(bandpass, model='STIS_Rieke', *, units='W/m^2/um', xunits='um',
+               sun_range=1.):
+    """
+    Compute the solar F averaged over a filter bandpass.
 
-    Return:             the mean solar F within the filter bandpass.
+    Args:
+        bandpass (Tabulation or tuple): The Tabulation of the filter bandpass,
+            with wavelength in units specified by `xunits` (if `model` is a
+            string) or in the same units as `model` (if `model` is a
+            Tabulation). Alternatively, a tuple of two arrays (wavelength,
+            fraction), each of the same size.
+        model (str or Tabulation, optional): Name of the model. Alternatively, a
+            Tabulation of the solar flux density, already in the desired units.
+        units (str, optional): Units for the flux.
+            Options are: "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
+            "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz", "erg/s/cm^2/Hz", "Jy",
+            or "uJy". "u" represents "mu" meaning micro. Ignored if `model` is a
+            Tabulation.
+        xunits (str, optional): Units for the x-axis.
+            Options are: "um", "nm", "A", or "Hz". "u" represents "mu" meaning
+            micro. Ignored if `model` is a Tabulation.
+        sun_range (float, optional): Distance from Sun to target in AU.
+
+    Returns:
+        float: The mean solar F within the filter bandpass.
+
+    Note:
+        If the bandpass of the filter is wider than the wavelength coverage
+        of the selected solar model, the computation will be restricted to the
+        wavelength range that is in common between the filter and the model.
     """
 
     return bandpass_flux_density(bandpass, model=model, units=units,
                                  xunits=xunits, sun_range=sun_range,
                                  solar_f=True)
 
 #===============================================================================
-def mean_f(center, width, model='STIS_Rieke', units='W/m^2/um', xunits='um',
-                          sun_range=1.):
-    """The solar F averaged over the bandpass of a "boxcar" filter, given its
-    center and full width.
-
-    Input:
-        center          the center of the bandpass.
-        width           the full width of the bandpass.
-        model           name of the model, default "STIS_Rieke". Alternatively,
-                        a Tabulation of the solar flux density, in which case it
-                        must be in the desired units already, and must be
-                        tabulated in the same units as the bandpass.
-        units           units to provide, default "W/m^2/um". Options are:
-                        "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
-                        "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz",
-                        "erg/s/cm^2/Hz", "Jy", "uJy". Ignored if the solar model
-                        is a Tabulation.
-        xunits          units for bandpass center and width. Options are: "um"
-                        (for microns), "nm", "A", or "Hz". Default is "um".
-        sun_range       optional distance from Sun to target in AU.
+def mean_f(center, width, model='STIS_Rieke', *, units='W/m^2/um', xunits='um',
+           sun_range=1.):
+    """
+    Compute average solar F over the bandpass of a "boxcar" filter.
 
-    Return:             the mean solar F within the specified bandpass.
+    Args:
+        center (float): The center of the bandpass (microns).
+        width (float): The full width of the bandpass (microns).
+        model (str or Tabulation, optional): Name of the model. Alternatively, a
+            Tabulation of the solar flux density, already in the desired units.
+        units (str, optional): Units for the flux.
+            Options are: "W/m^2/um", "W/m^2/nm", "W/m^2/A", "erg/s/cm^2/um",
+            "erg/s/cm^2/nm", "erg/s/cm^2/A", "W/m^2/Hz", "erg/s/cm^2/Hz", "Jy",
+            or "uJy". "u" represents "mu" meaning micro. Ignored if `model` is a
+            Tabulation.
+        xunits (str, optional): Units for the x-axis.
+            Options are: "um", "nm", "A", or "Hz". "u" represents "mu" meaning
+            micro. Ignored if `model` is a Tabulation.
+        sun_range (float, optional): Distance from Sun to target in AU.
+
+    Returns:
+        float: The mean solar flux density or solar F within the filter
+        bandpass.
+
+    Note:
+        If the bandpass of the filter is wider than the wavelength coverage
+        of the selected solar model, the computation will be restricted to the
+        wavelength range that is in common between the filter and the model.
     """
 
     return mean_flux_density(center, width, model=model, units=units,
                              xunits=xunits, sun_range=sun_range, solar_f=True)
 
 ################################################################################
```

### Comparing `rms_solar-1.0.2/solar/data_files/kurucz-fsunallp.2000resam125.txt` & `rms_solar-2.0.0/solar/data_files/kurucz-fsunallp.2000resam125.txt`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/solar/data_files/rieke-solar_spec.fits` & `rms_solar-2.0.0/solar/data_files/rieke-solar_spec.fits`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/solar/data_files/stis-sun_reference_stis_002.fits` & `rms_solar-2.0.0/solar/data_files/stis-sun_reference_stis_002.fits`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/solar/kurucz.py` & `rms_solar-2.0.0/solar/kurucz.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 RSUN = 695700.
 FACTOR = 4 * np.pi * (RSUN/solar.AU)**2
 
 # Read the file
 filepath = os.path.join(os.path.split(solar.__file__)[0],
                         'data_files', 'kurucz-fsunallp.2000resam125.txt')
 array = np.fromfile(filepath, sep=' ')
-array = array.reshape(-1,3)
+array = array.reshape(-1, 3)
 
 # column 1 is wavelength in nm
 # column 2 "flux moment"; see notes above for conversion
 
-wavelength = array[:,0]
-flux = array[:,1] * FACTOR
+wavelength = array[:, 0]
+flux = array[:, 1] * FACTOR
 
 FLUX_DENSITY = tab.Tabulation(wavelength, flux)
 UNITS = 'W/m^2/um'
 XUNITS = 'nm'
 
 ################################################################################
```

### Comparing `rms_solar-1.0.2/solar/rieke.py` & `rms_solar-2.0.0/solar/rieke.py`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/solar/stis.py` & `rms_solar-2.0.0/solar/stis.py`

 * *Files identical despite different names*

### Comparing `rms_solar-1.0.2/solar/stis_rieke.py` & `rms_solar-2.0.0/solar/stis_rieke.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ################################################################################
 # solar/stis_rieke.py: STIS and Rieke models merged.
 ################################################################################
 
 import numpy as np
 
-import solar.stis  as stis
+import solar.stis as stis
 import solar.rieke as rieke
 
 import tabulation as tab
 
-assert stis.UNITS  == rieke.UNITS
+assert stis.UNITS == rieke.UNITS
 assert stis.XUNITS == rieke.XUNITS
 
 tab1 = stis.FLUX_DENSITY
 tab2 = rieke.FLUX_DENSITY
 
 mask = (tab2.x > np.max(tab1.x))
```

