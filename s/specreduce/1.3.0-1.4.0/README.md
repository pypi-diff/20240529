# Comparing `tmp/specreduce-1.3.0.tar.gz` & `tmp/specreduce-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specreduce-1.3.0.tar", last modified: Mon Dec  5 19:15:51 2022, max compression
+gzip compressed data, was "specreduce-1.4.0.tar", last modified: Wed May 29 20:10:34 2024, max compression
```

## Comparing `specreduce-1.3.0.tar` & `specreduce-1.4.0.tar`

### file list

```diff
@@ -1,97 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.380611 specreduce-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.352609 specreduce-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.360609 specreduce-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2022-12-05 19:15:30.000000 specreduce-1.3.0/.github/workflows/cron-tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)      556 2022-12-05 19:15:30.000000 specreduce-1.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2022-12-05 19:15:30.000000 specreduce-1.3.0/.github/workflows/tox-tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)      735 2022-12-05 19:15:30.000000 specreduce-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      296 2022-12-05 19:15:30.000000 specreduce-1.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2022-12-05 19:15:30.000000 specreduce-1.3.0/CHANGES.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)     1137 2022-12-05 19:15:30.000000 specreduce-1.3.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (122)      300 2022-12-05 19:15:30.000000 specreduce-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1346 2022-12-05 19:15:51.380611 specreduce-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      932 2022-12-05 19:15:30.000000 specreduce-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.360609 specreduce-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     4581 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.352609 specreduce-1.3.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.360609 specreduce-1.3.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (122)      250 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (122)      251 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (122)      453 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)   212432 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/atm_transmission_secz1.5_1.6mm.dat
--rw-r--r--   0 runner    (1001) docker     (122)     7396 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4987 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/extinction.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/extraction_quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.364610 specreduce-1.3.0/docs/process/
--rw-r--r--   0 runner    (1001) docker     (122)    13015 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_MOS_arc.odg
--rw-r--r--   0 runner    (1001) docker     (122)    31208 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_MOS_arc.svg
--rw-r--r--   0 runner    (1001) docker     (122)    15565 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_MOS_flat.odg
--rw-r--r--   0 runner    (1001) docker     (122)    95754 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_MOS_flat.svg
--rw-r--r--   0 runner    (1001) docker     (122)    16067 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_MOS_science.odg
--rw-r--r--   0 runner    (1001) docker     (122)    54471 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_MOS_science.svg
--rw-r--r--   0 runner    (1001) docker     (122)    13131 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_MOS_trace.odg
--rw-r--r--   0 runner    (1001) docker     (122)    37781 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_MOS_trace.svg
--rw-r--r--   0 runner    (1001) docker     (122)      341 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_arcs.rst
--rw-r--r--   0 runner    (1001) docker     (122)      563 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_flats.rst
--rw-r--r--   0 runner    (1001) docker     (122)      467 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/NIR_science_data.rst
--rw-r--r--   0 runner    (1001) docker     (122)      824 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/process/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10460 2022-12-05 19:15:30.000000 specreduce-1.3.0/docs/specphot_standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.364610 specreduce-1.3.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2022-12-05 19:15:30.000000 specreduce-1.3.0/licenses/KOSMOS_LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2022-12-05 19:15:30.000000 specreduce-1.3.0/licenses/LICENSE.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.372610 specreduce-1.3.0/notebook_sandbox/
--rw-r--r--   0 runner    (1001) docker     (122)      181 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/README.md
--rw-r--r--   0 runner    (1001) docker     (122)  6658120 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/apo05.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     9455 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/compare_extractions.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   800893 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   351192 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/flatfield_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   136888 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/fluxcal_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.376610 specreduce-1.3.0/notebook_sandbox/horne_extract/
--rw-r--r--   0 runner    (1001) docker     (122)   594535 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/horne_extract/optimal_extract_VLT.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)       44 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/horne_extract/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)   134401 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/identify_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.376610 specreduce-1.3.0/notebook_sandbox/jwst_boxcar/
--rw-r--r--   0 runner    (1001) docker     (122)   154703 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/jwst_boxcar/boxcar_extraction.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   327528 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/jwst_boxcar/jwst_boxcar_algorithm.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/jwst_boxcar/pre-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      465 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/jwst_boxcar/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)    97320 2022-12-05 19:15:30.000000 specreduce-1.3.0/notebook_sandbox/tracing_options.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)      227 2022-12-05 19:15:30.000000 specreduce-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2022-12-05 19:15:51.380611 specreduce-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1601 2022-12-05 19:15:30.000000 specreduce-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.376610 specreduce-1.3.0/specreduce/
--rw-r--r--   0 runner    (1001) docker     (122)      395 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      377 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (122)    12548 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/background.py
--rw-r--r--   0 runner    (1001) docker     (122)    14482 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/calibration_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22404 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)    11762 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/fluxcal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1652 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.380611 specreduce-1.3.0/specreduce/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4462 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/test_background.py
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/test_extinction.py
--rw-r--r--   0 runner    (1001) docker     (122)     7685 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/test_get_reference_file_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     4598 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/test_image_parsing.py
--rw-r--r--   0 runner    (1001) docker     (122)      740 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/test_specphot_stds.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/test_synth_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4514 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tests/test_tracing.py
--rw-r--r--   0 runner    (1001) docker     (122)    14371 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.380611 specreduce-1.3.0/specreduce/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2022-12-05 19:15:30.000000 specreduce-1.3.0/specreduce/utils/synth_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-12-05 19:15:51.000000 specreduce-1.3.0/specreduce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 19:15:51.376610 specreduce-1.3.0/specreduce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1346 2022-12-05 19:15:51.000000 specreduce-1.3.0/specreduce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2022-12-05 19:15:51.000000 specreduce-1.3.0/specreduce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 19:15:51.000000 specreduce-1.3.0/specreduce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 19:15:51.000000 specreduce-1.3.0/specreduce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      124 2022-12-05 19:15:51.000000 specreduce-1.3.0/specreduce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-12-05 19:15:51.000000 specreduce-1.3.0/specreduce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3044 2022-12-05 19:15:30.000000 specreduce-1.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.282739 specreduce-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 20:10:24.000000 specreduce-1.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.266738 specreduce-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.270738 specreduce-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-29 20:10:24.000000 specreduce-1.4.0/.github/workflows/cron-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-29 20:10:24.000000 specreduce-1.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-29 20:10:24.000000 specreduce-1.4.0/.github/workflows/tox-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-29 20:10:24.000000 specreduce-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 20:10:24.000000 specreduce-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-29 20:10:24.000000 specreduce-1.4.0/CHANGES.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1321 2024-05-29 20:10:24.000000 specreduce-1.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 20:10:24.000000 specreduce-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-29 20:10:34.282739 specreduce-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-29 20:10:24.000000 specreduce-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-29 20:10:24.000000 specreduce-1.4.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.270738 specreduce-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.274739 specreduce-1.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/_static/logo_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    62134 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/_static/logo_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/_static/specreduce.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.266738 specreduce-1.4.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.274739 specreduce-1.4.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   212432 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/atm_transmission_secz1.5_1.6mm.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/extinction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/extraction_quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.274739 specreduce-1.4.0/docs/process/
+-rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_MOS_arc.odg
+-rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_MOS_arc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_MOS_flat.odg
+-rw-r--r--   0 runner    (1001) docker     (127)    95754 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_MOS_flat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_MOS_science.odg
+-rw-r--r--   0 runner    (1001) docker     (127)    54471 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_MOS_science.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_MOS_trace.odg
+-rw-r--r--   0 runner    (1001) docker     (127)    37781 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_MOS_trace.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_arcs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_flats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/NIR_science_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/process/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10447 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/specphot_standards.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/terms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-29 20:10:24.000000 specreduce-1.4.0/docs/wavelength_calibration.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.274739 specreduce-1.4.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-29 20:10:24.000000 specreduce-1.4.0/licenses/KOSMOS_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-29 20:10:24.000000 specreduce-1.4.0/licenses/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-29 20:10:25.000000 specreduce-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:10:34.282739 specreduce-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.278739 specreduce-1.4.0/specreduce/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14335 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19473 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/calibration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36677 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/fluxcal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/line_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.282739 specreduce-1.4.0/specreduce/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.282739 specreduce-1.4.0/specreduce/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    72000 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/data/transposed_det_image_seq5_MIRIMAGE_P750Lexp1_s2d.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_extinction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_get_reference_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_image_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_line_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_linelists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_specphot_stds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_synth_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tests/test_wavelength_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15646 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.282739 specreduce-1.4.0/specreduce/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/utils/synth_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 20:10:34.000000 specreduce-1.4.0/specreduce/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-05-29 20:10:25.000000 specreduce-1.4.0/specreduce/wavelength_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:10:34.282739 specreduce-1.4.0/specreduce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-29 20:10:34.000000 specreduce-1.4.0/specreduce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-29 20:10:34.000000 specreduce-1.4.0/specreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:10:34.000000 specreduce-1.4.0/specreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 20:10:34.000000 specreduce-1.4.0/specreduce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 20:10:34.000000 specreduce-1.4.0/specreduce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-29 20:10:25.000000 specreduce-1.4.0/tox.ini
```

### Comparing `specreduce-1.3.0/.github/workflows/publish-to-pypi.yml` & `specreduce-1.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/.gitignore` & `specreduce-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/CITATION.cff` & `specreduce-1.4.0/CITATION.cff`

 * *Files 5% similar despite different names*

```diff
@@ -25,11 +25,16 @@
     affiliation: Space Telescope Science Institute
     orcid: 'https://orcid.org/0000-0002-4679-5692'
   - given-names: Erik
     family-names: Tollerud
     email: erik.tollerud@gmail.com
     affiliation: Space Telescope Science Institute
     orcid: 'https://orcid.org/0000-0002-9599-310X'
+  - given-names: Clare
+    family-names: Shanahan
+    email: cshanahan@stsci.edu
+    affiliation: Space Telescope Science Institute
+    orcid: 'https://orcid.org/0009-0008-4112-7418X'
 identifiers:
   - type: doi
     value: 10.5281/zenodo.6608788
     description: 'Version 1.0.0: First Official Release'
```

### Comparing `specreduce-1.3.0/PKG-INFO` & `specreduce-1.4.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,30 @@
-Metadata-Version: 2.1
-Name: specreduce
-Version: 1.3.0
-Summary: Astropy affiliated package for Spectroscopic Reductions
-Home-page: http://astropy.org/
-Author: Astropy Specreduce contributors
-Author-email: astropy-dev@googlegroups.com
-License: BSD 3-Clause
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: data
-Provides-Extra: test
-Provides-Extra: docs
-License-File: licenses/LICENSE.rst
-
 Specreduce
 ==========
 
-.. image:: https://github.com/astropy/specreduce/workflows/Python%20Tests/badge.svg
-    :target: https://github.com/astropy/specreduce/actions
+.. image:: https://github.com/astropy/specreduce/actions/workflows/tox-tests.yml/badge.svg?branch=main
+    :target: https://github.com/astropy/specreduce/actions/workflows/tox-tests.yml
     :alt: CI Status
 
+.. image:: https://codecov.io/gh/astropy/specreduce/graph/badge.svg?token=3fLGjZ2Pe0
+    :target: https://codecov.io/gh/astropy/specreduce
+    :alt: Coverage
+
 .. image:: https://readthedocs.org/projects/specreduce/badge/?version=latest
-    :target: http://specreduce.readthedocs.io/en/latest/?badge=latest
+    :target: http://specreduce.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6608788.svg
-   :target: https://doi.org/10.5281/zenodo.6608788
-   :alt: Zenodo DOI 10.5281/zenodo.6608788
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6608787.svg
+   :target: https://zenodo.org/doi/10.5281/zenodo.6608787
+   :alt: Zenodo DOI 10.5281/zenodo.6608787
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
-    :target: http://www.astropy.org/
+   :target: http://www.astropy.org/
+   :alt: Powered by Astropy
 
-Specreduce is an Astropy affiliated package with the goal of providing a shared
+Specreduce is an Astropy coordinated package with the goal of providing a shared
 set of Python utilities that can be used to reduce and calibrate spectroscopic data.
 
 License
 -------
 
 Specreduce is licensed under a 3-clause BSD style license. Please see the licenses/LICENSE.rst file.
```

### Comparing `specreduce-1.3.0/docs/Makefile` & `specreduce-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/atm_transmission_secz1.5_1.6mm.dat` & `specreduce-1.4.0/docs/atm_transmission_secz1.5_1.6mm.dat`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/conf.py` & `specreduce-1.4.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,32 +21,25 @@
 # done. If the sys.path entry above is added, when the astropy.sphinx.conf
 # import occurs, it will import the *source* version of astropy instead of the
 # version installed (if invoked as "make html" or directly with sphinx), or the
 # version in the build directory (if "python setup.py build_sphinx" is used).
 # Thus, any C-extensions that are needed to build the documentation will *not*
 # be accessible, and the documentation will not build correctly.
 
-import os
 import sys
 import datetime
-from importlib import import_module
+
+from specreduce import __version__
 
 try:
     from sphinx_astropy.conf.v1 import *  # noqa
 except ImportError:
     print('ERROR: the documentation requires the sphinx-astropy package to be installed')
     sys.exit(1)
 
-# Get configuration information from setup.cfg
-from configparser import ConfigParser
-conf = ConfigParser()
-
-conf.read([os.path.join(os.path.dirname(__file__), '..', 'setup.cfg')])
-setup_cfg = dict(conf.items('metadata'))
-
 # -- General configuration ----------------------------------------------------
 
 # By default, highlight as Python 3.
 highlight_language = 'python3'
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.2'
@@ -63,30 +56,27 @@
 # be used globally.
 rst_epilog += """
 """
 
 # -- Project information ------------------------------------------------------
 
 # This does not *have* to match the package name, but typically does
-project = setup_cfg['name']
-author = setup_cfg['author']
+project = "specreduce"
+author = "Astropy Specreduce contributors"
 copyright = '{0}, {1}'.format(
-    datetime.datetime.now().year, setup_cfg['author'])
+    datetime.datetime.now().year, author)
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
-import_module(setup_cfg['name'])
-package = sys.modules[setup_cfg['name']]
-
 # The short X.Y version.
-version = package.__version__.split('-', 1)[0]
+version = __version__.split('-', 1)[0]
 # The full version, including alpha/beta/rc tags.
-release = package.__version__
+release = __version__
 
 
 # -- Options for HTML output --------------------------------------------------
 
 # A NOTE ON HTML THEMES
 # The global astropy configuration uses a custom theme, 'bootstrap-astropy',
 # which is installed along with astropy. A different theme can be used or
@@ -99,46 +89,51 @@
 # To use a different custom theme, add the directory containing the theme.
 #html_theme_path = []
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes. To override the custom theme, set this to the
 # name of a builtin theme or the name of a custom theme in html_theme_path.
 #html_theme = None
+html_static_path = ['_static']  # html_theme = None
+html_style = 'specreduce.css'
 
 
 html_theme_options = {
-    'logotext1': 'specreduce',  # white,  semi-bold
-    'logotext2': '',  # orange, light
+    'logotext1': 'spec',  # white,  semi-bold
+    'logotext2': 'reduce',  # orange, light
     'logotext3': ':docs'   # white,  light
     }
 
-
 # Custom sidebar templates, maps document names to template names.
 #html_sidebars = {}
+html_sidebars['**'] = ['localtoc.html']
+html_sidebars['index'] = ['globaltoc.html', 'localtoc.html']
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 #html_logo = ''
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = ''
+html_favicon = '_static/logo_icon.ico'
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 #html_last_updated_fmt = ''
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 html_title = '{0} v{1}'.format(project, release)
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = project + 'doc'
 
+# Prefixes that are ignored for sorting the Python module index
+modindex_common_prefix = ["specreduce."]
 
 # -- Options for LaTeX output -------------------------------------------------
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [('index', project + '.tex', project + u' Documentation',
                     author, 'manual')]
@@ -150,35 +145,23 @@
 # (source start file, name, description, authors, manual section).
 man_pages = [('index', project.lower(), project + u' Documentation',
               [author], 1)]
 
 
 # -- Options for the edit_on_github extension ---------------------------------
 
-if setup_cfg.get('edit_on_github').lower() == 'true':
-
-    extensions += ['sphinx_astropy.ext.edit_on_github']
-
-    edit_on_github_project = setup_cfg['github_project']
-    edit_on_github_branch = "main"
-
-    edit_on_github_source_root = ""
-    edit_on_github_doc_root = "docs"
-
-# -- Resolving issue number to links in changelog -----------------------------
-github_issues_url = 'https://github.com/{0}/issues/'.format(setup_cfg['github_project'])
-
 # -- Turn on nitpicky mode for sphinx (to warn about references not found) ----
 #
 nitpicky = True
 intersphinx_mapping.update(
     {
         'astropy': ('https://docs.astropy.org/en/stable/', None),
         'ccdproc': ('https://ccdproc.readthedocs.io/en/stable/', None),
-        'specutils': ('https://specutils.readthedocs.io/en/stable/', None)
+        'specutils': ('https://specutils.readthedocs.io/en/stable/', None),
+        'gwcs': ('https://gwcs.readthedocs.io/en/stable/', None)
     }
 )
 #
 # Some warnings are impossible to suppress, and you can list specific references
 # that should be ignored in a nitpick-exceptions file which should be inside
 # the docs/ directory. The format of the file should be:
 #
@@ -194,7 +177,15 @@
 #
 # for line in open('nitpick-exceptions'):
 #     if line.strip() == "" or line.startswith("#"):
 #         continue
 #     dtype, target = line.split(None, 1)
 #     target = target.strip()
 #     nitpick_ignore.append((dtype, six.u(target)))
+
+# -- Options for linkcheck output -------------------------------------------
+linkcheck_retry = 5
+linkcheck_ignore = [
+    "https://www.aanda.org/",
+]
+linkcheck_timeout = 180
+linkcheck_anchors = False
```

### Comparing `specreduce-1.3.0/docs/extinction.rst` & `specreduce-1.4.0/docs/extinction.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     fig, ax = plt.subplots(2, 1, sharex=True)
     for model in SUPPORTED_EXTINCTION_MODELS:
         ext = AtmosphericExtinction(model=model)
         ax[0].plot(ext.spectral_axis, ext.extinction_mag, label=model)
         ax[1].plot(ext.spectral_axis, ext.transmission)
     ax[0].legend(fancybox=True, shadow=True)
-    ax[1].set_xlabel("Wavelength ($\AA$)")
+    ax[1].set_xlabel("Wavelength (Angstroms)")
     ax[0].set_ylabel("Extinction (mag)")
     ax[1].set_ylabel("Transmission")
     plt.tight_layout()
     fig.show()
 
 A convenience class, `~specreduce.calibration_data.AtmosphericTransmission`, is provided for loading data files containing atmospheric transmission
 versus wavelength. The common use case for this would be loading the output of telluric models. By default it loads a telluric model for an
```

### Comparing `specreduce-1.3.0/docs/index.rst` & `specreduce-1.4.0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 ***********
 Calibration
 ***********
 
 .. toctree::
     :maxdepth: 1
 
+    wavelength_calibration.rst
     extinction.rst
     specphot_standards.rst
 
 
 *****
 Index
 *****
@@ -72,7 +73,9 @@
 Development Docs
 ****************
 
 .. toctree::
     :maxdepth: 1
 
     process/index
+    terms
+
```

### Comparing `specreduce-1.3.0/docs/make.bat` & `specreduce-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_MOS_arc.odg` & `specreduce-1.4.0/docs/process/NIR_MOS_arc.odg`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_MOS_arc.svg` & `specreduce-1.4.0/docs/process/NIR_MOS_arc.svg`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_MOS_flat.odg` & `specreduce-1.4.0/docs/process/NIR_MOS_flat.odg`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_MOS_flat.svg` & `specreduce-1.4.0/docs/process/NIR_MOS_flat.svg`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_MOS_science.odg` & `specreduce-1.4.0/docs/process/NIR_MOS_science.odg`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_MOS_science.svg` & `specreduce-1.4.0/docs/process/NIR_MOS_science.svg`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_MOS_trace.odg` & `specreduce-1.4.0/docs/process/NIR_MOS_trace.odg`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_MOS_trace.svg` & `specreduce-1.4.0/docs/process/NIR_MOS_trace.svg`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/NIR_flats.rst` & `specreduce-1.4.0/docs/process/NIR_flats.rst`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/process/index.rst` & `specreduce-1.4.0/docs/process/index.rst`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/docs/specphot_standards.rst` & `specreduce-1.4.0/docs/specphot_standards.rst`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 .. plot::
     :include-source:
 
     import matplotlib.pyplot as plt
     from specreduce.calibration_data import load_MAST_calspec, load_onedstds
 
-    s1 = load_MAST_calspec("ltt9491_002.fits", remote=True)
+    s1 = load_MAST_calspec("ltt9491_002.fits")
     s2 = load_onedstds("snfactory", "LTT9491.dat")
     s3 = load_onedstds("eso", "ctiostan/ltt9491.dat")
 
     fig, ax = plt.subplots()
     ax.step(s1.spectral_axis, s1.flux, label="MAST", where="mid")
     ax.step(s2.spectral_axis, s2.flux, label="SNFactory", where="mid")
     ax.step(s3.spectral_axis, s3.flux, label="ESO", where="mid")
```

### Comparing `specreduce-1.3.0/licenses/KOSMOS_LICENSE` & `specreduce-1.4.0/licenses/KOSMOS_LICENSE`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/licenses/LICENSE.rst` & `specreduce-1.4.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `specreduce-1.3.0/specreduce/background.py` & `specreduce-1.4.0/specreduce/background.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import warnings
 from dataclasses import dataclass, field
 
 import numpy as np
+from astropy import units as u
 from astropy.nddata import NDData
 from astropy.utils.decorators import deprecated_attribute
-from astropy import units as u
 from specutils import Spectrum1D
 
 from specreduce.core import _ImageParser
 from specreduce.extract import _ap_weight_image
 from specreduce.tracing import Trace, FlatTrace
 
 __all__ = ['Background']
@@ -28,17 +28,18 @@
         bg = Background.two_sided(image, trace, bkg_sep, width=bkg_width)
         subtracted_image = image - bg
 
     Parameters
     ----------
     image : `~astropy.nddata.NDData`-like or array-like
         image with 2-D spectral image data
-    traces : List
-        list of trace objects (or integers to define FlatTraces) to
-        extract the background
+    traces : trace, int, float (single or list)
+        Individual or list of trace object(s) (or integers/floats to define
+        FlatTraces) to extract the background. If None, a FlatTrace at the
+        center of the image (according to `disp_axis`) will be used.
     width : float
         width of extraction aperture in pixels
     statistic: string
         statistic to use when computing the background.  'average' will
         account for partial pixel weights, 'median' will include all partial
         pixels.
     disp_axis : int
@@ -78,38 +79,26 @@
             account for partial pixel weights, 'median' will include all partial
             pixels.
         disp_axis : int
             dispersion axis
         crossdisp_axis : int
             cross-dispersion axis
         """
-        def _to_trace(trace):
-            if not isinstance(trace, Trace):
-                trace = FlatTrace(self.image, trace)
-
-            # TODO: this check can be removed if/when implemented as a check in FlatTrace
-            if isinstance(trace, FlatTrace):
-                if trace.trace_pos < 1:
-                    raise ValueError('trace_object.trace_pos must be >= 1')
-            return trace
-
         self.image = self._parse_image(self.image)
 
         if self.width < 0:
             raise ValueError("width must be positive")
         if self.width == 0:
             self._bkg_array = np.zeros(self.image.shape[self.disp_axis])
             return
 
-        if isinstance(self.traces, Trace):
-            self.traces = [self.traces]
+        self._set_traces()
 
         bkg_wimage = np.zeros_like(self.image.data, dtype=np.float64)
         for trace in self.traces:
-            trace = _to_trace(trace)
             windows_max = trace.trace.data.max() + self.width/2
             windows_min = trace.trace.data.min() - self.width/2
             if windows_max >= self.image.shape[self.crossdisp_axis]:
                 warnings.warn("background window extends beyond image boundaries " +
                               f"({windows_max} >= {self.image.shape[self.crossdisp_axis]})")
             if windows_min < 0:
                 warnings.warn("background window extends beyond image boundaries " +
@@ -129,25 +118,64 @@
 
         if self.statistic == 'median':
             # make it clear in the expose image that partial pixels are fully-weighted
             bkg_wimage[bkg_wimage > 0] = 1
 
         self.bkg_wimage = bkg_wimage
 
+        # mask user-highlighted and invalid values (if any) before taking stats
+        or_mask = (np.logical_or(~np.isfinite(self.image.data), self.image.mask)
+                   if self.image.mask is not None
+                   else ~np.isfinite(self.image.data))
+
         if self.statistic == 'average':
-            self._bkg_array = np.average(self.image.data,
-                                         weights=self.bkg_wimage,
-                                         axis=self.crossdisp_axis)
+            image_ma = np.ma.masked_array(self.image.data, mask=or_mask)
+            self._bkg_array = np.ma.average(image_ma,
+                                            weights=self.bkg_wimage,
+                                            axis=self.crossdisp_axis).data
         elif self.statistic == 'median':
-            med_image = self.image.data.copy()
-            med_image[np.where(self.bkg_wimage) == 0] = np.nan
-            self._bkg_array = np.nanmedian(med_image, axis=self.crossdisp_axis)
+            med_mask = np.logical_or(self.bkg_wimage == 0, or_mask)
+            image_ma = np.ma.masked_array(self.image.data, mask=med_mask)
+            self._bkg_array = np.ma.median(image_ma, axis=self.crossdisp_axis).data
         else:
             raise ValueError("statistic must be 'average' or 'median'")
 
+    def _set_traces(self):
+        """Determine `traces` from input. If an integer/float or list if int/float
+           is passed in, use these to construct FlatTrace objects. These values
+           must be positive. If None (which is initialized to an empty list),
+           construct a FlatTrace using the center of image (according to disp.
+           axis). Otherwise, any Trace object or list of Trace objects can be
+           passed in."""
+
+        if self.traces == []:
+            # assume a flat trace at the image center if nothing is passed in.
+            trace_pos = self.image.shape[self.disp_axis] / 2.
+            self.traces = [FlatTrace(self.image, trace_pos)]
+
+        if isinstance(self.traces, Trace):
+            # if just one trace, turn it into iterable.
+            self.traces = [self.traces]
+            return
+
+        # finally, if float/int is passed in convert to FlatTrace(s)
+        if isinstance(self.traces, (float, int)):  # for a single number
+            self.traces = [self.traces]
+
+        if np.all([isinstance(x, (float, int)) for x in self.traces]):
+            self.traces = [FlatTrace(self.image, trace_pos) for trace_pos in self.traces]
+            return
+
+        else:
+            if not np.all([isinstance(x, Trace) for x in self.traces]):
+                raise ValueError('`traces` must be a `Trace` object or list of '
+                                 '`Trace` objects, a number or list of numbers to '
+                                 'define FlatTraces, or None to use a FlatTrace in '
+                                 'the middle of the image.')
+
     @classmethod
     def two_sided(cls, image, trace_object, separation, **kwargs):
         """
         Determine the background from an image for subtraction centered around
         an input trace.
 
 
@@ -173,15 +201,15 @@
             account for partial pixel weights, 'median' will include all partial
             pixels.
         disp_axis : int
             dispersion axis
         crossdisp_axis : int
             cross-dispersion axis
         """
-        image = cls._parse_image(cls, image)
+        image = _ImageParser._get_data_from_image(image) if image is not None else cls.image
         kwargs['traces'] = [trace_object-separation, trace_object+separation]
         return cls(image=image, **kwargs)
 
     @classmethod
     def one_sided(cls, image, trace_object, separation, **kwargs):
         """
         Determine the background from an image for subtraction above
@@ -210,15 +238,15 @@
             account for partial pixel weights, 'median' will include all partial
             pixels.
         disp_axis : int
             dispersion axis
         crossdisp_axis : int
             cross-dispersion axis
         """
-        image = cls._parse_image(cls, image)
+        image = _ImageParser._get_data_from_image(image) if image is not None else cls.image
         kwargs['traces'] = [trace_object+separation]
         return cls(image=image, **kwargs)
 
     def bkg_image(self, image=None):
         """
         Expose the background tiled to the dimension of ``image``.
 
@@ -228,15 +256,15 @@
             Image with 2-D spectral image data. Assumes cross-dispersion
             (spatial) direction is axis 0 and dispersion (wavelength)
             direction is axis 1. If None, will extract the background
             from ``image`` used to initialize the class. [default: None]
 
         Returns
         -------
-        Spectrum1D object with same shape as ``image``.
+        `~specutils.Spectrum1D` object with same shape as ``image``.
         """
         image = self._parse_image(image)
         return Spectrum1D(np.tile(self._bkg_array,
                                   (image.shape[0], 1)) * image.unit,
                           spectral_axis=image.spectral_axis)
 
     def bkg_spectrum(self, image=None):
@@ -257,34 +285,34 @@
             The background 1-D spectrum, with flux expressed in the same
             units as the input image (or u.DN if none were provided) and
             the spectral axis expressed in pixel units.
         """
         bkg_image = self.bkg_image(image)
 
         try:
-            return bkg_image.collapse(np.sum, axis=self.crossdisp_axis)
+            return bkg_image.collapse(np.nansum, axis=self.crossdisp_axis)
         except u.UnitTypeError:
             # can't collapse with a spectral axis in pixels because
             # SpectralCoord only allows frequency/wavelength equivalent units...
-            ext1d = np.sum(bkg_image.flux, axis=self.crossdisp_axis)
+            ext1d = np.nansum(bkg_image.flux, axis=self.crossdisp_axis)
             return Spectrum1D(ext1d, bkg_image.spectral_axis)
 
     def sub_image(self, image=None):
         """
         Subtract the computed background from ``image``.
 
         Parameters
         ----------
         image : nddata-compatible image or None
             image with 2-D spectral image data.  If None, will extract
             the background from ``image`` used to initialize the class.
 
         Returns
         -------
-        array with same shape as ``image``
+        `~specutils.Spectrum1D` object with same shape as ``image``.
         """
         image = self._parse_image(image)
 
         # a compare_wcs argument is needed for Spectrum1D.subtract() in order to
         # avoid a TypeError from SpectralCoord when image's spectral axis is in
         # pixels. it is not needed when image's spectral axis has physical units
         kwargs = ({'compare_wcs': None} if image.spectral_axis.unit == u.pix
@@ -309,19 +337,19 @@
             The background 1-D spectrum, with flux expressed in the same
             units as the input image (or u.DN if none were provided) and
             the spectral axis expressed in pixel units.
         """
         sub_image = self.sub_image(image=image)
 
         try:
-            return sub_image.collapse(np.sum, axis=self.crossdisp_axis)
+            return sub_image.collapse(np.nansum, axis=self.crossdisp_axis)
         except u.UnitTypeError:
             # can't collapse with a spectral axis in pixels because
             # SpectralCoord only allows frequency/wavelength equivalent units...
-            ext1d = np.sum(sub_image.flux, axis=self.crossdisp_axis)
+            ext1d = np.nansum(sub_image.flux, axis=self.crossdisp_axis)
             return Spectrum1D(ext1d, spectral_axis=sub_image.spectral_axis)
 
     def __rsub__(self, image):
         """
         Subtract the background from an image.
         """
         return self.sub_image(image)
```

### Comparing `specreduce-1.3.0/specreduce/calibration_data.py` & `specreduce-1.4.0/specreduce/calibration_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 """
 Utilities for defining, loading, and handling spectroscopic calibration data
 """
 
-import os
-import pkg_resources
 import warnings
+from pathlib import Path
+from typing import Sequence
 
-import astropy.units as u
-from astropy.table import Table
+from astropy import units as u
+from astropy.table import Table, vstack, QTable
 from astropy.utils.data import download_file
 from astropy.utils.exceptions import AstropyUserWarning
+from astropy.coordinates import SpectralCoord
 
-import synphot
 from specutils import Spectrum1D
+from specutils.utils.wcs_utils import vac_to_air
 
 __all__ = [
     'get_reference_file_path',
+    'get_pypeit_data_path',
+    'get_available_line_catalogs',
+    'load_pypeit_calibration_lines',
     'load_MAST_calspec',
     'load_onedstds',
     'AtmosphericExtinction',
     'AtmosphericTransmission'
 ]
 
-"""
-If specreduce_data is not available, we'll fall back to downloading and optionally caching it using
-`~astropy.utils.data`.
-"""
-LOCAL_DATA = True
-try:
-    import specreduce_data  # noqa
-except ModuleNotFoundError:
-    warnings.warn(
-        "Can't import specreduce_data package. Falling back to downloading data...",
-        AstropyUserWarning
-    )
-    LOCAL_DATA = False
-
 SUPPORTED_EXTINCTION_MODELS = [
     "kpno",
     "ctio",
     "apo",
     "lapalma",
     "mko",
     "mtham",
@@ -58,172 +48,351 @@
     "redcal",
     "snfactory",
     "spec16cal",
     "spec50cal",
     "spechayescal"
 ]
 
+PYPEIT_CALIBRATION_LINELISTS = [
+    'Ne_IR_MOSFIRE',
+    'ArII',
+    'CdI',
+    'OH_MOSFIRE_H',
+    'OH_triplespec',
+    'Ar_IR_MOSFIRE',
+    'OH_GNIRS',
+    'ThAr_XSHOOTER_VIS',
+    'ThAr_MagE',
+    'HgI',
+    'NeI',
+    'XeI',
+    'OH_MODS',
+    'ZnI',
+    'OH_GMOS',
+    'CuI',
+    'ThAr_XSHOOTER_VIS_air',
+    'ThAr_XSHOOTER_UVB',
+    'OH_NIRES',
+    'HeI',
+    'FeI',
+    'OH_MOSFIRE_J',
+    'KrI',
+    'Cd_DeVeny1200',
+    'Ar_IR_GNIRS',
+    'OH_MOSFIRE_Y',
+    'ThAr',
+    'FeII',
+    'OH_XSHOOTER',
+    'OH_FIRE_Echelle',
+    'OH_MOSFIRE_K',
+    'OH_R24000',
+    'Hg_DeVeny1200',
+    'ArI'
+]
+
+
+def get_available_line_catalogs() -> dict:
+    """
+    Returns a dictionary of available line catalogs. Currently only ``pypeit``
+    catalogs are fully supported.
+    """
+    return {
+        'pypeit': PYPEIT_CALIBRATION_LINELISTS
+    }
+
 
-def get_reference_file_path(path=None, cache=False, show_progress=False):
+def get_reference_file_path(
+        path: str | Path | None = None,
+        cache: bool = True,
+        repo_url: str = "https://raw.githubusercontent.com/astropy/specreduce-data",
+        repo_branch: str = "main",
+        repo_data_path: str = "specreduce_data/reference_data",
+        show_progress: bool = False
+) -> Path | None:
     """
-    Basic function to take a path to a file and load it via ``pkg_resources`` if
-    the ``specreduce_data`` package is available and load it via GitHub raw user content if not.
+    Utility to load reference data via GitHub raw user content. By default the ``specreduce_data``
+    repository at https://github.com/astropy/specreduce-data is used.
 
     Parameters
     ----------
-    path : str or None (default: None)
-        Filename of reference file relative to the reference_data directory within
-        ``specreduce_data`` package.
+    path : Path of reference file relative to the reference_data directory within
+        specified package.
+
+    cache : Set whether file is cached if file is downloaded.
+
+    repo_url : Base repository URL for the reference data.
 
-    cache : bool (default: False)
-        Set whether file is cached if file is downloaded.
+    repo_branch : Branch of repository from which to fetch the reference data.
 
-    show_progress : bool (default: False)
-        Set whether download progress bar is shown if file is downloaded.
+    repo_data_path : Path within the repository where the reference data is located.
+
+    show_progress : Set whether download progress bar is shown if file is downloaded.
 
     Returns
     -------
-    file_path : str or None
-        Path to reference data file or None if the path cannot be constructed or if the file
-        itself is not valid.
+    file_path : Local path to reference data file or None if the path cannot be constructed
+        or if the file itself is not valid.
 
     Examples
     --------
     >>> from specreduce.calibration_data import get_reference_file_path
     >>> kpno_extinction_file = get_reference_file_path("extinction/kpnoextinct.dat")
     """
     if path is None:
         return None
 
-    if LOCAL_DATA:
-        file_path = pkg_resources.resource_filename(
-            "specreduce_data",
-            os.path.join("reference_data", path)
-        )
-    else:
-        repo_url = "https://raw.githubusercontent.com/astropy/specreduce-data"
-        remote_url = f"{repo_url}/main/specreduce_data/reference_data/{path}"
-        try:
-            file_path = download_file(
+    remote_url = f"{repo_url}/{repo_branch}/{repo_data_path}/{path}"
+    try:
+        file_path = Path(
+            download_file(
                 remote_url,
                 cache=cache,
                 show_progress=show_progress,
                 pkgname='specreduce'
             )
-        except Exception as e:
-            msg = f"Downloading of {path} failed: {e}"
-            warnings.warn(msg, AstropyUserWarning)
-            return None
+        )
+    except Exception as e:
+        msg = f"Downloading of {remote_url} failed: {e}"
+        warnings.warn(msg, AstropyUserWarning)
+        return None
 
     # final sanity check to make sure file_path is actually a file.
-    if os.path.isfile(file_path):
+    if file_path.exists() and file_path.is_file():
         return file_path
     else:
         warnings.warn(f"Able to construct {file_path}, but it is not a file.")
         return None
 
 
-def load_MAST_calspec(filename, remote=True, cache=True, show_progress=False):
+def get_pypeit_data_path(
+        path: str | Path | None = None,
+        cache: bool = True,
+        show_progress: bool = False
+) -> Path | None:
     """
-    Load a standard star spectrum from the ``calspec`` database at MAST. These spectra are provided in
-    FITS format and are described in detail at:
+    Convenience utility to facilitate access to ``pypeit`` reference data. The data is accessed
+    directly from the release branch on GitHub and downloaded/cached
+    using `~astropy.utils.data.download_file`.
+
+    Parameters
+    ----------
+    path : Filename of reference file relative to the reference_data directory within
+        ``specreduce_data`` package.
+
+    cache : Set whether file is cached if file is downloaded.
 
-    https://www.stsci.edu/hst/instrumentation/reference-data-for-calibration-and-tools/astronomical-catalogs/calspec  # noqa
+    show_progress : Set whether download progress bar is shown if file is downloaded.
 
-    If ``remote`` is True, the spectrum will be downloaded from MAST. Set ``remote`` to False to load
-    a local file.
+    Returns
+    -------
+    file_path : Path to reference data file or None if the path cannot be
+        constructed or if the file itself is not valid.
+
+    Examples
+    --------
+    >>> from specreduce.calibration_data import get_pypeit_data_path
+    >>> pypeit_he_linelist = get_pypeit_data_path("arc_lines/lists/HeI_lines.dat")
+    """
+    repo_url = "https://raw.githubusercontent.com/pypeit/pypeit"
+    repo_branch = "release"
+    repo_data_path = "pypeit/data"
+
+    return get_reference_file_path(
+        path=path,
+        cache=cache,
+        repo_url=repo_url,
+        repo_branch=repo_branch,
+        repo_data_path=repo_data_path,
+        show_progress=show_progress
+    )
+
+
+def load_pypeit_calibration_lines(
+        lamps: Sequence | None = None,
+        wave_air: bool = False,
+        cache: bool = True,
+        show_progress: bool = False
+) -> QTable | None:
+    """
+    Load reference calibration lines from ``pypeit`` linelists. The ``pypeit`` linelists are
+    well-curated and have been tested across a wide range of spectrographs. The available
+    linelists are defined by ``PYPEIT_CALIBRATION_LINELISTS``.
+
+    Parameters
+    ----------
+    lamps : Lamp string, comma-separated list of lamps, or sequence of lamps to include in
+        output reference linelist. The parlance of "lamp" is retained here for consistency
+        with its use in ``pypeit`` and elsewhere. In several of the supported cases the
+        "lamp" is the sky itself (e.g. OH lines in the near-IR).
+        The available lamps are defined by ``PYPEIT_CALIBRATION_LINELISTS``.
+
+    wave_air : If True, convert the vacuum wavelengths used by ``pypeit`` to air wavelengths.
+
+    cache : Toggle caching of downloaded data
+
+    show_progress : Show download progress bar
+
+    Returns
+    -------
+    linelist:
+        Table containing the combined calibration line list. ``pypeit`` linelists have the
+        following columns:
+        * ``ion``: Ion or molecule generating the line.
+        * ``wavelength``: Vacuum wavelength of the line in Angstroms.
+        * ``NIST``: Flag denoting if NIST is the ultimate reference for the line's wavelength.
+        * ``Instr``: ``pypeit``-specific instrument flag.
+        * ``amplitude``: Amplitude of the line. Beware, not consistent between lists.
+        * ``Source``: Source of the line information.
+    """
+    if lamps is None:
+        return None
+
+    if not isinstance(lamps, Sequence):
+        raise ValueError(f"Invalid calibration lamps specification: {lamps}")
+
+    if isinstance(lamps, str):
+        if ',' in lamps:
+            lamps = [lamp.strip() for lamp in lamps.split(',')]
+        else:
+            lamps = [lamps]
+
+    linelists = []
+    for lamp in lamps:
+        if lamp in PYPEIT_CALIBRATION_LINELISTS:
+            list_path = f"arc_lines/lists/{lamp}_lines.dat"
+            lines_file = get_pypeit_data_path(
+                list_path,
+                cache=cache,
+                show_progress=show_progress
+            )
+            lines_tab = Table.read(
+                lines_file,
+                format='ascii.fixed_width',
+                comment='#'
+            )
+            if lines_tab is not None:
+                linelists.append(lines_tab)
+        else:
+            warnings.warn(
+                f"{lamp} not in the list of supported calibration "
+                "line lists: {PYPEIT_CALIBRATION_LINELISTS}."
+            )
+    if len(linelists) == 0:
+        warnings.warn(f"No calibration lines loaded from {lamps}.")
+        linelist = None
+    else:
+        linelist = vstack(linelists)
+        linelist.rename_column('wave', 'wavelength')
+        # pypeit linelists use vacuum wavelengths in angstroms
+        linelist['wavelength'] *= u.Angstrom
+        if wave_air:
+            linelist['wavelength'] = vac_to_air(linelist['wavelength'])
+        linelist = QTable(linelist)
+
+    return linelist
+
+
+def load_MAST_calspec(
+        filename: str | Path,
+        cache: bool = True,
+        show_progress: bool = False
+) -> Spectrum1D | None:
+    """
+    Load a standard star spectrum from the ``calspec`` database at MAST. These spectra are provided
+    in FITS format and are described in detail at:
+
+    https://www.stsci.edu/hst/instrumentation/reference-data-for-calibration-and-tools/astronomical-catalogs/calspec
+
+    If ``remote`` is True, the spectrum will be downloaded from MAST. Set ``remote`` to False to
+    load a local file.
+
+    .. note:: This function requires ``synphot`` to be installed separately.
 
     Parameters
     ----------
-    filename : str
-        FITS filename of the standard star spectrum, e.g. g191b2b_005.fits.
+    filename : FITS filename of a standard star spectrum, e.g. g191b2b_005.fits.
+        If this is a local file, it will be loaded. If not, then a download from
+        MAST will be attempted.
 
-    remote : bool (default = True)
-        If True, download the spectrum from MAST. If False, check if ``filename`` exists and load
-        it.
-    cache : bool (default = True)
-        Toggle whether downloaded data is cached or not.
-    show_progress : bool (default = True)
-        Toggle whether download progress bar is shown.
+    cache : Toggle whether downloaded data is cached or not.
+
+    show_progress : Toggle whether download progress bar is shown.
 
     Returns
     -------
-    spectrum : `~specutils.Spectrum1D` or None
-        If the spectrum can be loaded, return it as a `~specutils.Spectrum1D`.
+    spectrum : If the spectrum can be loaded, return it as a `~specutils.Spectrum1D`.
         Otherwise return None. The spectral_axis units are Å and the flux units are milli-Janskys.
     """
-    if remote:
+    filename = Path(filename)
+    if filename.exists() and filename.is_file():
+        file_path = filename
+    else:
         url = f"https://archive.stsci.edu/hlsps/reference-atlases/cdbs/calspec/{filename}"
         try:
             file_path = download_file(
                 url,
                 cache=cache,
                 show_progress=show_progress,
                 pkgname='specreduce'
             )
         except Exception as e:
-            msg = f"Downloading of {filename} failed: {e}"
-            warnings.warn(msg, AstropyUserWarning)
-            file_path = None
-    else:
-        if os.path.isfile(filename):
-            file_path = filename
-        else:
-            msg = f"Provided filename, {filename}, does not exist or is not a valid file."
+            msg = f"Downloading of {url} failed: {e}"
             warnings.warn(msg, AstropyUserWarning)
             file_path = None
 
     if file_path is None:
         return None
     else:
-        hdr, wave, flux = synphot.specio.read_fits_spec(file_path)
+        import synphot
+        _, wave, flux = synphot.specio.read_fits_spec(file_path)
 
+        # DEV: pllim does not think this is necessary at all but whatever.
         # the calspec data stores flux in synphot's FLAM units. convert to flux units
         # supported directly by astropy.units. mJy is chosen since it's the JWST
         # standard and can easily be converted to/from AB magnitudes.
         flux_mjy = synphot.units.convert_flux(wave, flux, u.mJy)
         spectrum = Spectrum1D(spectral_axis=wave, flux=flux_mjy)
         return spectrum
 
 
-def load_onedstds(dataset="snfactory", specfile="EG131.dat", cache=True, show_progress=False):
+def load_onedstds(
+        dataset: str = "snfactory",
+        specfile: str = "EG131.dat",
+        cache: bool = True,
+        show_progress: bool = False
+) -> Spectrum1D | None:
     """
     This is a convenience function for loading a standard star spectrum from the 'onedstds'
-    dataset in the ``specreduce_data`` package. If that package is installed, ``pkg_resources``
-    will be used to locate the data files locally. Otherwise they will be downloaded from the
-    repository on github.
+    dataset in the ``specreduce_data`` package. They will be downloaded from the
+    repository on GitHub and cached by default.
 
     Parameters
     ----------
-    dataset : str  (default = "snfactory")
-        Standard star spectrum database. Valid options are described in :ref:`specphot_standards`.
+    dataset : Standard star spectrum database. Valid options are described
+        in :ref:`specphot_standards`.
 
-    specfile : str (default = "EG131.dat")
-        Filename of the standard star spectrum.
+    specfile : Filename of the standard star spectrum.
 
-    cache : bool (default = True)
-        Enable caching of downloaded data.
+    cache : Enable caching of downloaded data.
 
-    show_progress : bool (default = False)
-        Show download progress bar if data is downloaded.
+    show_progress : Show download progress bar if data is downloaded.
 
     Returns
     -------
-    spectrum : None or `~specutils.Spectrum1D`
-        If the spectrum can be loaded, return it as a `~specutils.Spectrum1D`.
+    spectrum : If the spectrum can be loaded, return it as a `~specutils.Spectrum1D`.
         Otherwise return None. The spectral_axis units are Å and the flux units are milli-Janskys.
     """
     if dataset not in SPECPHOT_DATASETS:
         msg = (f"Specfied dataset, {dataset}, not in list of supported datasets of "
                f"spectrophotometric standard stars: f{SPECPHOT_DATASETS}")
         warnings.warn(msg, AstropyUserWarning)
         return None
 
     spec_path = get_reference_file_path(
-        path=os.path.join("onedstds", dataset, specfile),
+        path=Path("onedstds") / Path(dataset) / Path(specfile),
         cache=cache,
         show_progress=show_progress
     )
     if spec_path is None:
         msg = f"Can't load {specfile} from {dataset}."
         warnings.warn(msg, AstropyUserWarning)
         return None
@@ -245,49 +414,50 @@
     Spectrum container for atmospheric extinction in magnitudes as a function of wavelength.
     If extinction and spectral_axis are provided, this will use them to build a custom model.
     If they are not, the 'model' parameter will be used to lookup and load a pre-defined
     atmospheric extinction model from the ``specreduce_data`` package.
 
     Parameters
     ----------
-    model : str
-        Name of atmospheric extinction model provided by ``specreduce_data``. Valid
+    model : Name of atmospheric extinction model provided by ``specreduce_data``. Valid
         options are:
 
         kpno - Kitt Peak National Observatory (default)
         ctio - Cerro Tololo International Observatory
         apo - Apache Point Observatory
         lapalma - Roque de los Muchachos Observatory, La Palma, Canary Islands
         mko - Mauna Kea Observatories
         mtham - Lick Observatory, Mt. Hamilton station
         paranal - European Southern Observatory, Cerro Paranal station
 
-    extinction : `~astropy.units.LogUnit`, `~astropy.units.Magnitude`,
-    `~astropy.units.dimensionless_unscaled`, 1D list-like, or None
-        Optionally provided extinction data for this spectrum. Used along with spectral_axis
-        to build custom atmospheric extinction model. If no units are provided, assumed to
-        be given in magnitudes.
+    extinction : Optionally provided extinction data for this spectrum. Used along with
+        spectral_axis to build custom atmospheric extinction model. If no units are provided,
+        assumed to be given in magnitudes.
 
-    spectral_axis : `~astropy.units.Quantity` or `~astropy.coordinates.SpectralCoord` or None
-        Optional Dispersion information with the same shape as the last (or only)
+    spectral_axis : Optional Dispersion information with the same shape as the last (or only)
         dimension of flux, or one greater than the last dimension of flux
         if specifying bin edges. Used along with flux to build custom atmospheric
         extinction model.
 
     Properties
     ----------
-    extinction_mag : `~astropy.units.Magnitude`
-        Extinction expressed in dimensionless magnitudes
+    extinction_mag : Extinction expressed in dimensionless magnitudes
 
-    transmission : `~astropy.units.dimensionless_unscaled`
-        Extinction expressed as fractional transmission
+    transmission : Extinction expressed as fractional transmission
 
     """
-    def __init__(self, model="kpno", extinction=None, spectral_axis=None,
-                 cache=True, show_progress=False, **kwargs):
+    def __init__(
+        self,
+        model: str = "kpno",
+        extinction: Sequence[float] | u.Quantity | None = None,
+        spectral_axis: SpectralCoord | u.Quantity | None = None,
+        cache: bool = True,
+        show_progress: bool = False,
+        **kwargs: str
+    ) -> None:
         if extinction is not None:
             if not isinstance(extinction, u.Quantity):
                 warnings.warn(
                     "Input extinction is not a Quanitity. Assuming it is given in magnitudes...",
                     AstropyUserWarning
                 )
                 extinction = u.Magnitude(
@@ -309,15 +479,15 @@
         if extinction is None and spectral_axis is None:
             if model not in SUPPORTED_EXTINCTION_MODELS:
                 msg = (
                     f"Requested extinction model, {model}, not in list "
                     f"of available models: {SUPPORTED_EXTINCTION_MODELS}"
                 )
                 raise ValueError(msg)
-            model_file = os.path.join("extinction", f"{model}extinct.dat")
+            model_file = Path("extinction") / Path(f"{model}extinct.dat")
             model_path = get_reference_file_path(
                 path=model_file,
                 cache=cache,
                 show_progress=show_progress
             )
             t = Table.read(model_path, format="ascii", names=['wavelength', 'extinction'])
 
@@ -338,52 +508,55 @@
             flux=extinction,
             spectral_axis=spectral_axis,
             unit=u.dimensionless_unscaled,
             **kwargs
         )
 
     @property
-    def extinction_mag(self):
+    def extinction_mag(self) -> u.Quantity:
         """
         This property returns the extinction in magnitudes
         """
         return self.flux.to(u.mag(u.dimensionless_unscaled))
 
     @property
-    def transmission(self):
+    def transmission(self) -> u.Quantity:
         """
         This property returns the transmission as a fraction between 0 and 1
         """
         return self.flux
 
 
 class AtmosphericTransmission(AtmosphericExtinction):
     """
     Spectrum container for atmospheric transmission as a function of wavelength.
 
     Parameters
     ----------
-    data_file : str or `~pathlib.Path` or None
-        Name to file containing atmospheric transmission data. Data is assumed to have
+    data_file : Name to file containing atmospheric transmission data. Data is assumed to have
         two columns, wavelength and transmission (unscaled dimensionless). If
         this isn't provided, a model is built from a pre-calculated table of values
         from 0.9 to 5.6 microns. The values were generated by the ATRAN model,
-        https://atran.arc.nasa.gov/cgi-bin/atran/atran.cgi (Lord, S. D., 1992, NASA
+        https://ntrs.nasa.gov/citations/19930010877 (Lord, S. D., 1992, NASA
         Technical Memorandum 103957). The extinction is given as a linear transmission
         fraction at an airmass of 1 and 1 mm of precipitable water.
 
-    wave_unit : `~astropy.units.Unit` (default = u.um)
-        Units for spectral axis.
+    wave_unit : Units for spectral axis.
     """
-    def __init__(self, data_file=None, wave_unit=u.um, **kwargs):
+    def __init__(
+        self,
+        data_file: str | Path | None = None,
+        wave_unit: u.Unit = u.um,
+        **kwargs: str
+    ) -> None:
         if data_file is None:
-            data_path = os.path.join("extinction", "atm_trans_am1.0.dat")
+            data_path = Path("extinction") / Path("atm_trans_am1.0.dat")
             data_file = get_reference_file_path(path=data_path)
 
-        t = Table.read(data_file, format="ascii", names=['wavelength', 'extinction'])
+        t = Table.read(Path(data_file), format="ascii", names=['wavelength', 'extinction'])
 
         # spectral axis is given in microns
         spectral_axis = t['wavelength'].data * wave_unit
 
         # extinction is given in a dimensionless transmission fraction
         extinction = t['extinction'].data * u.dimensionless_unscaled
```

### Comparing `specreduce-1.3.0/specreduce/core.py` & `specreduce-1.4.0/specreduce/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import inspect
-import numpy as np
+from dataclasses import dataclass
 
+import numpy as np
 from astropy import units as u
 from astropy.nddata import VarianceUncertainty
-from dataclasses import dataclass
 from specutils import Spectrum1D
 
 __all__ = ['SpecreduceOperation']
 
 
 class _ImageParser:
     """
@@ -22,14 +22,15 @@
 
         - `~specutils.spectra.spectrum1d.Spectrum1D` (preferred)
         - `~astropy.nddata.ccddata.CCDData`
         - `~astropy.nddata.ndddata.NDDData`
         - `~astropy.units.quantity.Quantity`
         - `~numpy.ndarray`
     """
+
     def _parse_image(self, image, disp_axis=1):
         """
         Convert all accepted image types to a consistently formatted
         Spectrum1D object.
 
         Parameters
         ----------
@@ -46,20 +47,15 @@
         # operations (public attribute? private attribute? argument only?) so
         # it can be called from self instead of via kwargs...
 
         if image is None:
             # useful for Background's instance methods
             return self.image
 
-        if isinstance(image, np.ndarray):
-            img = image
-        elif isinstance(image, u.quantity.Quantity):
-            img = image.value
-        else:  # NDData, including CCDData and Spectrum1D
-            img = image.data
+        img = self._get_data_from_image(image)
 
         # mask and uncertainty are set as None when they aren't specified upon
         # creating a Spectrum1D object, so we must check whether these
         # attributes are absent *and* whether they are present but set as None
         if getattr(image, 'mask', None) is not None:
             mask = image.mask
         else:
@@ -74,14 +70,27 @@
 
         spectral_axis = getattr(image, 'spectral_axis',
                                 np.arange(img.shape[disp_axis]) * u.pix)
 
         return Spectrum1D(img * unit, spectral_axis=spectral_axis,
                           uncertainty=uncertainty, mask=mask)
 
+    @staticmethod
+    def _get_data_from_image(image):
+        """Extract data array from various input types for `image`.
+           Retruns `np.ndarray` of image data."""
+
+        if isinstance(image, u.quantity.Quantity):
+            img = image.value
+        if isinstance(image, np.ndarray):
+            img = image
+        else:  # NDData, including CCDData and Spectrum1D
+            img = image.data
+        return img
+
 
 @dataclass
 class SpecreduceOperation(_ImageParser):
     """
     An operation to perform as part of a spectroscopic reduction pipeline.
 
     This class primarily exists to define the basic API for operations:
```

### Comparing `specreduce-1.3.0/specreduce/fluxcal.py` & `specreduce-1.4.0/specreduce/fluxcal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import os
 
 import numpy as np
-
-import matplotlib.pyplot as plt
-
+from astropy import units as u
 from astropy.constants import c as cc
 from astropy.table import Table
-import astropy.units as u
-
 from scipy.interpolate import UnivariateSpline
-
 from specutils import Spectrum1D
+
 from specreduce.core import SpecreduceOperation
 
 
 __all__ = ['FluxCalibration']
 
 
 class FluxCalibration(SpecreduceOperation):
@@ -147,24 +143,24 @@
         ----------
         stdstar : str
             Name of the standard star file in the specreduce/datasets/onedstds
             directory to be used for the flux calibration. The user must provide the
             subdirectory and file name.
 
             For example:
-            >>> standard_sensfunc(obj_wave, obj_flux, stdstar='spec50cal/bd284211.dat', \
-             mode='spline')  # doctest: +SKIP
+
+            >>> standard_sensfunc(obj_wave, obj_flux, stdstar='spec50cal/bd284211.dat', mode='spline')  # doctest: +SKIP
 
             If no std is supplied, or an improper path is given, raises a ValueError.
 
         Returns
         -------
         standard: astropy.talbe.Table
             A table with the onedstd data.
-        """
+        """  # noqa: E501
         std_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)),
                                'datasets', 'onedstds')
 
         if not os.path.isfile(os.path.join(std_dir, stdstar)):
             msg = "No valid standard star found at: " + os.path.join(std_dir, stdstar)
             raise ValueError(msg)
 
@@ -194,14 +190,15 @@
         mode : str, optional
             Can be "linear", "spline", or "poly" (Default is linear).
         polydeg : float, optional
             if mode='poly', this is the order of the polynomial to fit through.
             (Default is 9.)
         display : bool, optional
             If True, plot the sensfunc. (Default is False.)
+            This requires ``matplotlib`` to be installed.
         badlines : array-like list
             A list of values (lines) to mask-out of when generating sensfunc.
 
         Returns
         -------
         sensfunc_spec : specutils.Spectrum1D
             The sensitivity function in the covered wavelength range
@@ -256,14 +253,15 @@
             sensfunc2 = np.polyval(fit, obj_wave.value)
 
         sensfunc_out = (10 ** sensfunc2) * standard['flux'].unit / obj_flux.unit
 
         sensfunc_spec = Spectrum1D(spectral_axis=obj_wave, flux=sensfunc_out)
 
         if display is True:
+            import matplotlib.pyplot as plt
             plt.figure()
             plt.plot(obj_wave, obj_flux * sensfunc_out, c="C0",
                      label="Observed x sensfunc", alpha=0.5)
 
             # plt.scatter(standard['wave'], std_flux, color='C1', alpha=0.75, label="stdstar")
             plt.scatter(obj_wave_ds, std_flux_ds, color='C1', alpha=0.75)
```

### Comparing `specreduce-1.3.0/specreduce/table_utils.py` & `specreduce-1.4.0/specreduce/table_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-"""Utility functions to parse main NIST table.
-"""
+"""Utility functions to parse main NIST table."""
 
-from astropy.table import Table, vstack
 import numpy as np
+from astropy.table import Table, vstack
+
+__all__ = []
 
 
 def sort_table_by_element(table, elem_list):
     """Build table based on list of elements
 
     Parameters
     ----------
```

### Comparing `specreduce-1.3.0/specreduce/tests/test_extinction.py` & `specreduce-1.4.0/specreduce/tests/test_extinction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,81 @@
-import pytest
-
 import numpy as np
-
-import astropy.units as u
+import pytest
+from astropy import units as u
 from astropy.utils.exceptions import AstropyUserWarning
 
-from ..calibration_data import (
+from specreduce.calibration_data import (
     AtmosphericExtinction,
     AtmosphericTransmission,
     SUPPORTED_EXTINCTION_MODELS
 )
 
 
+@pytest.mark.remote_data
 def test_supported_models():
     """
     Test loading of supported models
     """
     for model in SUPPORTED_EXTINCTION_MODELS:
         ext = AtmosphericExtinction(model=model)
         assert len(ext.extinction_mag) > 0
         assert len(ext.transmission) > 0
 
 
+@pytest.mark.remote_data
 def test_custom_mag_model():
     """
     Test creation of custom model from Quantity arrays
     """
     wave = np.linspace(0.3, 2.0, 50)
     extinction = u.Magnitude(1. / wave, u.MagUnit(u.dimensionless_unscaled))
     ext = AtmosphericExtinction(extinction=extinction, spectral_axis=wave * u.um)
     assert len(ext.extinction_mag) > 0
     assert len(ext.transmission) > 0
 
 
+@pytest.mark.remote_data
 def test_custom_raw_mag_model():
     """
     Test creation of custom model from Quantity arrays
     """
     wave = np.linspace(0.3, 2.0, 50)
     extinction = 1. / wave * u.mag
     ext = AtmosphericExtinction(extinction=extinction, spectral_axis=wave * u.um)
     assert len(ext.extinction_mag) > 0
     assert len(ext.transmission) > 0
 
 
+@pytest.mark.remote_data
 def test_custom_linear_model():
     """
     Test creation of custom model from Quantity arrays
     """
     wave = np.linspace(0.3, 2.0, 50)
     extinction = 1. / wave * u.dimensionless_unscaled
     ext = AtmosphericExtinction(extinction=extinction, spectral_axis=wave * u.um)
     assert len(ext.extinction_mag) > 0
     assert len(ext.transmission) > 0
 
 
+@pytest.mark.remote_data
 def test_missing_extinction_unit():
     """
     Test creation of custom model from Quantity arrays
     """
     wave = np.linspace(0.3, 2.0, 50)
     extinction = 1. / wave
     with pytest.warns(AstropyUserWarning):
         ext = AtmosphericExtinction(extinction=extinction, spectral_axis=wave * u.um)
 
     assert len(ext.extinction_mag) > 0
     assert len(ext.transmission) > 0
 
 
+@pytest.mark.remote_data
 def test_transmission_model():
     """
     Test creating of default atmospheric transmission model
     """
     ext = AtmosphericTransmission()
     assert len(ext.transmission) > 0
```

### Comparing `specreduce-1.3.0/specreduce/tests/test_image_parsing.py` & `specreduce-1.4.0/specreduce/tests/test_image_parsing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,23 @@
 import numpy as np
-
 from astropy import units as u
-from astropy.io import fits
-from astropy.nddata import CCDData, NDData, VarianceUncertainty
-from astropy.utils.data import download_file
+from specutils import Spectrum1D
 
+from specreduce.core import _ImageParser
 from specreduce.extract import HorneExtract
 from specreduce.tracing import FlatTrace
-from specutils import Spectrum1D, SpectralAxis
-
-
-# fetch test image
-fn = download_file('https://stsci.box.com/shared/static/exnkul627fcuhy5akf2gswytud5tazmw.fits',
-                   cache=True)
-
-# duplicate image in all accepted formats
-# (one Spectrum1D variant has a physical spectral axis; the other is in pixels)
-img = fits.getdata(fn).T
-flux = img * u.MJy / u.sr
-sax = SpectralAxis(np.linspace(14.377, 3.677, flux.shape[-1]) * u.um)
-unc = VarianceUncertainty(np.random.rand(*flux.shape))
-
-all_images = {}
-all_images['arr'] = img
-all_images['s1d'] = Spectrum1D(flux, spectral_axis=sax, uncertainty=unc)
-all_images['s1d_pix'] = Spectrum1D(flux, uncertainty=unc)
-all_images['ccd'] = CCDData(img, uncertainty=unc, unit=flux.unit)
-all_images['ndd'] = NDData(img, uncertainty=unc, unit=flux.unit)
-all_images['qnt'] = img * flux.unit
-
-# save default values used for spectral axis and uncertainty when they are not
-# available from the image object or provided by the user
-sax_def = np.arange(img.shape[1]) * u.pix
-unc_def = np.ones_like(img)
 
 
 # (for use inside tests)
-def compare_images(key, collection, compare='s1d'):
+def compare_images(all_images, key, collection, compare='s1d'):
+    # save default values used for spectral axis and uncertainty when they are not
+    # available from the image object or provided by the user
+    unc_def = np.ones_like(all_images['arr'])
+    sax_def = np.arange(unc_def.shape[1]) * u.pix
+
     # was input converted to Spectrum1D?
     assert isinstance(collection[key], Spectrum1D), (f"image '{key}' not "
                                                      "of type Spectrum1D")
 
     # do key's fluxes match its comparison's fluxes?
     assert np.allclose(collection[key].data,
                        collection[compare].data), (f"images '{key}' and "
@@ -67,39 +44,43 @@
     assert (getattr(collection[key], 'mask', None)
             is not None), f"no mask was created for image '{key}'"
     assert np.all(collection[key].mask == 0), ("mask not all False "
                                                f"for image '{key}'")
 
 
 # test consistency of general image parser results
-def test_parse_general():
-    all_images_parsed = {k: FlatTrace._parse_image(object, im)
-                         for k, im in all_images.items()}
+def test_parse_general(all_images):
 
+    all_images_parsed = {k: _ImageParser()._parse_image(im)
+                         for k, im in all_images.items()}
     for key in all_images_parsed.keys():
-        compare_images(key, all_images_parsed)
+        compare_images(all_images, key, all_images_parsed)
 
 
 # use verified general image parser results to check HorneExtract's image parser
-def test_parse_horne():
+def test_parse_horne(all_images):
+    # save default values used for uncertainty when it is
+    # available from the image object or provided by the user
+    unc_def = np.ones_like(all_images['arr'])
+
     # HorneExtract's parser is more stringent than the general one, hence the
     # separate test. Given proper inputs, both should produce the same results.
     images_collection = {k: {} for k in all_images.keys()}
 
     for key, col in images_collection.items():
         img = all_images[key]
-        col['general'] = FlatTrace._parse_image(object, img)
+        col['general'] = _ImageParser()._parse_image(img)
 
         if hasattr(all_images[key], 'uncertainty'):
             defaults = {}
         else:
             # save default values of attributes used in general parser when
             # they are not available from the image object. HorneExtract always
             # requires a variance, so it's chosen here to be on equal footing
             # with the general case
             defaults = {'variance': unc_def,
                         'mask': ~np.isfinite(img),
                         'unit': getattr(img, 'unit', u.DN)}
 
-        col[key] = HorneExtract._parse_image(object, img, **defaults)
+        col[key] = HorneExtract(img, FlatTrace(img, 2))._parse_image(img, **defaults)
 
-        compare_images(key, col, compare='general')
+        compare_images(all_images, key, col, compare='general')
```

### Comparing `specreduce-1.3.0/specreduce/tracing.py` & `specreduce-1.4.0/specreduce/tracing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
+import warnings
 from copy import deepcopy
 from dataclasses import dataclass, field
-import warnings
 
+import numpy as np
 from astropy.modeling import Model, fitting, models
 from astropy.nddata import NDData
 from astropy.stats import gaussian_sigma_to_fwhm
 from astropy.utils.decorators import deprecated
-import numpy as np
 
 from specreduce.core import _ImageParser
 
 __all__ = ['Trace', 'FlatTrace', 'ArrayTrace', 'FitTrace']
 
 
 @dataclass
@@ -106,14 +106,16 @@
         Set the trace position within the image
 
         Parameters
         ----------
         trace_pos : float
             Position of the trace
         """
+        if trace_pos < 1:
+            raise ValueError('`trace_pos` must be positive.')
         self.trace_pos = trace_pos
         self.trace = np.ones_like(self.image.data[0]) * self.trace_pos
         self._bound_trace()
 
 
 @dataclass
 class ArrayTrace(Trace, _ImageParser):
@@ -205,14 +207,16 @@
     window: int = None
     trace_model: Model = field(default=models.Polynomial1D(degree=1))
     peak_method: str = 'max'
     _crossdisp_axis = 0
     _disp_axis = 1
 
     def __post_init__(self):
+
+        # parse image
         self.image = self._parse_image(self.image)
 
         # mask any previously uncaught invalid values
         or_mask = np.logical_or(self.image.mask, ~np.isfinite(self.image.data))
         img = np.ma.masked_array(self.image.data, or_mask)
 
         # validate arguments
@@ -258,22 +262,28 @@
                  or self.window < 1)):
             raise ValueError(f"window must be >= 2 and less than {cols}, the "
                              "length of the image's spatial direction")
         elif self.window is not None and not isinstance(self.window, int):
             warnings.warn('TRACE: Converting window to int')
             self.window = int(self.window)
 
+        # fit the trace
+        self._fit_trace(img)
+
+    def _fit_trace(self, img):
+
+        yy = np.arange(img.shape[self._crossdisp_axis])
+
         # set max peak location by user choice or wavelength with max avg flux
         ztot = img.sum(axis=self._disp_axis) / img.shape[self._disp_axis]
         peak_y = self.guess if self.guess is not None else ztot.argmax()
         # NOTE: peak finder can be bad if multiple objects are on slit
 
-        yy = np.arange(img.shape[self._crossdisp_axis])
-
         if self.peak_method == 'gaussian':
+
             # guess the peak width as the FWHM, roughly converted to gaussian sigma
             yy_above_half_max = np.sum(ztot > (ztot.max() / 2))
             width_guess = yy_above_half_max / gaussian_sigma_to_fwhm
 
             # enforce some (maybe sensible?) rules about trace peak width
             width_guess = (2 if width_guess < 2
                            else 25 if width_guess > 25
@@ -288,33 +298,42 @@
             fitter = fitting.LevMarLSQFitter()
             popt_tot = fitter(profile, yy, ztot)
 
         # restrict fit to window (if one exists)
         ilum2 = (yy if self.window is None
                  else yy[np.arange(peak_y - self.window,
                                    peak_y + self.window, dtype=int)])
+
+        # check if everything in window region is masked
         if img[ilum2].mask.all():
             raise ValueError('All pixels in window region are masked. Check '
                              'for invalid values or use a larger window value.')
 
         x_bins = np.linspace(0, img.shape[self._disp_axis],
                              self.bins + 1, dtype=int)
         y_bins = np.tile(np.nan, self.bins)
 
+        warn_bins = []
         for i in range(self.bins):
-            # repeat earlier steps to create gaussian fit for each bin
+
+            # binned columns, summed along disp. axis.
+            # or just a single, unbinned column if no bins
             z_i = img[ilum2, x_bins[i]:x_bins[i+1]].sum(axis=self._disp_axis)
-            if not z_i.mask.all():
-                peak_y_i = ilum2[z_i.argmax()]
-            else:
-                warnings.warn(f"All pixels in bin {i} are masked. Falling "
-                              'to trace value from all-bin fit.')
-                peak_y_i = peak_y
+
+            # if this bin is fully masked, set bin peak to NaN so it can be
+            # filtered in the final fit to all bin peaks for the trace
+            if z_i.mask.all():
+                warn_bins.append(i)
+                y_bins[i] = np.nan
+                continue
 
             if self.peak_method == 'gaussian':
+
+                peak_y_i = ilum2[z_i.argmax()]
+
                 yy_i_above_half_max = np.sum(z_i > (z_i.max() / 2))
                 width_guess_i = yy_i_above_half_max / gaussian_sigma_to_fwhm
 
                 # NOTE: original KOSMOS code mandated width be greater than 2
                 # (to avoid cosmic rays) and less than 25 (to avoid fitting noise).
                 # we should extract values from img to derive similar limits
                 # width_guess_i = (2 if width_guess_i < 2
@@ -334,22 +353,41 @@
                     y_bins[i] = popt_tot.mean_0.value
                 else:
                     y_bins[i] = popt_i.mean_0.value
                     popt_tot = popt_i
 
             elif self.peak_method == 'centroid':
                 z_i_cumsum = np.cumsum(z_i)
-                # find the interpolated index where the cumulative array reaches half the total
-                # cumulative values
+                # find the interpolated index where the cumulative array reaches
+                # half the total cumulative values
                 y_bins[i] = np.interp(z_i_cumsum[-1]/2., z_i_cumsum, ilum2)
 
+                # NOTE this reflects current behavior, should eventually be changed
+                # to set to nan by default (or zero fill / interpoate option once
+                # available)
+
             elif self.peak_method == 'max':
                 # TODO: implement smoothing with provided width
                 y_bins[i] = ilum2[z_i.argmax()]
 
+                # NOTE: a fully masked should eventually be changed to set to
+                # nan by default (or zero fill / interpoate option once available)
+
+        # warn about fully-masked bins
+        if len(warn_bins) > 0:
+
+            # if there are a ton of bins, we don't want to print them all out
+            if len(warn_bins) > 20:
+                warn_bins = warn_bins[0: 10] + ['...'] + [warn_bins[-1]]
+
+            warnings.warn(f"All pixels in {'bins' if len(warn_bins) else 'bin'} "
+                          f"{', '.join([str(x) for x in warn_bins])}"
+                          " are fully masked. Setting bin"
+                          f" peak{'s' if len(warn_bins) else ''} to NaN.")
+
         # recenter bin positions
         x_bins = (x_bins[:-1] + x_bins[1:]) / 2
 
         # interpolate the fitted trace over the entire wavelength axis
         y_finite = np.where(np.isfinite(y_bins))[0]
         if y_finite.size > 0:
             x_bins = x_bins[y_finite]
```

### Comparing `specreduce-1.3.0/specreduce.egg-info/SOURCES.txt` & `specreduce-1.4.0/specreduce.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+.flake8
 .gitignore
-.readthedocs.yml
+.readthedocs.yaml
 CHANGES.rst
 CITATION.cff
 MANIFEST.in
 README.rst
+conftest.py
 pyproject.toml
-setup.cfg
-setup.py
 tox.ini
 .github/workflows/cron-tests.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/tox-tests.yml
 docs/Makefile
 docs/api.rst
 docs/atm_transmission_secz1.5_1.6mm.dat
 docs/conf.py
 docs/extinction.rst
 docs/extraction_quickstart.rst
 docs/index.rst
 docs/make.bat
 docs/specphot_standards.rst
+docs/terms.rst
+docs/wavelength_calibration.rst
+docs/_static/logo_icon.ico
+docs/_static/logo_icon.png
+docs/_static/specreduce.css
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 docs/process/NIR_MOS_arc.odg
 docs/process/NIR_MOS_arc.svg
 docs/process/NIR_MOS_flat.odg
 docs/process/NIR_MOS_flat.svg
@@ -33,49 +38,41 @@
 docs/process/NIR_MOS_trace.svg
 docs/process/NIR_arcs.rst
 docs/process/NIR_flats.rst
 docs/process/NIR_science_data.rst
 docs/process/index.rst
 licenses/KOSMOS_LICENSE
 licenses/LICENSE.rst
-notebook_sandbox/README.md
-notebook_sandbox/apo05.ipynb
-notebook_sandbox/compare_extractions.ipynb
-notebook_sandbox/dev.ipynb
-notebook_sandbox/flatfield_demo.ipynb
-notebook_sandbox/fluxcal_demo.ipynb
-notebook_sandbox/identify_demo.ipynb
-notebook_sandbox/tracing_options.ipynb
-notebook_sandbox/horne_extract/optimal_extract_VLT.ipynb
-notebook_sandbox/horne_extract/requirements.txt
-notebook_sandbox/jwst_boxcar/boxcar_extraction.ipynb
-notebook_sandbox/jwst_boxcar/jwst_boxcar_algorithm.ipynb
-notebook_sandbox/jwst_boxcar/pre-requirements.txt
-notebook_sandbox/jwst_boxcar/requirements.txt
 specreduce/__init__.py
-specreduce/_astropy_init.py
 specreduce/background.py
 specreduce/calibration_data.py
 specreduce/conftest.py
 specreduce/core.py
 specreduce/extract.py
 specreduce/fluxcal.py
+specreduce/line_matching.py
 specreduce/table_utils.py
 specreduce/tracing.py
 specreduce/version.py
+specreduce/wavelength_calibration.py
 specreduce.egg-info/PKG-INFO
 specreduce.egg-info/SOURCES.txt
 specreduce.egg-info/dependency_links.txt
-specreduce.egg-info/not-zip-safe
 specreduce.egg-info/requires.txt
 specreduce.egg-info/top_level.txt
 specreduce/tests/__init__.py
 specreduce/tests/test_background.py
 specreduce/tests/test_extinction.py
 specreduce/tests/test_extract.py
 specreduce/tests/test_get_reference_file_path.py
 specreduce/tests/test_image_parsing.py
+specreduce/tests/test_line_matching.py
+specreduce/tests/test_linelists.py
 specreduce/tests/test_specphot_stds.py
 specreduce/tests/test_synth_data.py
 specreduce/tests/test_tracing.py
+specreduce/tests/test_utils.py
+specreduce/tests/test_wavelength_calibration.py
+specreduce/tests/data/transposed_det_image_seq5_MIRIMAGE_P750Lexp1_s2d.fits
 specreduce/utils/__init__.py
-specreduce/utils/synth_data.py
+specreduce/utils/synth_data.py
+specreduce/utils/utils.py
```

### Comparing `specreduce-1.3.0/tox.ini` & `specreduce-1.4.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 [tox]
 envlist =
-    py{38,39,310}-test{,-devdeps,-datadeps}{,-cov}
-    py{38,39,310}-test-numpy{118,119,120,121}
-    py{38,39,310}-test-astropy{lts,rc}
-    build_docs
+    py{310,311,312}-test{,-alldeps}{,-oldestdeps,-devdeps,-predeps}{,-cov}
+    linkcheck
     codestyle
-requires =
-    setuptools >= 30.3.0
-    pip >= 19.3.1
-isolated_build = true
 
 [testenv]
 
 # Pass through the following environment variables which may be needed for the CI
-passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI
+passenv = HOME,WINDIR,CI
 
 setenv =
-    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scipy-wheels-nightly/simple
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/astropy/simple https://pypi.anaconda.org/liberfa/simple https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
 
 # Run the tests in a temporary directory to make sure that we don't import
 # this package from the source tree
 changedir = .tmp/{envname}
 
 # tox environments are constructed with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
@@ -28,78 +22,65 @@
 # see a list of example environments that can be run, along with a description,
 # run:
 #
 #     tox -l -v
 #
 description =
     run tests
-    datadeps: with specreduce_data package installed locally
-    devdeps: with the latest developer version of key dependencies
+    alldeps: with optional dependencies
     oldestdeps: with the oldest supported version of key dependencies
-    cov: and test coverage
-    numpy118: with numpy 1.18.*
-    numpy119: with numpy 1.19.*
-    numpy120: with numpy 1.20.*
-    numpy121: with numpy 1.21.*
-    astropylts: with the latest astropy LTS
+    devdeps: with the latest developer version of key dependencies
+    predeps: with pre-releases of key dependencies
+    cov: with test coverage
 
 # The following provides some specific pinnings for key packages
 deps =
 
-    numpy118: numpy==1.18.*
-    numpy119: numpy==1.19.*
-    numpy120: numpy==1.20.*
-    numpy121: numpy==1.21.*
-
-    astropy50: astropy==5.0.*
-    astropylts: astropy==5.0.*
-
     devdeps: numpy>=0.0.dev0
-    devdeps: git+https://github.com/astropy/astropy.git#egg=astropy
+    devdeps: scipy>=0.0.dev0
+    devdeps: pyerfa>=0.0.dev0
+    devdeps: astropy>=0.0.dev0
     devdeps: git+https://github.com/astropy/specutils.git#egg=specutils
+    devdeps: git+https://github.com/astropy/photutils.git#egg=photutils
+    devdeps: git+https://github.com/spacetelescope/synphot_refactor.git#egg=synphot
 
-    datadeps: git+https://github.com/astropy/specreduce-data.git#egg=specreduce_data
-
-    oldestdeps: numpy==1.18
-    oldestdeps: astropy==5.0
-    oldestdeps: scipy==1.6.0
-    oldestdeps: matplotlib==3.4
-    oldestdeps: photutils==1.0.0
-    oldestdeps: specutils==1.7.0
+    oldestdeps: numpy==1.22.*
+    oldestdeps: astropy==5.1.*
+    oldestdeps: scipy==1.8.*
+    oldestdeps: matplotlib==3.5.*
+    oldestdeps: photutils==1.0.*
+    oldestdeps: specutils==1.9.*
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
-    test: test
-    build_docs: docs
+    test
+    alldeps: all
+
+install_command =
+    !devdeps: python -I -m pip install
+    # Force dev dependency with C-extension (synphot) to also build with numpy-dev
+    devdeps: python -I -m pip install -v --pre
 
 commands =
     pip freeze
     !cov: pytest --pyargs specreduce {toxinidir}/docs {posargs}
-    cov: pytest --pyargs specreduce {toxinidir}/docs --cov specreduce --cov-config={toxinidir}/setup.cfg {posargs}
+    cov: pytest --pyargs specreduce {toxinidir}/docs --cov specreduce --cov-config={toxinidir}/pyproject.toml {posargs}
     cov: coverage xml -o {toxinidir}/coverage.xml
 
 pip_pre =
     predeps: true
     !predeps: false
 
-[testenv:build_docs]
-changedir = docs
-description = invoke sphinx-build to build the HTML docs
-extras = docs
-commands =
-    pip freeze
-    sphinx-build -W -b html . _build/html
-
 [testenv:linkcheck]
 changedir = docs
 description = check the links in the HTML docs
 extras = docs
 commands =
     pip freeze
     sphinx-build -W -b linkcheck . _build/html
 
 [testenv:codestyle]
 skip_install = true
 changedir = .
-description = check code style, e.g. with flake8
+description = check code style, e.g., with flake8
 deps = flake8
-commands = flake8 specreduce --count --max-line-length=100
+commands = flake8 specreduce --count
```

