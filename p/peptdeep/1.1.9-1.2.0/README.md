# Comparing `tmp/peptdeep-1.1.9.tar.gz` & `tmp/peptdeep-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptdeep-1.1.9.tar", last modified: Fri Apr 12 07:35:22 2024, max compression
+gzip compressed data, was "peptdeep-1.2.0.tar", last modified: Wed May 29 20:21:27 2024, max compression
```

## Comparing `peptdeep-1.1.9.tar` & `peptdeep-1.2.0.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.230252 peptdeep-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-12 07:34:59.000000 peptdeep-1.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 07:34:59.000000 peptdeep-1.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    40528 2024-04-12 07:35:22.230252 peptdeep-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32817 2024-04-12 07:34:59.000000 peptdeep-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/cli_argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/constants/_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/constants/default_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/constants/model_const.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll
--rw-r--r--   0 runner    (1001) docker     (127)   620032 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26311 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/pyrawfilereader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/mass_spec/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/mass_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/mass_spec/mass_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14429 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/mass_spec/match.py
--rw-r--r--   0 runner    (1001) docker     (127)    14666 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/mass_spec/ms_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/model/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31677 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/building_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/ccs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/featurize.py
--rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/generic_property_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    31129 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/model_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/model_shop.py
--rw-r--r--   0 runner    (1001) docker     (127)    26804 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/ms2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/rt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/pipeline_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41087 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/pretrained_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/protein/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/protein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/protein/fasta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/psm_frag_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/psm_frag_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/psm_frag_reader/maxquant_frag_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/psm_frag_reader/psm_frag_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/psm_frag_reader/psmlabel_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/rescore/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/rescore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/rescore/fdr.py
--rw-r--r--   0 runner    (1001) docker     (127)    39861 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/rescore/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/rescore/percolator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/spec_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/spec_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/spec_lib/library_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/spec_lib/predict_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/spec_lib/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/_pyinstaller_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/device_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/webui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/library_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/webui/logos/
--rw-r--r--   0 runner    (1001) docker     (127)   118381 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/logos/peptdeep.ico
--rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/logos/peptdeep.png
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/main_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/model_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/rescore_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/server_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/settings_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/startpage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/transfer_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/ui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40528 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:35:22.230252 peptdeep-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-12 07:34:59.000000 peptdeep-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.222252 peptdeep-1.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 07:34:59.000000 peptdeep-1.1.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 07:34:59.000000 peptdeep-1.1.9/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.427364 peptdeep-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-29 20:20:55.000000 peptdeep-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 20:20:55.000000 peptdeep-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40162 2024-05-29 20:21:27.427364 peptdeep-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32229 2024-05-29 20:20:55.000000 peptdeep-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.403364 peptdeep-1.2.0/peptdeep/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.407364 peptdeep-1.2.0/peptdeep/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/cli_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.407364 peptdeep-1.2.0/peptdeep/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/constants/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/constants/default_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/constants/model_const.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.407364 peptdeep-1.2.0/peptdeep/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.407364 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   620032 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26311 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/pyrawfilereader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.411364 peptdeep-1.2.0/peptdeep/mass_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/mass_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/mass_spec/mass_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/mass_spec/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/mass_spec/ms_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.411364 peptdeep-1.2.0/peptdeep/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31537 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/building_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/ccs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/featurize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15390 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/generic_property_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36564 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/model_shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26671 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/ms2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/rt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18706 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/pipeline_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40941 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/pretrained_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.411364 peptdeep-1.2.0/peptdeep/protein/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/protein/fasta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.411364 peptdeep-1.2.0/peptdeep/psm_frag_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/psm_frag_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/psm_frag_reader/maxquant_frag_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/psm_frag_reader/psm_frag_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/psm_frag_reader/psmlabel_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/rescore/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/rescore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/rescore/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39596 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/rescore/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/rescore/percolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/spec_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/spec_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/spec_lib/library_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/spec_lib/predict_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/spec_lib/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/_pyinstaller_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/device_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/webui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/library_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/webui/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)   118381 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/logos/peptdeep.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/logos/peptdeep.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/main_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/model_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/rescore_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/server_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/settings_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/startpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/transfer_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/ui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.419364 peptdeep-1.2.0/peptdeep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40162 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 20:20:55.000000 peptdeep-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:21:27.427364 peptdeep-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-29 20:20:55.000000 peptdeep-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.419364 peptdeep-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 20:20:55.000000 peptdeep-1.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 20:20:55.000000 peptdeep-1.2.0/tests/test_gui.py
```

### Comparing `peptdeep-1.1.9/LICENSE.txt` & `peptdeep-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.9/PKG-INFO` & `peptdeep-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptdeep
-Version: 1.1.9
+Version: 1.2.0
 Summary: The AlphaX deep learning framework for Proteomics
 Home-page: https://github.com/MannLabs/peptdeep
 Author: Mann Labs
 Author-email: jalew.zwf@qq.com
 License: Apache 2.0
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
@@ -45,15 +45,14 @@
 Requires-Dist: jupyter; extra == "development-stable"
 Requires-Dist: twine; extra == "development-stable"
 Requires-Dist: bumpversion; extra == "development-stable"
 Requires-Dist: pipdeptree; extra == "development-stable"
 Requires-Dist: ipykernel; extra == "development-stable"
 Requires-Dist: tqdm; extra == "development-stable"
 Requires-Dist: wget; extra == "development-stable"
-Requires-Dist: nbdev; extra == "development-stable"
 Requires-Dist: pyinstaller; extra == "development-stable"
 Requires-Dist: click; extra == "development-stable"
 Requires-Dist: pandas; extra == "development-stable"
 Requires-Dist: numpy; extra == "development-stable"
 Requires-Dist: seaborn; extra == "development-stable"
 Requires-Dist: matplotlib; extra == "development-stable"
 Requires-Dist: numba; extra == "development-stable"
@@ -70,25 +69,27 @@
 Requires-Dist: jinja2; extra == "development-stable"
 Requires-Dist: contextfilter; extra == "development-stable"
 Requires-Dist: furo; extra == "development-stable"
 Requires-Dist: torch; extra == "development-stable"
 Requires-Dist: streamlit>=1.23.0; extra == "development-stable"
 Requires-Dist: alphabase>=1.1.0; extra == "development-stable"
 Requires-Dist: alpharaw>=0.2.0; extra == "development-stable"
+Requires-Dist: pytest; extra == "development-stable"
+Requires-Dist: pre-commit==3.7.0; extra == "development-stable"
+Requires-Dist: nbmake==1.5.3; extra == "development-stable"
 Provides-Extra: development
 Requires-Dist: pywin32; sys_platform == "win32" and extra == "development"
 Requires-Dist: pythonnet; sys_platform == "win32" and extra == "development"
 Requires-Dist: jupyter; extra == "development"
 Requires-Dist: twine; extra == "development"
 Requires-Dist: bumpversion; extra == "development"
 Requires-Dist: pipdeptree; extra == "development"
 Requires-Dist: ipykernel; extra == "development"
 Requires-Dist: tqdm; extra == "development"
 Requires-Dist: wget; extra == "development"
-Requires-Dist: nbdev; extra == "development"
 Requires-Dist: pyinstaller; extra == "development"
 Requires-Dist: click; extra == "development"
 Requires-Dist: pandas; extra == "development"
 Requires-Dist: numpy; extra == "development"
 Requires-Dist: seaborn; extra == "development"
 Requires-Dist: matplotlib; extra == "development"
 Requires-Dist: numba; extra == "development"
@@ -105,14 +106,17 @@
 Requires-Dist: jinja2; extra == "development"
 Requires-Dist: contextfilter; extra == "development"
 Requires-Dist: furo; extra == "development"
 Requires-Dist: torch; extra == "development"
 Requires-Dist: streamlit; extra == "development"
 Requires-Dist: alphabase; extra == "development"
 Requires-Dist: alpharaw; extra == "development"
+Requires-Dist: pytest; extra == "development"
+Requires-Dist: pre-commit; extra == "development"
+Requires-Dist: nbmake; extra == "development"
 Provides-Extra: gui-stable
 Requires-Dist: pywin32; sys_platform == "win32" and extra == "gui-stable"
 Requires-Dist: pythonnet; sys_platform == "win32" and extra == "gui-stable"
 Requires-Dist: click; extra == "gui-stable"
 Requires-Dist: pandas; extra == "gui-stable"
 Requires-Dist: numpy; extra == "gui-stable"
 Requires-Dist: torch; extra == "gui-stable"
@@ -429,28 +433,14 @@
 ***By using the editable flag `-e`, all modifications to the [peptdeep
 source code folder](peptdeep) are directly reflected when running
 peptdeep. Note that the peptdeep folder cannot be moved and/or renamed
 if an editable version is installed. In case of confusion, you can
 always retrieve the location of any Python module with e.g. the command
 `import module` followed by `module.__file__`.***
 
-We used [nbdev v2](https://nbdev.fast.ai/) for developers to build
-Python source code and docs smoothly from Python notebooks, so please do
-not edit .py files directly, edit .ipynb in `nbdev_nbs` folder instead.
-After installing nbdev, cd to alphapeptdeep project folder and run:
-
-``` bash
-nbdev_install_hooks
-```
-
-to init gitconfig for nbdev. After editing the source code in .ipynb
-files, using `nbdev_export` to build python source code and `nbdev_test`
-to run all .ipynb files in `nbdev_nbs` for testing. Check [nbdev
-docs](https://nbdev.fast.ai/) for more information.
-
 ------------------------------------------------------------------------
 
 ## Usage
 
 There are three ways to use peptdeep:
 
 - [**GUI**](#gui)
@@ -527,15 +517,15 @@
 ```
 
 This command will export the default settings into the `settings.yaml`
 as a template, users can edit the yaml file to run other commands.
 
 Here is a section of the yaml file which controls global parameters for
 different tasks:
-  
+
 ```
 model_url: "https://github.com/MannLabs/alphapeptdeep/releases/download/pre-trained-models/pretrained_models.zip"
 
 task_type: library
 task_type_choices:
   - library
   - train
@@ -558,15 +548,15 @@
   - critical
 
 common:
   modloss_importance_level: 1.0
   user_defined_modifications: {}
   # For example,
   # user_defined_modifications:
-  #   "Dimethyl2@Any N-term": 
+  #   "Dimethyl2@Any N-term":
   #     composition: "H(2)2H(2)C(2)"
   #     modloss_composition: "H(0)" # can be without if no modloss
   #   "Dimethyl2@K":
   #     composition: "H(2)2H(2)C(2)"
   #   "Dimethyl6@Any N-term":
   #     composition: "2H(4)13C(2)"
   #   "Dimethyl6@K":
@@ -626,15 +616,15 @@
 ``` bash
 peptdeep cmd-flow ...
 ```
 
 Support CLI parameters to control `global_settings` for CLI users. It supports three workflows: `train`, `library` or `train library`, controlled by CLI parameter `--task_workflow`, for example, `--task_workflow train library`. All settings in [global_settings](peptdeep/constants/default_settings.yaml) are converted to CLI parameters using `--` as the dict level indicator, for example, `global_settings["library"]["var_mods"]` corresponds to `--library--var_mods`. See [test_cmd_flow.sh](tests/test_cmd_flow.sh) for example.
 
 There are three kinds of parameter types:
-  1. value type (int, float, bool, str): The CLI parameter only has a single value, for instance: `--model_mgr--default_instrument 30.0`. 
+  1. value type (int, float, bool, str): The CLI parameter only has a single value, for instance: `--model_mgr--default_instrument 30.0`.
   2. list type (list): The CLI parameter has a list of values seperated by a space, for instance `--library--var_mods "Oxidation@M" "Acetyl@Protein_N-term"`.
   3. dict type (dict): Only three parameters are `dict type`, `--library--labeling_channels`, `--model_mgr--transfer--psm_modification_mapping`, and `--common--user_defined_modifications`. Here are the examples:
     - `--library--labeling_channels`: labeling channels for the library. Example: `--library--labeling_channels "0:Dimethyl@Any_N-term;Dimethyl@K" "4:xx@Any_N-term;xx@K"`
     - `--model_mgr--transfer--psm_modification_mapping`: converting other search engines' modification names to alphabase modifications for transfer learning. Example: `--model_mgr--transfer--psm_modification_mapping "Dimethyl@Any_N-term:_(Dimethyl-n-0);_(Dimethyl)" "Dimethyl@K:K(Dimethyl-K-0);K(Dimethyl)"`. Note that `X(UniMod:id)` format can directly be recognized by alphabase.
     - `--common--user_defined_modification`: user defined modifications. Example:`--common--user_defined_modification "NewMod1@Any_N-term:H(2)2H(2)C(2)" "NewMod2@K:H(100)O(2)C(2)"`
 
 #### library
@@ -652,15 +642,15 @@
 library:
   infile_type: fasta
   infile_type_choices:
   - fasta
   - sequence_table
   - peptide_table # sequence with mods and mod_sites
   - precursor_table # peptide with charge state
-  infiles: 
+  infiles:
   - xxx.fasta
   fasta:
     protease: 'trypsin'
     protease_choices:
     - 'trypsin'
     - '([KR])'
     - 'trypsin_not_P'
@@ -670,15 +660,15 @@
     - 'lys-n'
     - '\w(?=K)'
     - 'chymotrypsin'
     - 'asp-n'
     - 'glu-c'
     max_miss_cleave: 2
     add_contaminants: False
-  fix_mods: 
+  fix_mods:
   - Carbamidomethyl@C
   var_mods:
   - Acetyl@Protein N-term
   - Oxidation@M
   special_mods: [] # normally for Phospho or GlyGly@K
   special_mods_cannot_modify_pep_n_term: False
   special_mods_cannot_modify_pep_c_term: False
@@ -781,15 +771,15 @@
 
 ``` python
 df
 ```
 
 |  | sequence | mods | mod_sites | charge |
 | --- | --- | --- | --- | --- |
-| 0 | ACDEFGHIK | Carbamidomethyl@C | 2 | 2 | 
+| 0 | ACDEFGHIK | Carbamidomethyl@C | 2 | 2 |
 | 1 | LMNPQRSTVK | Acetyl@Protein N-term;Phospho@S | 0;7 | 3 |
 | 2 | WYVSTR | | | 1 |
 
 > Columns of `proteins` and `genes` are optional for these txt/tsv/csv
 > files.
 
 peptdeep supports multiple files for library prediction, for example (in
@@ -859,22 +849,22 @@
     psm_num_to_train_ms2: 100000000
     psm_num_per_mod_to_train_ms2: 50
     psm_num_to_test_ms2: 0
     psm_num_to_train_rt_ccs: 100000000
     psm_num_per_mod_to_train_rt_ccs: 50
     psm_num_to_test_rt_ccs: 0
     top_n_mods_to_train: 10
-    psm_modification_mapping: {} 
+    psm_modification_mapping: {}
     # alphabase modification to modifications of other search engines
     # For example,
     # psm_modification_mapping:
-    #   Dimethyl@Any N-term: 
+    #   Dimethyl@Any N-term:
     #     - _(Dimethyl-n-0)
     #     - _(Dimethyl)
-    #   Dimethyl:2H(2)@K: 
+    #   Dimethyl:2H(2)@K:
     #     - K(Dimethyl-K-2)
     #   ...
 ```
 For DDA data, peptdeep can also extract MS2 intensities from the
 spectrum files from `model_mgr:transfer:ms_files` and
 `model_mgr:transfer:ms_file_type` for all PSMs. This will enable the
 transfer learning of the MS2 model.
@@ -941,15 +931,15 @@
   percolator_model_choices:
     pytorch_as_backend:
       - linear # not fully tested, performance may be unstable
       - mlp # not implemented yet
     sklearn_as_backend:
       - linear # logistic regression
       - random_forest
-  lr_percolator_torch_model: 0.1 # learning rate, only used when percolator_backend==pytorch 
+  lr_percolator_torch_model: 0.1 # learning rate, only used when percolator_backend==pytorch
   percolator_iter_num: 5 # percolator iteration number
   cv_fold: 1
   fdr: 0.01
   fdr_level: psm
   fdr_level_choices:
     - psm
     - precursor
@@ -968,15 +958,15 @@
       - alphapept_hdf
       - thermo_raw # if alpharaw is installed
       - mgf
       - mzml
     ms_files: []
     other_score_column_mapping:
       alphapept: {}
-      pfind: 
+      pfind:
         raw_score: Raw_Score
       msfragger:
         hyperscore: hyperscore
         nextscore: nextscore
       maxquant: {}
   output_folder: "{PEPTDEEP_HOME}/rescore"
 ```
@@ -1040,15 +1030,15 @@
 Pipeline APIs provides the same functionalities with [CLI](#cli),
 including [library prediction](#library), [transfer
 learning](#transfer), and [rescoring](#rescore).
 
 ``` python
 from peptdeep.pipeline_api import (
     generate_library,
-    transfer_learn, 
+    transfer_learn,
     rescore,
 )
 ```
 
 All these functionalities take a `settings_dict` as the inputs, the dict
 structure is the same as the settings yaml file. See the documatation of `generate_library`, `transfer_learn`, `rescore` in https://alphapeptdeep.readthedocs.io/en/latest/module_pipeline_api.html.
```

### Comparing `peptdeep-1.1.9/README.md` & `peptdeep-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -262,28 +262,14 @@
 ***By using the editable flag `-e`, all modifications to the [peptdeep
 source code folder](peptdeep) are directly reflected when running
 peptdeep. Note that the peptdeep folder cannot be moved and/or renamed
 if an editable version is installed. In case of confusion, you can
 always retrieve the location of any Python module with e.g. the command
 `import module` followed by `module.__file__`.***
 
-We used [nbdev v2](https://nbdev.fast.ai/) for developers to build
-Python source code and docs smoothly from Python notebooks, so please do
-not edit .py files directly, edit .ipynb in `nbdev_nbs` folder instead.
-After installing nbdev, cd to alphapeptdeep project folder and run:
-
-``` bash
-nbdev_install_hooks
-```
-
-to init gitconfig for nbdev. After editing the source code in .ipynb
-files, using `nbdev_export` to build python source code and `nbdev_test`
-to run all .ipynb files in `nbdev_nbs` for testing. Check [nbdev
-docs](https://nbdev.fast.ai/) for more information.
-
 ------------------------------------------------------------------------
 
 ## Usage
 
 There are three ways to use peptdeep:
 
 - [**GUI**](#gui)
@@ -360,15 +346,15 @@
 ```
 
 This command will export the default settings into the `settings.yaml`
 as a template, users can edit the yaml file to run other commands.
 
 Here is a section of the yaml file which controls global parameters for
 different tasks:
-  
+
 ```
 model_url: "https://github.com/MannLabs/alphapeptdeep/releases/download/pre-trained-models/pretrained_models.zip"
 
 task_type: library
 task_type_choices:
   - library
   - train
@@ -391,15 +377,15 @@
   - critical
 
 common:
   modloss_importance_level: 1.0
   user_defined_modifications: {}
   # For example,
   # user_defined_modifications:
-  #   "Dimethyl2@Any N-term": 
+  #   "Dimethyl2@Any N-term":
   #     composition: "H(2)2H(2)C(2)"
   #     modloss_composition: "H(0)" # can be without if no modloss
   #   "Dimethyl2@K":
   #     composition: "H(2)2H(2)C(2)"
   #   "Dimethyl6@Any N-term":
   #     composition: "2H(4)13C(2)"
   #   "Dimethyl6@K":
@@ -459,15 +445,15 @@
 ``` bash
 peptdeep cmd-flow ...
 ```
 
 Support CLI parameters to control `global_settings` for CLI users. It supports three workflows: `train`, `library` or `train library`, controlled by CLI parameter `--task_workflow`, for example, `--task_workflow train library`. All settings in [global_settings](peptdeep/constants/default_settings.yaml) are converted to CLI parameters using `--` as the dict level indicator, for example, `global_settings["library"]["var_mods"]` corresponds to `--library--var_mods`. See [test_cmd_flow.sh](tests/test_cmd_flow.sh) for example.
 
 There are three kinds of parameter types:
-  1. value type (int, float, bool, str): The CLI parameter only has a single value, for instance: `--model_mgr--default_instrument 30.0`. 
+  1. value type (int, float, bool, str): The CLI parameter only has a single value, for instance: `--model_mgr--default_instrument 30.0`.
   2. list type (list): The CLI parameter has a list of values seperated by a space, for instance `--library--var_mods "Oxidation@M" "Acetyl@Protein_N-term"`.
   3. dict type (dict): Only three parameters are `dict type`, `--library--labeling_channels`, `--model_mgr--transfer--psm_modification_mapping`, and `--common--user_defined_modifications`. Here are the examples:
     - `--library--labeling_channels`: labeling channels for the library. Example: `--library--labeling_channels "0:Dimethyl@Any_N-term;Dimethyl@K" "4:xx@Any_N-term;xx@K"`
     - `--model_mgr--transfer--psm_modification_mapping`: converting other search engines' modification names to alphabase modifications for transfer learning. Example: `--model_mgr--transfer--psm_modification_mapping "Dimethyl@Any_N-term:_(Dimethyl-n-0);_(Dimethyl)" "Dimethyl@K:K(Dimethyl-K-0);K(Dimethyl)"`. Note that `X(UniMod:id)` format can directly be recognized by alphabase.
     - `--common--user_defined_modification`: user defined modifications. Example:`--common--user_defined_modification "NewMod1@Any_N-term:H(2)2H(2)C(2)" "NewMod2@K:H(100)O(2)C(2)"`
 
 #### library
@@ -485,15 +471,15 @@
 library:
   infile_type: fasta
   infile_type_choices:
   - fasta
   - sequence_table
   - peptide_table # sequence with mods and mod_sites
   - precursor_table # peptide with charge state
-  infiles: 
+  infiles:
   - xxx.fasta
   fasta:
     protease: 'trypsin'
     protease_choices:
     - 'trypsin'
     - '([KR])'
     - 'trypsin_not_P'
@@ -503,15 +489,15 @@
     - 'lys-n'
     - '\w(?=K)'
     - 'chymotrypsin'
     - 'asp-n'
     - 'glu-c'
     max_miss_cleave: 2
     add_contaminants: False
-  fix_mods: 
+  fix_mods:
   - Carbamidomethyl@C
   var_mods:
   - Acetyl@Protein N-term
   - Oxidation@M
   special_mods: [] # normally for Phospho or GlyGly@K
   special_mods_cannot_modify_pep_n_term: False
   special_mods_cannot_modify_pep_c_term: False
@@ -614,15 +600,15 @@
 
 ``` python
 df
 ```
 
 |  | sequence | mods | mod_sites | charge |
 | --- | --- | --- | --- | --- |
-| 0 | ACDEFGHIK | Carbamidomethyl@C | 2 | 2 | 
+| 0 | ACDEFGHIK | Carbamidomethyl@C | 2 | 2 |
 | 1 | LMNPQRSTVK | Acetyl@Protein N-term;Phospho@S | 0;7 | 3 |
 | 2 | WYVSTR | | | 1 |
 
 > Columns of `proteins` and `genes` are optional for these txt/tsv/csv
 > files.
 
 peptdeep supports multiple files for library prediction, for example (in
@@ -692,22 +678,22 @@
     psm_num_to_train_ms2: 100000000
     psm_num_per_mod_to_train_ms2: 50
     psm_num_to_test_ms2: 0
     psm_num_to_train_rt_ccs: 100000000
     psm_num_per_mod_to_train_rt_ccs: 50
     psm_num_to_test_rt_ccs: 0
     top_n_mods_to_train: 10
-    psm_modification_mapping: {} 
+    psm_modification_mapping: {}
     # alphabase modification to modifications of other search engines
     # For example,
     # psm_modification_mapping:
-    #   Dimethyl@Any N-term: 
+    #   Dimethyl@Any N-term:
     #     - _(Dimethyl-n-0)
     #     - _(Dimethyl)
-    #   Dimethyl:2H(2)@K: 
+    #   Dimethyl:2H(2)@K:
     #     - K(Dimethyl-K-2)
     #   ...
 ```
 For DDA data, peptdeep can also extract MS2 intensities from the
 spectrum files from `model_mgr:transfer:ms_files` and
 `model_mgr:transfer:ms_file_type` for all PSMs. This will enable the
 transfer learning of the MS2 model.
@@ -774,15 +760,15 @@
   percolator_model_choices:
     pytorch_as_backend:
       - linear # not fully tested, performance may be unstable
       - mlp # not implemented yet
     sklearn_as_backend:
       - linear # logistic regression
       - random_forest
-  lr_percolator_torch_model: 0.1 # learning rate, only used when percolator_backend==pytorch 
+  lr_percolator_torch_model: 0.1 # learning rate, only used when percolator_backend==pytorch
   percolator_iter_num: 5 # percolator iteration number
   cv_fold: 1
   fdr: 0.01
   fdr_level: psm
   fdr_level_choices:
     - psm
     - precursor
@@ -801,15 +787,15 @@
       - alphapept_hdf
       - thermo_raw # if alpharaw is installed
       - mgf
       - mzml
     ms_files: []
     other_score_column_mapping:
       alphapept: {}
-      pfind: 
+      pfind:
         raw_score: Raw_Score
       msfragger:
         hyperscore: hyperscore
         nextscore: nextscore
       maxquant: {}
   output_folder: "{PEPTDEEP_HOME}/rescore"
 ```
@@ -873,15 +859,15 @@
 Pipeline APIs provides the same functionalities with [CLI](#cli),
 including [library prediction](#library), [transfer
 learning](#transfer), and [rescoring](#rescore).
 
 ``` python
 from peptdeep.pipeline_api import (
     generate_library,
-    transfer_learn, 
+    transfer_learn,
     rescore,
 )
 ```
 
 All these functionalities take a `settings_dict` as the inputs, the dict
 structure is the same as the settings yaml file. See the documatation of `generate_library`, `transfer_learn`, `rescore` in https://alphapeptdeep.readthedocs.io/en/latest/module_pipeline_api.html.
```

### Comparing `peptdeep-1.1.9/peptdeep/__init__.py` & `peptdeep-1.2.0/peptdeep/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 #     from . import protein # rely on spec_lib, import after
 # except (ImportError,RuntimeError, OSError):
 #     # happends when installation
 #     pass
 
 __project__ = "peptdeep"
-__version__ = "1.1.9"
+__version__ = "1.2.0"
 __license__ = "Apache 2.0"
 __description__ = "The AlphaX deep learning framework for Proteomics"
 __author__ = "Mann Labs"
 __author_email__ = "jalew.zwf@qq.com"
 __github__ = "https://github.com/MannLabs/peptdeep"
 __doc__ = "https://alphapeptdeep.readthedocs.io/en/latest/"
 __pypi__ = "https://pypi.org/project/peptdeep/"
```

### Comparing `peptdeep-1.1.9/peptdeep/__pycache__/__init__.cpython-39.pyc` & `peptdeep-1.2.0/peptdeep/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 12 07:34:59 2024 UTC, .py size: 1673 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 610d 0d0a 0000 0000 23e4 1866 8906 0000  a.......#..f....
+00000000: 610d 0d0a 0000 0000 278e 5766 8906 0000  a.......'.Wf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 5a07 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6700 6409 a201 5a09 640a 5a0a 6700  Z.g.d...Z.d.Z.g.
 00000060: 640b a201 5a0b 640c 6701 5a0c 640d 640e  d...Z.d.g.Z.d.d.
 00000070: 6506 6507 6508 640f 9c05 5a0d 6410 6411  e.e.e.d...Z.d.d.
 00000080: 6412 9c02 5a0e 6413 5300 2914 da08 7065  d...Z.d.S.)...pe
-00000090: 7074 6465 6570 7a05 312e 312e 397a 0a41  ptdeepz.1.1.9z.A
+00000090: 7074 6465 6570 7a05 312e 322e 307a 0a41  ptdeepz.1.2.0z.A
 000000a0: 7061 6368 6520 322e 307a 3154 6865 2041  pache 2.0z1The A
 000000b0: 6c70 6861 5820 6465 6570 206c 6561 726e  lphaX deep learn
 000000c0: 696e 6720 6672 616d 6577 6f72 6b20 666f  ing framework fo
 000000d0: 7220 5072 6f74 656f 6d69 6373 7a09 4d61  r Proteomicsz.Ma
 000000e0: 6e6e 204c 6162 737a 106a 616c 6577 2e7a  nn Labsz.jalew.z
 000000f0: 7766 4071 712e 636f 6d7a 2468 7474 7073  wf@qq.comz$https
 00000100: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d61  ://github.com/Ma
```

### Comparing `peptdeep-1.1.9/peptdeep/cli.py` & `peptdeep-1.2.0/peptdeep/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
     invoke_without_command=True
 )
 @click.pass_context
 @click.version_option(peptdeep.__version__, "-v", "--version")
 def run(ctx, **kwargs):
     click.echo(
 r'''
-     ____             __  ____                
-    / __ \___  ____  / /_/ __ \___  ___  ____ 
+     ____             __  ____
+    / __ \___  ____  / /_/ __ \___  ___  ____
    / /_/ / _ \/ __ \/ __/ / / / _ \/ _ \/ __ \
   / ____/  __/ /_/ / /_/ /_/ /  __/  __/ /_/ /
- /_/    \___/ .___/\__/_____/\___/\___/ .___/ 
-           /_/                       /_/      
+ /_/    \___/ .___/\__/_____/\___/\___/ .___/
+           /_/                       /_/
 ....................................................
 .{version}.
 .{url}.
 .{license}.
 ....................................................
 '''.format(
         version=peptdeep.__version__.center(50),
-        url=peptdeep.__github__.center(50), 
+        url=peptdeep.__github__.center(50),
         license=peptdeep.__license__.center(50),
     )
 )
     if ctx.invoked_subcommand is None:
         click.echo(run.get_help(ctx))
 
 @run.command("gui", help="Start graphical user interface.")
@@ -77,15 +77,15 @@
     else:
         download_models(model_file, overwrite=overwrite)
 
 _help_str = (
     "\n\nTo get the settings_yaml file,"
     " you can either export from the GUI,"
     " or use `peptdeep export-settings`."
-    " Visit https://github.com/mannlabs/alphapeptdeep/#cli" 
+    " Visit https://github.com/mannlabs/alphapeptdeep/#cli"
     " for detailed usages."
 )
 
 # @run.command("rescore", help=
 #     "Rescore PSMs using Percolator."+_help_str
 # )
 # @click.argument("settings_yaml", type=str)
@@ -118,25 +118,25 @@
     save_yaml(yaml_file, global_settings)
 
 class ParserHelper(click.Command):
     def format_help(self, ctx: Context, formatter: HelpFormatter) -> None:
         parser = get_parser()
         formatter.write(parser.format_help())
 
-@run.command("cmd-flow", 
+@run.command("cmd-flow",
     help="Using command line arguments to control the settings",
     cls=ParserHelper,
     context_settings=dict(
     ignore_unknown_options=True,
     allow_extra_args=True,
 ))
 @click.pass_context
 def _cmd_flow(ctx):
     parser = get_parser()
-    if len(ctx.args) == 0: 
+    if len(ctx.args) == 0:
         parser.print_help()
     else:
         parse_args_to_global_settings(parser, ctx.args)
         if "train" in global_settings["task_workflow"]:
             from peptdeep.pipeline_api import transfer_learn
             transfer_learn()
             if os.path.isfile(os.path.join(
@@ -156,8 +156,7 @@
             )):
                 global_settings["model_mgr"]["external_ccs_model"] = os.path.join(
                     global_settings["model_mgr"]["transfer"]["model_output_folder"], "ccs.pth"
                 )
         if "library" in global_settings["task_workflow"]:
             from peptdeep.pipeline_api import generate_library
             generate_library()
-
```

### Comparing `peptdeep-1.1.9/peptdeep/cli_argparse.py` & `peptdeep-1.2.0/peptdeep/cli_argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     global_settings, load_global_settings,
     _refine_global_settings
 )
 
 __argparse_dict_level_sep="--" # do not change
 
 def convert_dict_to_argparse(
-    settings:dict, 
+    settings:dict,
     prefix_key="",
     dict_level_sep=__argparse_dict_level_sep,
 ):
     if isinstance(settings, dict):
         if len(settings) == 0:
             return [(prefix_key, settings)]
         ret = []
@@ -30,15 +30,15 @@
             else:
                 ret += convert_dict_to_argparse(
                     val, prefix_key=(prefix_key+dict_level_sep+key) if prefix_key else key
                 )
         return ret
     else:
         return [(prefix_key, settings)]
-    
+
 def _set_dict_val(_dict, keys, val):
     if len(keys) < 1: return
     elif keys[0] == "labeling_channels":
         def _get(x:str):
             i = x.find(":")
             k,v = x[:i], x[i+1:]
             k = int(k) if k.isdigit() else k
@@ -64,15 +64,15 @@
     elif len(keys) == 1:
         _dict[keys[0]] = val
     else: _set_dict_val(_dict[keys[0]], keys[1:], val)
 
 def get_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        "--settings_yaml", type=str, default="", 
+        "--settings_yaml", type=str, default="",
         help="The yaml file for saved settings (default: %(default)s)"
     )
     arg_settings = convert_dict_to_argparse(global_settings)
     for arg, val in arg_settings:
         arg = "--"+arg
         if isinstance(val, (list,dict,set)):
             parser.add_argument(arg, nargs="*", default=val, help="(default: %(default)s)")
@@ -106,13 +106,13 @@
     args_dict.pop("settings_yaml")
     used_args = {}
     for arg in args:
         if arg.startswith("--"):
             arg = arg[2:].replace("--","__")
             if arg in args_dict:
                 used_args[arg] = args_dict[arg]
-    
+
     for key, val in used_args.items():
         keys = key.split("__")
         _set_dict_val(global_settings, keys, val)
     _refine_global_settings()
-    return global_settings
+    return global_settings
```

### Comparing `peptdeep-1.1.9/peptdeep/constants/default_settings.yaml` & `peptdeep-1.2.0/peptdeep/constants/default_settings.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   - critical
 
 common:
   modloss_importance_level: 1.0
   user_defined_modifications: {}
   # For example,
   # user_defined_modifications:
-  #   "Dimethyl2@Any_N-term": 
+  #   "Dimethyl2@Any_N-term":
   #     composition: "H(2)2H(2)C(2)"
   #     modloss_composition: "H(0)" # can be missing if no modloss
   #   "Dimethyl2@K":
   #     composition: "H(2)2H(2)C(2)"
   #   "Dimethyl6@Any_N-term":
   #     composition: "2H(4)13C(2)"
   #   "Dimethyl6@K":
@@ -147,18 +147,18 @@
     psm_num_to_train_rt_ccs: 100000000
     psm_num_per_mod_to_train_rt_ccs: 50
     psm_num_to_test_rt_ccs: 0
     top_n_mods_to_train: 10
     psm_modification_mapping: {} # alphabase modifications to modifications of other engine PSMs
     # Example (note that `X(UniMod:id)` format can directly be recognized by alphabase),
     # psm_modification_mapping:
-    #   Dimethyl@Any N-term: 
+    #   Dimethyl@Any N-term:
     #     - _(Dimethyl-n-0)
     #     - _(Dimethyl)
-    #   Dimethyl:2H(2)@K: 
+    #   Dimethyl:2H(2)@K:
     #     - K(Dimethyl-K-2)
     #   ...
 # percolator:
 #   require_model_tuning: True
 #   raw_num_to_tune: 8
 
 #   require_raw_specific_tuning: True
@@ -181,15 +181,15 @@
 #   percolator_model_choices:
 #     pytorch_as_backend:
 #       - linear # not fully tested, performance may be unstable
 #       - mlp # not implemented yet
 #     sklearn_as_backend:
 #       - linear # logistic regression
 #       - random_forest
-#   lr_percolator_torch_model: 0.1 # learning rate, only used when percolator_backend==pytorch 
+#   lr_percolator_torch_model: 0.1 # learning rate, only used when percolator_backend==pytorch
 #   percolator_iter_num: 5 # percolator iteration number
 #   cv_fold: 1
 #   fdr: 0.01
 #   fdr_level: psm
 #   fdr_level_choices:
 #     - psm
 #     - precursor
@@ -215,15 +215,15 @@
   infile_type: fasta
   infile_type_choices:
   - fasta
   - sequence_table
   - peptide_table # sequence with mods and mod_sites
   - precursor_table # peptide with charge state
   - all_other_psm_reader_types # see psm_type_choices in model_mgr section
-  infiles: 
+  infiles:
   - xxx.fasta
   fasta:
     protease: 'trypsin'
     protease_choices:
     - 'trypsin'
     - '([KR])'
     - 'trypsin_not_P'
@@ -233,15 +233,15 @@
     - 'lys-n'
     - '\w(?=K)'
     - 'chymotrypsin'
     - 'asp-n'
     - 'glu-c'
     max_miss_cleave: 2
     add_contaminants: False
-  fix_mods: 
+  fix_mods:
   - Carbamidomethyl@C
   var_mods:
   - Acetyl@Protein_N-term
   - Oxidation@M
   special_mods: [] # normally for Phospho or GlyGly@K
   special_mods_cannot_modify_pep_n_term: False
   special_mods_cannot_modify_pep_c_term: False
@@ -279,8 +279,8 @@
   output_tsv:
     enabled: False
     min_fragment_mz: 200.0
     max_fragment_mz: 2000.0
     min_relative_intensity: 0.001
     keep_higest_k_peaks: 12
     translate_batch_size: 100000
-    translate_mod_to_unimod_id: False
+    translate_mod_to_unimod_id: False
```

### Comparing `peptdeep-1.1.9/peptdeep/constants/model_const.yaml` & `peptdeep-1.2.0/peptdeep/constants/model_const.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,8 +117,8 @@
 - QE
 - Lumos
 - timsTOF
 - SciexTOF
 - ThermoTOF
 # DO NOT change values below, unless you know how to deal with them
 max_instrument_num: 8
-aa_embedding_size: 27
+aa_embedding_size: 27
```

### Comparing `peptdeep-1.1.9/peptdeep/gui.py` & `peptdeep-1.2.0/peptdeep/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     theme.append("--theme.backgroundColor=#FFFFFF")
     theme.append("--theme.secondaryBackgroundColor=#f0f2f6")
     theme.append("--theme.textColor=#262730")
     theme.append("--theme.font=sans serif")
     theme.append("--theme.primaryColor=#18212b")
 
     args = [
-        "streamlit", "run", 
-        file_path, "--global.developmentMode=false", 
-        f"--server.port={port}", 
+        "streamlit", "run",
+        file_path, "--global.developmentMode=false",
+        f"--server.port={port}",
         "--browser.gatherUsageStats=False",
         "--logger.level=error"
     ]
 
     args.extend(theme)
 
     sys.argv = args
 
-    sys.exit(stcli.main())
+    sys.exit(stcli.main())
```

### Comparing `peptdeep-1.1.9/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt` & `peptdeep-1.2.0/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 These License terms are an agreement between you and Thermo Finnigan LLC ("Licensor"). They apply to Licensor’s MSFileReader software program (“Software”), which includes documentation and any media on which you received it. These terms also apply to any updates or supplements for this Software, unless other terms accompany those items, in which case those terms apply. If you use this Software, you accept this License. If you do not accept this License, you are prohibited from using this software.  If you comply with these License terms, you have the rights set forth below.
 
 1. Rights Granted:
 
 1.1. You may install and use this Software on any of your computing devices.
 
-1.2. You may distribute this Software to others, but only in combination with other software components and/or programs that you provide and subject to the distribution requirements and restrictions below. 
+1.2. You may distribute this Software to others, but only in combination with other software components and/or programs that you provide and subject to the distribution requirements and restrictions below.
 
 2.  Use Restrictions:
 
 2.1. You may not decompile, disassemble, reverse engineer, use reflection or modify this Software.
 
 3. Distribution Requirements:
 
@@ -44,8 +44,8 @@
 
 5.6. This License shall be construed and controlled by the laws of the State of California, U.S.A., without regard to conflicts of law. You consent to the jurisdiction of the state and federal courts situated in the State of California in any action arising under this License. The application of the U.N. Convention on Contracts for the International Sale of Goods to this License is hereby expressly excluded. If any provision of this License shall be deemed unenforceable or contrary to law, the rest of this License shall remain in full effect and interpreted in an enforceable manner that most nearly captures the intent of the original language.
 
 5.7. THIS SOFTWARE IS LICENSED "AS IS". YOU BEAR ALL RISKS OF USING IT. LICENSOR GIVES NO AND DISCLAIMS ALL EXPRESS AND IMPLIED WARRANTIES, REPRESENTATIONS OR GUARANTEES.  YOU MAY HAVE ADDITIONAL CONSUMER RIGHTS UNDER YOUR LOCAL LAWS WHICH THIS LICENSE CANNOT CHANGE. TO THE EXTENT PERMITTED UNDER YOUR LOCAL LAWS, LICENSOR EXCLUDES THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT.
 
 5.8. LICENSOR’S TOTAL LIABILITY TO YOU FOR DIRECT DAMAGES ARISING UNDER THIS LICENSE IS LIMITED TO U.S. $1.00. YOU CANNOT RECOVER ANY OTHER DAMAGES, INCLUDING CONSEQUENTIAL, LOST PROFITS, SPECIAL, INDIRECT OR INCIDENTAL DAMAGES, EVEN IF LICENSOR IS EXPRESSLY MADE AWARE OF THE POSSIBILITY THEREOF OR IS NEGLIGENT. THIS LIMITATION APPLIES TO ANYTHING RELATED TO THIS SOFTWARE, SERVICES, CONTENT (INCLUDING CODE) ON THIRD PARTY INTERNET SITES, OR THIRD PARTY PROGRAMS, AND CLAIMS FOR BREACH OF CONTRACT, BREACH OF WARRANTY, GUARANTEE  OR CONDITION, STRICT LIABILITY, NEGLIGENCE, OR OTHER TORT TO THE EXTENT PERMITTED BY APPLICABLE LAW.
 
-5.9. Use, duplication or disclosure of this Software by the U.S. Government is subject to the restricted rights applicable to commercial computer software (under FAR 52.227019 and DFARS 252.227-7013 or parallel regulations). The manufacturer for this purpose is Thermo Finnigan LLC, 355 River Oaks Parkway, San Jose, California 95134, U.S.A.
+5.9. Use, duplication or disclosure of this Software by the U.S. Government is subject to the restricted rights applicable to commercial computer software (under FAR 52.227019 and DFARS 252.227-7013 or parallel regulations). The manufacturer for this purpose is Thermo Finnigan LLC, 355 River Oaks Parkway, San Jose, California 95134, U.S.A.
```

### Comparing `peptdeep-1.1.9/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll` & `peptdeep-1.2.0/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.9/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll` & `peptdeep-1.2.0/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.9/peptdeep/legacy/thermo_raw/pyrawfilereader.py` & `peptdeep-1.2.0/peptdeep/legacy/thermo_raw/pyrawfilereader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.9/peptdeep/mass_spec/mass_calibration.py` & `peptdeep-1.2.0/peptdeep/mass_spec/mass_calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 class MassCalibratorForRT_KNN:
     """Using KNN to calibrate measured m/z across RT.
     """
     def __init__(self, n_neighbors=5):
         self._n_neighbors = n_neighbors
         self.model = KNeighborsRegressor(n_neighbors)
-    
+
     def fit(self, psm_df:pd.DataFrame, mass_error_df:pd.DataFrame):
         mass_error_df = mass_error_df.replace(np.inf, np.nan)
         mean_merrs = psm_df[['frag_start_idx','frag_stop_idx']].apply(
             get_fragment_median, axis=1, frag_df=mass_error_df
         ).values
         self.model.fit(psm_df.rt.values.reshape((-1,1)), mean_merrs.reshape(-1,1))
 
-    def calibrate(self, 
+    def calibrate(self,
         psm_df:pd.DataFrame, mass_error_df:pd.DataFrame
     )->pd.DataFrame:
         psm_df['frag_mass_shift'] = self.model.predict(
             psm_df.rt.values.reshape((-1,1))
         ).reshape(-1)
         psm_df[['frag_start_idx','frag_stop_idx','frag_mass_shift']].apply(
             calibrate_one, axis=1, frag_df=mass_error_df
```

### Comparing `peptdeep-1.1.9/peptdeep/mass_spec/match.py` & `peptdeep-1.2.0/peptdeep/mass_spec/match.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import numpy as np
 import numba
 import pandas as pd
 import tqdm
 
 from alphabase.peptide.fragment import (
-    create_fragment_mz_dataframe, 
+    create_fragment_mz_dataframe,
     get_charged_frag_types
 )
 from peptdeep.mass_spec.ms_reader import (
     ms2_reader_provider, MSReaderBase
 )
 
 @numba.njit
 def match_centroid_mz(
-    spec_mzs:np.ndarray, 
-    query_mzs:np.ndarray, 
+    spec_mzs:np.ndarray,
+    query_mzs:np.ndarray,
     spec_mz_tols:np.ndarray,
 )->np.ndarray:
     """
-    Matching query masses against sorted MS2/spec centroid masses, 
+    Matching query masses against sorted MS2/spec centroid masses,
     only closest (minimal abs mass error) peaks are returned.
-    
+
     Parameters
     ----------
     spec_mzs : np.ndarray
         MS2 or spec mz values, 1-D float array
 
     query_mzs : np.ndarray
         query mz values, n-D float array
@@ -45,15 +45,15 @@
     for i,idx in np.ndenumerate(idxes):
         min_merr = abs(spec_mzs[idx-1]-query_mzs[i])
         min_idx = -1
         if min_merr <= spec_mz_tols[idx-1]:
             min_idx = idx-1
         if idx < len(spec_mzs):
             merr = abs(spec_mzs[idx]-query_mzs[i])
-            if merr <= spec_mz_tols[idx] and merr < min_merr: 
+            if merr <= spec_mz_tols[idx] and merr < min_merr:
                 min_idx = idx
         ret_indices[i] = min_idx
     return ret_indices
 
 
 @numba.njit
 def match_profile_mz(
@@ -88,15 +88,15 @@
     ret_indices = np.empty_like(query_mzs, dtype=np.int32)
     for i,idx in np.ndenumerate(idxes):
         if idx == len(spec_mzs):
             idx = idx-1
 
         highest = 0
         highest_idx = -1
-            
+
         for _idx in range(idx, -1, -1):
             if abs(spec_mzs[_idx]-query_mzs[i])>spec_mz_tols[_idx]:
                 break
             if highest < spec_intens[_idx]:
                 highest = spec_intens[_idx]
                 highest_idx = _idx
         for _idx in range(idx+1, len(spec_mzs)):
@@ -128,15 +128,15 @@
 
     spec_mz_tols : np.ndarray
         Da tolerance array, same shape as spec_mzs
 
     Returns
     -------
     np.ndarray
-        2D np.ndarray of int32 with first and last matched index 
+        2D np.ndarray of int32 with first and last matched index
         for the query mz. The shape is the same as (len(query_mzs),2).
         -1 means no peaks are matched for the query mz
     """
     idxes = np.searchsorted(spec_mzs, query_mzs)
     first_indices = np.empty_like(
         query_mzs, dtype=np.int32
     )
@@ -161,39 +161,39 @@
     return first_indices, last_indices
 
 
 @numba.njit
 def match_one_raw_with_numba(
     spec_idxes, frag_start_idxes, frag_stop_idxes,
     all_frag_mzs,
-    all_spec_mzs, all_spec_intensities, 
+    all_spec_mzs, all_spec_intensities,
     peak_start_idxes, peak_end_idxes,
     matched_intensities, matched_mz_errs,
     ppm, tol,
 ):
-    """ 
+    """
     Internel function to match fragment mz values to spectrum mz values.
     Matched_mz_errs[i] = np.inf if no peaks are matched.
     """
     for spec_idx, frag_start, frag_end in zip(
         spec_idxes, frag_start_idxes, frag_stop_idxes
     ):
         peak_start = peak_start_idxes[spec_idx]
         peak_end = peak_end_idxes[spec_idx]
         if peak_end == peak_start: continue
         spec_mzs = all_spec_mzs[peak_start:peak_end]
         spec_intens = all_spec_intensities[peak_start:peak_end]
-        
+
         if ppm:
             spec_mz_tols = spec_mzs*tol*1e-6
         else:
             spec_mz_tols = np.full_like(spec_mzs, tol)
 
         frag_mzs = all_frag_mzs[frag_start:frag_end,:].copy()
-        
+
         matched_idxes = match_centroid_mz(
             spec_mzs, frag_mzs, spec_mz_tols
         ).reshape(-1)
 
         matched_intens = spec_intens[matched_idxes]
         matched_intens[matched_idxes==-1] = 0
 
@@ -227,26 +227,26 @@
         pass
 
     def get_fragment_mz_df(self, psm_df):
         return create_fragment_mz_dataframe(
             psm_df, self.charged_frag_types
         )
 
-    def match_ms2_one_raw(self, 
+    def match_ms2_one_raw(self,
         psm_df_one_raw: pd.DataFrame,
         ms2_file:str,
         ms2_file_type:str='alphapept',
         ppm:bool=True, tol:float=20.0,
     )->tuple:
         """Matching psm_df_one_raw against ms2_file
 
         Parameters
         ----------
         psm_df_one_raw : pd.DataFrame
-            psm dataframe 
+            psm dataframe
             that contains only one raw file
 
         ms2_file : str
             ms2 file path
 
         ms2_file_type : str, optional
             ms2 file type, could be ["thermo","alphapept","mgf"].
@@ -258,22 +258,22 @@
         tol : float, optional
             tolerance value. Defaults to 20.0.
 
         Returns
         -------
         tuple:
             pd.DataFrame: psm dataframe with fragment index information.
-            
+
             pd.DataFrame: fragment mz dataframe.
-            
+
             pd.DataFrame: matched intensity dataframe.
-            
-            pd.DataFrame: matched mass error dataframe. 
+
+            pd.DataFrame: matched mass error dataframe.
             np.inf if a fragment is not matched.
-            
+
         """
         self._preprocess_psms(psm_df_one_raw)
         psm_df = psm_df_one_raw
         if isinstance(ms2_file, MSReaderBase):
             ms2_reader = ms2_file
         else:
             ms2_reader = ms2_reader_provider.get_reader(
@@ -282,15 +282,15 @@
             ms2_reader.load(ms2_file)
 
         add_spec_info_list = []
         if 'rt_norm' not in psm_df.columns:
             add_spec_info_list.append('rt')
 
         if (
-            'mobility' not in psm_df.columns and 
+            'mobility' not in psm_df.columns and
             'mobility' in ms2_reader.spectrum_df.columns
         ):
             add_spec_info_list.append('mobility')
 
         if (
             'nce' not in psm_df.columns and
             'nce' in ms2_reader.spectrum_df.columns
@@ -305,33 +305,33 @@
                 on='spec_idx',
             ).set_index('index')
 
             if 'rt' in add_spec_info_list:
                 psm_df['rt_norm'] = psm_df.rt/ms2_reader.spectrum_df.rt.max()
 
         fragment_mz_df = self.get_fragment_mz_df(psm_df)
-        
+
         matched_intensity_df = pd.DataFrame(
             np.zeros_like(
                 fragment_mz_df.values, dtype=np.float64
-            ), 
+            ),
             columns=fragment_mz_df.columns
         )
 
         matched_mz_err_df = pd.DataFrame(
             np.full_like(
                 fragment_mz_df.values, np.inf, dtype=np.float64
-            ), 
+            ),
             columns=fragment_mz_df.columns
         )
-        
+
         for (
             spec_idx, frag_start_idx, frag_stop_idx
         ) in psm_df[[
-            'spec_idx', 'frag_start_idx', 
+            'spec_idx', 'frag_start_idx',
             'frag_stop_idx'
         ]].values:
             (
                 spec_mzs, spec_intens
             ) = ms2_reader.get_peaks(spec_idx)
             if len(spec_mzs)==0: continue
 
@@ -339,15 +339,15 @@
                 mz_tols = spec_mzs*tol*1e-6
             else:
                 mz_tols = np.full_like(spec_mzs, tol)
 
             frag_mzs = fragment_mz_df.values[
                 frag_start_idx:frag_stop_idx,:
             ]
-            
+
             matched_idxes = match_centroid_mz(
                 spec_mzs, frag_mzs, mz_tols
             )
             matched_intens = spec_intens[matched_idxes]
             matched_intens[matched_idxes==-1] = 0
 
             matched_mz_errs = np.abs(
@@ -360,15 +360,15 @@
             ] = matched_intens
 
             matched_mz_err_df.values[
                 frag_start_idx:frag_stop_idx,:
             ] = matched_mz_errs
 
         return (
-            psm_df, fragment_mz_df, 
+            psm_df, fragment_mz_df,
             matched_intensity_df, matched_mz_err_df
         )
 
     def _match_ms2_centroid_one_raw(self, raw_name, df_group):
         if raw_name in self._ms2_file_dict:
             if isinstance(self._ms2_file_dict[raw_name], MSReaderBase):
                 ms2_reader = self._ms2_file_dict[raw_name]
@@ -391,23 +391,23 @@
                 ] = _df[['rt','rt_norm']]
 
             match_one_raw_with_numba(
                 df_group.spec_idx.values,
                 df_group.frag_start_idx.values,
                 df_group.frag_stop_idx.values,
                 self.fragment_mz_df.values,
-                ms2_reader.peak_df.mz.values, 
+                ms2_reader.peak_df.mz.values,
                 ms2_reader.peak_df.intensity.values,
                 ms2_reader.spectrum_df.peak_start_idx.values,
                 ms2_reader.spectrum_df.peak_end_idx.values,
                 self.matched_intensity_df.values,
                 self.matched_mz_err_df.values,
                 self.ppm, self.tol
             )
-    
+
     def match_ms2_centroid(self,
         psm_df: pd.DataFrame,
         ms2_file_dict: dict, #raw_name: ms2_file_path or ms_reader object
         ms2_file_type:str = 'alphapept', # or 'mgf', or 'thermo'
         ppm=True, tol=20.0,
     ):
         """Matching PSM dataframe against the ms2 files in ms2_file_dict
@@ -422,47 +422,47 @@
         psm_df : pd.DataFrame
             PSM dataframe
 
         ms2_file_dict : dict
             {raw_name: ms2 path}
 
         ms2_file_type : str, optional
-            Could be 'alphapept', 'mgf' or 'thermo'. 
+            Could be 'alphapept', 'mgf' or 'thermo'.
             Defaults to 'alphapept'.
 
         ppm : bool, optional
             Defaults to True.
 
         tol : float, optional
             PPM units, defaults to 20.0.
-            
+
         """
         self._preprocess_psms(psm_df)
         self.psm_df = psm_df
 
         if 'frag_start_idx' in self.psm_df.columns:
             del self.psm_df['frag_start_idx']
             del self.psm_df['frag_stop_idx']
-            
+
         self.fragment_mz_df = self.get_fragment_mz_df(self.psm_df)
-        
+
         self.matched_intensity_df = pd.DataFrame(
             np.zeros_like(
                 self.fragment_mz_df.values, dtype=np.float64
-            ), 
+            ),
             columns=self.fragment_mz_df.columns
         )
 
         self.matched_mz_err_df = pd.DataFrame(
             np.full_like(
                 self.fragment_mz_df.values, np.inf, dtype=np.float64
-            ), 
+            ),
             columns=self.fragment_mz_df.columns
         )
-        
+
         self._ms2_file_dict = ms2_file_dict
         self._ms2_file_type = ms2_file_type
         self.ppm = ppm
         self.tol = tol
 
         if 'rt_norm' not in self.psm_df.columns:
             self.rt_not_in_df = True
```

### Comparing `peptdeep-1.1.9/peptdeep/mass_spec/ms_reader.py` & `peptdeep-1.2.0/peptdeep/mass_spec/ms_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
             scan number list
 
         scan_indices : np.array
             starts and end positions of ms2
             peaks for each scan
 
         rt_list : list
-            retention time (minutes) for each scan 
+            retention time (minutes) for each scan
 
         mobility_list : list, optional
             mobility for each scan. Defaults to None.
-            
+
         """
         def set_col(col, indexes, values, dtype, na_value):
             self.spectrum_df.loc[indexes, col] = values
             self.spectrum_df[col].fillna(na_value, inplace=True)
             self.spectrum_df[col] = self.spectrum_df[col].astype(dtype)
 
         scan_list = np.array(scan_list, dtype=np.int32)
@@ -71,15 +71,15 @@
 
     def get_peaks(self, spec_idx:int):
         """Get peak (mz and intensity) values by `spec_idx`
 
         Parameters
         ----------
         spec_idx : int
-            indicator for a spectrum, 
+            indicator for a spectrum,
             could be scan_num-1 for thermo data.
 
         Returns
         -------
         np.array
             mz values for the given spec_idx
 
@@ -108,47 +108,47 @@
         Returns
         -------
         np.array
             mz values for the given spec_idx (scan)
 
         np.array
             intensity values for the given spec_idx
-            
+
         """
         return self.get_peaks(scan_num-1)
 
 class AlphaPept_HDF_MS1_Reader(MSReaderBase):
     """MS1 from AlphaPept HDF"""
     def load(self, file_path):
         hdf = HDF_File(file_path)
         self.peak_df['mz'] = hdf.Raw.MS1_scans.mass_list_ms1.values
         self.peak_df['intensity'] = hdf.Raw.MS1_scans.int_list_ms1.values
         self.build_spectrum_df(
-            scan_list=hdf.Raw.MS1_scans.scan_list_ms1.values, 
+            scan_list=hdf.Raw.MS1_scans.scan_list_ms1.values,
             scan_indices=hdf.Raw.MS1_scans.indices_ms1.values,
             rt_list=hdf.Raw.MS1_scans.rt_list_ms1.values,
-            mobility_list=hdf.Raw.MS1_scans.mobility.values 
+            mobility_list=hdf.Raw.MS1_scans.mobility.values
             if hasattr(hdf.Raw.MS1_scans, 'mobility') else None,
         )
 
 class AlphaPept_HDF_MS2_Reader(MSReaderBase):
     """MS2 from AlphaPept HDF"""
     def load(self, file_path):
         hdf = HDF_File(file_path)
         self.peak_df['mz'] = hdf.Raw.MS2_scans.mass_list_ms2.values
         self.peak_df['intensity'] = hdf.Raw.MS2_scans.int_list_ms2.values
         if hasattr(hdf.Raw.MS2_scans, 'mobility2'):
             scan_list = np.arange(len(hdf.Raw.MS2_scans.rt_list_ms2))
         else:
             scan_list = hdf.Raw.MS2_scans.scan_list_ms2.values
         self.build_spectrum_df(
-            scan_list=scan_list, 
+            scan_list=scan_list,
             scan_indices=hdf.Raw.MS2_scans.indices_ms2.values,
             rt_list=hdf.Raw.MS2_scans.rt_list_ms2.values,
-            mobility_list=hdf.Raw.MS2_scans.mobility2.values 
+            mobility_list=hdf.Raw.MS2_scans.mobility2.values
             if hasattr(hdf.Raw.MS2_scans, 'mobility2') else None,
         )
 
 class MZMLReader(MSReaderBase):
     def load(self, mzmlF):
         if isinstance(mzmlF, str):
             f = mzml.read(mzmlF)
@@ -224,15 +224,15 @@
     value : list
         Input list of arrays.
 
     Returns
     -------
     indices
         A numpy array with indices.
-        
+
     """
     indices = np.zeros(len(ragged_list) + 1, np.int64)
     indices[1:] = [len(i) for i in ragged_list]
     indices = np.cumsum(indices)
 
     return indices
 
@@ -271,33 +271,33 @@
                     scan = parse_pfind_scan_from_TITLE(title)
                 if scan in scanset: continue
                 scanset.add(scan)
                 scan_list.append(scan)
                 rt_list.append(RT)
                 masses_list.append(np.array(masses))
                 intens_list.append(np.array(intens))
-        if isinstance(mgf, str): 
+        if isinstance(mgf, str):
             f.close()
         self.build_spectrum_df(
-            scan_list, 
-            index_ragged_list(masses_list), 
+            scan_list,
+            index_ragged_list(masses_list),
             rt_list
         )
         self.peak_df['mz'] = np.concatenate(masses_list)
         self.peak_df['intensity'] = np.concatenate(intens_list)
 
 class MSReaderProvider:
     """Factory class to register and get MS Readers"""
     def __init__(self):
         self.reader_dict = {}
     def register_reader(self, ms2_type, reader_class):
         self.reader_dict[ms2_type.lower()] = reader_class
 
     def get_reader(self, file_type)->MSReaderBase:
-        if file_type not in self.reader_dict: 
+        if file_type not in self.reader_dict:
             frameinfo = getframeinfo(currentframe())
             logging.warn(f'{frameinfo.filename}#L{frameinfo.lineno}: "{file_type}" is not registered in `MSReaderProvider` yet.')
             return None
         else: return self.reader_dict[file_type.lower()]()
 
 ms2_reader_provider = MSReaderProvider()
 ms2_reader_provider.register_reader('mgf', MGFReader)
@@ -309,28 +309,28 @@
 ms1_reader_provider.register_reader('alphapept', AlphaPept_HDF_MS1_Reader)
 ms1_reader_provider.register_reader('alphapept_hdf', AlphaPept_HDF_MS1_Reader)
 
 if RawFileReader is None:
     class ThermoRawMS1Reader:
         def __init__(self):
             raise NotImplementedError("RawFileReader is not available")
-    
+
     class ThermoRawMS2Reader:
         def __init__(self):
             raise NotImplementedError("RawFileReader is not available")
 else:
     class ThermoRawMS1Reader(MSReaderBase):
         """Thermo Raw MS1 Reader"""
         def __init__(self):
             super().__init__()
             self.profile_mode = False
 
         def load(self, raw_path):
             rawfile = RawFileReader(raw_path)
- 
+
             spec_indices = np.array(
                 range(rawfile.FirstSpectrumNumber, rawfile.LastSpectrumNumber + 1)
             )
             scan_list = []
             rt_list = []
             masses_list = []
             intens_list = []
@@ -350,15 +350,15 @@
 
                 except KeyboardInterrupt as e:
                     raise e
                 except SystemExit as e:
                     raise e
                 except Exception as e:
                     print(f"Bad scan={i} in raw file '{raw_path}'")
-            
+
             self.build_spectrum_df(
                 scan_list,
                 index_ragged_list(masses_list),
                 rt_list,
             )
             self.peak_df['mz'] = np.concatenate(masses_list)
             self.peak_df['intensity'] = np.concatenate(intens_list)
@@ -368,15 +368,15 @@
         """Thermo RAW MS2 Reader"""
         def __init__(self):
             super().__init__()
             self.profile_mode = False
 
         def load(self, raw_path):
             rawfile = RawFileReader(raw_path)
- 
+
             spec_indices = np.array(
                 range(rawfile.FirstSpectrumNumber, rawfile.LastSpectrumNumber + 1)
             )
             scan_list = []
             rt_list = []
             masses_list = []
             intens_list = []
@@ -396,21 +396,21 @@
 
                 except KeyboardInterrupt as e:
                     raise e
                 except SystemExit as e:
                     raise e
                 # except Exception as e:
                 #     print(f"Bad scan={i} in raw file '{raw_path}'")
-            
+
             self.build_spectrum_df(
                 scan_list,
                 index_ragged_list(masses_list),
                 rt_list,
             )
             self.peak_df['mz'] = np.concatenate(masses_list)
             self.peak_df['intensity'] = np.concatenate(intens_list)
             rawfile.Close()
-    
+
     ms2_reader_provider.register_reader('thermo', ThermoRawMS2Reader)
     ms2_reader_provider.register_reader('thermo_raw', ThermoRawMS2Reader)
     ms1_reader_provider.register_reader('thermo', ThermoRawMS1Reader)
     ms1_reader_provider.register_reader('thermo_raw', ThermoRawMS1Reader)
```

### Comparing `peptdeep-1.1.9/peptdeep/model/building_block.py` & `peptdeep-1.2.0/peptdeep/model/building_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,30 +60,30 @@
     return encoder_extended_attention_mask
 
 
 init_state = xavier_param
 
 class SeqCNN_MultiKernel(torch.nn.Module):
     """
-    Extract sequence features using `torch.nn.Conv1D` with 
-    different kernel sizes (1(residue connection),3,5,7), 
+    Extract sequence features using `torch.nn.Conv1D` with
+    different kernel sizes (1(residue connection),3,5,7),
     and then concatenate the outputs of these Conv1Ds.
     """
     def __init__(self, out_features:int):
         """
         Parameters
         ----------
         out_features : int
             Must be divided by 4.
 
         Raises
         ------
         ValueError
             "out_features must be divided by 4"
-            
+
         """
         super().__init__()
 
         hidden = out_features//4
         if hidden*4 != out_features:
             raise ValueError('out_features must be divided by 4')
 
@@ -106,16 +106,16 @@
         x2 = self.cnn_medium(x)
         x3 = self.cnn_long(x)
         return torch.cat((x, x1, x2, x3), dim=1).transpose(1,2)
 
 #legacy
 class SeqCNN(torch.nn.Module):
     """
-    Extract sequence features using `torch.nn.Conv1D` with 
-    different kernel sizes (1(residue connection),3,5,7), and then concatenate 
+    Extract sequence features using `torch.nn.Conv1D` with
+    different kernel sizes (1(residue connection),3,5,7), and then concatenate
     the outputs of these Conv1Ds. The Output dim is 4*embedding_hidden.
     """
     def __init__(self, embedding_hidden):
         super().__init__()
 
         self.cnn_short = torch.nn.Conv1d(
             embedding_hidden, embedding_hidden,
@@ -152,38 +152,38 @@
         super().__init__()
         encoder_layers = torch.nn.TransformerEncoderLayer(
             in_features, nheads, hidden_features, dropout
         )
         self.transformer_encoder = torch.nn.TransformerEncoder(
             encoder_layers, nlayers
         )
-        
+
     def forward(self, x):
         return self.transformer_encoder(x.permute(1,0,2)).permute(1,0,2)
 
 
 class Hidden_Transformer(torch.nn.Module):
     """
     Transformer NN based on pytorch's built-in TransformerLayer class
     """
-    def __init__(self, 
+    def __init__(self,
         hidden, hidden_expand=4,
         nheads=8, nlayers=4, dropout=0.1
     ):
         super().__init__()
         self.transormer = Seq_Transformer(
-            hidden, hidden*hidden_expand, nheads=nheads, 
+            hidden, hidden*hidden_expand, nheads=nheads,
             nlayers=nlayers, dropout=dropout
         )
     def forward(self, x):
         return self.transormer(x)
 
 class _Pseudo_Bert_Config:
-    def __init__(self, 
-        hidden_dim=256, 
+    def __init__(self,
+        hidden_dim=256,
         intermediate_size=1024,
         num_attention_heads=8,
         num_bert_layers=4,
         dropout=0.1,
         output_attentions=False,
     ):
         self.add_cross_attention = False
@@ -197,20 +197,21 @@
         self.hidden_size = hidden_dim
         self.initializer_range = 0.02
         self.intermediate_size = intermediate_size
         self.layer_norm_eps = 1e-8
         self.num_attention_heads = num_attention_heads
         self.num_hidden_layers = num_bert_layers
         self.output_attentions = output_attentions
+        self._attn_implementation = "eager" # Add this for transformers-4.41.0
 
 class Hidden_HFace_Transformer(torch.nn.Module):
     """
     Transformer NN based on HuggingFace's BertEncoder class
     """
-    def __init__(self, 
+    def __init__(self,
         hidden_dim, hidden_expand=4,
         nheads=8, nlayers=4, dropout=0.1,
         output_attentions=False,
     ):
         super().__init__()
         self.config = _Pseudo_Bert_Config(
             hidden_dim=hidden_dim,
@@ -218,30 +219,30 @@
             num_attention_heads=nheads,
             num_bert_layers=nlayers,
             dropout=dropout,
             output_attentions=False
         )
         self.output_attentions = output_attentions
         self.bert = BertEncoder(self.config)
-    def forward(self, x:torch.Tensor, 
+    def forward(self, x:torch.Tensor,
         attention_mask:torch.Tensor=None,
     )->tuple:
         """
         Parameters
         ----------
         x : torch.Tensor
             shape = (batch, seq_len, dim)
         attention_mask : torch.Tensor
             shape = (batch, seq_len), [0,1] tensor , 1=enable
 
         Returns
         -------
         (Tensor, [Tensor])
-            out[0] is the hidden layer output, 
-            and out[1] is the output attention 
+            out[0] is the hidden layer output,
+            and out[1] is the output attention
             if self.output_attentions==True
         """
         if attention_mask is not None:
             attention_mask = invert_attention_mask(
                 attention_mask, dtype=x.dtype
             )
         return self.bert(
@@ -289,15 +290,15 @@
         super().__init__()
         self.pos_encoder = PositionalEncoding(hidden_dim, max_len=max_len)
         self.bert = Hidden_HFace_Transformer(
             hidden_dim=hidden_dim, hidden_expand=hidden_expand,
             nheads=nheads, nlayers=nlayers, dropout=dropout,
             output_attentions=output_attentions
         )
-    def forward(self, 
+    def forward(self,
         x:torch.Tensor,
         attention_mask:torch.Tensor=None,
     )->tuple:
         """
         Parameters
         ----------
         x : torch.Tensor
@@ -312,15 +313,15 @@
         x = self.pos_encoder(x)
         return self.bert(x, attention_mask)
 
 class SeqLSTM(torch.nn.Module):
     """
     returns LSTM applied on sequence input
     """
-    def __init__(self, in_features, out_features, 
+    def __init__(self, in_features, out_features,
                  rnn_layer=2, bidirectional=True
         ):
         super().__init__()
 
         if bidirectional:
             if out_features%2 != 0:
                 raise ValueError("'out_features' must be able to be divided by 2")
@@ -331,15 +332,15 @@
         self.rnn_h0 = init_state(
             rnn_layer+rnn_layer*bidirectional,
             1, hidden
         )
         self.rnn_c0 = init_state(
             rnn_layer+rnn_layer*bidirectional,
             1, hidden
-        ) 
+        )
         self.rnn = torch.nn.LSTM(
             input_size = in_features,
             hidden_size = hidden,
             num_layers = rnn_layer,
             batch_first = True,
             bidirectional = bidirectional,
         )
@@ -350,30 +351,30 @@
         x, _ = self.rnn(x, (h0,c0))
         return x
 
 class SeqGRU(torch.nn.Module):
     """
     returns GRU applied on sequence input
     """
-    def __init__(self, in_features, out_features, 
+    def __init__(self, in_features, out_features,
                  rnn_layer=2, bidirectional=True
         ):
         super().__init__()
 
         if bidirectional:
             if out_features%2 != 0:
                 raise ValueError("'out_features' must be able to be divided by 2")
             # to make sure that output dim is out_features
             # as `bidirectional` will cat forward and reverse RNNs
             hidden = out_features//2
         else:
             hidden = out_features
-        
+
         self.rnn_h0 = init_state(
-            rnn_layer+rnn_layer*bidirectional, 
+            rnn_layer+rnn_layer*bidirectional,
             1, hidden
         )
         self.rnn = torch.nn.GRU(
             input_size = in_features,
             hidden_size = hidden,
             num_layers = rnn_layer,
             batch_first = True,
@@ -391,15 +392,15 @@
     """
     def __init__(self, in_features):
         super().__init__()
         self.attn = torch.nn.Sequential(
             torch.nn.Linear(in_features, 1, bias=False),
             torch.nn.Softmax(dim=1),
         )
-    
+
     def forward(self, x):
         attn = self.attn(x)
         return torch.sum(torch.mul(x, attn), dim=1)
 
 class PositionalEncoding(torch.nn.Module):
     """
     transform sequence input into a positional representation
@@ -434,15 +435,15 @@
 
     def forward(self, x:torch.Tensor):
         return x + self.pos_emb(torch.arange(
             x.size(1), dtype=torch.long, device=x.device
         ).unsqueeze(0))
 
 class Meta_Embedding(torch.nn.Module):
-    """Encodes Charge state, Normalized Collision Energy (NCE) and Instrument for a given spectrum 
+    """Encodes Charge state, Normalized Collision Energy (NCE) and Instrument for a given spectrum
     into a 'meta' single layer network
     """
     def __init__(self,
         out_features,
     ):
         super().__init__()
         self.nn = torch.nn.Linear(
@@ -475,15 +476,15 @@
             bias=False
         )
 
     def forward(self,
         mod_x,
     ):
         return torch.cat((
-            mod_x[:,:,:self.k], 
+            mod_x[:,:,:self.k],
             self.nn(mod_x[:,:,self.k:])
         ), 2)
 #legacy
 InputModNetFixFirstK = Mod_Embedding_FixFirstK
 
 class AA_Mod_Embedding(torch.nn.Module):
     """
@@ -537,16 +538,16 @@
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
         self.aa_emb = aa_embedding(
             out_features-mod_hidden
         )
         self.pos_encoder = PositionalEncoding(
             out_features, max_len
         )
-        
-    def forward(self, 
+
+    def forward(self,
         aa_indices, mod_x
     ):
         mod_x = self.mod_nn(mod_x)
         x = self.aa_emb(aa_indices)
         return self.pos_encoder(torch.cat((x, mod_x), 2))
 #legacy
 AATransformerEncoding = Input_26AA_Mod_PositionalEncoding
@@ -561,16 +562,16 @@
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
         self.aa_emb = ascii_embedding(
             out_features-mod_hidden
         )
         self.pos_encoder = PositionalEncoding(
             out_features, max_len
         )
-        
-    def forward(self, 
+
+    def forward(self,
         aa_indices, mod_x
     ):
         mod_x = self.mod_nn(mod_x)
         x = self.aa_emb(aa_indices)
         return self.pos_encoder(torch.cat((x, mod_x), 2))
 
 class Input_AA_Mod_Charge_PositionalEncoding(torch.nn.Module):
@@ -584,16 +585,16 @@
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
         self.aa_emb = ascii_embedding(
             out_features-mod_hidden-self.charge_dim
         )
         self.pos_encoder = PositionalEncoding(
             out_features, max_len
         )
-        
-    def forward(self, 
+
+    def forward(self,
         aa_indices, mod_x, charges
     ):
         mod_x = self.mod_nn(mod_x)
         x = self.aa_emb(aa_indices)
         charge_x = charges[:, None, None].repeat(
             1, mod_x.size(1), self.charge_dim
         )
@@ -609,45 +610,45 @@
     ):
         super().__init__()
         mod_hidden = 8
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
         self.lstm = SeqLSTM(
             aa_embedding_size+mod_hidden,
             out_features,
-            n_lstm_layers=n_lstm_layers, 
+            n_lstm_layers=n_lstm_layers,
             bidirectional=True
         )
     def forward(self, aa_indices, mod_x):
         mod_x = self.mod_nn(mod_x)
         x = aa_one_hot(aa_indices, mod_x)
         return self.lstm(x)
 #legacy
 InputAALSTM = Input_26AA_Mod_LSTM
 
-        
+
 class Input_26AA_Mod_Meta_LSTM(torch.nn.Module):
     """
     Applies a LSTM network to a AA (26 AA letters) sequence and modifications,
-    and concatenates with 'meta' information (charge, nce, instrument_indices) 
+    and concatenates with 'meta' information (charge, nce, instrument_indices)
     """
     def __init__(self,
         out_features,
     ):
         super().__init__()
         meta_dim = 4
         mod_hidden = 8
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
         self.meta_nn = Meta_Embedding(meta_dim)
         self.nn = SeqLSTM(
             aa_embedding_size+mod_hidden,
             out_features-meta_dim,
             rnn_layer=1, bidirectional=True
         )
-        
-    def forward(self, 
+
+    def forward(self,
         aa_indices, mod_x, charges, NCEs, instrument_indices
     ):
         mod_x = self.mod_nn(mod_x)
         x = aa_one_hot(aa_indices, mod_x)
         x = self.nn(x)
         meta_x = self.meta_nn(
             charges, NCEs, instrument_indices
@@ -655,68 +656,68 @@
         return torch.cat((x, meta_x), 2)
 #legacy
 InputAALSTM_cat_Meta = Input_26AA_Mod_Meta_LSTM
 
 
 class Input_26AA_Mod_Charge_LSTM(torch.nn.Module):
     """
-    Applies a LSTM network to a AA (26 AA letters) sequence and modifications, 
+    Applies a LSTM network to a AA (26 AA letters) sequence and modifications,
     and concatenates with charge state information
     """
     def __init__(self,
         out_features,
     ):
         super().__init__()
         self.charge_dim = 2
         mod_hidden = 8
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
         self.nn = SeqLSTM(
             aa_embedding_size+mod_hidden,
             out_features-self.charge_dim,
             rnn_layer=1, bidirectional=True
         )
-        
+
     def forward(self, aa_indices, mod_x, charges):
         mod_x = self.mod_nn(mod_x)
         x = aa_one_hot(aa_indices, mod_x)
         x = self.nn(x)
         charge_x = charges.unsqueeze(1).repeat(
             1, mod_x.size(1), self.charge_dim
         )
         return torch.cat((x, charge_x), 2)
 #legacy
 InputAALSTM_cat_Charge = Input_26AA_Mod_Charge_LSTM
 
 
 class Seq_Meta_LSTM(torch.nn.Module):
     """
-    Takes a hidden layer which processes the hidden tensor 
+    Takes a hidden layer which processes the hidden tensor
     as well as the 'meta' information of NCE, Instrument, Charge
     """
     def __init__(self,
         in_features,
         out_features,
     ):
         super().__init__()
         meta_dim = 4
         self.meta_nn = Meta_Embedding(meta_dim)
         self.nn = SeqLSTM(
             in_features+meta_dim,
             out_features,
             rnn_layer=1, bidirectional=False
         )
-        
+
     def forward(self, x, charges, NCEs, instrument_indices):
         meta_x = self.meta_nn(
             charges, NCEs, instrument_indices
         ).unsqueeze(1).repeat(1, x.size(1), 1)
         return self.nn(torch.cat((x, meta_x), 2))
 #legacy
 OutputLSTM_cat_Meta = Seq_Meta_LSTM
-    
+
 class Seq_Meta_Linear(torch.nn.Module):
     """
     takes a hidden linear which processed the 'meta' information of NCE, Instrument, Charge
     """
     def __init__(self,
         in_features,
         out_features,
@@ -725,33 +726,33 @@
         meta_dim = 4
         self.meta_nn = Meta_Embedding(meta_dim)
         self.nn = torch.nn.Linear(
             in_features+meta_dim,
             out_features,
             bias=False
         )
-        
+
     def forward(self, x, charges, NCEs, instrument_indices):
         meta_x = self.meta_nn(
             charges, NCEs, instrument_indices
         ).unsqueeze(1).repeat(1, x.size(1), 1)
         return self.nn(torch.cat((x, meta_x), 2))
 #legacy
 OutputLinear_cat_Meta = Seq_Meta_Linear
 
 class Encoder_26AA_Mod_LSTM(torch.nn.Module):
     """
     Two LSTM layers on AA (26 AA letters) and modifications.
     """
     def __init__(self, out_features, n_lstm_layers=1):
         super().__init__()
-        
+
         self.input_nn = Input_26AA_Mod_LSTM(out_features)
         self.nn = SeqLSTM(
-            out_features, out_features, 
+            out_features, out_features,
             rnn_layer=n_lstm_layers
         )
 
     def forward(self, aa_indices, mod_x):
         x = self.input_nn(aa_indices, mod_x)
         x = self.nn(x)
         return x
@@ -768,15 +769,15 @@
         super().__init__()
 
         mod_hidden = 8
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
         input_dim = aa_embedding_size+mod_hidden
         self.input_cnn = SeqCNN(input_dim)
         self.hidden_nn = SeqLSTM(
-            input_dim*4, out_features, 
+            input_dim*4, out_features,
             rnn_layer=n_lstm_layers
         ) #SeqCNN outputs 4*input_dim
 
     def forward(self, aa_indices, mod_x):
         mod_x = self.mod_nn(mod_x)
         x = aa_one_hot(aa_indices, mod_x)
         x = self.input_cnn(x)
@@ -784,27 +785,27 @@
         return x
 
 #legacy
 Input_AA_CNN_Encoder = Encoder_26AA_Mod_CNN_LSTM
 
 class Encoder_26AA_Mod_CNN_LSTM_AttnSum(torch.nn.Module):
     """
-    Encode AAs (26 AA letters) and modifications by CNN and LSTM layers, 
+    Encode AAs (26 AA letters) and modifications by CNN and LSTM layers,
     then by 'SeqAttentionSum'.
     """
     def __init__(self, out_features, n_lstm_layers=2):
         super().__init__()
-        
+
         mod_hidden = 8
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
 
         input_dim = aa_embedding_size+mod_hidden
         self.input_cnn = SeqCNN(input_dim)
         self.hidden_nn = SeqLSTM(
-            input_dim*4, out_features, 
+            input_dim*4, out_features,
             rnn_layer=n_lstm_layers
         ) #SeqCNN outputs 4*input_dim
         self.attn_sum = SeqAttentionSum(out_features)
 
     def forward(self, aa_indices, mod_x):
         mod_x = self.mod_nn(mod_x)
         x = aa_one_hot(aa_indices, mod_x)
@@ -813,54 +814,54 @@
         x = self.attn_sum(x)
         return x
 #legacy
 Input_AA_CNN_LSTM_Encoder = Encoder_26AA_Mod_CNN_LSTM_AttnSum
 
 class Encoder_AA_Mod_CNN_LSTM_AttnSum(torch.nn.Module):
     """
-    Encode AAs (128 ASCII codes) and modifications by CNN and LSTM layers, 
+    Encode AAs (128 ASCII codes) and modifications by CNN and LSTM layers,
     and then by 'SeqAttentionSum'.
     """
     def __init__(self, out_features, n_lstm_layers=2):
         super().__init__()
-        
+
         mod_hidden = 8
         input_dim = out_features//4
         self.aa_mod_embedding = AA_Mod_Embedding(
             input_dim, mod_feature_size=mod_hidden
         )
         self.input_cnn = SeqCNN(input_dim)
         self.hidden_nn = SeqLSTM(
-            input_dim*4, out_features, 
+            input_dim*4, out_features,
             rnn_layer=n_lstm_layers
         ) #SeqCNN outputs 4*input_dim
         self.attn_sum = SeqAttentionSum(out_features)
 
     def forward(self, aa_indices, mod_x):
         x = self.aa_mod_embedding(aa_indices, mod_x)
         x = self.input_cnn(x)
         x = self.hidden_nn(x)
         x = self.attn_sum(x)
         return x
 
 
 class Encoder_AA_Mod_Transformer(torch.nn.Module):
     """
-    AAs (128 ASCII codes) and modifications embedded by Bert, 
+    AAs (128 ASCII codes) and modifications embedded by Bert,
     then encoded by 'SeqAttentionSum'.
     """
     def __init__(self,out_features,
         dropout=0.1,
         nlayers=4,
         output_attentions=False
     ):
         super().__init__()
 
         self.dropout = torch.nn.Dropout(dropout)
-        
+
         self.input_nn = Input_AA_Mod_PositionalEncoding(out_features)
 
         self.output_attentions = output_attentions
         self.encoder = Hidden_HFace_Transformer(
             out_features, nlayers=nlayers, dropout=dropout,
             output_attentions=output_attentions
         )
@@ -887,36 +888,36 @@
         dropout=0.1,
         nlayers=4,
         output_attentions=False
     ):
         super().__init__()
 
         self.dropout = torch.nn.Dropout(dropout)
-        
+
         self.encoder_nn = Encoder_AA_Mod_Transformer(
             out_features, dropout=dropout, nlayers=nlayers,
-            output_attentions=output_attentions 
+            output_attentions=output_attentions
         )
         self.attn_sum = SeqAttentionSum(out_features)
-        
+
     def forward(self, aa_indices, mod_x):
         x = self.encoder_nn(aa_indices, mod_x)
         return self.dropout(self.attn_sum(x))
 
 class Encoder_AA_Mod_Charge_Transformer(torch.nn.Module):
     """
     Encode AAs (128 ASCII codes), modifications and charge by transformers.
     """
     def __init__(self,out_features,
         dropout=0.1,
         nlayers=4,
         output_attentions=False
     ):
         super().__init__()
-        
+
         self.dropout = torch.nn.Dropout(dropout)
         self.input_nn = Input_AA_Mod_Charge_PositionalEncoding(out_features)
 
         self.output_attentions = output_attentions
         self.encoder = Hidden_HFace_Transformer(
             out_features, nlayers=nlayers, dropout=dropout,
             output_attentions=output_attentions
@@ -934,57 +935,57 @@
             self.attentions = x[1]
         else:
             self.attentions = None
         return x[0]
 
 class Encoder_AA_Mod_Charge_Transformer_AttnSum(torch.nn.Module):
     """
-    Encode AAs (128 ASCII codes), modifications and charge by transformers, 
+    Encode AAs (128 ASCII codes), modifications and charge by transformers,
     and then by 'SeqAttentionSum'
     """
     def __init__(self,out_features,
         dropout=0.1,
         nlayers=4,
         output_attentions=False
     ):
         super().__init__()
 
         self.dropout = torch.nn.Dropout(dropout)
-        
+
         self.encoder_nn = Encoder_AA_Mod_Charge_Transformer(
             out_features, dropout=dropout, nlayers=nlayers,
-            output_attentions=output_attentions 
+            output_attentions=output_attentions
         )
         self.attn_sum = SeqAttentionSum(out_features)
     def forward(self, aa_indices, mod_x, charges):
         x = self.encoder_nn(aa_indices, mod_x, charges)
         return self.dropout(self.attn_sum(x))
 
 class Encoder_26AA_Mod_Charge_CNN_LSTM_AttnSum(torch.nn.Module):
     """
-    Encode AAs (26 AA letters), modifications and charge by transformers, 
+    Encode AAs (26 AA letters), modifications and charge by transformers,
     and then by 'SeqAttentionSum'
     """
     def __init__(self, out_features):
         super().__init__()
-        
+
         mod_hidden = 8
         self.mod_nn = Mod_Embedding_FixFirstK(mod_hidden)
 
         input_dim = aa_embedding_size+mod_hidden+1
         self.input_cnn = SeqCNN(input_dim)
         self.hidden_nn = SeqLSTM(
             input_dim*4, out_features, rnn_layer=2
         ) #SeqCNN outputs 4*input_dim
         self.attn_sum = SeqAttentionSum(out_features)
 
     def forward(self, aa_indices, mod_x, charges):
         mod_x = self.mod_nn(mod_x)
         x = aa_one_hot(
-            aa_indices, mod_x, 
+            aa_indices, mod_x,
             charges.unsqueeze(1).repeat(1,mod_x.size(1),1)
         )
         x = self.input_cnn(x)
         x = self.hidden_nn(x)
         x = self.attn_sum(x)
         return x
 
@@ -1004,15 +1005,15 @@
             in_features, out_features,
             rnn_layer=1, bidirectional=False,
         )
 
         self.output_nn = torch.nn.Linear(
             hidden, out_features, bias=False
         )
-    
+
     def forward(self, x:torch.tensor, output_len):
         x = self.rnn(
             x.unsqueeze(1).repeat(1,output_len,1)
         )
         x = self.output_nn(x)
         return x
 #legacy
@@ -1030,15 +1031,15 @@
             in_features, out_features,
             rnn_layer=1, bidirectional=False,
         )
 
         self.output_nn = torch.nn.Linear(
             hidden, out_features, bias=False
         )
-    
+
     def forward(self, x:torch.tensor, output_len):
         x = self.rnn(
             x.unsqueeze(1).repeat(1,output_len,1)
         )
         x = self.output_nn(x)
         return x
 #legacy
```

### Comparing `peptdeep-1.1.9/peptdeep/model/ccs.py` & `peptdeep-1.2.0/peptdeep/model/ccs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 import torch
 import pandas as pd
-import numpy as np
 import typing
 
-from tqdm import tqdm
-
-from alphabase.peptide.fragment import update_precursor_mz
 
 from alphabase.peptide.mobility import (
     ccs_to_mobility_for_df,
     mobility_to_ccs_for_df
 )
 
-from peptdeep.model.featurize import (
-    get_batch_aa_indices, 
-    get_batch_mod_feature
-)
-
-from peptdeep.settings import model_const
-
 import peptdeep.model.base as model_base
 from peptdeep.utils import evaluate_linear_regression
 
 
 class Model_CCS_Bert(torch.nn.Module):
     """
     Transformer model for CCS prediction
@@ -37,15 +26,15 @@
         super().__init__()
 
         self.dropout = torch.nn.Dropout(dropout)
 
         self.input_nn = model_base.AATransformerEncoding(hidden-2)
 
         self._output_attentions = output_attentions
-        
+
         self.hidden_nn = model_base.Hidden_HFace_Transformer(
             hidden, nlayers=nlayers, dropout=dropout,
             output_attentions=output_attentions
         )
 
         self.output_nn = torch.nn.Sequential(
             model_base.SeqAttentionSum(hidden),
@@ -59,16 +48,16 @@
         return self._output_attentions
 
     @output_attentions.setter
     def output_attentions(self, val:bool):
         self._output_attentions = val
         self.hidden_nn.output_attentions = val
 
-    def forward(self, 
-        aa_indices, 
+    def forward(self,
+        aa_indices,
         mod_x,
         charges:torch.Tensor,
     ):
         x = self.dropout(self.input_nn(
             aa_indices, mod_x
         ))
         charges = charges.unsqueeze(1).repeat(1,x.size(1),2)
@@ -85,31 +74,31 @@
 
 class Model_CCS_LSTM(torch.nn.Module):
     """LSTM model for CCS prediction"""
     def __init__(self,
         dropout=0.1
     ):
         super().__init__()
-        
+
         self.dropout = torch.nn.Dropout(dropout)
-        
+
         hidden = 256
 
         self.ccs_encoder = (
             model_base.Encoder_26AA_Mod_Charge_CNN_LSTM_AttnSum(
                 hidden
             )
         )
 
         self.ccs_decoder = model_base.Decoder_Linear(
             hidden+1, 1
         )
 
-    def forward(self, 
-        aa_indices, 
+    def forward(self,
+        aa_indices,
         mod_x,
         charges,
     ):
         x = self.ccs_encoder(aa_indices, mod_x, charges)
         x = self.dropout(x)
         x = torch.cat((x, charges),1)
         return self.ccs_decoder(x).squeeze(1)
@@ -136,47 +125,47 @@
     )
     return precursor_df
 
 class AlphaCCSModel(model_base.ModelInterface):
     """
     `ModelInterface` for `Model_CCS_LSTM` or `Model_CCS_Bert`
     """
-    def __init__(self, 
+    def __init__(self,
         dropout=0.1,
         model_class:torch.nn.Module=Model_CCS_LSTM,
         device:str='gpu',
         **kwargs,
     ):
         super().__init__(device=device)
         self.model:Model_CCS_LSTM = None
         self.build(
             model_class,
-            dropout=dropout, 
+            dropout=dropout,
             **kwargs
         )
         self.charge_factor = 0.1
 
         self.target_column_to_predict = 'ccs_pred'
         self.target_column_to_train = 'ccs'
 
-    def test(self, 
-        precursor_df: pd.DataFrame, 
+    def test(self,
+        precursor_df: pd.DataFrame,
         *,
-        x:typing.Literal["ccs_pred","mobility_pred"]="ccs_pred", 
+        x:typing.Literal["ccs_pred","mobility_pred"]="ccs_pred",
         y:typing.Literal["ccs","mobility"]="ccs",
         batch_size:int = 1024,
     ):
         return evaluate_linear_regression(
             self.predict(
                 precursor_df, batch_size=batch_size
             ),
             x=x, y=y
         )
 
-    def _get_features_from_batch_df(self, 
+    def _get_features_from_batch_df(self,
         batch_df: pd.DataFrame,
     ):
         aa_indices = self._get_26aa_indice_features(batch_df)
 
         mod_x = self._get_mod_features(batch_df)
 
         charges = self._as_tensor(
```

### Comparing `peptdeep-1.1.9/peptdeep/model/charge.py` & `peptdeep-1.2.0/peptdeep/model/charge.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     Model_for_Generic_ModAASeq_BinaryClassification_Transformer,
 )
 
 class _ChargeModelInterface:
     def __init__(self, *args, **kwargs):
         raise TypeError("Interface class cannot be instantiated.")
     def predict_charges_as_prob(self,
-        pep_df:pd.DataFrame, 
+        pep_df:pd.DataFrame,
         min_precursor_charge:int,
         max_precursor_charge:int,
     ):
         df = self.predict_mp(
-            pep_df.copy(), 
+            pep_df.copy(),
             batch_size=self.predict_batch_size,
         )
         df.rename(columns={"charge_probs":"charge_prob"}, inplace=True)
         df["charge"] = [self.charge_range[
             min_precursor_charge-self.min_predict_charge:
             max_precursor_charge-self.min_predict_charge+1
         ]]*len(df)
@@ -33,15 +33,15 @@
         )
         df = df.explode(
             ["charge","charge_prob"], ignore_index=True
         ).dropna(subset=["charge"])
         df["charge"] = df.charge.astype(np.int8)
         df["charge_prob"] = df.charge_prob.astype(np.float32)
         return df
-    
+
     def predict_prob_for_charge(self,
         precursor_df:pd.DataFrame,
     ):
         if "charge" not in precursor_df.columns:
             raise KeyError("precursor_df must contain `charge` column")
         precursor_df = self.predict_mp(
             precursor_df,
@@ -49,16 +49,16 @@
         )
         precursor_df["charge_prob"] = precursor_df[["charge_probs","charge"]].apply(
             lambda x: x.iloc[0][x.iloc[1]-self.min_predict_charge], axis=1
         ).astype(np.float32)
         precursor_df.drop(columns="charge_probs", inplace=True)
         return precursor_df
 
-    def predict_and_clip_charges(self, 
-        pep_df:pd.DataFrame, 
+    def predict_and_clip_charges(self,
+        pep_df:pd.DataFrame,
         min_precursor_charge:int,
         max_precursor_charge:int,
         charge_prob_cutoff:float,
     ):
         df = self.predict_mp(
             pep_df.copy(),
             batch_size=self.predict_batch_size,
@@ -75,27 +75,36 @@
         ).dropna(subset=["charge"])
         df["charge"] = df.charge.astype(np.int8)
         df = df.query(
             f"charge>={min_precursor_charge} and charge<={max_precursor_charge}"
         ).reset_index(drop=True)
         df["charge_prob"] = df.charge_prob.astype(np.float32)
         return df
-    
+
 class ChargeModelForModAASeq(
     ModelInterface_for_Generic_ModAASeq_MultiLabelClassification,
     _ChargeModelInterface
 ):
     """
     ModelInterface for charge prediction for modified peptides
+
+     Parameters
+    ----------
+    min_charge : int, optional
+        Minimum charge to predict, by default 1
+    max_charge : int, optional
+        Maximum charge to predict, by default 6
+    device : str, optional
+        Device to use for training and prediction, by default "gpu"
     """
-    def __init__(self, min_charge:int=1, max_charge:int=6):
+    def __init__(self, min_charge:int=1, max_charge:int=6, device:str="gpu"):
         super().__init__(
             num_target_values=max_charge-min_charge+1,
             model_class=Model_for_Generic_ModAASeq_BinaryClassification_Transformer,
-            nlayers=4, hidden_dim=128, dropout=0.1
+            nlayers=4, hidden_dim=128, dropout=0.1, device=device
         )
 
         self.target_column_to_predict = "charge_probs"
         self.target_column_to_train = "charge_indicators"
         self.min_predict_charge = min_charge
         self.max_predict_charge = max_charge
         self.charge_range = np.arange(
@@ -105,20 +114,29 @@
 
 class ChargeModelForAASeq(
     ModelInterface_for_Generic_AASeq_MultiLabelClassification,
     _ChargeModelInterface
 ):
     """
     ModelInterface for charge prediction for amino acid sequence
+
+    Parameters
+    ----------
+    min_charge : int, optional
+        Minimum charge to predict, by default 1
+    max_charge : int, optional
+        Maximum charge to predict, by default 6
+    device : str, optional
+        Device to use for training and prediction, by default "gpu"
     """
-    def __init__(self, min_charge:int=1, max_charge:int=6):
+    def __init__(self, min_charge:int=1, max_charge:int=6,device:str="gpu"):
         super().__init__(
             num_target_values=max_charge-min_charge+1,
             model_class=Model_for_Generic_AASeq_BinaryClassification_Transformer,
-            nlayers=4, hidden_dim=128, dropout=0.1
+            nlayers=4, hidden_dim=128, dropout=0.1, device=device
         )
 
         self.target_column_to_predict = "charge_probs"
         self.target_column_to_train = "charge_indicators"
         self.min_predict_charge = min_charge
         self.max_predict_charge = max_charge
         self.charge_range = np.arange(
@@ -154,8 +172,8 @@
     min_charge:int,
     max_charge:int,
 ):
     charge_indicators = np.zeros(max_charge-min_charge+1)
     for charge in charge_list:
         if charge <= max_charge and charge >= min_charge:
             charge_indicators[charge-min_charge] = 1.0
-    return charge_indicators
+    return charge_indicators
```

### Comparing `peptdeep-1.1.9/peptdeep/model/featurize.py` & `peptdeep-1.2.0/peptdeep/model/featurize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import numpy as np
 import pandas as pd
 from typing import List, Union
 
 from peptdeep.settings import (
-    model_const, mod_feature_size, MOD_TO_FEATURE, 
+    model_const, mod_feature_size, MOD_TO_FEATURE,
     mod_elements, mod_elem_to_idx,
     _parse_mod_formula, update_all_mod_features,
 )
 
 def parse_mod_feature(
-    nAA:int, 
-    mod_names:List[str], 
+    nAA:int,
+    mod_names:List[str],
     mod_sites:List[int]
 )->np.ndarray:
     '''
-    Get modification feature of a given peptide (len=nAA). 
-    Note that `site=0` is for peptide N-term modification, 
-    `site=1` is for peptide C-term modification, and 
+    Get modification feature of a given peptide (len=nAA).
+    Note that `site=0` is for peptide N-term modification,
+    `site=1` is for peptide C-term modification, and
     `1<=site<=nAA` is for residue modifications on the peptide.
 
     Parameters
     ----------
     nAA : int
         the lenght of the peptide sequence
 
@@ -86,17 +86,17 @@
     return mod_x_batch
 
 def get_batch_aa_indices(
     seq_array: Union[List, np.ndarray]
 )->np.ndarray:
     '''
     Convert peptide sequences into AA ID array. ID=0 is reserved for masking,
-    so ID of 'A' is 1, ID of 'B' is 2, ..., ID of 'Z' is 26 (maximum). 
+    so ID of 'A' is 1, ID of 'B' is 2, ..., ID of 'Z' is 26 (maximum).
     Zeros are padded into the N- and C-term for each sequence.
-    
+
     Parameters
     ----------
     seq_array : Union[List,np.ndarray]
         list or 1-D array of sequences with the same length
 
     Returns
     -------
@@ -112,41 +112,41 @@
     # padding zeros at the N- and C-term
     return np.pad(x, [(0,0)]*(len(x.shape)-1)+[(1,1)])
 
 def get_ascii_indices(
     seq_array: Union[List, np.ndarray]
 )->np.ndarray:
     '''
-    Convert peptide sequences into ASCII code array. 
-    The values are from 0 to 127. 
+    Convert peptide sequences into ASCII code array.
+    The values are from 0 to 127.
     Zeros are padded into the N- and C-term for each sequence.
 
     Parameters
     ----------
     seq_array : Union[List,np.ndarray]
         list or 1-D array of sequences.
 
     Returns
     -------
     np.ndarray
         2-D `np.int32` array with the shape
-        `(len(seq_array), max seq length+2)`. 
+        `(len(seq_array), max seq length+2)`.
         For the the sequence whose length is shorter than max seq length,
         zeros are padded to the missing values.
-        
+
     '''
-    
+
     x = np.array(seq_array).view(np.int32).reshape(
         len(seq_array), -1
     )
     return np.pad(x, [(0,0)]*(len(x.shape)-1)+[(1,1)])
 
 instrument_dict = dict(
     zip(
-        [inst.upper() for inst in model_const['instruments']], 
+        [inst.upper() for inst in model_const['instruments']],
         range(len(model_const['instruments']))
     )
 )
 unknown_inst_index = model_const['max_instrument_num']-1
 
 def parse_instrument_indices(instrument_list):
     instrument_list = [inst.upper() for inst in instrument_list]
```

### Comparing `peptdeep-1.1.9/peptdeep/model/generic_property_prediction.py` & `peptdeep-1.2.0/peptdeep/model/generic_property_prediction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import torch
 import pandas as pd
 import numpy as np
 
 import peptdeep.model.building_block as building_block
-from peptdeep.model.model_interface import ModelInterface, is_precursor_sorted
+from peptdeep.model.model_interface import ModelInterface
+from alphabase.peptide.precursor import is_precursor_refined
 
 ASCII_NUM=128
 
 class Model_for_Generic_AASeq_Regression_LSTM(torch.nn.Module):
     """Generic LSTM regression model for AA sequence"""
-    def __init__(self, 
+    def __init__(self,
         *,
         hidden_dim=256,
         output_dim=1,
         nlayers=4,
         dropout=0.1,
         **kwargs,
     ):
         super().__init__()
         self.dropout = torch.nn.Dropout(dropout)
-        
+
         self.nn = torch.nn.Sequential(
             building_block.ascii_embedding(hidden_dim//4),
             building_block.SeqCNN(hidden_dim//4),
             self.dropout,
             building_block.SeqLSTM(
-                hidden_dim, hidden_dim, 
+                hidden_dim, hidden_dim,
                 rnn_layer=nlayers
             ),
             building_block.SeqAttentionSum(hidden_dim),
             self.dropout,
             torch.nn.Linear(hidden_dim,64),
             torch.nn.GELU(),
             torch.nn.Linear(64, output_dim),
@@ -51,15 +52,15 @@
         super().__init__()
 
         self.dropout = torch.nn.Dropout(dropout)
 
         self.input_nn = building_block.ascii_embedding(hidden_dim)
 
         self.output_attentions = output_attentions
-        
+
         self.hidden_nn = building_block.HFace_Transformer_with_PositionalEncoder(
             hidden_dim, nlayers=nlayers, dropout=dropout,
             output_attentions=output_attentions
         )
 
         self.output_nn = torch.nn.Sequential(
             building_block.SeqAttentionSum(hidden_dim),
@@ -89,16 +90,16 @@
         return self.output_nn(aa_x).squeeze(1)
 
 
 class ModelInterface_for_Generic_AASeq_Regression(ModelInterface):
     """
     `ModelInterface` for Generic_AASeq_Regression models
     """
-    def __init__(self, 
-        model_class:torch.nn.Module=Model_for_Generic_AASeq_Regression_LSTM, 
+    def __init__(self,
+        model_class:torch.nn.Module=Model_for_Generic_AASeq_Regression_LSTM,
         dropout=0.1,
         device:str='gpu',
         hidden_dim=256,
         output_dim=1,
         nlayers=4,
         **kwargs,
     ):
@@ -114,15 +115,15 @@
         self.loss_func = torch.nn.L1Loss() # for regression
 
         self.target_column_to_predict = 'predicted_property'
         self.target_column_to_train = 'detected_property'
 
 class Model_for_Generic_ModAASeq_Regression_LSTM(torch.nn.Module):
     """Generic LSTM regression model for modified sequence"""
-    def __init__(self, 
+    def __init__(self,
         *,
         hidden_dim=256,
         output_dim=1,
         nlayers=4,
         dropout=0.1,
         **kwargs,
     ):
@@ -157,15 +158,15 @@
         super().__init__()
 
         self.dropout = torch.nn.Dropout(dropout)
 
         self.input_nn = building_block.AA_Mod_Embedding(hidden_dim)
 
         self._output_attentions = output_attentions
-        
+
         self.hidden_nn = building_block.HFace_Transformer_with_PositionalEncoder(
             hidden_dim, nlayers=nlayers, dropout=dropout,
             output_attentions=output_attentions
         )
 
         self.output_nn = torch.nn.Sequential(
             building_block.SeqAttentionSum(hidden_dim),
@@ -178,16 +179,16 @@
     def output_attentions(self)->bool:
         return self._output_attentions
 
     @output_attentions.setter
     def output_attentions(self, val:bool):
         self._output_attentions = val
 
-    def forward(self, 
-        aa_indices, 
+    def forward(self,
+        aa_indices,
         mod_x,
     ):
         x = self.dropout(self.input_nn(
             aa_indices, mod_x
         ))
 
         hidden_x = self.hidden_nn(x)
@@ -199,15 +200,15 @@
 
         return self.output_nn(x).squeeze(1)
 
 class ModelInterface_for_Generic_ModAASeq_Regression(ModelInterface):
     """
     `ModelInterface` for all Generic_ModAASeq_Regression models
     """
-    def __init__(self, 
+    def __init__(self,
         model_class:torch.nn.Module=Model_for_Generic_ModAASeq_Regression_LSTM,
         dropout=0.1,
         device:str='gpu',
         hidden_dim=256,
         output_dim=1,
         nlayers=4,
         **kwargs,
@@ -222,25 +223,25 @@
             **kwargs
         )
         self.loss_func = torch.nn.L1Loss() # for regression
 
         self.target_column_to_predict = 'predicted_property'
         self.target_column_to_train = 'detected_property'
 
-    def _get_features_from_batch_df(self, 
+    def _get_features_from_batch_df(self,
         batch_df: pd.DataFrame,
         **kwargs,
     ):
         return self._get_aa_mod_features(batch_df)
 
 class Model_for_Generic_AASeq_BinaryClassification_LSTM(
     Model_for_Generic_AASeq_Regression_LSTM
 ):
     """Generic LSTM classification model for AA sequence"""
-    def __init__(self, 
+    def __init__(self,
         *,
         hidden_dim=256,
         output_dim=1,
         nlayers=4,
         dropout=0.1,
         **kwargs,
     ):
@@ -265,15 +266,15 @@
         output_dim = 1,
         nlayers = 4,
         output_attentions=False,
         dropout = 0.1,
         **kwargs,
     ):
         """
-        Model based on a transformer Architecture from 
+        Model based on a transformer Architecture from
         Huggingface's BertEncoder class.
         """
         super().__init__(
             nlayers=nlayers,
             hidden_dim=hidden_dim,
             output_dim=output_dim,
             output_attentions=output_attentions,
@@ -285,15 +286,15 @@
         x = super().forward(aa_x)
         return torch.sigmoid(x)
 
 class ModelInterface_for_Generic_AASeq_BinaryClassification(ModelInterface):
     """
     `ModelInterface` for all Generic_AASeq_BinaryClassification models
     """
-    def __init__(self, 
+    def __init__(self,
         model_class:torch.nn.Module=Model_for_Generic_AASeq_BinaryClassification_LSTM,
         dropout=0.1,
         device:str='gpu',
         hidden_dim=256,
         output_dim=1,
         nlayers=4,
         **kwargs,
@@ -314,15 +315,15 @@
         self.target_column_to_predict = 'predicted_prob'
         self.target_column_to_train = 'detected_prob'
 
 class Model_for_Generic_ModAASeq_BinaryClassification_LSTM(
     Model_for_Generic_ModAASeq_Regression_LSTM
 ):
     """Generic LSTM classification model for modified sequence"""
-    def __init__(self, 
+    def __init__(self,
         *,
         hidden_dim=256,
         output_dim=1,
         nlayers=4,
         dropout=0.1,
         **kwargs,
     ):
@@ -365,27 +366,27 @@
     def output_attentions(self)->bool:
         return self._output_attentions
 
     @output_attentions.setter
     def output_attentions(self, val:bool):
         self._output_attentions = val
 
-    def forward(self, 
-        aa_indices, 
+    def forward(self,
+        aa_indices,
         mod_x,
     ):
         x = super().forward(aa_indices, mod_x)
         return torch.sigmoid(x)
 
 
 class ModelInterface_for_Generic_ModAASeq_BinaryClassification(ModelInterface):
     """
     `ModelInterface` for Generic_ModAASeq_BinaryClassification
     """
-    def __init__(self, 
+    def __init__(self,
         model_class:torch.nn.Module=Model_for_Generic_ModAASeq_BinaryClassification_LSTM,
         dropout=0.1,
         device:str='gpu',
         hidden_dim=256,
         output_dim=1,
         nlayers=4,
         **kwargs,
@@ -400,24 +401,24 @@
             **kwargs
         )
         self.loss_func = torch.nn.BCELoss() # for classification
 
         self.target_column_to_predict = 'predicted_prob'
         self.target_column_to_train = 'detected_prob'
 
-    def _get_features_from_batch_df(self, 
+    def _get_features_from_batch_df(self,
         batch_df: pd.DataFrame,
     ):
         return self._get_aa_mod_features(batch_df)
-    
+
 
 class ModelInterface_for_Generic_AASeq_MultiLabelClassification(
     ModelInterface_for_Generic_AASeq_BinaryClassification
 ):
-    def __init__(self, 
+    def __init__(self,
         num_target_values:int=6,
         model_class:torch.nn.Module=Model_for_Generic_AASeq_BinaryClassification_Transformer,
         nlayers=4, hidden_dim=256, device='gpu',
         dropout=0.1, **kwargs,
     ):
         self.num_target_values = num_target_values
         super().__init__(
@@ -428,20 +429,20 @@
             **kwargs
         )
         self.target_column_to_train = 'target_probs'
         self.target_column_to_predict = 'target_probs_pred'
 
     def _get_targets_from_batch_df(self, batch_df, **kwargs):
         return self._as_tensor(
-            np.stack(batch_df[self.target_column_to_train].values), 
+            np.stack(batch_df[self.target_column_to_train].values),
             dtype=torch.float32
         )
-    
+
     def _check_predict_in_order(self, precursor_df:pd.DataFrame):
-        if not is_precursor_sorted(precursor_df):
+        if not is_precursor_refined(precursor_df):
             # multilabel prediction can only predict in order
             precursor_df.sort_values("nAA", inplace=True)
             precursor_df.reset_index(drop=True, inplace=True)
 
     def _prepare_predict_data_df(self, precursor_df, **kwargs):
         precursor_df[self.target_column_to_predict] = [
             [0]*self.num_target_values
@@ -452,15 +453,15 @@
         self.predict_df.loc[:,self.target_column_to_predict].values[
             batch_df.index.values[0]:batch_df.index.values[-1]+1
         ] = list(predict_values)
 
 class ModelInterface_for_Generic_ModAASeq_MultiLabelClassification(
     ModelInterface_for_Generic_ModAASeq_BinaryClassification
 ):
-    def __init__(self, 
+    def __init__(self,
         num_target_values:int=6,
         model_class:torch.nn.Module=Model_for_Generic_ModAASeq_BinaryClassification_Transformer,
         nlayers=4, hidden_dim=256, device='gpu',
         dropout=0.1, **kwargs,
     ):
         self.num_target_values = num_target_values
         super().__init__(
@@ -471,20 +472,20 @@
             **kwargs
         )
         self.target_column_to_train = 'target_probs'
         self.target_column_to_predict = 'target_probs_pred'
 
     def _get_targets_from_batch_df(self, batch_df, **kwargs):
         return self._as_tensor(
-            np.stack(batch_df[self.target_column_to_train].values), 
+            np.stack(batch_df[self.target_column_to_train].values),
             dtype=torch.float32
         )
-    
+
     def _check_predict_in_order(self, precursor_df:pd.DataFrame):
-        if not is_precursor_sorted(precursor_df):
+        if not is_precursor_refined(precursor_df):
             # multilabel prediction can only predict in order
             precursor_df.sort_values("nAA", inplace=True)
             precursor_df.reset_index(drop=True, inplace=True)
 
     def _prepare_predict_data_df(self, precursor_df, **kwargs):
         precursor_df[self.target_column_to_predict] = [
             [0]*self.num_target_values
```

### Comparing `peptdeep-1.1.9/peptdeep/model/model_interface.py` & `peptdeep-1.2.0/peptdeep/model/model_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,78 +14,186 @@
 
 from torch.optim.lr_scheduler import LambdaLR
 # from transformers.optimization import get_cosine_schedule_with_warmup
 
 from zipfile import ZipFile
 from typing import IO, Tuple, List, Union
 from alphabase.yaml_utils import save_yaml, load_yaml
-from alphabase.peptide.precursor import is_precursor_sorted
+from alphabase.peptide.precursor import is_precursor_refined
 
 from peptdeep.settings import model_const
-from peptdeep.utils import ( 
+from peptdeep.utils import (
     logging, process_bar, get_device,
     get_available_device
 )
 from peptdeep.settings import global_settings
 
 from peptdeep.model.featurize import (
     get_ascii_indices, get_batch_aa_indices,
     get_batch_mod_feature
 )
 
-# `transformers.optimization.get_cosine_schedule_with_warmup` will import tensorflow,
-# resulting in some package version issues.
-# Here we copy the code from transformers.optimization
-def _get_cosine_schedule_with_warmup_lr_lambda(
-    current_step: int, *, num_warmup_steps: int, num_training_steps: int, num_cycles: float
-):
-    if current_step < num_warmup_steps:
-        return float(current_step+1) / float(max(1, num_warmup_steps))
-    progress = float(current_step - num_warmup_steps) / float(num_training_steps - num_warmup_steps)
-    return (
-        max(1e-10, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
-    )
-    # if current_step < num_warmup_steps:
-    #     return float(current_step) / float(max(1, num_warmup_steps))
-    # progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
-    # return max(0.0, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
-
-
-def get_cosine_schedule_with_warmup(
-    optimizer, num_warmup_steps: int, num_training_steps: int, num_cycles: float = 0.5, last_epoch: int = -1
-):
+class LR_SchedulerInterface(object):
+    def __init__(self, optimizer:torch.optim.Optimizer, **kwargs):
+        raise NotImplementedError
+
+    def step(self, epoch:int, loss:float):
+        """
+        This method must be implemented in the sub-class. It will be called to get the learning rate for the next epoch.
+        While the one we are using here does not need the loss value, this is left in case of using something like the ReduceLROnPlateau scheduler.
+
+        Parameters
+        ----------
+        epoch : int
+            The current epoch number.
+        loss : float
+            The loss value of the current epoch.
+        """
+        raise NotImplementedError
+
+    def get_last_lr(self)->float:
+        """
+        Get the last learning rate.
+
+        Returns
+        -------
+        float
+            The last learning rate.
+        """
+        raise NotImplementedError
+
+class WarmupLR_Scheduler(LR_SchedulerInterface):
+    """
+    A learning rate scheduler that includes a warmup phase and then a cosine annealing phase.
     """
-    Create a schedule with a learning rate that decreases following the values of the cosine function between the
-    initial lr set in the optimizer to 0, after a warmup period during which it increases linearly between 0 and the
-    initial lr set in the optimizer.
-
-    Args:
-        optimizer ([`~torch.optim.Optimizer`]):
-            The optimizer for which to schedule the learning rate.
-        num_warmup_steps (`int`):
-            The number of steps for the warmup phase.
-        num_training_steps (`int`):
-            The total number of training steps.
-        num_cycles (`float`, *optional*, defaults to 0.5):
-            The number of waves in the cosine schedule (the defaults is to just decrease from the max value to 0
-            following a half-cosine).
-        last_epoch (`int`, *optional*, defaults to -1):
-            The index of the last epoch when resuming training.
 
-    Return:
-        `torch.optim.lr_scheduler.LambdaLR` with the appropriate schedule.
+    def __init__(self,
+        optimizer:torch.optim.Optimizer,
+        num_warmup_steps:int,
+        num_training_steps:int,
+        num_cycles:float=0.5,
+        last_epoch:int=-1
+    ):
+        self.optimizer = optimizer
+        self.lambda_lr = self.get_cosine_schedule_with_warmup(
+            optimizer, num_warmup_steps, num_training_steps, num_cycles, last_epoch
+        )
+
+    def step(self, epoch:int, loss:float):
+        """
+        Get the learning rate for the next epoch.
+
+        Parameters
+        ----------
+        epoch : int
+            The current epoch number.
+        loss : float
+            The loss value of the current epoch.
+
+        """
+        return self.lambda_lr.step(epoch)
+
+    def get_last_lr(self)->float:
+        """
+        Get the last learning rate.
+
+        Returns
+        -------
+        float
+            The last learning rate.
+        """
+        return self.lambda_lr.get_last_lr()
+
+
+    # `transformers.optimization.get_cosine_schedule_with_warmup` will import tensorflow,
+    # resulting in some package version issues.
+    # Here we copy the code from transformers.optimization
+    def _get_cosine_schedule_with_warmup_lr_lambda(self,
+        current_step: int, *, num_warmup_steps: int, num_training_steps: int, num_cycles: float
+    ):
+        if current_step < num_warmup_steps:
+            return float(current_step+1) / float(max(1, num_warmup_steps))
+
+        progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
+        return max(1e-10, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
+
+
+
+    def get_cosine_schedule_with_warmup( self,
+        optimizer, num_warmup_steps: int, num_training_steps: int, num_cycles: float = 0.5, last_epoch: int = -1
+    ):
+        """
+        Create a schedule with a learning rate that decreases following the values of the cosine function between the
+        initial lr set in the optimizer to 0, after a warmup period during which it increases linearly between 0 and the
+        initial lr set in the optimizer.
+
+        Args:
+            optimizer ([`~torch.optim.Optimizer`]):
+                The optimizer for which to schedule the learning rate.
+            num_warmup_steps (`int`):
+                The number of steps for the warmup phase.
+            num_training_steps (`int`):
+                The total number of training steps.
+            num_cycles (`float`, *optional*, defaults to 0.5):
+                The number of waves in the cosine schedule (the defaults is to just decrease from the max value to 0
+                following a half-cosine).
+            last_epoch (`int`, *optional*, defaults to -1):
+                The index of the last epoch when resuming training.
+
+        Return:
+            `torch.optim.lr_scheduler.LambdaLR` with the appropriate schedule.
+        """
+
+        lr_lambda = functools.partial(
+            self._get_cosine_schedule_with_warmup_lr_lambda,
+            num_warmup_steps=num_warmup_steps,
+            num_training_steps=num_training_steps,
+            num_cycles=num_cycles,
+        )
+        return LambdaLR(optimizer, lr_lambda, last_epoch)
+
+class CallbackHandler:
+    """
+    A CallbackHandler class that can be used to add callbacks to the training process for both
+    epoch-level and batch-level events. To have more control over the training process, you can
+    create a subclass of this class and override the methods you need.
     """
+    def epoch_callback(self, epoch:int, epoch_loss:float) -> bool:
+        """
+        This method will be called at the end of each epoch. The callback can also be used to
+        stop the training by returning False. If the return value is None, or True, the training
+        will continue.
+
+        Parameters
+        ----------
+        epoch : int
+            The current epoch number.
+        epoch_loss : float
+            The loss value of the current epoch.
 
-    lr_lambda = functools.partial(
-        _get_cosine_schedule_with_warmup_lr_lambda,
-        num_warmup_steps=num_warmup_steps,
-        num_training_steps=num_training_steps,
-        num_cycles=num_cycles,
-    )
-    return LambdaLR(optimizer, lr_lambda, last_epoch)
+        Returns
+        -------
+        continue_training : bool
+            If False, the training will stop.
+        """
+        continue_training = True
+        return continue_training
+    def batch_callback(self, batch:int, batch_loss:float):
+        """
+        This method will be called at the end of each batch.
+
+        Parameters
+        ----------
+        batch : int
+            The current batch number.
+        batch_loss : float
+            The loss value of the current batch.
+
+        """
+        pass
 
 def append_nAA_column_if_missing(precursor_df):
     """
     Append a column containing the number of Amino Acids
     """
     if 'nAA' not in precursor_df.columns:
         precursor_df['nAA'] = precursor_df.sequence.str.len()
@@ -95,46 +203,48 @@
 
 class ModelInterface(object):
     """
     Provides standardized methods to interact
     with ml models. Inherit into new class and override
     the abstract (i.e. not implemented) methods.
     """
-    
+
     def __init__(self,
         device:str='gpu',
         fixed_sequence_len:int = 0,
         min_pred_value:float = 0.0,
         **kwargs
     ):
         """
         Parameters
         ----------
         device : str, optional
             device type in 'get_available', 'cpu', 'mps', 'gpu' (or 'cuda'),
             by default 'gpu'
-        
+
         fixed_sequence_len : int, optional
             See :attr:`fixed_sequence_len`, defaults to 0.
 
         min_pred_value : float, optional
             See :attr:`min_pred_value`, defaults to 0.0.
         """
         self.model:torch.nn.Module = None
         self.optimizer = None
         self.model_params:dict = {}
         self.set_device(device)
         self.fixed_sequence_len = fixed_sequence_len
         self.min_pred_value = min_pred_value
+        self.lr_scheduler_class = WarmupLR_Scheduler
+        self.callback_handler = CallbackHandler()
 
     @property
     def fixed_sequence_len(self)->int:
         """
         This attribute controls how to train and infer for variable-length sequences:
-        
+
         - if the value is 0, all sequence tensors will be grouped by nAA and train/infer on same nAA in batch.
         - if the value is > 0: all sequence tensors will be padded by zeros to the fixed length.
         - if the value is < 0: in each batch, padded by zeros to max length of the batch.
         """
         return self._fixed_sequence_len
 
     @fixed_sequence_len.setter
@@ -154,15 +264,15 @@
         self._min_pred_value = val
         self.model_params['min_pred_value'] = val
 
     @property
     def device_type(self)->str:
         """Read-only"""
         return self._device_type
-    
+
     @property
     def device(self)->torch.device:
         """Read-only"""
         return self._device
 
     @property
     def device_ids(self)->list:
@@ -181,50 +291,78 @@
     def target_column_to_train(self)->str:
         return self._target_column_to_train
 
     @target_column_to_train.setter
     def target_column_to_train(self, column:str):
         self._target_column_to_train = column
 
-    def set_device(self, 
-        device_type:str = 'gpu', 
+    def set_lr_scheduler_class(self, lr_scheduler_class:LR_SchedulerInterface) -> None:
+        """
+        Set the learning rate scheduler class. We require the user pass a class that is a subclass of
+        LR_SchedulerInterface because the current implementation will create an instance of it within this class.
+
+        Parameters
+        ----------
+        lr_scheduler_class : LR_SchedulerInterface
+            The learning rate scheduler class. Since we create an instance of it within this class,
+            the ModelInterface needs the class to take the arguments `optimizer`, `num_warmup_steps`, `num_training_steps`
+
+        """
+        if not issubclass(lr_scheduler_class, LR_SchedulerInterface):
+            raise ValueError(
+                "The lr_scheduler_class must be a subclass of LR_SchedulerInterface"
+            )
+        else:
+            self.lr_scheduler_class = lr_scheduler_class
+    def set_callback_handler(self, callback_handler:CallbackHandler) -> None:
+        """
+        Set the callback handler. It has to be a subclass of CallbackHandler.
+        """
+        if isinstance(callback_handler, CallbackHandler):
+            self.callback_handler = callback_handler
+        else:
+            raise ValueError(
+                "The callback handler passed must be a subclass of model_interface.CallbackHandler"
+            )
+    def set_device(self,
+        device_type:str = 'gpu',
         device_ids:list = []
     ):
         """
         Set the device (e.g. gpu (cuda), mps, cpu, ...) to be used for the model.
 
         Parameters
         ----------
         device_type : str, optional
             Device type, see :data:`peptdeep.utils.torch_device_dict`.
-            It will check available devices using 
-            :meth:`peptdeep.utils.get_available_device()` 
+            It will check available devices using
+            :meth:`peptdeep.utils.get_available_device()`
             if device_type=='get_available'.
             By default 'gpu'
 
         device_ids : list, optional
-            List of int. Device ids for cuda/gpu (e.g. [1,3] for cuda:1,3). 
+            List of int. Device ids for cuda/gpu (e.g. [1,3] for cuda:1,3).
             By default []
         """
         self._device_ids = device_ids
 
         if device_type == 'get_available':
             self._device, self._device_type = get_available_device()
         else:
             self._device, self._device_type = get_device(
                 device_type, device_ids
             )
 
         self._model_to_device()
 
     def _model_to_device(self):
-        """ 
+        """
         Enable multiple GPUs using torch.nn.DataParallel.
 
-        TODO It is better to use torch.nn.parallel.DistributedDataParallel, 
+        TODO It is better to use torch.nn.parallel.DistributedDataParallel,
         but this may need more setups for models and optimizers.
         """
         if self.model is None: return
         if self.device_type != 'cuda':
             self.model.to(self.device)
         else:
             if (
@@ -238,55 +376,55 @@
             self.model.to(self.device)
 
     def build(self,
         model_class: torch.nn.Module,
         **kwargs
     ):
         """
-        Builds the model by specifying the PyTorch module, 
+        Builds the model by specifying the PyTorch module,
         the parameters, the device, the loss function ...
         """
         self.model = model_class(**kwargs)
         self.model_params.update(**kwargs)
         self._model_to_device()
         self._init_for_training()
 
     def set_bert_trainable(self,
         bert_layer_name="hidden_nn",
         bert_layer_idxes=[1,2], # [0,1,2,3] in ms2 model
-        trainable=True,  
+        trainable=True,
     ):
         self.set_layer_trainable(
             layer_names=[
                 f"{bert_layer_name}.bert.layer.{layer}"
                 for layer in bert_layer_idxes
             ],
             trainable=trainable,
         )
 
-    def set_layer_trainable(self, 
+    def set_layer_trainable(self,
         layer_names=[],
-        trainable=True, 
+        trainable=True,
     ):
         for layer in layer_names:
             self.model.get_submodule(layer).requires_grad_(trainable)
 
     def train_with_warmup(self,
         precursor_df: pd.DataFrame,
         *,
-        batch_size=1024, 
-        epoch=10, 
+        batch_size=1024,
+        epoch=10,
         warmup_epoch=5,
         lr=1e-4,
         verbose=False,
         verbose_each_epoch=False,
         **kwargs
     ):
         """
-        Train the model according to specifications. Includes a warumup 
+        Train the model according to specifications. Includes a warumup
         phase with linear increasing and cosine decreasing for lr scheduling).
         """
         self._prepare_training(precursor_df, lr, **kwargs)
 
         lr_scheduler = self._get_lr_schedule_with_warmup(
             warmup_epoch, epoch
         )
@@ -301,26 +439,31 @@
             else:
                 batch_cost = self._train_one_epoch_by_padding_zeros(
                     precursor_df, epoch,
                     batch_size, verbose_each_epoch,
                     **kwargs
                 )
 
-            lr_scheduler.step()
+            lr_scheduler.step(epoch=epoch, loss=np.mean(batch_cost))
             if verbose: print(
                 f'[Training] Epoch={epoch+1}, lr={lr_scheduler.get_last_lr()[0]}, loss={np.mean(batch_cost)}'
             )
-        
+            continue_training = self.callback_handler.epoch_callback(
+                epoch=epoch, epoch_loss=np.mean(batch_cost)
+            )
+            if not continue_training:
+                print(f"Training stopped at epoch {epoch}")
+                break
         torch.cuda.empty_cache()
 
     def train(self,
         precursor_df: pd.DataFrame,
         *,
-        batch_size=1024, 
-        epoch=10, 
+        batch_size=1024,
+        epoch=10,
         warmup_epoch:int=0,
         lr=1e-4,
         verbose=False,
         verbose_each_epoch=False,
         **kwargs
     ):
         """
@@ -355,15 +498,21 @@
                 else:
                     batch_cost = self._train_one_epoch_by_padding_zeros(
                         precursor_df, epoch,
                         batch_size, verbose_each_epoch,
                         **kwargs
                     )
                 if verbose: print(f'[Training] Epoch={epoch+1}, Mean Loss={np.mean(batch_cost)}')
-            
+
+                continue_training = self.callback_handler.epoch_callback(
+                    epoch=epoch, epoch_loss=np.mean(batch_cost)
+                    )
+                if not continue_training:
+                    print(f"Training stopped at epoch {epoch}")
+                    break
             torch.cuda.empty_cache()
 
     def predict(self,
         precursor_df:pd.DataFrame,
         *,
         batch_size:int=1024,
         verbose:bool=False,
@@ -380,32 +529,32 @@
         self.model.eval()
 
         _grouped = precursor_df.groupby('nAA')
         if verbose:
             batch_tqdm = tqdm(_grouped)
         else:
             batch_tqdm = _grouped
-        with torch.no_grad():
+        with _inference_mode():
             for nAA, df_group in batch_tqdm:
                 for i in range(0, len(df_group), batch_size):
                     batch_end = i+batch_size
-                    
+
                     batch_df = df_group.iloc[i:batch_end,:]
 
                     features = self._get_features_from_batch_df(
                         batch_df, **kwargs
                     )
 
                     if isinstance(features, tuple):
                         predicts = self._predict_one_batch(*features)
                     else:
                         predicts = self._predict_one_batch(features)
 
                     self._set_batch_predict_data(
-                        batch_df, predicts, 
+                        batch_df, predicts,
                         **kwargs
                     )
 
         torch.cuda.empty_cache()
         return self.predict_df
 
     def predict_mp(self,
@@ -421,21 +570,21 @@
         Note this multiprocessing method only works for models those predict
         values within (inplace of) the precursor_df.
         """
         precursor_df = append_nAA_column_if_missing(precursor_df)
 
         if self.device_type != 'cpu':
             return self.predict(
-                precursor_df, 
+                precursor_df,
                 batch_size=batch_size,
                 verbose=True,
                 **kwargs
             )
-            
-        _predict_func = functools.partial(self.predict, 
+
+        _predict_func = functools.partial(self.predict,
             batch_size=batch_size, verbose=False, **kwargs
         )
 
         def batch_df_gen(precursor_df, mp_batch_size):
             for i in range(0, len(precursor_df), mp_batch_size):
                 yield precursor_df.iloc[i:i+mp_batch_size]
 
@@ -451,15 +600,15 @@
                     batch_df_gen(precursor_df, mp_batch_size),
                 ), len(precursor_df)//mp_batch_size+1
             ):
                 df_list.append(ret_df)
 
         self.predict_df = pd.concat(df_list)
         self.predict_df.reset_index(drop=True, inplace=True)
-        
+
         return self.predict_df
 
     def save(self, filename:str):
         """
         Save the model state, the constants used, the code defining the model and the model parameters.
         """
         # TODO save tf.keras.Model
@@ -500,15 +649,15 @@
     def build_from_py_codes(self,
         model_code_file_or_zip:str,
         code_file_in_zip:str=None,
         include_model_params_yaml:bool=True,
         **kwargs
     ):
         """
-        Build the model based on a python file. Must contain a PyTorch 
+        Build the model based on a python file. Must contain a PyTorch
         model implemented as 'class Model(...'
         """
         if model_code_file_or_zip.lower().endswith('.zip'):
             with ZipFile(model_code_file_or_zip, 'r') as model_zip:
                 with model_zip.open(code_file_in_zip,'r') as f:
                     codes = f.read()
                 if include_model_params_yaml:
@@ -522,15 +671,15 @@
                 codes = f.read()
             if include_model_params_yaml:
                 params = load_yaml(
                     model_code_file_or_zip[:-len('model.py')]+'param.yaml'
                 )
 
         compiled_codes = compile(
-            codes, 
+            codes,
             filename='model_file_py',
             mode='exec'
         )
         _module = ModuleType('_apd_nn_codes')
         #codes must contains torch model codes 'class Model(...'
         exec(compiled_codes, _module.__dict__)
 
@@ -547,28 +696,28 @@
     def _init_for_training(self):
         """
         Set the loss function, and more attributes for different tasks.
         The default loss function is nn.L1Loss.
         """
         self.loss_func = torch.nn.L1Loss()
 
-    def _as_tensor(self, 
-        data:np.ndarray, 
+    def _as_tensor(self,
+        data:np.ndarray,
         dtype:torch.dtype=torch.float32
     )->torch.Tensor:
         """Convert numerical np.array to pytorch tensor.
         The tensor will be stored in self.device
 
         Parameters
         ----------
         data : np.ndarray
             Numerical np.ndarray to be converted as a tensor
-            
+
         dtype : torch.dtype, optional
-            The dtype of the indices used for embedding should be `torch.long`. 
+            The dtype of the indices used for embedding should be `torch.long`.
             Defaults to `torch.float32`
 
         Returns
         -------
         torch.Tensor
             The tensor stored in self.device
         """
@@ -581,15 +730,15 @@
 
     def _load_model_from_pytorchfile(self, model_file):
         with open(model_file,'rb') as pt_file:
             self._load_model_from_stream(pt_file)
 
     def _load_model_from_stream(self, stream):
         (
-            missing_keys, unexpect_keys 
+            missing_keys, unexpect_keys
         ) = self.model.load_state_dict(torch.load(
             stream, map_location=self.device),
             strict=False
         )
         if len(missing_keys) > 0:
             logging.warn(f"nn parameters {missing_keys} are MISSING while loading models in {self.__class__}")
         if len(unexpect_keys) > 0:
@@ -603,16 +752,16 @@
             class_code = inspect.getsource(self.model.__class__)
             code += 'class Model' + class_code[class_code.find('('):]
             with open(save_as, 'w') as f:
                 f.write(code)
         except (TypeError, ValueError, KeyError) as e:
             logging.info(f'Cannot save model source codes: {str(e)}')
 
-    def _train_one_epoch_by_padding_zeros(self, 
-        precursor_df, epoch, batch_size, verbose_each_epoch, 
+    def _train_one_epoch_by_padding_zeros(self,
+        precursor_df, epoch, batch_size, verbose_each_epoch,
         **kwargs
     ):
         """Training for an epoch by padding zeros"""
         batch_cost = []
         rnd_df = precursor_df.sample(frac=1)
         if verbose_each_epoch:
             batch_tqdm = tqdm(range(0, len(rnd_df), batch_size))
@@ -632,23 +781,23 @@
                 batch_cost.append(
                     self._train_one_batch(targets, *features)
                 )
             else:
                 batch_cost.append(
                     self._train_one_batch(targets, features)
                 )
-                
+            self.callback_handler.batch_callback(i//batch_size, batch_cost[-1])
         if verbose_each_epoch:
             batch_tqdm.set_description(
                 f'Epoch={epoch+1}, batch={len(batch_cost)}, loss={batch_cost[-1]:.4f}'
             )
         return batch_cost
 
-    def _train_one_epoch(self, 
-        precursor_df, epoch, batch_size, verbose_each_epoch, 
+    def _train_one_epoch(self,
+        precursor_df, epoch, batch_size, verbose_each_epoch,
         **kwargs
     ):
         """Training for an epoch"""
         batch_cost = []
         _grouped = list(precursor_df.sample(frac=1).groupby('nAA'))
         rnd_nAA = np.random.permutation(len(_grouped))
         if verbose_each_epoch:
@@ -672,24 +821,24 @@
                     batch_cost.append(
                         self._train_one_batch(targets, *features)
                     )
                 else:
                     batch_cost.append(
                         self._train_one_batch(targets, features)
                     )
-                
+                self.callback_handler.batch_callback(i//batch_size, batch_cost[-1])
             if verbose_each_epoch:
                 batch_tqdm.set_description(
                     f'Epoch={epoch+1}, nAA={nAA}, batch={len(batch_cost)}, loss={batch_cost[-1]:.4f}'
                 )
         return batch_cost
 
     def _train_one_batch(
-        self, 
-        targets:torch.Tensor, 
+        self,
+        targets:torch.Tensor,
         *features,
     ):
         """Training for a mini batch"""
         self.optimizer.zero_grad()
         predicts = self.model(*features)
         cost = self.loss_func(predicts, targets)
         cost.backward()
@@ -719,83 +868,83 @@
 
         Returns
         -------
         torch.Tensor
             Target value tensor
         """
         return self._as_tensor(
-            batch_df[self.target_column_to_train].values, 
+            batch_df[self.target_column_to_train].values,
             dtype=torch.float32
         )
 
     def _get_aa_indice_features_padding_zeros(
         self, batch_df:pd.DataFrame
     )->torch.LongTensor:
         """
-        Get indices values of variable length sequences 
+        Get indices values of variable length sequences
         using 128 ascii codes
         """
         if self.fixed_sequence_len < 0:
             max_len = batch_df.nAA.max()
         else:
             max_len = self.fixed_sequence_len
         return self._as_tensor(
             get_ascii_indices(
                 batch_df['sequence'].apply(
                     lambda seq: seq + chr(0)*(max_len-len(seq))
                 ).values.astype('U')
-            ), 
+            ),
             dtype=torch.long
         )
 
     def _get_aa_indice_features(
         self, batch_df:pd.DataFrame
     )->torch.LongTensor:
         """
-        Get indices values for fixed length sequences 
+        Get indices values for fixed length sequences
         with 128 ascii codes.
         """
         return self._as_tensor(
             get_ascii_indices(
                 batch_df['sequence'].values.astype('U')
-            ), 
+            ),
             dtype=torch.long
         )
 
     def _get_26aa_indice_features(
         self, batch_df:pd.DataFrame
     )->torch.LongTensor:
         """
-        Get indices values for 26 upper-case letters (amino acids), 
+        Get indices values for 26 upper-case letters (amino acids),
         from 1 to 26. 0 is used for padding.
         """
         return self._as_tensor(
             get_batch_aa_indices(
                 batch_df['sequence'].values.astype('U')
-            ), 
+            ),
             dtype=torch.long
         )
-        
+
     def _get_features_from_batch_df(self,
         batch_df:pd.DataFrame, **kwargs,
     )->Union[torch.LongTensor, Tuple[torch.Tensor]]:
         """
         Any sub-class must re-implement this method:
-        
-        - Return `self._get_aa_features()` for sequence-level prediciton 
+
+        - Return `self._get_aa_features()` for sequence-level prediciton
         - Return `self._get_aa_mod_features()` for modified sequence-level
 
         Parameters
         ----------
         batch_df : pd.DataFrame
             Batch of precursor dataframe.
 
         Returns
         -------
-        Union[torch.LongTensor, Tuple[torch.Tensor]]: 
+        Union[torch.LongTensor, Tuple[torch.Tensor]]:
             A LongTensor if the sub-class call `self._get_aa_features(batch_df)` (default).
             Or a tuple of tensors if call `self._get_aa_mod_features(batch_df)`.
         """
         return self._get_aa_features(batch_df)
 
     def _get_aa_mod_features(self,
         batch_df:pd.DataFrame, **kwargs,
@@ -814,39 +963,39 @@
         if self.fixed_sequence_len < 0:
             batch_df = batch_df.copy()
             batch_df['nAA'] = batch_df.nAA.max()
         return self._as_tensor(
             get_batch_mod_feature(batch_df)
         )
 
-    def _get_aa_features(self, 
+    def _get_aa_features(self,
         batch_df:pd.DataFrame
     )->torch.LongTensor:
         """
         Get AA indices
         """
         if self.fixed_sequence_len == 0:
             return self._get_aa_indice_features(batch_df)
         else:
             return self._get_aa_indice_features_padding_zeros(batch_df)
 
     def _prepare_predict_data_df(self,
-        precursor_df:pd.DataFrame, 
+        precursor_df:pd.DataFrame,
         **kwargs
     ):
         """
-        This methods fills 0s in the column of 
+        This methods fills 0s in the column of
         `self.target_column_to_predict` in `precursor_df`,
         and then does `self.predict_df=precursor_df`.
         """
         precursor_df[self.target_column_to_predict] = 0.0
         self.predict_df = precursor_df
 
     def _prepare_train_data_df(self,
-        precursor_df:pd.DataFrame, 
+        precursor_df:pd.DataFrame,
         **kwargs
     ):
         """Changes to the training dataframe can be implemented here.
 
         Parameters
         ----------
         precursor_df : pd.DataFrame
@@ -892,40 +1041,49 @@
         else:
             for g in self.optimizer.param_groups:
                 g['lr'] = lr
 
     def _get_lr_schedule_with_warmup(self, warmup_epoch, epoch):
         if warmup_epoch > epoch:
             warmup_epoch = epoch//2
-        return get_cosine_schedule_with_warmup(
-            self.optimizer, warmup_epoch, epoch
+        return self.lr_scheduler_class(
+            self.optimizer,
+            num_warmup_steps=warmup_epoch,
+            num_training_steps=epoch
         )
 
     def _pad_zeros_if_fixed_len(self, precursor_df:pd.DataFrame):
         if self.fixed_sequence_len > 0:
             precursor_df.drop(
                 index=precursor_df[
                     precursor_df.nAA>self.fixed_sequence_len
-                ].index, 
+                ].index,
                 inplace=True,
             )
             precursor_df.reset_index(drop=True, inplace=True)
             precursor_df['nAA'] = self.fixed_sequence_len
 
-    def _prepare_training(self, 
-        precursor_df:pd.DataFrame, 
-        lr:float, 
+    def _prepare_training(self,
+        precursor_df:pd.DataFrame,
+        lr:float,
         **kwargs
     ):
         if 'nAA' not in precursor_df.columns:
             precursor_df['nAA'] = precursor_df.sequence.str.len()
         self._pad_zeros_if_fixed_len(precursor_df)
         self._prepare_train_data_df(precursor_df, **kwargs)
         self.model.train()
 
         self.set_lr(lr)
 
     def _check_predict_in_order(self, precursor_df:pd.DataFrame):
-        if is_precursor_sorted(precursor_df):
+        if is_precursor_refined(precursor_df):
             self._predict_in_order = True
         else:
             self._predict_in_order = False
+
+def _inference_mode():
+    # torch.inference_mode() only available in torch>=1.9.0
+    if float(torch.__version__[:torch.__version__.rfind(".")]) >= 1.9:
+        return torch.inference_mode()
+    else:
+        return torch.no_grad()
```

### Comparing `peptdeep-1.1.9/peptdeep/model/ms2.py` & `peptdeep-1.2.0/peptdeep/model/ms2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 import warnings
 
 from typing import List, Tuple, IO
 
 from tqdm import tqdm
 
 from alphabase.peptide.fragment import (
-    init_fragment_by_precursor_dataframe, 
-    update_sliced_fragment_dataframe, 
-    get_sliced_fragment_dataframe, 
+    init_fragment_by_precursor_dataframe,
+    update_sliced_fragment_dataframe,
+    get_sliced_fragment_dataframe,
     get_charged_frag_types
 )
 
 from peptdeep.utils import get_available_device
 
 from peptdeep.model.featurize import (
-    get_batch_aa_indices, parse_instrument_indices, 
+    get_batch_aa_indices, parse_instrument_indices,
     get_batch_mod_feature
 )
 
 from peptdeep.settings import (
-    global_settings as settings, 
+    global_settings as settings,
     model_const
 )
 
 import peptdeep.model.model_interface as model_interface
 import peptdeep.model.building_block as building_block
 
 class ModelMS2Transformer(torch.nn.Module):
@@ -80,15 +80,15 @@
             hidden, nlayers=nlayers, dropout=dropout
         )
 
         self.output_nn = building_block.Decoder_Linear(
             hidden,
             self._num_non_modloss,
         )
-        
+
         if num_modloss_types > 0:
             # for transfer learning of modloss frags
             self.modloss_nn = torch.nn.ModuleList([
                 building_block.Hidden_Transformer(
                     hidden, nlayers=1, dropout=dropout
                 ),
                 building_block.Decoder_Linear(
@@ -173,15 +173,15 @@
             output_attentions=output_attentions
         )
 
         self.output_nn = building_block.Decoder_Linear(
             hidden,
             self._num_non_modloss,
         )
-        
+
         if num_modloss_types > 0:
             # for transfer learning of modloss frags
             self.modloss_nn = torch.nn.ModuleList([
                 building_block.Hidden_HFace_Transformer(
                     hidden, nlayers=1, dropout=dropout,
                     output_attentions=output_attentions
                 ),
@@ -191,15 +191,15 @@
             ])
         else:
             self.modloss_nn = None
 
     @property
     def output_attentions(self):
         return self._output_attentions
-        
+
     @output_attentions.setter
     def output_attentions(self, val:bool):
         self._output_attentions = val
         self.hidden_nn.output_attentions = val
         self.modloss_nn[0].output_attentions = val
 
     def forward(self,
@@ -273,28 +273,28 @@
         BiRNN = True
         hidden=512
         hidden_rnn_layer=2
 
         self.input_nn = building_block.InputAALSTM_cat_Meta(hidden)
 
         self.hidden_nn = building_block.SeqLSTM(
-            hidden, hidden, rnn_layer=hidden_rnn_layer, 
+            hidden, hidden, rnn_layer=hidden_rnn_layer,
             bidirectional=BiRNN
         )
 
         self.output_nn = building_block.OutputLSTM_cat_Meta(
             hidden,
             self._num_non_modloss,
         )
 
         if num_modloss_types:
             # for transfer learning of modloss frags
             self.modloss_nn = torch.nn.ModuleList([
                 building_block.SeqLSTM(
-                    hidden, hidden, 
+                    hidden, hidden,
                     rnn_layer=1, bidirectional=BiRNN
                 ),
                 building_block.SeqLSTM(
                     hidden, num_modloss_types,
                     rnn_layer=1, bidirectional=False
                 ),
             ])
@@ -306,24 +306,24 @@
         mod_x,
         charges:torch.Tensor,
         NCEs:torch.Tensor,
         instrument_indices,
     ):
 
         in_x = self.input_nn(
-            aa_indices, mod_x, 
+            aa_indices, mod_x,
             charges, NCEs, instrument_indices
         )
         in_x = self.dropout(in_x)
 
         hidden_x = self.hidden_nn(in_x)
         hidden_x = self.dropout(hidden_x)
 
         out_x = self.output_nn(
-            hidden_x, 
+            hidden_x,
             charges, NCEs, instrument_indices
         )
 
         # modloss is mainly only for Phospho@S/T
         if self._num_modloss_types > 0:
             if self._mask_modloss:
                 out_x = torch.cat((out_x, torch.zeros(
@@ -379,15 +379,15 @@
         self.charged_frag_types = charged_frag_types
         self._get_modloss_frags(modloss_type)
 
         self.charge_factor = 0.1
         self.NCE_factor = 0.01
         self.model:ModelMS2Bert = None
         self.build(
-            model_class, 
+            model_class,
             num_frag_types = len(self.charged_frag_types),
             num_modloss_types = len(self._modloss_frag_types),
             mask_modloss=mask_modloss,
             dropout=dropout,
             **kwargs, # other model params
         )
 
@@ -396,15 +396,15 @@
 
     def _get_modloss_frags(self, modloss='modloss'):
         self._modloss_frag_types = []
         for i,frag in enumerate(self.charged_frag_types):
             if modloss in frag:
                 self._modloss_frag_types.append(i)
 
-    def _prepare_train_data_df(self, 
+    def _prepare_train_data_df(self,
         precursor_df:pd.DataFrame,
         fragment_intensity_df:pd.DataFrame=None,
     ):
         self.frag_inten_df = fragment_intensity_df[self.charged_frag_types]
         # if np.all(precursor_df['nce'].values > 1):
         #     precursor_df['nce'] = precursor_df['nce']*self.NCE_factor
 
@@ -413,34 +413,34 @@
 
     def _prepare_predict_data_df(self,
         precursor_df:pd.DataFrame,
         reference_frag_df:pd.DataFrame=None,
     ):
         if reference_frag_df is None and precursor_df.nAA.is_monotonic_increasing:
             self._predict_in_order = True
-            
+
             if 'frag_start_idx' in precursor_df.columns:
                 precursor_df.drop(
                     columns=['frag_start_idx','frag_stop_idx'],
                     inplace=True
                 )
         else:
             self._predict_in_order = False
-        
+
         self.predict_df = init_fragment_by_precursor_dataframe(
-            precursor_df, self.charged_frag_types, 
-            reference_fragment_df=reference_frag_df, 
+            precursor_df, self.charged_frag_types,
+            reference_fragment_df=reference_frag_df,
             dtype=np.float32
         )
 
         # if np.all(precursor_df['nce'].values > 1):
         #     precursor_df['nce'] = precursor_df['nce']*self.NCE_factor
 
-    def _get_features_from_batch_df(self, 
-        batch_df: pd.DataFrame, 
+    def _get_features_from_batch_df(self,
+        batch_df: pd.DataFrame,
         **kwargs,
     ) -> Tuple[torch.Tensor]:
         aa_indices = self._get_26aa_indice_features(batch_df)
 
         mod_x = self._get_mod_features(batch_df)
 
         charges = self._as_tensor(
@@ -453,43 +453,43 @@
 
         instrument_indices = self._as_tensor(
             parse_instrument_indices(batch_df['instrument']),
             dtype=torch.long
         )
         return aa_indices, mod_x, charges, nces, instrument_indices
 
-    def _get_targets_from_batch_df(self, 
+    def _get_targets_from_batch_df(self,
         batch_df: pd.DataFrame,
         fragment_intensity_df:pd.DataFrame=None
     ) -> torch.Tensor:
         return self._as_tensor(
             get_sliced_fragment_dataframe(
-                fragment_intensity_df, 
+                fragment_intensity_df,
                 batch_df[
                     ['frag_start_idx','frag_stop_idx']
                 ].values
             ).values
-        ).view(-1, 
-            batch_df.nAA.values[0]-1, 
+        ).view(-1,
+            batch_df.nAA.values[0]-1,
             len(self.charged_frag_types)
         )
 
-    def _set_batch_predict_data(self, 
-        batch_df: pd.DataFrame, 
+    def _set_batch_predict_data(self,
+        batch_df: pd.DataFrame,
         predicts:np.ndarray,
         **kwargs,
     ):
         apex_intens = predicts.reshape((len(batch_df), -1)).max(axis=1)
         apex_intens[apex_intens<=0] = 1
         predicts /= apex_intens.reshape((-1,1,1))
         predicts[predicts<self.min_inten] = 0.0
         if self._predict_in_order:
             self.predict_df.values[
                 batch_df.frag_start_idx.values[0]:
-                batch_df.frag_stop_idx.values[-1], 
+                batch_df.frag_stop_idx.values[-1],
             :] = predicts.reshape(
                     (-1, len(self.charged_frag_types))
                 )
         else:
             update_sliced_fragment_dataframe(
                 self.predict_df,
                 self.predict_df.to_numpy(copy=True),
@@ -498,109 +498,109 @@
                 ),
                 batch_df[
                     ['frag_start_idx','frag_stop_idx']
                 ].values,
             )
 
     def train_with_warmup(self,
-        precursor_df: pd.DataFrame, 
-        fragment_intensity_df, 
-        *, 
-        batch_size=1024, 
+        precursor_df: pd.DataFrame,
+        fragment_intensity_df,
+        *,
+        batch_size=1024,
         epoch=10,
         warmup_epoch=5,
         lr = 1e-5,
-        verbose=False, 
+        verbose=False,
         verbose_each_epoch=False,
         **kwargs
     ):
         return super().train_with_warmup(
-            precursor_df, 
+            precursor_df,
             fragment_intensity_df=fragment_intensity_df,
-            batch_size=batch_size, 
+            batch_size=batch_size,
             epoch=epoch,
             warmup_epoch=warmup_epoch,
             lr=lr,
-            verbose=verbose, 
+            verbose=verbose,
             verbose_each_epoch=verbose_each_epoch,
             **kwargs
         )
-    
-    def test(self, 
+
+    def test(self,
         precursor_df:pd.DataFrame,
         fragment_intensity_df:pd.DataFrame,
         default_instrument:str = "Lumos",
         default_nce:float = 30.0,
     )->pd.DataFrame:
         if "instrument" not in precursor_df.columns:
             precursor_df["instrument"] = default_instrument
         if "nce" not in precursor_df.columns:
             precursor_df["nce"] = default_nce
         columns = np.intersect1d(
             self.charged_frag_types,
             fragment_intensity_df.columns.values,
         )
         return calc_ms2_similarity(
-            precursor_df, 
+            precursor_df,
             self.predict(
                 precursor_df, reference_frag_df=fragment_intensity_df
-            )[columns], 
+            )[columns],
             fragment_intensity_df=fragment_intensity_df[columns]
         )[-1]
 
-    def train(self, 
-        precursor_df: pd.DataFrame, 
-        fragment_intensity_df, 
-        *, 
-        batch_size=1024, 
+    def train(self,
+        precursor_df: pd.DataFrame,
+        fragment_intensity_df,
+        *,
+        batch_size=1024,
         epoch=20,
         warmup_epoch=0,
         lr = 1e-5,
-        verbose=False, 
+        verbose=False,
         verbose_each_epoch=False,
         **kwargs
     ):
         return super().train(
-            precursor_df, 
+            precursor_df,
             fragment_intensity_df=fragment_intensity_df,
-            batch_size=batch_size, 
-            epoch=epoch, 
+            batch_size=batch_size,
+            epoch=epoch,
             warmup_epoch=warmup_epoch,
             lr=lr,
-            verbose=verbose, 
+            verbose=verbose,
             verbose_each_epoch=verbose_each_epoch,
             **kwargs
         )
 
-    def predict(self, 
-        precursor_df: pd.DataFrame, 
-        *, 
-        batch_size=1024, 
-        verbose=False, 
+    def predict(self,
+        precursor_df: pd.DataFrame,
+        *,
+        batch_size=1024,
+        verbose=False,
         reference_frag_df=None,
         **kwargs
     ) -> pd.DataFrame:
         return super().predict(
-            precursor_df, 
-            batch_size=batch_size, 
-            verbose=verbose, 
-            reference_frag_df=reference_frag_df, 
+            precursor_df,
+            batch_size=batch_size,
+            verbose=verbose,
+            reference_frag_df=reference_frag_df,
             **kwargs
         )
 
-    def predict_mp(self, 
+    def predict_mp(self,
         **kwargs
     ) -> pd.DataFrame:
         warnings.warn(
             "Please use pretrained_models.ModelManager::predict_all() "
             "for MS2 prediction with multiprocessing"
         )
 
-    def bootstrap_nce_search(self, 
-        psm_df:pd.DataFrame, 
+    def bootstrap_nce_search(self,
+        psm_df:pd.DataFrame,
         fragment_intensity_df:pd.DataFrame,
         nce_first=15, nce_last=45, nce_step=3,
         instrument = 'Lumos',
         charged_frag_types:List = None,
         metric = 'PCC>0.9', # or 'median PCC'
         max_psm_subset = 3000,
         n_bootstrap = 3,
@@ -616,15 +616,15 @@
                 metric, max_psm_subset, n_bootstrap,
                 callback
             )
             nce_list.append(nce)
         return np.median(nce_list), instrument
 
     def grid_nce_search(self,
-        psm_df:pd.DataFrame, 
+        psm_df:pd.DataFrame,
         fragment_intensity_df:pd.DataFrame,
         nce_first=15, nce_last=45, nce_step=3,
         search_instruments = ['Lumos'],
         charged_frag_types:List = None,
         metric = 'PCC>0.9', # or 'median PCC'
         max_psm_subset = 1000000,
         callback = None
@@ -643,45 +643,45 @@
             for inst in search_instruments
         ])
         for inst in search_instruments:
             for nce in np.arange(nce_first, nce_last+nce_step, nce_step):
                 psm_df['nce'] = nce
                 psm_df['instrument'] = inst
                 predict_inten_df = self.predict(
-                    psm_df, 
+                    psm_df,
                     reference_frag_df=fragment_intensity_df
                 )
                 df, metrics = calc_ms2_similarity(
                     psm_df,
-                    predict_inten_df, 
+                    predict_inten_df,
                     fragment_intensity_df,
                     charged_frag_types=charged_frag_types,
                     metrics=['PCC']
                 )
                 pcc = metrics.loc[metric_row, 'PCC']
                 if pcc > best_pcc:
                     best_pcc = pcc
                     best_nce = nce
                     best_instrument = inst
         return best_nce, best_instrument
 
 
 def normalize_fragment_intensities(
-    psm_df:pd.DataFrame, 
+    psm_df:pd.DataFrame,
     frag_intensity_df:pd.DataFrame
 ):
     """Normalize the intensities to 0-1 values inplace
 
     Parameters
     ----------
     psm_df : pd.DataFrame
         PSM DataFrame
 
     frag_intensity_df : pd.DataFrame
-        Fragment intensity DataFrame to be normalized. 
+        Fragment intensity DataFrame to be normalized.
         Intensities will be normalzied inplace.
     """
     frag_intensity_df_np = frag_intensity_df.to_numpy()
     for i, (frag_start_idx, frag_stop_idx) in enumerate(
         psm_df[['frag_start_idx','frag_stop_idx']].values
     ):
         intens = frag_intensity_df_np[frag_start_idx:frag_stop_idx]
@@ -741,15 +741,15 @@
 
     y : torch.Tensor
         Shape (Batch, n)
 
     """
     x_rank = _get_ranks(x, device).to(torch.float32)
     y_rank = _get_ranks(y, device).to(torch.float32)
-    
+
     n = x.size(1)
     upper = 6 * torch.sum((x_rank - y_rank).pow(2), dim=1)
     down = n * (n ** 2 - 1.0)
     return 1.0 - (upper / down)
 
 #legacy
 spearman = spearman_correlation
@@ -789,34 +789,34 @@
     else:
         batch_tqdm = _grouped
 
     for met in metrics:
         psm_df[met] = 0.0
 
     for nAA, df_group in batch_tqdm:
-        for i in range(0, len(df_group), batch_size):   
+        for i in range(0, len(df_group), batch_size):
             batch_end = i+batch_size
             batch_df = df_group.iloc[i:batch_end,:]
 
             pred_intens = torch.tensor(
                 get_sliced_fragment_dataframe(
-                    predict_intensity_df, 
+                    predict_intensity_df,
                     batch_df[
                         ['frag_start_idx','frag_stop_idx']
                     ].values,
                     charged_frag_types
                 ).values,
                 dtype=torch.float32, device=device
             ).reshape(
                 -1, (nAA-1)*len(charged_frag_types)
             )
 
             frag_intens = torch.tensor(
                 get_sliced_fragment_dataframe(
-                    fragment_intensity_df, 
+                    fragment_intensity_df,
                     batch_df[
                         ['frag_start_idx','frag_stop_idx']
                     ].values,
                     charged_frag_types
                 ).values,
                 dtype=torch.float32, device=device
             ).reshape(
@@ -831,15 +831,15 @@
             if 'COS' in metrics or 'SA' in metrics:
                 cos = torch.cosine_similarity(
                     pred_intens, frag_intens, dim=1
                 )
                 psm_df.loc[
                     batch_df.index,'COS'
                 ] = cos.cpu().detach().numpy()
-                
+
                 if 'SA' in metrics:
                     psm_df.loc[
                         batch_df.index,'SA'
                     ] = spectral_angle(
                         cos
                     ).cpu().detach().numpy()
```

### Comparing `peptdeep-1.1.9/peptdeep/model/rt.py` & `peptdeep-1.2.0/peptdeep/model/rt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import pandas as pd
 import numpy as np
 
 from peptdeep.model.featurize import (
-    get_batch_aa_indices, 
+    get_batch_aa_indices,
     get_batch_mod_feature
 )
 
 from peptdeep.settings import model_const
 
 import peptdeep.model.model_interface as model_interface
 import peptdeep.model.building_block as building_block
@@ -48,15 +48,15 @@
         super().__init__()
 
         self.dropout = torch.nn.Dropout(dropout)
 
         self.input_nn = building_block.AATransformerEncoding(hidden)
 
         self._output_attentions = output_attentions
-        
+
         self.hidden_nn = building_block.Hidden_HFace_Transformer(
             hidden, nlayers=nlayers, dropout=dropout,
             output_attentions=output_attentions
         )
 
         self.output_nn = torch.nn.Sequential(
             building_block.SeqAttentionSum(hidden),
@@ -70,16 +70,16 @@
         return self._output_attentions
 
     @output_attentions.setter
     def output_attentions(self, val:bool):
         self._output_attentions = val
         self.hidden_nn.output_attentions = val
 
-    def forward(self, 
-        aa_indices, 
+    def forward(self,
+        aa_indices,
         mod_x,
     ):
         x = self.dropout(self.input_nn(
             aa_indices, mod_x
         ))
 
         hidden_x = self.hidden_nn(x)
@@ -90,46 +90,46 @@
         x = self.dropout(hidden_x[0]+x*0.2)
 
         return self.output_nn(x).squeeze(1)
 
 
 class Model_RT_LSTM_CNN(torch.nn.Module):
     """CNN+LSTM model for RT prediction"""
-    def __init__(self, 
+    def __init__(self,
         dropout=0.2,
     ):
         super().__init__()
-        
+
         self.dropout = torch.nn.Dropout(dropout)
-        
+
         hidden = 256
         self.rt_encoder = building_block.Encoder_26AA_Mod_CNN_LSTM_AttnSum(
             hidden
         )
 
         self.rt_decoder = building_block.Decoder_Linear(
             hidden, 1
         )
 
-    def forward(self, 
-        aa_indices, 
+    def forward(self,
+        aa_indices,
         mod_x,
     ):
         x = self.rt_encoder(aa_indices, mod_x)
         x = self.dropout(x)
 
         return self.rt_decoder(x).squeeze(1)
 #legacy
 Model_RT_LSTM = Model_RT_LSTM_CNN
 
 class AlphaRTModel(model_interface.ModelInterface):
     """
     `ModelInterface` for RT models
     """
-    def __init__(self, 
+    def __init__(self,
         dropout=0.1,
         model_class:torch.nn.Module=Model_RT_LSTM_CNN, #model defined above
         device:str='gpu',
         **kwargs,
     ):
         super().__init__(device=device)
         self.model:Model_RT_LSTM_CNN = None
@@ -137,27 +137,27 @@
             model_class,
             dropout=dropout,
             **kwargs
         )
         self.target_column_to_predict = 'rt_pred'
         self.target_column_to_train = 'rt_norm'
 
-    def test(self, 
-        precursor_df: pd.DataFrame, 
+    def test(self,
+        precursor_df: pd.DataFrame,
         *,
         batch_size:int = 1024,
     ):
         return evaluate_linear_regression(
             self.predict(
                 precursor_df, batch_size=batch_size
             ),
             x="rt_pred", y="rt_norm"
         )
 
-    def _get_features_from_batch_df(self, 
+    def _get_features_from_batch_df(self,
         batch_df: pd.DataFrame,
     ):
         return (
             self._get_26aa_indice_features(batch_df),
             self._get_mod_features(batch_df)
         )
 
@@ -182,9 +182,7 @@
         # slope = np.sum(x*y)/np.sum(x*x)
         # intercept = irt_mean - slope*rt_pred_mean
         # end linear regression
         slope = eval_df.slope.values[0]
         intercept = eval_df.intercept.values[0]
         precursor_df['irt_pred'] = precursor_df.rt_pred*slope + intercept
         return precursor_df
-
-
```

### Comparing `peptdeep-1.1.9/peptdeep/pipeline_api.py` & `peptdeep-1.2.0/peptdeep/pipeline_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,126 +1,123 @@
 import os
 import traceback
-import psutil
 
 import numpy as np
 import pandas as pd
 
 from typing import Tuple
 
 from alphabase.yaml_utils import save_yaml
-from alphabase.io.psm_reader import psm_reader_provider
+from alphabase.psm_reader import psm_reader_provider
 from alphabase.peptide.fragment import (
     get_charged_frag_types,
-    concat_precursor_fragment_dataframes
-)
-from alphabase.spectral_library.reader import (
-    LibraryReaderBase
+    concat_precursor_fragment_dataframes,
 )
+from alphabase.spectral_library.reader import LibraryReaderBase
 
 from peptdeep.spec_lib.translate import mod_to_unimod_dict
 from peptdeep.settings import global_settings, add_user_defined_modifications
-from peptdeep.utils import (
-    logging, set_logger, 
-    show_platform_info, show_python_info
-)
+from peptdeep.utils import logging, set_logger, show_platform_info, show_python_info
+
 # from peptdeep.rescore.percolator import Percolator
-from peptdeep.spec_lib.library_factory import (
-    library_maker_provider
-)
+from peptdeep.spec_lib.library_factory import library_maker_provider
 
 from peptdeep.pretrained_models import ModelManager
 
 # from peptdeep.rescore.feature_extractor import match_one_raw
 from alpharaw.match.psm_match import (
-    PepSpecMatch, PepSpecMatch_DIA, 
-    parse_ms_files_to_dict, get_ion_count_scores
+    PepSpecMatch,
+    PepSpecMatch_DIA,
+    parse_ms_files_to_dict,
+    get_ion_count_scores,
 )
 
 from peptdeep.model.ms2 import calc_ms2_similarity
 import peptdeep.model.rt as rt_module
 
 DIA_max_spec_per_query = 3
 DIA_min_ion_count = 6
 DIA_min_frag_mz = 200.0
 
+
 def _check_is_file(fname):
     if isinstance(fname, str) and not os.path.isfile(fname):
         logging.info(f" -- File `{fname}` does not exist.")
         return False
     else:
         return True
 
-def import_psm_df(psm_files:list, psm_type:str)->pd.DataFrame:
+
+def import_psm_df(psm_files: list, psm_type: str) -> pd.DataFrame:
     """Import PSM files of a search engine as a pd.DataFrame
 
     Parameters
     ----------
     psm_files : list
         List[str]. PSM file paths
-        
+
     psm_type : str
         PSM type or search engine name/type
 
     Returns
     -------
     pd.DataFrame
         DataFrame that contains all PSM information
     """
     psm_reader = psm_reader_provider.get_reader(
-        psm_type, 
-        modification_mapping=global_settings[
-            'model_mgr']['transfer'
-        ]['psm_modification_mapping']
+        psm_type,
+        modification_mapping=global_settings["model_mgr"]["transfer"][
+            "psm_modification_mapping"
+        ],
     )
     psm_df_list = []
     for psm_file in psm_files:
-        if not _check_is_file(psm_file): continue
+        if not _check_is_file(psm_file):
+            continue
         psm_reader.import_file(psm_file)
 
         psm_df_list.append(psm_reader.psm_df)
     return pd.concat(psm_df_list).reset_index(drop=True)
 
+
 def get_median_pccs_for_dia_psms(
-    psm_match:PepSpecMatch_DIA,
-    psm_df:pd.DataFrame, 
-    fragment_mz_df:pd.DataFrame,
-    fragment_intensity_df:pd.DataFrame,
+    psm_match: PepSpecMatch_DIA,
+    psm_df: pd.DataFrame,
+    fragment_mz_df: pd.DataFrame,
+    fragment_intensity_df: pd.DataFrame,
 ):
-    _frag_df = fragment_intensity_df.mask(
-        fragment_mz_df<psm_match.min_frag_mz, 0.0
-    )
-    frag_len = len(_frag_df)//psm_match.max_spec_per_query
-    psm_len = len(psm_match.psm_df)//psm_match.max_spec_per_query
+    _frag_df = fragment_intensity_df.mask(fragment_mz_df < psm_match.min_frag_mz, 0.0)
+    frag_len = len(_frag_df) // psm_match.max_spec_per_query
+    psm_len = len(psm_match.psm_df) // psm_match.max_spec_per_query
     _df = psm_match.psm_df.iloc[:psm_len].copy()
     median_pccs = np.zeros(len(psm_df))
     metrics_list = []
     for i in range(psm_match.max_spec_per_query):
         pcc_list = []
         for j in range(psm_match.max_spec_per_query):
-            if i == j: continue
-            _df,metrics_df = calc_ms2_similarity(
+            if i == j:
+                continue
+            _df, metrics_df = calc_ms2_similarity(
                 _df,
-                _frag_df[i*frag_len:(i+1)*frag_len],
-                _frag_df[j*frag_len:(j+1)*frag_len],
+                _frag_df[i * frag_len : (i + 1) * frag_len],
+                _frag_df[j * frag_len : (j + 1) * frag_len],
             )
             pcc_list.append(_df.PCC.values)
             metrics_list.append(metrics_df)
-        pccs = np.median(np.array(pcc_list),axis=0)
-        median_pccs[i*psm_len:(i+1)*psm_len] = pccs
+        pccs = np.median(np.array(pcc_list), axis=0)
+        median_pccs[i * psm_len : (i + 1) * psm_len] = pccs
 
     logging.info(
-        f"Average MS2 similarity metrics among {psm_match.max_spec_per_query} DIA scans at frag_mz>={psm_match.min_frag_mz}:\n" 
+        f"Average MS2 similarity metrics among {psm_match.max_spec_per_query} DIA scans at frag_mz>={psm_match.min_frag_mz}:\n"
         f"{str(sum(metrics_list)/len(metrics_list))}"
     )
     return median_pccs
 
-def match_psms()->Tuple[
-    pd.DataFrame,pd.DataFrame,pd.DataFrame
-]:
+
+def match_psms() -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     """
     Match the PSMs against the MS files.
 
     All required information is in global_settings:
     ```
     mgr_settings = global_settings['model_mgr']
     mgr_settings['transfer']['psm_files'] # list. PSM file paths
@@ -136,119 +133,121 @@
     Returns
     -------
     Tuple[pd.DataFrame,pd.DataFrame,pd.DataFrame]
         pd.DataFrame: the PSM DataFrame
         pd.DataFrame: the fragment mz DataFrame
         pd.DataFrame: the matched fragment intensity DataFrame
     """
-    mgr_settings = global_settings['model_mgr']
+    mgr_settings = global_settings["model_mgr"]
 
     frag_types = []
-    if mgr_settings['mask_modloss']:
-        for _type in global_settings['model']['frag_types']:
-            if 'modloss' not in _type:
+    if mgr_settings["mask_modloss"]:
+        for _type in global_settings["model"]["frag_types"]:
+            if "modloss" not in _type:
                 frag_types.append(_type)
     else:
-        frag_types = global_settings['model']['frag_types']
+        frag_types = global_settings["model"]["frag_types"]
 
-    max_charge = global_settings['model']['max_frag_charge']
+    max_charge = global_settings["model"]["max_frag_charge"]
     charged_frag_types = get_charged_frag_types(frag_types, max_charge)
 
     psm_df = import_psm_df(
-        mgr_settings['transfer']['psm_files'],
-        mgr_settings['transfer']['psm_type'],
+        mgr_settings["transfer"]["psm_files"],
+        mgr_settings["transfer"]["psm_type"],
     )
 
-    ms2_file_list:list = mgr_settings['transfer']['ms_files']
+    ms2_file_list: list = mgr_settings["transfer"]["ms_files"]
     for _ms_file in [f for f in ms2_file_list]:
         if not os.path.isfile(_ms_file):
-            logging.warn(f"`{_ms_file}` is invalid, please check the paths of `ms_files`")
+            logging.warn(
+                f"`{_ms_file}` is invalid, please check the paths of `ms_files`"
+            )
             ms2_file_list.remove(_ms_file)
 
     if (
-        mgr_settings['transfer']['psm_type'].lower()
-        in mgr_settings['transfer']['dda_psm_types'] 
+        mgr_settings["transfer"]["psm_type"].lower()
+        in mgr_settings["transfer"]["dda_psm_types"]
     ):
         psm_match = PepSpecMatch(
             charged_frag_types=charged_frag_types,
-            use_ppm=global_settings['peak_matching']['ms2_ppm'], 
-            tol_value=global_settings['peak_matching']['ms2_tol_value'],
+            use_ppm=global_settings["peak_matching"]["ms2_ppm"],
+            tol_value=global_settings["peak_matching"]["ms2_tol_value"],
         )
     else:
         psm_match = PepSpecMatch_DIA(
             charged_frag_types=charged_frag_types,
-            use_ppm=global_settings['peak_matching']['ms2_ppm'], 
-            tol_value=global_settings['peak_matching']['ms2_tol_value'],
+            use_ppm=global_settings["peak_matching"]["ms2_ppm"],
+            tol_value=global_settings["peak_matching"]["ms2_tol_value"],
         )
         psm_match.max_spec_per_query = DIA_max_spec_per_query
-        psm_match.min_frag_mz = global_settings["library"]["output_tsv"]["min_fragment_mz"]
+        psm_match.min_frag_mz = global_settings["library"]["output_tsv"][
+            "min_fragment_mz"
+        ]
 
     thread_num = global_settings["thread_num"]
     if len(ms2_file_list) > thread_num:
         psm_match.ms_loader_thread_num = 1
     else:
-        psm_match.ms_loader_thread_num = thread_num//len(ms2_file_list)
+        psm_match.ms_loader_thread_num = thread_num // len(ms2_file_list)
         thread_num = len(ms2_file_list)
 
-    ms2_file_dict = parse_ms_files_to_dict(
-        ms2_file_list
-    )
+    ms2_file_dict = parse_ms_files_to_dict(ms2_file_list)
 
     logging.info(
-        f"{len(ms2_file_dict)} MS files for fragment extraction: \n" +
-        "\n".join([
-            f"  - {raw_name} : {_path}" for raw_name, _path 
-            in ms2_file_dict.items()
-        ])
+        f"{len(ms2_file_dict)} MS files for fragment extraction: \n"
+        + "\n".join(
+            [f"  - {raw_name} : {_path}" for raw_name, _path in ms2_file_dict.items()]
+        )
         + "\n"
     )
 
-    psm_df = psm_df[
-        psm_df.raw_name.isin(ms2_file_dict)
-    ].reset_index(drop=True)
+    psm_df = psm_df[psm_df.raw_name.isin(ms2_file_dict)].reset_index(drop=True)
 
     logging.info(f"Loaded {len(psm_df)} PSMs for fragment extraction.")
 
     (
-        psm_df, frag_mz_df,
-        frag_inten_df, frag_mz_err_df,
+        psm_df,
+        frag_mz_df,
+        frag_inten_df,
+        frag_mz_err_df,
     ) = psm_match.match_ms2_multi_raw(
         psm_df=psm_df,
         ms_files=ms2_file_dict,
-        ms_file_type=mgr_settings['transfer']['ms_file_type'],
+        ms_file_type=mgr_settings["transfer"]["ms_file_type"],
         process_num=thread_num,
     )
 
     logging.info(f"Extracted {len(psm_df)} PSMs.")
 
     if isinstance(psm_match, PepSpecMatch_DIA):
         psm_df["ion_count"] = get_ion_count_scores(
-            frag_mz_df.values, frag_inten_df.values,
+            frag_mz_df.values,
+            frag_inten_df.values,
             psm_df.frag_start_idx.values,
             psm_df.frag_stop_idx.values,
             DIA_min_frag_mz,
         )
         if psm_match.max_spec_per_query > 1:
             psm_df["median_pcc"] = get_median_pccs_for_dia_psms(
-                psm_match, psm_df,
-                frag_mz_df, frag_inten_df
+                psm_match, psm_df, frag_mz_df, frag_inten_df
             )
             psm_df = psm_df.query(f"ion_count>={DIA_min_ion_count} and median_pcc>=0.9")
             logging.info(
                 f"Kept {len(psm_df)} PSMs at ion_count>={DIA_min_ion_count} "
-                 "and median_pcc>=0.9 for training/testing."
-                )
+                "and median_pcc>=0.9 for training/testing."
+            )
         else:
             psm_df = psm_df.query(f"ion_count>={DIA_min_ion_count}")
 
     return psm_df, frag_mz_df, frag_inten_df
 
+
 def transfer_learn(verbose=True):
     """Transfer learn / refine the RT/CCS(/MS2) models.
-    
+
     Required information in global_settings:
 
     ```python
     mgr_settings = global_settings['model_mgr']
     mgr_settings['transfer']['verbose'] = verbose # bool
     global_settings['PEPTDEEP_HOME'] # str. The folder to store all refined models. By default "~/peptdeep".
     ```
@@ -264,115 +263,110 @@
     global_settings['peak_matching']['ms2_ppm'] # bool. If use ppm as MS2 tolerance
     global_settings['peak_matching']['ms2_tol_value'] # float. MS2 tolerance value
     ```
 
     Parameters
     ----------
     verbose : bool
-        Print the training details. 
+        Print the training details.
         Optional, default True
 
     Raises
     ------
     Exception
         Any kinds of exception if the pipeline fails.
     """
     try:
         add_user_defined_modifications()
-        mgr_settings = global_settings['model_mgr']
-        mgr_settings['transfer']['verbose'] = verbose
+        mgr_settings = global_settings["model_mgr"]
+        mgr_settings["transfer"]["verbose"] = verbose
 
         output_folder = os.path.expanduser(
-            mgr_settings['transfer']['model_output_folder']
+            mgr_settings["transfer"]["model_output_folder"]
         )
         if not output_folder:
             output_folder = os.path.join(
-                os.path.expanduser(
-                    global_settings['PEPTDEEP_HOME']
-                ),
-                'transfer_models'
+                os.path.expanduser(global_settings["PEPTDEEP_HOME"]), "transfer_models"
             )
         if not os.path.exists(output_folder):
             os.makedirs(output_folder)
 
         set_logger(
-            log_file_name=os.path.join(output_folder, 'peptdeep_transfer.log'),
-            log_level=global_settings['log_level'],
-            overwrite=True, stream=True, 
+            log_file_name=os.path.join(output_folder, "peptdeep_transfer.log"),
+            log_level=global_settings["log_level"],
+            overwrite=True,
+            stream=True,
         )
         logging.info("[PeptDeep] Running train task ...")
         show_platform_info()
         show_python_info()
 
-        model_mgr:ModelManager = ModelManager()
+        model_mgr: ModelManager = ModelManager()
         model_mgr.reset_by_global_settings()
 
-        logging.info('Loading PSMs and extracting fragments ...')
-        
-        if (
-            mgr_settings['transfer']['psm_type'].lower() == 'speclib_tsv'
-        ):
+        logging.info("Loading PSMs and extracting fragments ...")
+
+        if mgr_settings["transfer"]["psm_type"].lower() == "speclib_tsv":
             dfs = []
             frag_inten_dfs = []
-            for psm_file in mgr_settings['transfer']['psm_files']:
+            for psm_file in mgr_settings["transfer"]["psm_files"]:
                 _lib = LibraryReaderBase(
-                    modification_mapping=mgr_settings[
-                        'transfer']['psm_modification_mapping'
+                    modification_mapping=mgr_settings["transfer"][
+                        "psm_modification_mapping"
                     ]
                 )
-                if not _check_is_file(psm_file): continue
+                if not _check_is_file(psm_file):
+                    continue
                 dfs.append(_lib.import_file(psm_file))
                 frag_inten_dfs.append(_lib.fragment_intensity_df)
-            psm_df, frag_df = concat_precursor_fragment_dataframes(
-                dfs, frag_inten_dfs
-            )
-        elif len(mgr_settings['transfer']['ms_files'])>0:
+            psm_df, frag_df = concat_precursor_fragment_dataframes(dfs, frag_inten_dfs)
+        elif len(mgr_settings["transfer"]["ms_files"]) > 0:
             psm_df, frag_mz_df, frag_df = match_psms()
         else:
             psm_df = import_psm_df(
-                mgr_settings['transfer']['psm_files'],
-                mgr_settings['transfer']['psm_type'],
+                mgr_settings["transfer"]["psm_files"],
+                mgr_settings["transfer"]["psm_type"],
             )
             frag_df = None
-        
+
         if model_mgr.psm_num_to_train_ms2 <= 0:
             frag_df = None
 
         logging.info(f"Loaded {len(psm_df)} PSMs for training and testing")
 
-        if "ccs" in psm_df.columns and (psm_df.ccs!=0).all():
+        if "ccs" in psm_df.columns and (psm_df.ccs != 0).all():
             logging.info("Training CCS model ...")
             model_mgr.train_ccs_model(psm_df)
             logging.info("Finished training CCS model")
 
         logging.info("Training RT model ...")
         model_mgr.train_rt_model(psm_df)
         logging.info("Finished training RT model")
 
-        if frag_df is not None and len(frag_df)>0:
+        if frag_df is not None and len(frag_df) > 0:
             logging.info("Training MS2 model ...")
             model_mgr.train_ms2_model(psm_df, frag_df)
             logging.info("Finished training MS2 model")
 
-        model_mgr.ccs_model.save(os.path.join(output_folder, 'ccs.pth'))
-        model_mgr.rt_model.save(os.path.join(output_folder, 'rt.pth'))
-        model_mgr.ms2_model.save(os.path.join(output_folder, 'ms2.pth'))
-        
+        model_mgr.ccs_model.save(os.path.join(output_folder, "ccs.pth"))
+        model_mgr.rt_model.save(os.path.join(output_folder, "rt.pth"))
+        model_mgr.ms2_model.save(os.path.join(output_folder, "ms2.pth"))
+
         save_yaml(
-            os.path.join(output_folder, 'peptdeep_settings.yaml'),
-            global_settings
+            os.path.join(output_folder, "peptdeep_settings.yaml"), global_settings
         )
         logging.info(f"Models were saved in {output_folder}")
     except Exception as e:
         logging.error(traceback.format_exc())
         raise e
 
+
 def generate_library():
     """Generate/predict a spectral library.
-    
+
     Required information in global_settings:
 
     ```python
     lib_settings = global_settings['library']
     output_folder = lib_settings['output_folder'] # str. Output folder of the library
     lib_settings['infile_type'] # str. Input type for the library, could be 'fasta', 'sequence', 'peptide', or 'precursor'
     lib_settings['infiles'] # list of str. Input files to generate librarys
@@ -381,88 +375,92 @@
     Raises
     ------
     Exception
         Any kinds of exception if the pipeline fails.
     """
     try:
         add_user_defined_modifications()
-        lib_settings = global_settings['library']
-        output_folder = os.path.expanduser(
-            lib_settings['output_folder']
-        )
+        lib_settings = global_settings["library"]
+        output_folder = os.path.expanduser(lib_settings["output_folder"])
         if not os.path.exists(output_folder):
             os.makedirs(output_folder)
         set_logger(
-            log_file_name=os.path.join(output_folder, 'peptdeep_library.log'),
-            log_level=global_settings['log_level'],
-            overwrite=True, stream=True, 
+            log_file_name=os.path.join(output_folder, "peptdeep_library.log"),
+            log_level=global_settings["log_level"],
+            overwrite=True,
+            stream=True,
         )
         logging.info("[PeptDeep] Running library task ...")
-        logging.info(f"Input files ({lib_settings['infile_type']}): " + str(lib_settings['infiles']))
+        logging.info(
+            f"Input files ({lib_settings['infile_type']}): "
+            + str(lib_settings["infiles"])
+        )
         show_platform_info()
         show_python_info()
 
-        model_mgr:ModelManager = ModelManager()
+        model_mgr: ModelManager = ModelManager()
         model_mgr.reset_by_global_settings()
 
         lib_maker = library_maker_provider.get_maker(
-            lib_settings['infile_type'],
-            model_manager=model_mgr
+            lib_settings["infile_type"], model_manager=model_mgr
         )
 
         if os.path.isfile(lib_settings["irt_library"]):
             logging.info(f"Use `{lib_settings['irt_library']}` to translate irt")
             irt_reader = psm_reader_provider.get_reader(
                 lib_settings["irt_library_type"],
-                modification_mapping=global_settings[
-                    'model_mgr']['transfer'
-                ]['psm_modification_mapping']
+                modification_mapping=global_settings["model_mgr"]["transfer"][
+                    "psm_modification_mapping"
+                ],
+            )
+            rt_module.IRT_PEPTIDE_DF = irt_reader.import_file(
+                lib_settings["irt_library"]
             )
-            rt_module.IRT_PEPTIDE_DF = irt_reader.import_file(lib_settings["irt_library"])
             rt_module.IRT_PEPTIDE_DF["irt"] = rt_module.IRT_PEPTIDE_DF["rt"]
         else:
-            logging.info(f"{lib_settings['irt_library']} does not exist, use default IRT_PEPTIDE_DF to translate irt")
+            logging.info(
+                f"{lib_settings['irt_library']} does not exist, use default IRT_PEPTIDE_DF to translate irt"
+            )
+
+        if (
+            lib_settings["infile_type"].lower()
+            in library_maker_provider.library_maker_dict
+        ):
+            lib_maker.make_library(lib_settings["infiles"])
+        else:  # PSMReaderLibraryMaker
+            lib_maker.make_library(
+                (lib_settings["infile_type"], lib_settings["infiles"])
+            )
 
-        if lib_settings['infile_type'].lower() in library_maker_provider.library_maker_dict:
-            lib_maker.make_library(lib_settings['infiles'])
-        else: # PSMReaderLibraryMaker
-            lib_maker.make_library((lib_settings['infile_type'],lib_settings['infiles']))
-        
         save_yaml(
-            os.path.join(output_folder, 'peptdeep_settings.yaml'),
-            global_settings
-        )
-        
-        hdf_path = os.path.join(
-            output_folder, 
-            'predict.speclib.hdf'
+            os.path.join(output_folder, "peptdeep_settings.yaml"), global_settings
         )
+
+        hdf_path = os.path.join(output_folder, "predict.speclib.hdf")
         logging.info(f"Saving HDF library to {hdf_path} ...")
         lib_maker.spec_lib.save_hdf(hdf_path)
-        if lib_settings['output_tsv']['enabled']:
-            tsv_path = os.path.join(
-                output_folder, 
-                'predict.speclib.tsv'
-            )
+        if lib_settings["output_tsv"]["enabled"]:
+            tsv_path = os.path.join(output_folder, "predict.speclib.tsv")
             lib_maker.translate_to_tsv(
-                tsv_path, 
-                translate_mod_dict=mod_to_unimod_dict 
-                if lib_settings['output_tsv']['translate_mod_to_unimod_id'] 
-                else None
+                tsv_path,
+                translate_mod_dict=mod_to_unimod_dict
+                if lib_settings["output_tsv"]["translate_mod_to_unimod_id"]
+                else None,
             )
         logging.info("Library generated!!")
     except Exception as e:
         logging.error(traceback.format_exc())
         raise e
 
+
 # def rescore():
 #     """Generate/predict a spectral library.
-    
+
 #     All required information in global_settings:
-    
+
 #     ```python
 #     perc_settings = global_settings['percolator']
 #     output_folder = perc_settings['output_folder'] # str. Output folder of the rescored results
 #     perc_settings['input_files']['psm_files'] # list of str. all PSM files (at 100% FDR and including decoys) from the search engines
 #     perc_settings['input_files']['psm_type'] # str. PSM or search engine type, e.g. pfind, alphapept, maxquant
 #     perc_settings['input_files']['ms_file_type'] # str. Could be alphapept_hdf, thermo, ...
 #     perc_settings['input_files']['ms_files'] # list of str. MS file list to match MS2 peaks
@@ -479,15 +477,15 @@
 #             perc_settings['output_folder']
 #         )
 #         if not os.path.exists(output_folder):
 #             os.makedirs(output_folder)
 #         set_logger(
 #             log_file_name=os.path.join(output_folder, 'peptdeep_rescore.log'),
 #             log_level=global_settings['log_level'],
-#             overwrite=True, stream=True, 
+#             overwrite=True, stream=True,
 #         )
 #         show_platform_info()
 #         show_python_info()
 
 #         model_mgr:ModelManager = ModelManager()
 #         model_mgr.reset_by_global_settings()
 #         percolator = Percolator(model_mgr=model_mgr)
@@ -497,29 +495,27 @@
 #         )
 
 #         ms_file_dict = parse_ms_file_names_to_dict(
 #             perc_settings['input_files']['ms_files']
 #         )
 
 #         psm_df = percolator.extract_features(
-#             psm_df, ms_file_dict, 
+#             psm_df, ms_file_dict,
 #             perc_settings['input_files']['ms_file_type']
 #         )
 
 #         df_fdr = psm_df[
 #             (psm_df.fdr<0.01)&(psm_df.decoy==0)
 #         ]
 #         df_fdr.to_csv(
-#             os.path.join(output_folder, 'peptdeep_fdr.tsv'), 
+#             os.path.join(output_folder, 'peptdeep_fdr.tsv'),
 #             sep='\t', index=False
 #         )
-        
+
 #         psm_df = percolator.re_score(psm_df)
 #         psm_df.to_csv(
-#             os.path.join(output_folder, 'peptdeep.tsv'), 
+#             os.path.join(output_folder, 'peptdeep.tsv'),
 #             sep='\t', index=False
 #         )
 #     except Exception as e:
 #         logging.error(traceback.format_exc())
 #         raise e
-
-
```

### Comparing `peptdeep-1.1.9/peptdeep/pretrained_models.py` & `peptdeep-1.2.0/peptdeep/pretrained_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 import torch.multiprocessing as mp
 if sys.platform.lower().startswith("linux"):
     # to prevent `too many open files` bug on Linux
     mp.set_sharing_strategy("file_system")
 
 from typing import Dict
 from zipfile import ZipFile
-from typing import Tuple, Union
+from typing import Union
 
 from alphabase.peptide.fragment import (
     create_fragment_mz_dataframe,
-    get_charged_frag_types,
     concat_precursor_fragment_dataframes
 )
 from alphabase.peptide.precursor import (
     refine_precursor_df,
     update_precursor_mz
 )
 from alphabase.peptide.mobility import (
@@ -77,19 +76,19 @@
 def download_models(
     url:str=model_url, overwrite=True
 ):
     """
     Parameters
     ----------
     url : str, optional
-        Remote or local path. 
+        Remote or local path.
         Defaults to `peptdeep.pretrained_models.model_url`
 
     overwrite : bool, optional
-        overwirte old model files. 
+        overwirte old model files.
         Defaults to True.
 
     Raises
     ------
     FileNotFoundError
         If remote url is not accessible.
     """
@@ -97,16 +96,16 @@
         logging.info(f'Downloading {model_zip_name} ...')
         try:
             context = ssl._create_unverified_context()
             requests = urllib.request.urlopen(url, context=context, timeout=10)
             with open(model_zip, 'wb') as f:
                 f.write(requests.read())
         except (
-            socket.timeout, 
-            urllib.error.URLError, 
+            socket.timeout,
+            urllib.error.URLError,
             urllib.error.HTTPError
         ) as e:
             raise FileNotFoundError(
                 'Downloading model failed! Please download the '
                 f'zip or tar file by yourself from "{url}",'
                 ' and use \n'
                 f'"peptdeep --install-model /path/to/{model_zip_name}.zip"\n'
@@ -130,16 +129,16 @@
     mod_dict = {}
     mod_dict['mutation'] = {}
     mod_dict['mutation']['spec_count'] = 0
     for one_mods in mods.values:
         for mod in set(one_mods):
             items = mod.split('->')
             if (
-                len(items)==2 
-                and len(items[0])==3 
+                len(items)==2
+                and len(items[0])==3
                 and len(items[1])==5
             ):
                 mod_dict['mutation']['spec_count'] += 1
             elif mod not in mod_dict:
                 mod_dict[mod] = {}
                 mod_dict[mod]['spec_count'] = 1
             else:
@@ -149,17 +148,17 @@
         ).reset_index(drop=False).rename(
             columns={'index':'mod'}
         ).sort_values(
             'spec_count',ascending=False
         ).reset_index(drop=True)
 
 def psm_sampling_with_important_mods(
-    psm_df, n_sample, 
+    psm_df, n_sample,
     top_n_mods = 10,
-    n_sample_each_mod = 0, 
+    n_sample_each_mod = 0,
     uniform_sampling_column = None,
     random_state=1337,
 ):
     psm_df_list = []
     if uniform_sampling_column is None:
         def _sample(psm_df, n):
             if n < len(psm_df):
@@ -231,42 +230,42 @@
     for col in fragment_mz_df.columns.values:
         if 'modloss' in col:
             fragment_intensity_df.loc[
                 fragment_mz_df[col]==0,col
             ] = 0
 
 class ModelManager(object):
-    """ 
+    """
     The manager class to access MS2/RT/CCS models.
-                
+
     Attributes
     ----------
     ms2_model : peptdeep.model.ms2.pDeepModel
         The MS2 prediction model.
 
     rt_model : peptdeep.model.rt.AlphaRTModel
         The RT prediction model.
 
     ccs_model : peptdeep.model.ccs.AlphaCCSModel
         The CCS prediciton model.
 
     psm_num_to_train_ms2 : int
-        Number of PSMs to train the MS2 model. 
+        Number of PSMs to train the MS2 model.
         Defaults to global_settings['model_mgr']['transfer']['psm_num_to_train_ms2'].
 
     epoch_to_train_ms2 : int
-        Number of epoches to train the MS2 model. 
+        Number of epoches to train the MS2 model.
         Defaults to global_settings['model_mgr']['transfer']['epoch_ms2'].
 
     psm_num_to_train_rt_ccs : int
-        Number of PSMs to train RT/CCS model. 
+        Number of PSMs to train RT/CCS model.
         Defaults to global_settings['model_mgr']['transfer']['psm_num_to_train_rt_ccs'].
 
     epoch_to_train_rt_ccs : int
-        Number of epoches to train RT/CCS model. 
+        Number of epoches to train RT/CCS model.
         Defaults to global_settings['model_mgr']['transfer']['epoch_rt_ccs'].
 
     nce : float
         Default NCE value for a precursor_df without the 'nce' column.
         Defaults to global_settings['model_mgr']['default_nce'].
 
     instrument : str
@@ -274,24 +273,24 @@
         Defaults to global_settings['model_mgr']['default_instrument'].
 
     use_grid_nce_search : bool
         If self.ms2_model uses `peptdeep.model.ms2.pDeepModel.grid_nce_search()` to determine optimal
         NCE and instrument type. This will change `self.nce` and `self.instrument` values.
         Defaults to global_settings['model_mgr']['transfer']['grid_nce_search'].
     """
-    def __init__(self, 
+    def __init__(self,
         mask_modloss:bool=False,
         device:str="gpu",
     ):
         """
         Parameters
         ----------
         mask_modloss : bool, optional
-            If modloss ions are masked to zeros in the ms2 model. `modloss` 
-            ions are mostly useful for phospho MS2 prediciton model. 
+            If modloss ions are masked to zeros in the ms2 model. `modloss`
+            ions are mostly useful for phospho MS2 prediciton model.
             Defaults to True.
 
         device : str, optional
             Device for DL models, could be 'gpu' ('cuda') or 'cpu'.
             if device=='gpu' but no GPUs are detected, it will automatically switch to 'cpu'.
             Defaults to 'gpu'
         """
@@ -326,15 +325,15 @@
             self.load_external_models(
                 ms2_model_file = mgr_settings['external_ms2_model'],
                 rt_model_file = mgr_settings['external_rt_model'],
                 ccs_model_file = mgr_settings['external_ccs_model'],
             )
 
             self.ms2_model.model._mask_modloss = global_settings['model_mgr']['mask_modloss']
-            
+
             device = global_settings['torch_device']['device_type']
             self.ms2_model.set_device(device)
             self.rt_model.set_device(device)
             self.ccs_model.set_device(device)
 
         self.use_grid_nce_search = mgr_settings[
             'transfer'
@@ -414,15 +413,15 @@
                 'instrument_group'
             ][instrument_name]
         else:
             self._instrument = 'Lumos'
 
     def set_default_nce_instrument(self, df):
         """
-        Append 'nce' and 'instrument' columns into df 
+        Append 'nce' and 'instrument' columns into df
         with self.nce and self.instrument
         """
         if 'nce' not in df.columns and 'instrument' not in df.columns:
             df['nce'] = float(self.nce)
             df['instrument'] = self.instrument
         elif 'nce' not in df.columns:
             df['nce'] = float(self.nce)
@@ -441,59 +440,61 @@
         folder : str
             folder to save
         """
         if os.path.isdir(folder):
             self.ms2_model.save(os.path.join(folder, 'ms2.pth'))
             self.rt_model.save(os.path.join(folder, 'rt.pth'))
             self.ccs_model.save(os.path.join(folder, 'ccs.pth'))
+            if self.charge_model is not None:
+                self.charge_model.save(os.path.join(folder, 'charge.pth'))
         elif not os.path.exists(folder):
             os.makedirs(folder)
             self.save_models(folder)
 
-    def load_installed_models(self, 
+    def load_installed_models(self,
         model_type:str='generic'
     ):
         """ Load built-in MS2/CCS/RT models.
-        
+
         Parameters
         ----------
         model_type : str, optional
-            To load the installed MS2/RT/CCS models or phos MS2/RT/CCS models. 
+            To load the installed MS2/RT/CCS models or phos MS2/RT/CCS models.
             It could be 'digly', 'phospho', 'HLA', or 'generic'.
             Defaults to 'generic'.
         """
         if model_type.lower() in [
             'phospho','phos','phosphorylation'
         ]:
             self.ms2_model.load(
                 model_zip,
                 model_path_in_zip='generic/ms2.pth'
             )
             self.rt_model.load(
-                model_zip, 
+                model_zip,
                 model_path_in_zip='phospho/rt_phos.pth'
             )
             self.ccs_model.load(
-                model_zip, 
+                model_zip,
                 model_path_in_zip='generic/ccs.pth'
             )
         elif model_type.lower() in [
-            'digly','glygly','ubiquitylation', 
+            'digly','glygly','ubiquitylation',
             'ubiquitination','ubiquitinylation'
         ]:
             self.ms2_model.load(
                 model_zip,
                 model_path_in_zip='generic/ms2.pth'
             )
             self.rt_model.load(
-                model_zip, 
+                model_zip,
                 model_path_in_zip='digly/rt_digly.pth'
             )
             self.ccs_model.load(
-                model_zip, 
+                model_zip,
                 model_path_in_zip='generic/ccs.pth'
             )
         elif model_type.lower() in ['regular','common','generic']:
             self.ms2_model.load(
                 model_zip, model_path_in_zip='generic/ms2.pth'
             )
             self.rt_model.load(
@@ -519,23 +520,23 @@
         ccs_model_file: Union[str, io.BytesIO]='',
     ):
         """Load external MS2/RT/CCS models.
 
         Parameters
         ----------
         ms2_model_file : Tuple[str, io.BytesIO], optional
-            MS2 model file or stream. Do nothing if the value is '' or None. 
+            MS2 model file or stream. Do nothing if the value is '' or None.
             Defaults to ''.
 
         rt_model_file : Tuple[str, io.BytesIO], optional
             RT model file or stream. Do nothing if the value is '' or None.
             Defaults to ''.
 
         ccs_model_file : Tuple[str, io.BytesIO], optional
-            CCS model or stream. Do nothing if the value is '' or None. 
+            CCS model or stream. Do nothing if the value is '' or None.
             Defaults to ''.
         """
 
         def _load_file(model, model_file):
             if model_file is None: return
             try:
                 if isinstance(model_file, str):
@@ -555,26 +556,26 @@
         _load_file(self.ms2_model, ms2_model_file)
 
         if isinstance(rt_model_file, str) and rt_model_file:
             logging.info(f"Using external rt model: '{rt_model_file}'")
             if not os.path.isfile(rt_model_file):
                 logging.info(" -- This model file does not exist")
         _load_file(self.rt_model, rt_model_file)
-        
+
         if isinstance(ccs_model_file, str) and ccs_model_file:
             logging.info(f"Using external ccs model: '{ccs_model_file}'")
             if not os.path.isfile(ccs_model_file):
                 logging.info(" -- This model file does not exist")
         _load_file(self.ccs_model, ccs_model_file)
 
     def train_rt_model(self,
         psm_df:pd.DataFrame,
     ):
-        """ 
-        Train/fine-tune the RT model. The fine-tuning will be skipped 
+        """
+        Train/fine-tune the RT model. The fine-tuning will be skipped
         if `self.psm_num_to_train_rt_ccs` is zero.
 
         Parameters
         ----------
         psm_df : pd.DataFrame
             Training psm_df which contains 'rt_norm' column.
         """
@@ -592,15 +593,15 @@
             else:
                 tr_df = psm_df
 
             if self._train_psm_logging:
                 logging.info(f"{len(tr_df)} PSMs for RT model training/transfer learning")
         else:
             tr_df = []
-        
+
         if self.psm_num_to_test_rt_ccs > 0:
             if len(tr_df) > 0:
                 test_psm_df = psm_df[
                     ~psm_df.sequence.isin(set(tr_df.sequence))
                 ].copy()
                 if len(test_psm_df) > self.psm_num_to_test_rt_ccs:
                     test_psm_df = test_psm_df.sample(
@@ -613,39 +614,39 @@
                     )
                     test_psm_df = []
             else:
                 test_psm_df = psm_df
         else:
             test_psm_df = []
 
-        if len(test_psm_df) > 0:    
+        if len(test_psm_df) > 0:
             logging.info(
-                "Testing pretrained RT model:\n" + 
+                "Testing pretrained RT model:\n" +
                 str(self.rt_model.test(test_psm_df))
             )
-        
+
         if len(tr_df) > 0:
-            self.rt_model.train(tr_df, 
+            self.rt_model.train(tr_df,
                 batch_size=self.batch_size_to_train_rt_ccs,
                 epoch=self.epoch_to_train_rt_ccs,
                 warmup_epoch=self.warmup_epoch_to_train_rt_ccs,
                 lr=self.lr_to_train_rt_ccs,
                 verbose=self.train_verbose,
             )
-        
-        if len(test_psm_df) > 0:    
+
+        if len(test_psm_df) > 0:
             logging.info(
-                "Testing refined RT model:\n" + 
+                "Testing refined RT model:\n" +
                 str(self.rt_model.test(test_psm_df))
             )
 
     def train_ccs_model(self,
         psm_df:pd.DataFrame,
     ):
-        """ 
+        """
         Train/fine-tune the CCS model. The fine-tuning will be skipped
         if `self.psm_num_to_train_rt_ccs` is zero.
 
         Parameters
         ----------
         psm_df : pd.DataFrame
             Training psm_df which contains 'ccs' or 'mobility' column.
@@ -675,15 +676,15 @@
                 ).copy()
             else:
                 tr_df = psm_df
             if self._train_psm_logging:
                 logging.info(f"{len(tr_df)} PSMs for CCS model training/transfer learning")
         else:
             tr_df = []
-        
+
         if self.psm_num_to_test_rt_ccs > 0:
             if len(tr_df) > 0:
                 test_psm_df = psm_df[
                     ~psm_df.sequence.isin(set(tr_df.sequence))
                 ].copy()
                 if len(test_psm_df) > self.psm_num_to_test_rt_ccs:
                     test_psm_df = test_psm_df.sample(
@@ -698,42 +699,42 @@
             else:
                 test_psm_df = psm_df
         else:
             test_psm_df = []
 
         if len(test_psm_df) > 0:
             logging.info(
-                "Testing pretrained CCS model:\n" + 
+                "Testing pretrained CCS model:\n" +
                 str(self.ccs_model.test(test_psm_df))
             )
 
         if len(tr_df) > 0:
-            self.ccs_model.train(tr_df, 
+            self.ccs_model.train(tr_df,
                 batch_size=self.batch_size_to_train_rt_ccs,
                 epoch=self.epoch_to_train_rt_ccs,
                 warmup_epoch=self.warmup_epoch_to_train_rt_ccs,
                 lr=self.lr_to_train_rt_ccs,
                 verbose=self.train_verbose,
             )
-          
-        if len(test_psm_df) > 0:  
+
+        if len(test_psm_df) > 0:
             logging.info(
-                "Testing refined CCS model:\n" + 
+                "Testing refined CCS model:\n" +
                 str(self.ccs_model.test(test_psm_df))
             )
 
     def train_ms2_model(self,
         psm_df: pd.DataFrame,
         matched_intensity_df: pd.DataFrame,
     ):
         """
-        Using matched_intensity_df to train/fine-tune the ms2 model. 
-        
+        Using matched_intensity_df to train/fine-tune the ms2 model.
+
         1. It will sample `n=self.psm_num_to_train_ms2` PSMs into training dataframe (`tr_df`) to for fine-tuning.
-        2. This method will also consider some important PTMs (`n=self.top_n_mods_to_train`) into `tr_df` for fine-tuning. 
+        2. This method will also consider some important PTMs (`n=self.top_n_mods_to_train`) into `tr_df` for fine-tuning.
         3. If `self.use_grid_nce_search==True`, this method will call `self.ms2_model.grid_nce_search` to find the best NCE and instrument.
 
         Parameters
         ----------
         psm_df : pd.DataFrame
             PSM dataframe for fine-tuning
 
@@ -812,15 +813,15 @@
             logging.info(
                 "Testing pretrained MS2 model on testing df:\n"+
                 str(self.ms2_model.test(test_psm_df, tr_inten_df))
             )
         if len(tr_df) > 0:
             if self._train_psm_logging:
                 logging.info(f"{len(tr_df)} PSMs for MS2 model training/transfer learning")
-            self.ms2_model.train(tr_df, 
+            self.ms2_model.train(tr_df,
                 fragment_intensity_df=tr_inten_df,
                 batch_size=self.batch_size_to_train_ms2,
                 epoch=self.epoch_to_train_ms2,
                 warmup_epoch=self.warmup_epoch_to_train_ms2,
                 lr=self.lr_to_train_ms2,
                 verbose=self.train_verbose,
             )
@@ -831,92 +832,92 @@
         if len(test_psm_df) > 0:
             logging.info(
                 "Testing refined MS2 model on testing df:\n"+
                 str(self.ms2_model.test(test_psm_df, tr_inten_df))
             )
 
 
-    def predict_ms2(self, precursor_df:pd.DataFrame, 
-        *, 
+    def predict_ms2(self, precursor_df:pd.DataFrame,
+        *,
         batch_size:int=512,
         reference_frag_df:pd.DataFrame = None,
     )->pd.DataFrame:
         """Predict MS2 for the given precursor_df
 
         Parameters
         ----------
         precursor_df : pd.DataFrame
             Precursor dataframe for MS2 prediction
 
         batch_size : int, optional
-            Batch size for prediction. 
+            Batch size for prediction.
             Defaults to 512.
 
         reference_frag_df : pd.DataFrame, optional
-            If precursor_df has 'frag_start_idx' pointing to reference_frag_df. 
+            If precursor_df has 'frag_start_idx' pointing to reference_frag_df.
             Defaults to None
 
         Returns
         -------
         pd.DataFrame
-            Predicted fragment intensity dataframe. 
-            If there are no such two columns in precursor_df, 
-            it will insert 'frag_start_idx' and `frag_stop_idx` in 
+            Predicted fragment intensity dataframe.
+            If there are no such two columns in precursor_df,
+            it will insert 'frag_start_idx' and `frag_stop_idx` in
             precursor_df pointing to this predicted fragment dataframe.
         """
         self.set_default_nce_instrument(precursor_df)
         if self.verbose:
             logging.info('Predicting MS2 ...')
-        return self.ms2_model.predict(precursor_df, 
+        return self.ms2_model.predict(precursor_df,
             batch_size=batch_size,
             reference_frag_df=reference_frag_df,
             verbose=self.verbose
         )
 
     def predict_rt(self, precursor_df:pd.DataFrame,
-        *, 
+        *,
         batch_size:int=1024
     )->pd.DataFrame:
         """ Predict RT ('rt_pred') inplace into `precursor_df`.
 
         Parameters
         ----------
         precursor_df : pd.DataFrame
             precursor_df for RT prediction
 
         batch_size : int, optional
-            Batch size for prediction. 
+            Batch size for prediction.
             Defaults to 1024.
 
         Returns
         -------
         pd.DataFrame
             df with 'rt_pred' and 'rt_norm_pred' columns.
         """
         if self.verbose:
             logging.info("Predicting RT ...")
-        df = self.rt_model.predict(precursor_df, 
+        df = self.rt_model.predict(precursor_df,
             batch_size=batch_size, verbose=self.verbose
         )
         df['rt_norm_pred'] = df.rt_pred
         return df
 
     def predict_mobility(self, precursor_df:pd.DataFrame,
-        *, 
+        *,
         batch_size:int=1024
     )->pd.DataFrame:
         """ Predict mobility (`ccs_pred` and `mobility_pred`) inplace into `precursor_df`.
 
         Parameters
         ----------
         precursor_df : pd.DataFrame
             Precursor_df for CCS/mobility prediction
 
         batch_size : int, optional
-            Batch size for prediction. 
+            Batch size for prediction.
             Defaults to 1024.
 
         Returns
         -------
         pd.DataFrame
             df with 'ccs_pred' and 'mobility_pred' columns.
         """
@@ -936,15 +937,15 @@
             multiprocessing=False, **arg_dict
         )
 
     def predict_all_mp(self, precursor_df:pd.DataFrame,
         *,
         predict_items:list = [
             'rt' ,'mobility' ,'ms2'
-        ], 
+        ],
         frag_types:list =  None,
         process_num:int = 8,
         mp_batch_size:int = 100000,
     ):
         self.ms2_model.model.share_memory()
         self.rt_model.model.share_memory()
         self.ccs_model.model.share_memory()
@@ -985,17 +986,17 @@
             )
         verbose_bak = self.verbose
         self.verbose = False
 
         with mp.get_context('spawn').Pool(process_num) as p:
             for ret_dict in process_bar(
                 p.imap_unordered(
-                    self._predict_func_for_mp, 
+                    self._predict_func_for_mp,
                     mp_param_generator(df_groupby)
-                ), 
+                ),
                 get_batch_num_mp(df_groupby)
             ):
                 precursor_df_list.append(ret_dict['precursor_df'])
                 if fragment_mz_df_list is not None:
                     fragment_mz_df_list.append(
                         ret_dict['fragment_mz_df']
                     )
@@ -1008,73 +1009,73 @@
             (
                 precursor_df, fragment_mz_df, fragment_intensity_df
             ) = concat_precursor_fragment_dataframes(
                 precursor_df_list,
                 fragment_mz_df_list,
                 fragment_intensity_df_list,
             )
-            
+
             return {
-                'precursor_df': precursor_df, 
+                'precursor_df': precursor_df,
                 'fragment_mz_df': fragment_mz_df,
-                'fragment_intensity_df': fragment_intensity_df, 
+                'fragment_intensity_df': fragment_intensity_df,
             }
         else:
             precursor_df = pd.concat(precursor_df_list)
             precursor_df.reset_index(drop=True, inplace=True)
-            
-            return {'precursor_df': precursor_df} 
+
+            return {'precursor_df': precursor_df}
 
     def predict_all(self, precursor_df:pd.DataFrame,
-        *, 
+        *,
         predict_items:list = [
             'rt' ,'mobility' ,'ms2'
-        ], 
+        ],
         frag_types:list =  None,
         multiprocessing:bool = True,
         min_required_precursor_num_for_mp:int = 3000,
         process_num:int = 8,
         mp_batch_size:int = 100000,
     )->Dict[str, pd.DataFrame]:
-        """ 
-        Predict all items defined by `predict_items`, 
-        which may include rt, mobility, fragment_mz 
+        """
+        Predict all items defined by `predict_items`,
+        which may include rt, mobility, fragment_mz
         and fragment_intensity.
 
         Parameters
         ----------
         precursor_df : pd.DataFrame
-            Precursor dataframe contains `sequence`, `mods`, `mod_sites`, `charge` ... columns. 
+            Precursor dataframe contains `sequence`, `mods`, `mod_sites`, `charge` ... columns.
 
         predict_items : list, optional
             items ('rt', 'mobility', 'ms2') to predict.
             Defaults to ['rt' ,'mobility' ,'ms2'].
 
         frag_types : list, optional
-            Fragment types to predict. 
-            If it is None, it then depends on `self.ms2_model.charged_frag_types` and 
+            Fragment types to predict.
+            If it is None, it then depends on `self.ms2_model.charged_frag_types` and
             `self.ms2_model.model._mask_modloss`.
             Defaults to None.
 
         multiprocessing : bool, optional
             If use multiprocessing is gpu is not available
             Defaults to True.
 
         process_num : int, optional
             Defaults to 4
 
         min_required_precursor_num_for_mp : int, optional
-            It will not use multiprocessing when the number of precursors in precursor_df 
-            is lower than this value. 
+            It will not use multiprocessing when the number of precursors in precursor_df
+            is lower than this value.
             Defaults to 3000.
 
         mp_batch_size : int, optional
-            Splitting data into batches for multiprocessing. 
+            Splitting data into batches for multiprocessing.
             Defaults to 100000.
-              
+
         Returns
         -------
         Dict[str, pd.DataFrame]
             `{'precursor_df': precursor_df}`
             and if 'ms2' in predict_items, it also contains:
             ```
             {
@@ -1098,38 +1099,38 @@
             else:
                 frag_types = self.ms2_model.charged_frag_types
 
         if 'precursor_mz' not in precursor_df.columns:
             update_precursor_mz(precursor_df)
 
         if (
-            self.ms2_model.device_type!='cpu' 
+            self.ms2_model.device_type!='cpu'
             or not multiprocessing or process_num <= 1
             or len(precursor_df) < min_required_precursor_num_for_mp
         ):
             refine_df(precursor_df)
             if 'rt' in predict_items:
-                self.predict_rt(precursor_df, 
+                self.predict_rt(precursor_df,
                     batch_size=model_mgr_settings['predict']['batch_size_rt_ccs']
                 )
             if 'mobility' in predict_items:
                 self.predict_mobility(precursor_df,
                     batch_size=model_mgr_settings['predict']['batch_size_rt_ccs']
                 )
             if 'ms2' in predict_items:
                 if 'frag_start_idx' in precursor_df.columns:
                     precursor_df.drop(
-                        columns=['frag_start_idx','frag_stop_idx'], 
+                        columns=['frag_start_idx','frag_stop_idx'],
                         inplace=True
                     )
 
                 fragment_mz_df = create_fragment_mz_dataframe(
                     precursor_df, frag_types
                 )
-                
+
                 fragment_intensity_df = self.predict_ms2(
                     precursor_df,
                     batch_size=model_mgr_settings['predict']['batch_size_ms2']
                 )
 
                 fragment_intensity_df.drop(
                     columns=[
@@ -1139,21 +1140,21 @@
                 )
 
                 clear_error_modloss_intensities(
                     fragment_mz_df, fragment_intensity_df
                 )
 
                 return {
-                    'precursor_df': precursor_df, 
+                    'precursor_df': precursor_df,
                     'fragment_mz_df': fragment_mz_df,
-                    'fragment_intensity_df': fragment_intensity_df, 
+                    'fragment_intensity_df': fragment_intensity_df,
                 }
             else:
                 return {'precursor_df': precursor_df}
         else:
             logging.info(f"Using multiprocessing with {process_num} processes ...")
             return self.predict_all_mp(
-                precursor_df, 
+                precursor_df,
                 predict_items=predict_items,
                 process_num = process_num,
                 mp_batch_size=mp_batch_size,
             )
```

### Comparing `peptdeep-1.1.9/peptdeep/protein/fasta.py` & `peptdeep-1.2.0/peptdeep/protein/fasta.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         charged_frag_types:list = ['b_z1','b_z2','y_z1','y_z2'],
         protease:str = 'trypsin',
         max_missed_cleavages:int = 2,
         peptide_length_min:int = 7,
         peptide_length_max:int = 35,
         precursor_charge_min:int = 2,
         precursor_charge_max:int = 4,
-        precursor_mz_min:float = 400.0, 
+        precursor_mz_min:float = 400.0,
         precursor_mz_max:float = 1800.0,
         var_mods:list = ['Acetyl@Protein N-term','Oxidation@M'],
         min_var_mod_num:int = 0,
         max_var_mod_num:int = 2,
         fix_mods:list = ['Carbamidomethyl@C'],
         labeling_channels:dict = None,
         special_mods:list = [],
@@ -38,25 +38,25 @@
         """
         Parameters
         ----------
         model_manager : ModelManager, optional
             ModelManager of MS2/RT/CCS... models, by default None
 
         charged_frag_types : list, optional
-            Fragment types with charge, 
+            Fragment types with charge,
             by default [ 'b_z1','b_z2','y_z1', 'y_z2' ]
 
         protease : str, optional
             Could be pre-defined protease name defined in :data:`protease_dict`,
-            or a regular expression. 
+            or a regular expression.
             By default 'trypsin'
 
         max_missed_cleavages : int, optional
             Maximal missed cleavages, by default 2
-            
+
         peptide_length_min : int, optional
             Minimal cleaved peptide length, by default 7
 
         peptide_length_max : int, optional
             Maximal cleaved peptide length, by default 35
 
         precursor_charge_min : int, optional
@@ -68,81 +68,81 @@
         precursor_mz_min : float, optional
             Minimal precursor mz, by default 200.0
 
         precursor_mz_max : float, optional
             Maximal precursor mz, by default 2000.0
 
         var_mods : list, optional
-            list of variable modifications, 
+            list of variable modifications,
             by default ['Acetyl@Protein N-term','Oxidation@M']
 
         max_var_mod_num : int, optional
-            Minimal number of variable modifications on a peptide sequence, 
+            Minimal number of variable modifications on a peptide sequence,
             by default 0
 
         max_var_mod_num : int, optional
-            Maximal number of variable modifications on a peptide sequence, 
+            Maximal number of variable modifications on a peptide sequence,
             by default 2
 
         fix_mods : list, optional
             list of fixed modifications, by default ['Carbamidomethyl@C']
 
         labeling_channels : dict, optional
-            Add isotope labeling with different channels, 
-            see :meth:`add_peptide_labeling()`. 
+            Add isotope labeling with different channels,
+            see :meth:`add_peptide_labeling()`.
             Defaults to None
 
         special_mods : list, optional
             Special modifications.
-            It is useful for modificaitons like Phospho which may largely 
+            It is useful for modificaitons like Phospho which may largely
             explode the number of candidate modified peptides.
-            The number of special_mods per peptide 
+            The number of special_mods per peptide
             is controlled by `max_append_mod_num`.
             Defaults to [].
 
         min_special_mod_num : int, optional
             Control the min number of special_mods per peptide, by default 0.
 
         max_special_mod_num : int, optional
             Control the max number of special_mods per peptide, by default 1.
 
         special_mods_cannot_modify_pep_c_term : bool, optional
-            Some modifications cannot modify the peptide C-term, 
-            this will be useful for GlyGly@K as if C-term is di-Glyed, 
-            it cannot be cleaved/digested. 
+            Some modifications cannot modify the peptide C-term,
+            this will be useful for GlyGly@K as if C-term is di-Glyed,
+            it cannot be cleaved/digested.
             Defaults to False.
 
         special_mods_cannot_modify_pep_n_term : bool, optional
             Similar to `special_mods_cannot_modify_pep_c_term`, but at N-term.
             Defaults to False.
 
         decoy : str, optional
             Decoy type, see `alphabase.spectral_library.decoy_library`,
             by default None
 
         include_contaminants : bool, optional
             If include contaminants.fasta, by default False
 
         generate_precursor_isotope : bool, optional
-            If :meth:`peptdeep.spec_lib.predict_lib.PredictSpecLib.predict_all()` 
+            If :meth:`peptdeep.spec_lib.predict_lib.PredictSpecLib.predict_all()`
             includes :meth:`peptdeep.spec_lib.predict_lib.PredictSpecLib.calc_precursor_isotope()`.
             Defaults to False
-        
+
         rt_to_irt : bool, optional
             If convert predicted RT to iRT values, by default False
         """
         SpecLibFasta.__init__(self,
             charged_frag_types=charged_frag_types,
             protease=protease,
             max_missed_cleavages=max_missed_cleavages,
             peptide_length_min=peptide_length_min,
             peptide_length_max=peptide_length_max,
             precursor_charge_min=precursor_charge_min,
             precursor_charge_max=precursor_charge_max,
-            precursor_mz_min=precursor_mz_min, 
+            precursor_mz_min=precursor_mz_min,
             precursor_mz_max=precursor_mz_max,
             var_mods=var_mods,
             min_var_mod_num=min_var_mod_num,
             max_var_mod_num=max_var_mod_num,
             fix_mods=fix_mods,
             labeling_channels=labeling_channels,
             special_mods=special_mods,
@@ -176,18 +176,18 @@
     def add_charge(self):
         if self.model_manager.charge_model is None:
             super().add_charge()
         else:
             print(f"Predicting charge states for {len(self.precursor_df)} peptides ...")
             if self.model_manager.use_predicted_charge_in_speclib:
                 self._precursor_df = self.model_manager.charge_model.predict_and_clip_charges(
-                    self.precursor_df, 
+                    self.precursor_df,
                     min_precursor_charge=self.min_precursor_charge,
                     max_precursor_charge=self.max_precursor_charge,
                     charge_prob_cutoff=self.model_manager.charge_prob_cutoff
                 )
             else:
                 self._precursor_df = self.model_manager.charge_model.predict_charges_as_prob(
-                    self.precursor_df, 
+                    self.precursor_df,
                     min_precursor_charge=self.min_precursor_charge,
                     max_precursor_charge=self.max_precursor_charge
                 )
```

### Comparing `peptdeep-1.1.9/peptdeep/psm_frag_reader/maxquant_frag_reader.py` & `peptdeep-1.2.0/peptdeep/psm_frag_reader/maxquant_frag_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,153 +1,150 @@
-import pandas as pd
 import numpy as np
-import numba
 
-from alphabase.peptide.fragment import (
-    init_fragment_by_precursor_dataframe
-)
-from alphabase.io.psm_reader.maxquant_reader import (
-    MaxQuantReader
-)
+from alphabase.peptide.fragment import init_fragment_by_precursor_dataframe
+from alphabase.psm_reader.maxquant_reader import MaxQuantReader
 
 from peptdeep.psm_frag_reader.psm_frag_reader import (
     PSMReader_w_FragBase,
-    psm_w_frag_reader_provider
+    psm_w_frag_reader_provider,
 )
 
+
 def parse_phos_probs(mods, prob_seq, prob):
-    if mods == 'Unmodified': return '', ''
-    idx = mods.find('Phospho')
-    if idx == -1: return '', ''
-    elif idx == 0 or mods[idx-1]==',':
+    if mods == "Unmodified":
+        return "", ""
+    idx = mods.find("Phospho")
+    if idx == -1:
+        return "", ""
+    elif idx == 0 or mods[idx - 1] == ",":
         num_phos = 1
-    elif mods[idx-2].isdigit():
-        num_phos = int(mods[idx-2])
+    elif mods[idx - 2].isdigit():
+        num_phos = int(mods[idx - 2])
     else:
-        return 'x', 'x'
-    
-    idx = prob_seq.find('(')
+        return "x", "x"
+
+    idx = prob_seq.find("(")
     keep_probs = []
     keep_sites = []
     while idx != -1:
-        end = prob_seq.find(')',idx+2)
-        if prob_seq[idx-1] in 'STY':
-            if float(prob_seq[idx+1:end])>=prob:
-                keep_probs.append(prob_seq[idx+1:end])
+        end = prob_seq.find(")", idx + 2)
+        if prob_seq[idx - 1] in "STY":
+            if float(prob_seq[idx + 1 : end]) >= prob:
+                keep_probs.append(prob_seq[idx + 1 : end])
                 keep_sites.append(str(idx))
-        prob_seq = prob_seq[:idx]+prob_seq[end+1:]
-        idx = prob_seq.find('(',idx)
-    if len(keep_probs) >= num_phos: 
-        return ';'.join(keep_probs),';'.join(keep_sites)
-    else: return 'x','x'
+        prob_seq = prob_seq[:idx] + prob_seq[end + 1 :]
+        idx = prob_seq.find("(", idx)
+    if len(keep_probs) >= num_phos:
+        return ";".join(keep_probs), ";".join(keep_sites)
+    else:
+        return "x", "x"
+
 
 def filter_phos(mq_df, prob):
-    if 'Phospho (STY) Probabilities' not in mq_df.columns:
-        mq_df['PhosProbs'] = ''
-        mq_df['PhosSites'] = ''
+    if "Phospho (STY) Probabilities" not in mq_df.columns:
+        mq_df["PhosProbs"] = ""
+        mq_df["PhosSites"] = ""
         return mq_df
 
-    (
-        mq_df['PhosProbs'], mq_df['PhosSites']
-    ) = zip(*mq_df[['Modifications','Phospho (STY) Probabilities']].apply(
-        lambda x: parse_phos_probs(x[0],x[1],prob), axis=1
-    ))
-    return mq_df[mq_df['PhosProbs']!='x']
-    
+    (mq_df["PhosProbs"], mq_df["PhosSites"]) = zip(
+        *mq_df[["Modifications", "Phospho (STY) Probabilities"]].apply(
+            lambda x: parse_phos_probs(x[0], x[1], prob), axis=1
+        )
+    )
+    return mq_df[mq_df["PhosProbs"] != "x"]
+
 
 class MaxQuantMSMSReader(MaxQuantReader, PSMReader_w_FragBase):
-    def __init__(self,
-        frag_types=['b','y','b_modloss','y_modloss'], 
+    def __init__(
+        self,
+        frag_types=["b", "y", "b_modloss", "y_modloss"],
         max_frag_charge=2,
         score_threshold=100,
-        rt_unit='minute',
-        **kwargs
+        rt_unit="minute",
+        **kwargs,
     ):
-        PSMReader_w_FragBase.__init__(self,
-            frag_types = frag_types,
-            max_frag_charge = max_frag_charge,
-            **kwargs
+        PSMReader_w_FragBase.__init__(
+            self, frag_types=frag_types, max_frag_charge=max_frag_charge, **kwargs
         )
 
         MaxQuantReader.__init__(self, rt_unit=rt_unit)
 
-        self.column_mapping['phos_probs'] = 'PhosProbs'
-        self.column_mapping['phos_sites'] = 'PhosSites'
+        self.column_mapping["phos_probs"] = "PhosProbs"
+        self.column_mapping["phos_sites"] = "PhosSites"
         self._score_thres = score_threshold
         self._phos_prob = 0.75
-    
+
     @property
     def fragment_intensity_df(self):
         return self._fragment_intensity_df
 
     def _load_file(self, filename):
         df = MaxQuantReader._load_file(self, filename)
         df = filter_phos(df, self._phos_prob)
         df = df[
-            (df.Score >= self._score_thres)|
-            ((df.Score>=60)&(df.PhosProbs!=''))]
+            (df.Score >= self._score_thres) | ((df.Score >= 60) & (df.PhosProbs != ""))
+        ]
         df.reset_index(drop=True, inplace=True)
         return df
 
-    def _post_process(self, 
-        mq_df
-    ):  
-        self._psm_df['nAA'] = self._psm_df.sequence.str.len()
-        mq_df['nAA'] = self._psm_df.nAA
+    def _post_process(self, mq_df):
+        self._psm_df["nAA"] = self._psm_df.sequence.str.len()
+        mq_df["nAA"] = self._psm_df.nAA
         self.normalize_rt_by_raw_name()
 
         self._fragment_intensity_df = init_fragment_by_precursor_dataframe(
             mq_df, self.charged_frag_types
         )
 
-        frag_col_dict = dict(zip(
-            self.charged_frag_types, 
-            range(len(self.charged_frag_types))
-        ))
+        frag_col_dict = dict(
+            zip(self.charged_frag_types, range(len(self.charged_frag_types)))
+        )
 
-        for ith_psm, (nAA, start,end) in enumerate(
-            mq_df[['nAA','frag_start_idx','frag_stop_idx']].values
+        for ith_psm, (nAA, start, end) in enumerate(
+            mq_df[["nAA", "frag_start_idx", "frag_stop_idx"]].values
         ):
-            intens = np.zeros((nAA-1, len(self.charged_frag_types)))
+            intens = np.zeros((nAA - 1, len(self.charged_frag_types)))
 
-            frag_types = mq_df['Matches'].values[ith_psm]
-            frag_intens = mq_df['Intensities'].values[ith_psm]
+            frag_types = mq_df["Matches"].values[ith_psm]
+            frag_intens = mq_df["Intensities"].values[ith_psm]
             for frag_type, frag_inten in zip(
-                frag_types.split(';'), frag_intens.split(';')
+                frag_types.split(";"), frag_intens.split(";")
             ):
-                if '-' in frag_type: continue
-                if any(_.isupper() for _ in frag_type): continue
-                idx = frag_type.find('(')
-                charge = '1'
+                if "-" in frag_type:
+                    continue
+                if any(_.isupper() for _ in frag_type):
+                    continue
+                idx = frag_type.find("(")
+                charge = "1"
                 if idx > 0:
-                    frag_type, charge = frag_type[:idx], frag_type[idx+1:-2]
-                if not frag_type[1].isdigit(): continue # no H2O or NH3 loss
+                    frag_type, charge = frag_type[:idx], frag_type[idx + 1 : -2]
+                if not frag_type[1].isdigit():
+                    continue  # no H2O or NH3 loss
                 frag_type, frag_pos = frag_type[0], frag_type[1:]
-                if frag_pos.endswith('*'):
+                if frag_pos.endswith("*"):
                     frag_pos = int(frag_pos[:-1])
-                    modloss=True
-                else: 
+                    modloss = True
+                else:
                     frag_pos = int(frag_pos)
-                    modloss=False
-                if frag_type in 'xyz':
-                    frag_pos = nAA - frag_pos -1
+                    modloss = False
+                if frag_type in "xyz":
+                    frag_pos = nAA - frag_pos - 1
                 else:
-                    frag_pos -= 1 
-                frag_type += ('_modloss_z' if modloss else '_z') +charge
-                if frag_type not in frag_col_dict: continue
+                    frag_pos -= 1
+                frag_type += ("_modloss_z" if modloss else "_z") + charge
+                if frag_type not in frag_col_dict:
+                    continue
                 frag_col = frag_col_dict[frag_type]
-                intens[frag_pos,frag_col] = float(frag_inten)
+                intens[frag_pos, frag_col] = float(frag_inten)
 
-            if np.any(intens>0):
+            if np.any(intens > 0):
                 intens /= np.max(intens)
-            self._fragment_intensity_df.iloc[
-                start:end,:
-            ] = intens
-        
-        self._psm_df[
-            ['frag_start_idx','frag_stop_idx']
-        ] = mq_df[['frag_start_idx','frag_stop_idx']]
+            self._fragment_intensity_df.iloc[start:end, :] = intens
+
+        self._psm_df[["frag_start_idx", "frag_stop_idx"]] = mq_df[
+            ["frag_start_idx", "frag_stop_idx"]
+        ]
 
         self._psm_df = self._psm_df[~self._psm_df.mods.isna()]
 
 
-psm_w_frag_reader_provider.register_reader('maxquant', MaxQuantMSMSReader)
+psm_w_frag_reader_provider.register_reader("maxquant", MaxQuantMSMSReader)
```

### Comparing `peptdeep-1.1.9/peptdeep/psm_frag_reader/psmlabel_reader.py` & `peptdeep-1.2.0/peptdeep/psm_frag_reader/psmlabel_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,171 +1,173 @@
 import pandas as pd
 import numpy as np
-import typing
 from tqdm import tqdm
 
-import alphabase.constants.modification as ap_mod
 from alphabase.peptide.fragment import (
     concat_precursor_fragment_dataframes,
-    init_fragment_by_precursor_dataframe
+    init_fragment_by_precursor_dataframe,
 )
 
-from alphabase.io.psm_reader.pfind_reader import (
-    pFindReader, get_pFind_mods, translate_pFind_mod
+from alphabase.psm_reader.pfind_reader import (
+    pFindReader,
+    get_pFind_mods,
+    translate_pFind_mod,
 )
 
 from peptdeep.psm_frag_reader.psm_frag_reader import (
-    PSMReader_w_FragBase, psm_w_frag_reader_provider
+    PSMReader_w_FragBase,
+    psm_w_frag_reader_provider,
 )
 
 
-class PSMLabelReader(pFindReader,PSMReader_w_FragBase):
-    def __init__(self, 
-        frag_types=['b','y','b_modloss','y_modloss'], 
+class PSMLabelReader(pFindReader, PSMReader_w_FragBase):
+    def __init__(
+        self,
+        frag_types=["b", "y", "b_modloss", "y_modloss"],
         max_frag_charge=2,
-        **kwargs
+        **kwargs,
     ):
-        PSMReader_w_FragBase.__init__(self,
-            frag_types=frag_types,
-            max_frag_charge=max_frag_charge,
-            **kwargs
+        PSMReader_w_FragBase.__init__(
+            self, frag_types=frag_types, max_frag_charge=max_frag_charge, **kwargs
         )
         pFindReader.__init__(self)
 
-        psmlabel_columns = 'b,b-NH3,b-H20,b-ModLoss,y,y-HN3,y-H20,y-ModLoss'.split(',')
+        psmlabel_columns = "b,b-NH3,b-H20,b-ModLoss,y,y-HN3,y-H20,y-ModLoss".split(",")
         self.psmlabel_frag_columns = []
         self.frag_df_columns = {}
         for _type in psmlabel_columns:
             frag_idxes = [
-                i for i,_t in enumerate(
-                    self.charged_frag_types
-                ) if _t.startswith(_type.replace('-','_').lower()+'_')
+                i
+                for i, _t in enumerate(self.charged_frag_types)
+                if _t.startswith(_type.replace("-", "_").lower() + "_")
             ]
             if frag_idxes:
                 self.psmlabel_frag_columns.append(_type)
-                self.frag_df_columns[_type] = np.array(
-                    frag_idxes, dtype=int
-                )
+                self.frag_df_columns[_type] = np.array(frag_idxes, dtype=int)
 
     def _init_column_mapping(self):
         self.column_mapping = {
-            'sequence': 'peptide',
-            'charge': 'charge',
-            'rt': 'RT',
-            'raw_name': 'raw_name',
-            'query_id': 'spec',
-            'scan_num': 'scan_num',
+            "sequence": "peptide",
+            "charge": "charge",
+            "rt": "RT",
+            "raw_name": "raw_name",
+            "query_id": "spec",
+            "scan_num": "scan_num",
         }
 
     def _load_file(self, filename):
         psmlabel_df = pd.read_csv(filename, sep="\t")
-        psmlabel_df.fillna('', inplace=True)
+        psmlabel_df.fillna("", inplace=True)
 
-        if psmlabel_df['spec'].values[0].count('.')>=4: #pfind
-            psmlabel_df['raw_name'], psmlabel_df['scan_num'], psmlabel_df['charge'] = zip(
-                *psmlabel_df['spec'].str.split('.').apply(lambda x: (x[0], x[-4], x[-3]))
+        if psmlabel_df["spec"].values[0].count(".") >= 4:  # pfind
+            psmlabel_df["raw_name"], psmlabel_df["scan_num"], psmlabel_df["charge"] = (
+                zip(
+                    *psmlabel_df["spec"]
+                    .str.split(".")
+                    .apply(lambda x: (x[0], x[-4], x[-3]))
+                )
             )
         else:
-            psmlabel_df['raw_name'], psmlabel_df['scan_num'] = zip(
-                *psmlabel_df['spec'].str.split('.').apply(lambda x: (x[0], x[1]))
+            psmlabel_df["raw_name"], psmlabel_df["scan_num"] = zip(
+                *psmlabel_df["spec"].str.split(".").apply(lambda x: (x[0], x[1]))
             )
-        psmlabel_df['scan_num'] = psmlabel_df['scan_num'].astype(int)
-        psmlabel_df['charge'] = psmlabel_df['charge'].astype(int)
+        psmlabel_df["scan_num"] = psmlabel_df["scan_num"].astype(int)
+        psmlabel_df["charge"] = psmlabel_df["charge"].astype(int)
         return psmlabel_df
 
     def _load_modifications(self, psmlabel_df: pd.DataFrame):
-        (
-            self._psm_df['mods'], self._psm_df['mod_sites'] 
-        ) = zip(*psmlabel_df['modinfo'].apply(get_pFind_mods))
+        (self._psm_df["mods"], self._psm_df["mod_sites"]) = zip(
+            *psmlabel_df["modinfo"].apply(get_pFind_mods)
+        )
 
     def _translate_decoy(self, df):
         pass
+
     def _translate_score(self, df):
         pass
 
     def _translate_modifications(self):
-        self._psm_df['mods'] = self._psm_df['mods'].apply(translate_pFind_mod)
+        self._psm_df["mods"] = self._psm_df["mods"].apply(translate_pFind_mod)
 
     def _post_process(self, psmlabel_df: pd.DataFrame):
-        psmlabel_df['nAA'] = psmlabel_df.peptide.str.len()
-        self._psm_df['nAA'] = psmlabel_df.nAA
-        psmlabel_df = psmlabel_df[
-            ~self._psm_df['mods'].isna()
-        ].reset_index(drop=True)
-        
-        self._psm_df = self._psm_df[
-            ~self._psm_df['mods'].isna()
-        ].reset_index(drop=True)
+        psmlabel_df["nAA"] = psmlabel_df.peptide.str.len()
+        self._psm_df["nAA"] = psmlabel_df.nAA
+        psmlabel_df = psmlabel_df[~self._psm_df["mods"].isna()].reset_index(drop=True)
+
+        self._psm_df = self._psm_df[~self._psm_df["mods"].isna()].reset_index(drop=True)
 
         self._fragment_intensity_df = init_fragment_by_precursor_dataframe(
             psmlabel_df, self.charged_frag_types
         )
 
-        for ith_psm, (nAA, start,end) in enumerate(
-            psmlabel_df[['nAA','frag_start_idx','frag_stop_idx']].values
+        for ith_psm, (nAA, start, end) in enumerate(
+            psmlabel_df[["nAA", "frag_start_idx", "frag_stop_idx"]].values
         ):
-            intens = np.zeros((nAA-1, len(self.charged_frag_types)))
+            intens = np.zeros((nAA - 1, len(self.charged_frag_types)))
             for ion_type in self.psmlabel_frag_columns:
-                if ion_type not in psmlabel_df.columns: continue
+                if ion_type not in psmlabel_df.columns:
+                    continue
 
-                pos_end = ion_type.find('-')-len(ion_type)-2 if '-' in ion_type else -2
-                typed_frags = psmlabel_df.loc[ith_psm,ion_type]
-                if not typed_frags: continue
-                typed_frags = typed_frags.strip(';').split(';')
+                pos_end = (
+                    ion_type.find("-") - len(ion_type) - 2 if "-" in ion_type else -2
+                )
+                typed_frags = psmlabel_df.loc[ith_psm, ion_type]
+                if not typed_frags:
+                    continue
+                typed_frags = typed_frags.strip(";").split(";")
                 frag_pos = []
                 frag_charge = []
                 frag_inten = []
 
                 for frag in typed_frags:
-                    frag, inten = frag.split(',')
+                    frag, inten = frag.split(",")
                     frag_pos.append(int(frag[1:pos_end]))
                     frag_charge.append(int(frag[-1]))
                     frag_inten.append(float(inten))
-                if not frag_inten: continue
-                
+                if not frag_inten:
+                    continue
+
                 frag_pos = np.array(frag_pos, dtype=int)
-                frag_col = np.array(frag_charge, dtype=int)-1
-                
-                if ion_type[0] in 'xyz':
-                    frag_pos = nAA - frag_pos -1
+                frag_col = np.array(frag_charge, dtype=int) - 1
+
+                if ion_type[0] in "xyz":
+                    frag_pos = nAA - frag_pos - 1
                 else:
                     frag_pos -= 1
-                intens[frag_pos,self.frag_df_columns[ion_type][frag_col]] = frag_inten
-            if np.any(intens>0):
+                intens[frag_pos, self.frag_df_columns[ion_type][frag_col]] = frag_inten
+            if np.any(intens > 0):
                 intens /= np.max(intens)
-            self._fragment_intensity_df.iloc[
-                start:end,:
-            ] = intens
-        
-        self._psm_df[
-            ['frag_start_idx','frag_stop_idx']
-        ] = psmlabel_df[['frag_start_idx','frag_stop_idx']]
+            self._fragment_intensity_df.iloc[start:end, :] = intens
+
+        self._psm_df[["frag_start_idx", "frag_stop_idx"]] = psmlabel_df[
+            ["frag_start_idx", "frag_stop_idx"]
+        ]
+
+
+psm_w_frag_reader_provider.register_reader("psmlabel", PSMLabelReader)
 
-psm_w_frag_reader_provider.register_reader(
-    'psmlabel', PSMLabelReader
-)
 
 def load_psmlabel_list(
     psmlabel_list,
     nce_list,
     instrument_list,
-    frag_types=['b','y','b_modloss','y_modloss'], 
+    frag_types=["b", "y", "b_modloss", "y_modloss"],
     frag_charge=2,
     include_mod_list=[
-        'Oxidation@M','Phospho@S','Phospho@T','Phospho@Y','Acetyl@Protein N-term'
-    ]
+        "Oxidation@M",
+        "Phospho@S",
+        "Phospho@T",
+        "Phospho@Y",
+        "Acetyl@Protein N-term",
+    ],
 ):
     psm_df_list = []
     fragment_inten_df_list = []
-    for i,psmlabel in tqdm(enumerate(psmlabel_list)):
-        psm_reader = PSMLabelReader(
-            frag_types=frag_types,
-            max_frag_charge = frag_charge
-        )
+    for i, psmlabel in tqdm(enumerate(psmlabel_list)):
+        psm_reader = PSMLabelReader(frag_types=frag_types, max_frag_charge=frag_charge)
         psm_reader.import_file(psmlabel)
         psm_reader.filter_psm_by_modifications(include_mod_list)
-        psm_reader.psm_df['nce'] = nce_list[i]
-        psm_reader.psm_df['instrument'] = instrument_list[i]
+        psm_reader.psm_df["nce"] = nce_list[i]
+        psm_reader.psm_df["instrument"] = instrument_list[i]
         psm_df_list.append(psm_reader.psm_df)
         fragment_inten_df_list.append(psm_reader.fragment_intensity_df)
     return concat_precursor_fragment_dataframes(psm_df_list, fragment_inten_df_list)
-
```

### Comparing `peptdeep-1.1.9/peptdeep/rescore/fdr.py` & `peptdeep-1.2.0/peptdeep/rescore/fdr.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     fdr_values:np.ndarray
 )->np.ndarray:
     """convert FDR values to q_values.
 
     Parameters
     ----------
     fdr_values : np.ndarray
-        FDR values, they should be 
+        FDR values, they should be
         sorted according to the descending order of the `score`
 
     Returns
     -------
     np.ndarray
         q_values
 
@@ -26,30 +26,30 @@
         fdr = fdr_values[i]
         if fdr < min_q_value:
             min_q_value = fdr
         q_values[i] = min_q_value
     return q_values
 
 def calc_fdr(
-    df:pd.DataFrame, 
-    score_column:str, 
+    df:pd.DataFrame,
+    score_column:str,
     decoy_column:str='decoy'
 )->pd.DataFrame:
     """Calculate FDR values (q_values in fact) for the given dataframe
 
     Parameters
     ----------
     df : pd.DataFrame
         PSM dataframe to calculate FDRs
 
     score_column : str
         score column to sort in decending order
 
     decoy_column : str, optional
-        decoy column in the dataframe. 
+        decoy column in the dataframe.
         1=target, 0=decoy. Defaults to 'decoy'.
 
     Returns
     -------
     pd.DataFrame
         PSM dataframe with 'fdr' column added
 
@@ -65,30 +65,30 @@
     return df
 
 #wrapper
 calc_fdr_for_df = calc_fdr
 
 @numba.njit
 def fdr_from_ref(
-    sorted_scores:np.ndarray, 
-    ref_scores:np.ndarray, 
+    sorted_scores:np.ndarray,
+    ref_scores:np.ndarray,
     ref_fdr_values:np.ndarray
 )->np.ndarray:
-    """ Calculate FDR values from the given reference scores and fdr_values. 
-    It is used to extend peptide-level or sequence-level FDR (reference) 
+    """ Calculate FDR values from the given reference scores and fdr_values.
+    It is used to extend peptide-level or sequence-level FDR (reference)
     to each PSM, as PSMs are more useful for quantification.
 
     Parameters
     ----------
     sorted_scores : np.array
-        the scores to calculate FDRs, 
+        the scores to calculate FDRs,
         they must be sorted in decending order.
 
     ref_scores : np.array
-        reference scores that used to 
+        reference scores that used to
         calculate ref_fdr_values, also sorted in decending order.
 
     ref_fdr_values : np.array
         fdr values corresponding to ref_scores
 
     Returns
     -------
@@ -107,42 +107,42 @@
     while i < len(sorted_scores):
         q_values[i] = ref_fdr_values[-1]
         i += 1
     return q_values
 
 def calc_fdr_from_ref(
     df: pd.DataFrame,
-    ref_scores:np.ndarray, 
+    ref_scores:np.ndarray,
     ref_fdr_values:np.ndarray,
-    score_column:str, 
+    score_column:str,
     decoy_column:str='decoy'
 )->pd.DataFrame:
     """ Calculate FDR values for a PSM dataframe from the given reference
-     scores and fdr_values. It is used to extend peptide-level or 
-     sequence-level FDR (reference) to each PSM, as PSMs are more useful 
+     scores and fdr_values. It is used to extend peptide-level or
+     sequence-level FDR (reference) to each PSM, as PSMs are more useful
      for quantification.
     ``
 
     Parameters
     ----------
     df : pd.DataFrame
         PSM dataframe
 
     ref_scores : np.array
-        reference scores that used to 
+        reference scores that used to
         calculate ref_fdr_values, also sorted in decending order.
 
     ref_fdr_values : np.array
         fdr values corresponding to ref_scores
 
     score_column : str
         score column in the dataframe
 
     decoy_column : str, optional
-        decoy column in the dataframe. 
+        decoy column in the dataframe.
         1=target, 0=decoy. Defaults to 'decoy'.
 
     Returns
     -------
     pd.DataFrame
         dataframe with 'fdr' column added
```

### Comparing `peptdeep-1.1.9/peptdeep/rescore/feature_extractor.py` & `peptdeep-1.2.0/peptdeep/rescore/feature_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,45 +32,45 @@
 ):
     """ Internal function """
     match = PepSpecMatch(
         charged_frag_types=frag_types_to_match
     )
 
     (
-        psm_df, fragment_mz_df, 
+        psm_df, fragment_mz_df,
         matched_intensity_df, matched_mz_err_df
     ) = match.match_ms2_one_raw(
         refine_precursor_df(psm_df_one_raw),
         ms2_file=ms2_file,
-        ms2_file_type=ms2_file_type, 
+        ms2_file_type=ms2_file_type,
         ppm=ms2_ppm, tol=ms2_tol,
     )
 
     if calibrate_frag_mass_error:
         from peptdeep.mass_spec.mass_calibration import (
             MassCalibratorForRT_KNN
         )
         frag_mass_calibrator = MassCalibratorForRT_KNN()
         _df_fdr = psm_df.query("fdr<0.01")
-        
+
         frag_mass_calibrator.fit(
             _df_fdr, matched_mz_err_df
         )
         matched_mz_err_df =  frag_mass_calibrator.calibrate(
             psm_df, matched_mz_err_df
         )
 
     return (
-        psm_df, fragment_mz_df, 
+        psm_df, fragment_mz_df,
         matched_intensity_df, matched_mz_err_df
     )
 
 def get_psm_scores(
     psm_df:pd.DataFrame,
-    predict_intensity_df:pd.DataFrame, 
+    predict_intensity_df:pd.DataFrame,
     matched_intensity_df:pd.DataFrame,
     matched_mass_err_df:pd.DataFrame,
 )->pd.DataFrame:
     """
     AlphaPeptDeep has a built-in score for PSMs,
     it works much better than other scores such as X!Tandem
 
@@ -87,15 +87,15 @@
 
     Returns
     -------
     DataFrame
         `psm_df` with "*_score" columns appended inplace
     """
     matched_norm_intensity_df = pd.DataFrame(
-        np.log(matched_intensity_df.values+1), 
+        np.log(matched_intensity_df.values+1),
         columns=matched_intensity_df.columns.values
     )
     matched_merr_weight_df = matched_mass_err_df.mask(matched_mass_err_df>1000000, 0).abs()
     max_merr = matched_merr_weight_df.values.max()
     if max_merr > 0:
         matched_merr_weight_df /= max_merr
     matched_merr_weight_df = 1-matched_merr_weight_df.pow(4)
@@ -103,15 +103,15 @@
     peak_score_df = matched_norm_intensity_df*matched_merr_weight_df
 
     pred_weighted_score_df = peak_score_df*predict_intensity_df
 
     def _get_one_score(
         frag_start_end,
         peak_score_values,
-        pred_weighted_score_values, 
+        pred_weighted_score_values,
     ):
         frag_start, frag_end = frag_start_end
         frag_ratio = (peak_score_values[frag_start:frag_end]>0).mean()**0.5
         return (
             peak_score_values[frag_start:frag_end].sum()*frag_ratio,
             pred_weighted_score_values[frag_start:frag_end].sum()*frag_ratio
         )
@@ -128,17 +128,17 @@
 
 def get_ms2_features(
     psm_df, frag_types,
     predict_intensity_df,
     matched_intensity_df,
     matched_mass_err_df,
 )->pd.DataFrame:
-    """ Extract ms2 features from the given 
+    """ Extract ms2 features from the given
     predict_intensity_df and matched_intensity_df. It will add columns into psm_df:
-    
+
     - cos: cosine similarity between predicted and matched fragments
     - pcc: pearson correlation between predicted and matched fragments
     - sa: spectral angle between predicted and matched fragments
     - spc: Spearman's rank correlation between predicted and matched fragments.
     - cos_bion: ...
     - cos_yion: ...
     - pcc_bion: ...
@@ -225,42 +225,42 @@
         ].sum()
         if pred_frag_rel_to_matched > 0:
             pred_frag_rel_to_matched /= predicted_inten_values[
                 frag_start:frag_end
             ].sum()
 
         return (
-            matched_frag_num, matched_frag_ratio, 
+            matched_frag_num, matched_frag_ratio,
             both_matched_pred_frag_num,
             both_matched_pred_frag_to_matched,
             both_matched_pred_frag_to_pred,
             matched_not_pred_frag_num,
             matched_not_pred_frag_ratio,
             pred_not_matched_frag_num,
             pred_not_matched_frag_ratio,
             matched_frag_rel_to_pred,
             pred_frag_rel_to_matched,
         )
 
     psm_df, ms2_metrics_df = calc_ms2_similarity(
-        psm_df, predict_intensity_df, 
+        psm_df, predict_intensity_df,
         matched_intensity_df,
         charged_frag_types=used_frag_types,
         metrics=['COS','SA','SPC','PCC'],
         spc_top_k=perc_settings['top_k_frags_to_calc_spc']
     )
     psm_df.rename(
         columns={
             'COS':'cos','SA':'sa','SPC':'spc','PCC':'pcc',
         },
         inplace=True
     )
 
     psm_df = get_psm_scores(
-        psm_df, 
+        psm_df,
         predict_intensity_df=predict_intensity_df[used_frag_types],
         matched_intensity_df=matched_intensity_df[used_frag_types],
         matched_mass_err_df=matched_mass_err_df[used_frag_types]
     )
     psm_df.rename(
         columns={
             'merr_weighted_score':'merr_weighted_frag_score',
@@ -272,56 +272,56 @@
     has_matched_intens=matched_intensity_df[
         used_frag_types
     ].values > 0
     has_predicted_intens=predict_intensity_df[
         used_frag_types
     ].values > 0.001
     has_both_matched_predicted = has_matched_intens&has_predicted_intens
-    
+
     (
         psm_df['matched_frag_num'],
         psm_df['matched_frag_ratio'],
-        psm_df['both_matched_pred_frag_num'], 
+        psm_df['both_matched_pred_frag_num'],
         psm_df['both_matched_pred_frag_to_matched'],
         psm_df['both_matched_pred_frag_to_pred'],
-        psm_df['matched_not_pred_frag_num'], 
+        psm_df['matched_not_pred_frag_num'],
         psm_df['matched_not_pred_frag_ratio'],
         psm_df['pred_not_matched_frag_num'],
         psm_df['pred_not_matched_frag_ratio'],
         psm_df['matched_frag_rel_to_pred'],
         psm_df['pred_frag_rel_to_matched'],
     ) = zip(*psm_df[['frag_start_idx','frag_stop_idx']].apply(
         _get_frag_features, axis=1,
         matched_inten_values=matched_intensity_df[used_frag_types].values,
         predicted_inten_values=predict_intensity_df[used_frag_types].values,
-        has_matched_intens=has_matched_intens, 
+        has_matched_intens=has_matched_intens,
         has_predicted_intens=has_predicted_intens,
         has_both_matched_predicted=has_both_matched_predicted,
     ))
 
     b_frag_types = [
-        _t for _t in used_frag_types 
+        _t for _t in used_frag_types
         if _t.startswith('b')
     ]
     if len(b_frag_types) > 0:
         psm_df, ms2_metrics_df = calc_ms2_similarity(
-            psm_df, predict_intensity_df, 
+            psm_df, predict_intensity_df,
             matched_intensity_df,
             charged_frag_types=b_frag_types,
             metrics=['COS','SA','SPC','PCC'],
         )
         psm_df.rename(
             columns={
                 'COS':'cos_bion','SA':'sa_bion','SPC':'spc_bion',
                 'PCC':'pcc_bion'
             },
             inplace=True
         )
         psm_df = get_psm_scores(
-            psm_df, 
+            psm_df,
             predict_intensity_df=predict_intensity_df[b_frag_types],
             matched_intensity_df=matched_intensity_df[b_frag_types],
             matched_mass_err_df=matched_mass_err_df[b_frag_types]
         )
         psm_df.rename(
             columns={
                 'merr_weighted_score':'merr_weighted_bion_score',
@@ -333,69 +333,69 @@
         has_matched_intens=matched_intensity_df[
             b_frag_types
         ].values>0
         has_predicted_intens=predict_intensity_df[
             b_frag_types
         ].values>0
         has_both_matched_predicted = has_matched_intens&has_predicted_intens
-        
+
         (
             psm_df['matched_bion_num'],
             psm_df['matched_bion_ratio'],
-            psm_df['both_matched_pred_bion_num'], 
+            psm_df['both_matched_pred_bion_num'],
             psm_df['both_matched_pred_bion_to_matched'],
             psm_df['both_matched_pred_bion_to_pred'],
-            psm_df['matched_not_pred_bion_num'], 
+            psm_df['matched_not_pred_bion_num'],
             psm_df['matched_not_pred_bion_ratio'],
             psm_df['pred_not_matched_bion_num'],
             psm_df['pred_not_matched_bion_ratio'],
             psm_df['matched_bion_rel_to_pred'],
             psm_df['pred_bion_rel_to_matched'],
         ) = zip(*psm_df[['frag_start_idx','frag_stop_idx']].apply(
             _get_frag_features, axis=1,
             matched_inten_values=matched_intensity_df[b_frag_types].values,
             predicted_inten_values=predict_intensity_df[b_frag_types].values,
-            has_matched_intens=has_matched_intens, 
+            has_matched_intens=has_matched_intens,
             has_predicted_intens=has_predicted_intens,
             has_both_matched_predicted=has_both_matched_predicted,
         ))
     else:
         psm_df[[
-            'matched_bion_num', 'matched_bion_ratio', 
-            'both_matched_pred_bion_num', 
+            'matched_bion_num', 'matched_bion_ratio',
+            'both_matched_pred_bion_num',
             'both_matched_pred_bion_to_matched',
             'both_matched_pred_bion_to_pred',
-            'matched_not_pred_bion_num', 
+            'matched_not_pred_bion_num',
             'matched_not_pred_bion_ratio',
             'pred_not_matched_bion_num',
             'pred_not_matched_bion_ratio',
             'matched_bion_rel_to_pred',
             'pred_bion_rel_to_matched'
         ]] = 0
 
     y_frag_types = [
-        _t for _t in used_frag_types 
+        _t for _t in used_frag_types
         if _t.startswith('y')
     ]
     if len(y_frag_types) > 0:
         psm_df, ms2_metrics_df = calc_ms2_similarity(
-            psm_df, predict_intensity_df, 
+            psm_df, predict_intensity_df,
             matched_intensity_df,
             charged_frag_types=y_frag_types,
             metrics=['COS','SA','SPC', 'PCC'],
         )
         psm_df.rename(
             columns={
                 'COS':'cos_yion','SA':'sa_yion','SPC':'spc_yion',
                 'PCC':'pcc_yion',
             },
             inplace=True
         )
         psm_df = get_psm_scores(
-            psm_df, 
+            psm_df,
             predict_intensity_df=predict_intensity_df[b_frag_types],
             matched_intensity_df=matched_intensity_df[b_frag_types],
             matched_mass_err_df=matched_mass_err_df[b_frag_types]
         )
         psm_df.rename(
             columns={
                 'merr_weighted_score':'merr_weighted_yion_score',
@@ -407,49 +407,49 @@
         has_matched_intens=matched_intensity_df[
             y_frag_types
         ].values > 0
         has_predicted_intens=predict_intensity_df[
             y_frag_types
         ].values > 0
         has_both_matched_predicted = has_matched_intens&has_predicted_intens
-        
+
         (
             psm_df['matched_yion_num'],
             psm_df['matched_yion_ratio'],
-            psm_df['both_matched_pred_yion_num'], 
+            psm_df['both_matched_pred_yion_num'],
             psm_df['both_matched_pred_yion_to_matched'],
             psm_df['both_matched_pred_yion_to_pred'],
-            psm_df['matched_not_pred_yion_num'], 
+            psm_df['matched_not_pred_yion_num'],
             psm_df['matched_not_pred_yion_ratio'],
             psm_df['pred_not_matched_yion_num'],
             psm_df['pred_not_matched_yion_ratio'],
             psm_df['matched_yion_rel_to_pred'],
             psm_df['pred_yion_rel_to_matched'],
         ) = zip(*psm_df[['frag_start_idx','frag_stop_idx']].apply(
             _get_frag_features, axis=1,
             matched_inten_values=matched_intensity_df[y_frag_types].values,
             predicted_inten_values=predict_intensity_df[y_frag_types].values,
-            has_matched_intens=has_matched_intens, 
+            has_matched_intens=has_matched_intens,
             has_predicted_intens=has_predicted_intens,
             has_both_matched_predicted=has_both_matched_predicted,
         ))
     else:
         psm_df[[
-            'matched_yion_num', 'matched_yion_ratio', 
-            'both_matched_pred_yion_num', 
+            'matched_yion_num', 'matched_yion_ratio',
+            'both_matched_pred_yion_num',
             'both_matched_pred_yion_to_matched',
             'both_matched_pred_yion_to_pred',
-            'matched_not_pred_yion_num', 
+            'matched_not_pred_yion_num',
             'matched_not_pred_yion_ratio',
             'pred_not_matched_yion_num',
             'pred_not_matched_yion_ratio',
             'matched_yion_rel_to_pred',
             'pred_yion_rel_to_matched'
         ]] = 0
-        
+
     def _charge_one_hot(ch):
         x = [0]*7
         if ch>6:
             x[-1] = 1
         else:
             x[ch-1] = 1
         return tuple(x)
@@ -472,30 +472,30 @@
     psm_df['mod_num'] = psm_df.mods.apply(_mod_count)
 
     return psm_df
 
 # for imap/imap_unordered with multiprocessing.Pool()
 def match_one_raw_mp(args):
     return match_one_raw(*args)
-    
+
 # for imap/imap_unordered with multiprocessing.Pool()
 def get_ms2_features_mp(args):
     return get_ms2_features(*args)
 
 
 class ScoreFeatureExtractor:
-    """ ScoreFeatureExtractor: Feature extractor for percolator 
+    """ ScoreFeatureExtractor: Feature extractor for percolator
             with a single process.
 
     Parameters
     ----------
     model_mgr : ModelManager
         The ModelManager in peptdeep.pretrained_models.
     """
-    def __init__(self, 
+    def __init__(self,
         model_mgr:ModelManager
     ):
         self.model_mgr = model_mgr
         self.model_mgr.verbose = False
 
         self.raw_num_to_tune = perc_settings['raw_num_to_tune']
 
@@ -506,39 +506,39 @@
             'rt_delta_abs', 'mobility_delta_abs',
             'merr_weighted_frag_score',
             'pred_weighted_frag_score',
             'merr_weighted_bion_score',
             'pred_weighted_bion_score',
             'merr_weighted_yion_score',
             'pred_weighted_yion_score',
-            'matched_frag_num', 'matched_frag_ratio', 
-            'both_matched_pred_frag_num', 
+            'matched_frag_num', 'matched_frag_ratio',
+            'both_matched_pred_frag_num',
             'both_matched_pred_frag_to_matched',
             'both_matched_pred_frag_to_pred',
-            'matched_not_pred_frag_num', 
+            'matched_not_pred_frag_num',
             'matched_not_pred_frag_ratio',
             'pred_not_matched_frag_num',
             'pred_not_matched_frag_ratio',
             'matched_frag_rel_to_pred',
             'pred_frag_rel_to_matched',
-            'matched_bion_num', 'matched_bion_ratio', 
-            'both_matched_pred_bion_num', 
+            'matched_bion_num', 'matched_bion_ratio',
+            'both_matched_pred_bion_num',
             'both_matched_pred_bion_to_matched',
             'both_matched_pred_bion_to_pred',
-            'matched_not_pred_bion_num', 
+            'matched_not_pred_bion_num',
             'matched_not_pred_bion_ratio',
             'pred_not_matched_bion_num',
             'pred_not_matched_bion_ratio',
             'matched_bion_rel_to_pred',
             'pred_bion_rel_to_matched',
-            'matched_yion_num', 'matched_yion_ratio', 
-            'both_matched_pred_yion_num', 
+            'matched_yion_num', 'matched_yion_ratio',
+            'both_matched_pred_yion_num',
             'both_matched_pred_yion_to_matched',
             'both_matched_pred_yion_to_pred',
-            'matched_not_pred_yion_num', 
+            'matched_not_pred_yion_num',
             'matched_not_pred_yion_ratio',
             'pred_not_matched_yion_num',
             'pred_not_matched_yion_ratio',
             'matched_yion_rel_to_pred',
             'pred_yion_rel_to_matched',
             'pep_z1','pep_z2','pep_z3','pep_z4',
             'pep_z5','pep_z6','pep_z_gt_6',
@@ -560,15 +560,15 @@
         self.calibrate_frag_mass_error = perc_settings[
             'calibrate_frag_mass_error'
         ]
 
     def _select_raw_to_tune(self,
         psm_df:pd.DataFrame,
     )->tuple:
-        """ Randomly select `self.raw_num_to_tune` raw files 
+        """ Randomly select `self.raw_num_to_tune` raw files
         to tune the models. If # raw files is less than `self.raw_num_to_tune`,
         all raw files will be used to tune the model.
 
         Parameters
         ----------
         psm_df : pd.DataFrame
             dataframe contains PSMs of all raw files.
@@ -576,15 +576,15 @@
         Returns
         -------
         df_groupby_raw
             psm_df.groupby('raw_name')
 
         list
             selected raw_name list
-            
+
         """
         if 'fdr' not in psm_df.columns:
             psm_df = calc_fdr_for_df(psm_df, 'score')
         df_fdr = psm_df[(psm_df.fdr<0.01)&(psm_df.decoy==0)]
 
         df_groupby_raw = df_fdr.groupby('raw_name')
 
@@ -627,29 +627,29 @@
             ['b_z1','b_z2','y_z1'...]
 
         ms2_ppm : bool
             is ppm tolerance for ms2 matching
 
         ms2_tol : float
             tolerance value for ms2 matching
-            
+
         """
         logging.info('Preparing for fine-tuning ...')
 
         (
             df_groupby_raw, raw_list
         ) = self._select_raw_to_tune(psm_df)
 
         psm_df_list = []
         matched_intensity_df_list = []
         for raw_name, df in process_bar(
             df_groupby_raw, df_groupby_raw.ngroups
         ):
             if (
-                raw_name not in raw_list 
+                raw_name not in raw_list
                 or raw_name not in ms2_file_dict
             ):
                 continue
             (
                 df, _, inten_df, _
             ) = match_one_raw(
                 df, ms2_file_dict[raw_name],
@@ -670,27 +670,27 @@
             )
         )
         logging.info('Fine-tuning done')
 
     def _save_models(self):
         # save the model for future uses
         model_folder = os.path.join(
-            perc_settings['output_folder'], 
+            perc_settings['output_folder'],
             "tuned_models"
         )
         self.model_mgr.save_models(model_folder)
         with open(os.path.join(
             model_folder, 'grid_instrument_nce_search.txt'
         ), 'w') as f:
             f.write(f"# The ms2 model is tuned for following instrument and nce, after grid instrument and nce search.\n")
             f.write(f"instrument={self.model_mgr.instrument}\n")
             f.write(f"nce={self.model_mgr.nce}\n")
 
     def _tune(self,
-        psm_df, 
+        psm_df,
         matched_intensity_df
     ):
         self.model_mgr.train_ccs_model(psm_df)
         self.model_mgr.train_rt_model(psm_df)
         _grid_nce = self.model_mgr.use_grid_nce_search
         if self.model_mgr.ms2_model.device_type == 'cpu':
             self.model_mgr.use_grid_nce_search = False
@@ -717,15 +717,15 @@
             )
 
             (
                 self.model_mgr.psm_num_to_train_rt_ccs
             ) = perc_settings['psm_num_per_raw_to_tune']
 
             self.model_mgr.psm_num_per_mod_to_train_rt_ccs = 0
-            
+
             (
                 self.model_mgr.epoch_to_train_rt_ccs
             ) = perc_settings['epoch_per_raw_to_tune']
             self.model_mgr.train_rt_model(
                 psm_df[(psm_df.fdr<0.01)&(psm_df.decoy==0)]
             )
 
@@ -767,15 +767,15 @@
     def extract_mobility_features(self, psm_df):
         if (
             'mobility' in psm_df.columns
         ):
             psm_df = self.model_mgr.predict_mobility(
                 psm_df
             )
-            
+
             psm_df[
                 'mobility_delta'
             ] = (
                 psm_df.mobility_pred-psm_df.mobility
             )
 
             mean_delta = psm_df.loc[
@@ -788,15 +788,15 @@
 
             psm_df['mobility_delta_abs'] = (
                 psm_df.mobility_delta-mean_delta
             ).abs()
         else:
             psm_df['mobility_delta'] = 0
             psm_df['mobility_delta_abs'] = 0
-    
+
 
     def match_ms2(self,
         psm_df: pd.DataFrame,
         ms2_file_dict, #raw_name: ms2_file_path or ms_reader object
         ms2_file_type:str,
         frag_types_to_match:list = get_charged_frag_types(['b','y'], 2),
         ms2_ppm=True, ms2_tol=20,
@@ -804,74 +804,74 @@
         self.match = PepSpecMatch(
             charged_frag_types=frag_types_to_match
         )
 
         self.match.match_ms2_centroid(
             refine_precursor_df(psm_df),
             ms2_file_dict=ms2_file_dict,
-            ms2_file_type=ms2_file_type, 
+            ms2_file_type=ms2_file_type,
             ppm=ms2_ppm, tol=ms2_tol,
         )
-        
+
     def _get_model_frag_types(self, frag_types):
         used_frag_types = []
         for frag_type in frag_types:
             if frag_type in (
                 self.model_mgr.ms2_model.charged_frag_types
             ):
                 used_frag_types.append(frag_type)
         return used_frag_types
 
     def extract_features(self,
         psm_df: pd.DataFrame,
-        ms2_file_dict, 
-        ms2_file_type, 
+        ms2_file_dict,
+        ms2_file_type,
         frag_types:list = get_charged_frag_types(['b','y'], 2),
-        ms2_ppm=global_settings['peak_matching']['ms2_ppm'], 
+        ms2_ppm=global_settings['peak_matching']['ms2_ppm'],
         ms2_tol=global_settings['peak_matching']['ms2_tol_value'],
     )->pd.DataFrame:
         """ Extract features and add columns (`self.score_feature_list`) into psm_df
 
         Parameters
         ----------
         psm_df : pd.DataFrame
             psm dataframe to extract features
 
         ms2_file_dict : [type]
             MS2 file path dict: {raw_name: ms2_path}
 
         ms2_file_type : str, optional
-            MS2 file type, coult be 
+            MS2 file type, coult be
             'alphapept', 'mgf', or 'raw'.
 
         frag_types : list, optional
-            fragment types. 
+            fragment types.
             Defaults to `alphabase.fragment.get_charged_frag_types(['b','y'], 2)`.
 
         ms2_ppm : bool, optional
-            Matching MS2 mass tolerance unit. 
+            Matching MS2 mass tolerance unit.
             Defaults to True.
 
         ms2_tol : int, optional
-            Matching mass tolerance. 
+            Matching mass tolerance.
             Defaults to 20.
 
         Returns
         -------
         pd.DataFrame
             psm_df with feature columns added
 
         """
-        
+
         frag_types = self._get_model_frag_types(frag_types)
 
         if self.require_model_tuning:
             logging.info('Fine-tuning models ...')
             self.fine_tune_models(
-                psm_df, 
+                psm_df,
                 ms2_file_dict, ms2_file_type,
                 frag_types, ms2_ppm, ms2_tol
             )
 
         logging.info(f'Extracting peptdeep features for {len(psm_df)} PSMs ...')
         result_psm_list = []
         groupby = psm_df.groupby('raw_name')
@@ -892,33 +892,33 @@
             self.extract_rt_features(df)
             self.extract_mobility_features(df)
 
             predict_inten_df = self.model_mgr.predict_ms2(df)
 
             result_psm_list.append(
                 get_ms2_features(
-                    df, frag_types, 
+                    df, frag_types,
                     predict_inten_df,
                     frag_inten_df,
                     frag_merr_df,
                 )
             )
-            
+
         self.psm_df = pd.concat(
             result_psm_list, ignore_index=True
         )
         logging.info('Finish extracting features')
         return self.psm_df
-        
+
 
 class ScoreFeatureExtractorMP(ScoreFeatureExtractor):
-    def __init__(self, 
+    def __init__(self,
         model_mgr:ModelManager
     ):
-        """ ScoreFeatureExtractorMP: Feature extractor for percolator 
+        """ ScoreFeatureExtractorMP: Feature extractor for percolator
               with multiprocessing.
 
         Parameters
         ----------
         model_mgr : ModelManager
             The ModelManager in peptdeep.pretrained_models.
 
@@ -965,35 +965,35 @@
         (
             df_groupby_raw, raw_list
         ) = self._select_raw_to_tune(psm_df)
 
         def one_raw_param_generator(df_groupby_raw):
             for raw_name, df in df_groupby_raw:
                 if (
-                    raw_name not in raw_list 
+                    raw_name not in raw_list
                     or raw_name not in ms2_file_dict
                 ):
                     continue
 
                 yield (
                     df,
                     ms2_file_dict[raw_name],
                     ms2_file_type,
                     frag_types_to_match,
                     ms2_ppm, ms2_tol,
                     self.calibrate_frag_mass_error,
                 )
-        
-        logging.info('Preparing for fine-tuning ...')  
+
+        logging.info('Preparing for fine-tuning ...')
         psm_df_list = []
-        matched_intensity_df_list = []  
+        matched_intensity_df_list = []
         with mp.get_context('spawn').Pool(global_settings['thread_num']) as p:
             for df, _, inten_df, _ in process_bar(
                 p.imap_unordered(
-                    match_one_raw_mp, 
+                    match_one_raw_mp,
                     one_raw_param_generator(df_groupby_raw)
                 ), df_groupby_raw.ngroups
             ):
                 psm_df_list.append(df)
                 matched_intensity_df_list.append(inten_df)
 
         logging.info('Fine-tuning ...')
@@ -1006,87 +1006,87 @@
         )
 
     def extract_features_one_raw_mp(self,args):
         return self.extract_features_one_raw(*args)
 
     def extract_features_one_raw(self,
         df_one_raw: pd.DataFrame,
-        ms2_file, 
+        ms2_file,
         ms2_file_type,
         frag_types,
         ms2_ppm, ms2_tol,
         calibrate_frag_mass_error,
     ):
         (
             df, frag_mz_df, frag_inten_df, frag_merr_df
-        ) = match_one_raw(df_one_raw, 
+        ) = match_one_raw(df_one_raw,
             ms2_file, ms2_file_type, frag_types,
             ms2_ppm, ms2_tol,
             calibrate_frag_mass_error,
         )
 
         self.extract_rt_features(df)
         self.extract_mobility_features(df)
 
         predict_inten_df = self.model_mgr.predict_ms2(df)
 
-        return get_ms2_features(df, 
-            frag_types, 
+        return get_ms2_features(df,
+            frag_types,
             predict_inten_df,
             frag_inten_df,
             frag_merr_df,
         )
 
     def extract_features(self,
         psm_df: pd.DataFrame,
         ms2_file_dict,
         ms2_file_type,
         frag_types:list = get_charged_frag_types(['b','y'], 2),
-        ms2_ppm=global_settings['peak_matching']['ms2_ppm'], 
+        ms2_ppm=global_settings['peak_matching']['ms2_ppm'],
         ms2_tol=global_settings['peak_matching']['ms2_tol_value'],
     )->pd.DataFrame:
-        """ Extract (multiprocessing) features and 
+        """ Extract (multiprocessing) features and
         add columns (self.score_feature_list) into psm_df.
 
         Parameters
         ----------
         psm_df : pd.DataFrame
             psm dataframe to extract features
 
         ms2_file_dict : [type]
             MS2 file path dict: {raw_name: ms2_path}
 
         ms2_file_type : str, optional
-            MS2 file type, coult be 
+            MS2 file type, coult be
             'alphapept', 'mgf', or 'thermo'.
 
         frag_types : list, optional
-            fragment types. 
+            fragment types.
             Defaults to `alphabase.fragment.get_charged_frag_types(['b','y'], 2)`.
 
         ms2_ppm : bool, optional
-            Matching MS2 mass tolerance unit. 
+            Matching MS2 mass tolerance unit.
             Defaults to True.
 
         ms2_tol : int, optional
-            Matching mass tolerance. 
+            Matching mass tolerance.
             Defaults to 20.
 
         Returns
         -------
         pd.DataFrame
             psm_df with feature columns added
         """
 
         used_frag_types = self._get_model_frag_types(frag_types)
 
         if self.require_model_tuning:
             logging.info('Require fine-tuning models ...')
             self.fine_tune_models(
-                psm_df, 
+                psm_df,
                 ms2_file_dict, ms2_file_type,
                 used_frag_types, ms2_ppm, ms2_tol
             )
 
         self.model_mgr._train_psm_logging = False
 
         def one_raw_param_generator(df_groupby_raw):
@@ -1107,36 +1107,36 @@
         )
         df_groupby_raw = psm_df.groupby('raw_name')
         result_psm_list = []
 
         if (
             self.require_raw_specific_tuning or
             self.model_mgr.ms2_model.device_type!='cpu'
-            
+
         ):
             # multiprocessing is only used for ms2 matching
             def prediction_gen(df_groupby_raw):
                 with mp.get_context('spawn').Pool(global_settings['thread_num']) as _p:
                     for (
                         df, frag_mz_df, frag_inten_df, frag_merr_df
                     ) in _p.imap_unordered(
-                        match_one_raw_mp, 
+                        match_one_raw_mp,
                         one_raw_param_generator(df_groupby_raw)
                     ):
                         # outsite multiprocessing region
                         self.extract_rt_features(df)
                         self.extract_mobility_features(df)
 
                         if (
-                            self.require_raw_specific_tuning 
+                            self.require_raw_specific_tuning
                             and self.raw_specific_ms2_tuning
                         ):
                             (
-                                psm_num_to_train_ms2, 
-                                psm_num_per_mod_to_train_ms2, 
+                                psm_num_to_train_ms2,
+                                psm_num_per_mod_to_train_ms2,
                                 epoch_to_train_ms2,
                                 use_grid_nce_search
                             ) = (
                                 self.model_mgr.psm_num_to_train_ms2,
                                 self.model_mgr.psm_num_per_mod_to_train_ms2,
                                 self.model_mgr.epoch_to_train_ms2,
                                 self.model_mgr.use_grid_nce_search
@@ -1162,41 +1162,41 @@
 
                             (
                                 self.model_mgr.psm_num_to_train_ms2,
                                 self.model_mgr.psm_num_per_mod_to_train_ms2,
                                 self.model_mgr.epoch_to_train_ms2,
                                 self.model_mgr.use_grid_nce_search
                             ) = (
-                                psm_num_to_train_ms2, 
-                                psm_num_per_mod_to_train_ms2, 
+                                psm_num_to_train_ms2,
+                                psm_num_per_mod_to_train_ms2,
                                 epoch_to_train_ms2,
                                 use_grid_nce_search
                             )
-                            
+
                         predict_inten_df = self.model_mgr.predict_ms2(df)
 
                         yield (
-                            df, used_frag_types, 
+                            df, used_frag_types,
                             predict_inten_df,
                             frag_inten_df, frag_merr_df,
                         )
 
             with mp.get_context('spawn').Pool(global_settings['thread_num']) as p:
                 for df in process_bar(p.imap_unordered(
-                    get_ms2_features_mp, 
+                    get_ms2_features_mp,
                     prediction_gen(df_groupby_raw)
                 ), df_groupby_raw.ngroups):
                     result_psm_list.append(df)
 
         else:
-            # use multiprocessing for prediction 
+            # use multiprocessing for prediction
             # only when no GPUs are available
             with mp.get_context('spawn').Pool(global_settings['thread_num']) as p:
                 for _df in process_bar(p.imap_unordered(
-                    self.extract_features_one_raw_mp, 
+                    self.extract_features_one_raw_mp,
                     one_raw_param_generator(df_groupby_raw)
                 ), df_groupby_raw.ngroups):
                     result_psm_list.append(_df)
 
         self.psm_df = pd.concat(
             result_psm_list, ignore_index=True
         )
```

### Comparing `peptdeep-1.1.9/peptdeep/rescore/percolator.py` & `peptdeep-1.2.0/peptdeep/rescore/percolator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import torch
 import os
 import multiprocessing as mp
 from tqdm import tqdm
 
 from alphabase.peptide.fragment import get_charged_frag_types
-from alphabase.io.psm_reader import psm_reader_provider
+from alphabase.psm_reader import psm_reader_provider
 
 from peptdeep.rescore.feature_extractor import (
     ScoreFeatureExtractor,
     ScoreFeatureExtractorMP
 )
 
 from peptdeep.rescore.fdr import (
@@ -60,29 +60,29 @@
 class NNRescore:
     def __init__(self, num_features, nn_model_type='linear'):
         self.nn_model = rescore_model_provider.get_model(
             nn_model_type, num_features
         )
         self.train_batch_size = 10000
         self.predict_batch_size = 100000
-            
+
         self.optimizer = torch.optim.Adam(
-            self.nn_model.parameters(), 
+            self.nn_model.parameters(),
             lr=perc_settings['lr_percolator_torch_model']
         )
         self.loss_func = torch.nn.BCEWithLogitsLoss()
 
         if torch.cuda.is_available():
             self.device = torch.device('cuda')
             self.nn_model.to(self.device)
         else:
             self.device = torch.device('cpu')
         self.epoch = 20
 
-    
+
 
     def fit(self, features, labels):
         labels = torch.tensor(
             labels, dtype=torch.float, device=self.device
         )
         sample_idxes = np.random.RandomState(
             1337
@@ -127,54 +127,54 @@
     """
     def __init__(self,
         *,
         percolator_model:str=perc_settings['percolator_model'],
         percolator_backend:str=perc_settings['percolator_backend'],
         cv_fold:int = perc_settings['cv_fold'],
         iter_num:int = perc_settings['percolator_iter_num'],
-        ms2_ppm:bool = global_settings['peak_matching']['ms2_ppm'], 
+        ms2_ppm:bool = global_settings['peak_matching']['ms2_ppm'],
         ms2_tol:float = global_settings['peak_matching']['ms2_tol_value'],
         model_mgr:ModelManager = None
     ):
         """
         Parameters
         ----------
         percolator_model : str, optional
-            machine learning 
+            machine learning
             model type for rescoring, could be:
             "linear": logistic regression
             "random_forest": random forest
             Defaults to perc_settings['percolator_model'].
 
         percolator_backend : str, optional
             `sklearn` or `pytorch`.
             Defaults to perc_settings['percolator_backend']
 
         cv_fold : int, optional
-            cross-validation fold. 
+            cross-validation fold.
             Defaults to perc_settings['cv_fold'].
 
         iter_num : int, optional
-            percolator iteration number. 
+            percolator iteration number.
             Defaults to perc_settings['percolator_iter_num'].
 
         ms2_ppm : bool, optional
-            is ms2 tolerance the ppm. 
+            is ms2 tolerance the ppm.
             Defaults to perc_settings['ms2_ppm'].
 
         ms2_tol : float, optional
-            ms2 tolerance. 
+            ms2 tolerance.
             Defaults to perc_settings['ms2_tol'].
 
         model_mgr : ModelManager, optional
             peptdeep.pretrained_model.ModelManager.
             If None, self.model_mgr will be init by default (see `peptdeep.pretrained_models.ModelManager`).
             Defaults to None.
         """
-        
+
         if model_mgr is None:
             self.model_mgr = ModelManager()
         else:
             self.model_mgr = model_mgr
         self.charged_frag_types = perc_settings['frag_types']
         self.ms2_ppm = ms2_ppm
         self.ms2_tol = ms2_tol
@@ -198,16 +198,16 @@
 
         self.max_train_sample = perc_settings['max_perc_train_sample']
         self.min_train_sample = perc_settings['min_perc_train_sample']
         self.per_raw_fdr = perc_settings['use_fdr_for_each_raw']
 
         self.init_percolator_model(percolator_model, percolator_backend)
 
-    def init_percolator_model(self, 
-        percolator_model="linear", 
+    def init_percolator_model(self,
+        percolator_model="linear",
         percolator_backend="sklearn"
     ):
         from sklearn.ensemble import RandomForestClassifier
         from sklearn.linear_model import LogisticRegression
         self.percolator_model = percolator_model.lower()
         self.percolator_backend = percolator_backend.lower()
         if percolator_backend.lower() == 'pytorch':
@@ -232,34 +232,34 @@
             )
             self.percolator_model = 'linear'
             self.percolator_backend = 'sklearn'
 
     def enable_model_fine_tuning(self, flag=True):
         self.feature_extractor.require_model_tuning = flag
         self.feature_extractor.require_raw_specific_rt_tuning = flag
-    
+
     def disable_model_fine_tuning(self):
         self.feature_extractor.require_model_tuning = False
         self.feature_extractor.require_raw_specific_rt_tuning = False
 
-    def _estimate_fdr(self, 
+    def _estimate_fdr(self,
         df:pd.DataFrame,
         fdr_level:str=None,
         per_raw_fdr:bool=None,
     )->pd.DataFrame:
         df = df.sort_values(['ml_score','decoy'], ascending=False)
         df = df.reset_index(drop=True)
-        if fdr_level is None: 
+        if fdr_level is None:
             fdr_level = self.fdr_level
-        if per_raw_fdr is None: 
+        if per_raw_fdr is None:
             per_raw_fdr = self.per_raw_fdr
         if per_raw_fdr:
             df_list = []
             for raw_name, df_raw in df.groupby('raw_name'):
-                df_list.append(self._estimate_fdr(df_raw, 
+                df_list.append(self._estimate_fdr(df_raw,
                     fdr_level = fdr_level,
                     per_raw_fdr = False
                 ))
             return pd.concat(df_list)
         if fdr_level == 'psm':
             target_values = 1-df['decoy'].values
             decoy_cumsum = np.cumsum(df['decoy'].values)
@@ -281,37 +281,37 @@
             _df = _df.sort_values(['ml_score','decoy'], ascending=False)
             target_values = 1-_df['decoy'].values
             decoy_cumsum = np.cumsum(_df['decoy'].values)
             target_cumsum = np.cumsum(target_values)
             fdr_values = decoy_cumsum/target_cumsum
             _df['fdr'] = fdr_to_q_values(fdr_values)
             df['fdr'] = fdr_from_ref(
-                df['ml_score'].values, _df['ml_score'].values, 
+                df['ml_score'].values, _df['ml_score'].values,
                 _df['fdr'].values
             )
         return df
 
     def _train(self, train_t_df, train_d_df):
         if len(train_t_df) > self.max_train_sample:
             train_t_df = train_t_df.sample(
-                n=self.max_train_sample, 
+                n=self.max_train_sample,
                 random_state=1337
             )
         if len(train_d_df) > self.max_train_sample:
             train_d_df = train_d_df.sample(
                 n=self.max_train_sample,
                 random_state=1337
             )
 
         train_df = pd.concat((train_t_df, train_d_df))
         train_label = np.ones(len(train_df),dtype=np.int32)
         train_label[len(train_t_df):] = 0
 
         self.model.fit(
-            train_df[self.feature_list].values, 
+            train_df[self.feature_list].values,
             train_label
         )
 
     def _predict(self, test_df):
         if self.percolator_model != 'random_forest':
             test_df['ml_score'] = self.model.decision_function(
                 test_df[self.feature_list].values
@@ -325,59 +325,59 @@
     def _cv_score(self, df:pd.DataFrame)->pd.DataFrame:
         df = df.sample(
             frac=1, random_state=1337
         ).reset_index(drop=True)
         df_target = df[df.decoy == 0]
         df_decoy = df[df.decoy != 0]
         if (
-            np.sum(df_target.fdr<0.01) < 
-            self.min_train_sample*self.cv_fold 
+            np.sum(df_target.fdr<0.01) <
+            self.min_train_sample*self.cv_fold
             or len(df_decoy) < self.min_train_sample*self.cv_fold
         ):
             logging.info(
                 "[PERC] "
                 f'#target={np.sum(df_target.fdr<0.01)} or #decoy={len(df_decoy)} '
                 f'< minimal training sample={self.min_train_sample} '
                 f'for cv-fold={self.cv_fold}. Skip rescoring!!!'
             )
             return df
-        
+
         if self.cv_fold > 1:
             test_df_list = []
             for i in range(self.cv_fold):
                 t_mask = np.ones(len(df_target), dtype=bool)
                 _slice = slice(i, len(df_target), self.cv_fold)
                 t_mask[_slice] = False
                 cv_df_target = df_target[t_mask]
                 train_t_df = cv_df_target[
                     cv_df_target.fdr <= self.fdr
                 ]
                 test_t_df = df_target[_slice]
-                
+
                 d_mask = np.ones(len(df_decoy), dtype=bool)
                 _slice = slice(i, len(df_decoy), self.cv_fold)
                 d_mask[_slice] = False
                 train_d_df = df_decoy[d_mask]
                 test_d_df = df_decoy[_slice]
 
                 self._train(train_t_df, train_d_df)
 
                 test_df = pd.concat((test_t_df, test_d_df))
                 test_df_list.append(self._predict(test_df))
-        
+
             return pd.concat(test_df_list)
         else:
             train_t_df = df_target[df_target.fdr <= self.fdr]
 
             self._train(train_t_df, df_decoy)
             test_df = pd.concat((df_target, df_decoy))
-        
+
             return self._predict(test_df)
 
-    def load_psms(self, 
+    def load_psms(self,
         psm_file_list:list, psm_type:str
     )->pd.DataFrame:
         """Load PSM dataframe from file path list.
 
         Parameters
         ----------
         psm_file_list : list
@@ -385,15 +385,15 @@
 
         psm_type : str
             PSM type, could be alphapept, pfind, ...
 
         Returns
         -------
         pd.DataFrame
-            PSM dataframe with 100% FDR including decoys. 
+            PSM dataframe with 100% FDR including decoys.
         """
         reader = psm_reader_provider.get_reader(
             psm_type, fdr=1, keep_decoy=True
         )
         psm_df_list = []
         for psm_file in psm_file_list:
             _df = reader.import_file(psm_file)
@@ -421,17 +421,17 @@
         -------
         pd.DataFrame
             psm_df with feature columns appended inplace.
         """
         psm_df['ml_score'] = psm_df.score
         psm_df = self._estimate_fdr(psm_df, 'psm')
         psm_df = self.feature_extractor.extract_features(
-            psm_df, ms2_file_dict, 
+            psm_df, ms2_file_dict,
             ms2_file_type,
-            frag_types=self.charged_frag_types, 
+            frag_types=self.charged_frag_types,
             ms2_ppm=self.ms2_ppm, ms2_tol=self.ms2_tol
         )
 
         return psm_df
 
     def re_score(self, df:pd.DataFrame)->pd.DataFrame:
         """Rescore
```

### Comparing `peptdeep-1.1.9/peptdeep/settings.py` & `peptdeep-1.2.0/peptdeep/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from peptdeep.constants._const import CONST_FOLDER
 
 global_settings = load_yaml(
     os.path.join(CONST_FOLDER, 'default_settings.yaml')
 )
 """
-Global settings in peptdeep, 
+Global settings in peptdeep,
 it controls all functionalities of PeptDeep.
 """
 
 model_const = load_yaml(
     os.path.join(CONST_FOLDER, 'model_const.yaml')
 )
 
@@ -51,23 +51,23 @@
 
 
 def add_user_defined_modifications(
     user_mods:dict=None
 ):
     """
     Add user-defined modifications into the system,
-    this is userful for isotope labeling. 
+    this is userful for isotope labeling.
 
     Parameters
     ----------
     user_mods : dict, optional
         Example:
         ```
         {
-        "Dimethyl2@Any N-term": { 
+        "Dimethyl2@Any N-term": {
         "composition": "H(2)2H(2)C(2)",
         "modloss_composition": ""
         }, ...
         }
         ```
         Set as `global_settings["user_defined_modifications"]` if it is None.
         By default None.
@@ -124,19 +124,19 @@
     update_settings(global_settings, new_settings)
     _refine_global_settings()
 
 def load_global_settings(yaml:str):
     d = load_yaml(yaml)
     update_global_settings(d)
 
-def update_modifications(tsv:str="", 
+def update_modifications(tsv:str="",
     modloss_importance_level:float=1.0
 ):
     """
-    Load modification tsv either from alphabase default 
+    Load modification tsv either from alphabase default
     `modification.tsv <https://github.com/MannLabs/alphabase/blob/main/alphabase/constants/const_files/modification.tsv>`_
     or an external tsv file.
 
     Parameters
     ----------
     tsv : str, optional
         External modification tsv file, "" refers to the default alphabase tsv,
@@ -144,11 +144,11 @@
     modloss_importance_level : float, optional
         Only keep the important modification losses, by default 1.0
     """
     if os.path.isfile(tsv):
         load_mod_df(tsv, modloss_importance_level=modloss_importance_level)
     else:
         keep_modloss_by_importance(modloss_importance_level)
-    
+
     add_user_defined_modifications()
 
-update_modifications()
+update_modifications()
```

### Comparing `peptdeep-1.1.9/peptdeep/spec_lib/library_factory.py` & `peptdeep-1.2.0/peptdeep/spec_lib/library_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from peptdeep.pretrained_models import ModelManager
 from peptdeep.utils import logging,read_peptide_table
 
 class PredictLibraryMakerBase(object):
     """
     Base class to predict libraries
     """
-    def __init__(self, 
+    def __init__(self,
         model_manager:ModelManager = None,
     ):
         lib_settings = global_settings['library']
         self.spec_lib = PredictSpecLibFasta(
             model_manager=model_manager,
             charged_frag_types = get_charged_frag_types(
                 lib_settings['frag_types'],
@@ -34,15 +34,15 @@
             ),
             protease = lib_settings['fasta']['protease'],
             max_missed_cleavages = lib_settings['fasta']['max_miss_cleave'],
             peptide_length_min = lib_settings['min_peptide_len'],
             peptide_length_max = lib_settings['max_peptide_len'],
             precursor_charge_min = lib_settings['min_precursor_charge'],
             precursor_charge_max = lib_settings['max_precursor_charge'],
-            precursor_mz_min = lib_settings['min_precursor_mz'], 
+            precursor_mz_min = lib_settings['min_precursor_mz'],
             precursor_mz_max = lib_settings['max_precursor_mz'],
             var_mods = lib_settings['var_mods'],
             min_var_mod_num = lib_settings['min_var_mod_num'],
             max_var_mod_num = lib_settings['max_var_mod_num'],
             fix_mods = lib_settings['fix_mods'],
             labeling_channels = lib_settings['labeling_channels'],
             special_mods = lib_settings['special_mods'],
@@ -76,15 +76,15 @@
         return self.spec_lib.fragment_intensity_df
 
     @property
     def fragment_mz_df(self)->pd.DataFrame:
         return self.spec_lib.fragment_mz_df
 
     def make_library(self, infiles:Union[str,list,pd.DataFrame]):
-        """Predict a library for the `infiles`, 
+        """Predict a library for the `infiles`,
         this function runs the following methods.
 
         - self._input(infiles)
         - self._check_df()
         - self._predict()
 
         Parameters
@@ -108,29 +108,29 @@
                 'Predicting the spectral library with '
                 f'{len(self.precursor_df)} precursors '
                 f'and {np.prod(self.fragment_mz_df.values.shape, dtype=float)*(1e-6):.2f}M fragments '
                 f'used {psutil.Process(os.getpid()).memory_info().rss/1024**3:.4f} GB memory'
             )
         except ValueError as e:
             raise e
-    
-    def translate_to_tsv(self, 
-        tsv_path:str, 
+
+    def translate_to_tsv(self,
+        tsv_path:str,
         translate_mod_dict:dict=None
     ):
         """Translate the predicted DataFrames into a TSV file
         """
         logging.info(f"Translating to {tsv_path} for DiaNN/Spectronaut...")
         lib_settings = global_settings['library']
 
         if 'proteins' not in self.spec_lib._precursor_df.columns:
             self.spec_lib.append_protein_name()
-        
+
         translate_to_tsv(
-            self.spec_lib, 
+            self.spec_lib,
             tsv_path,
             keep_k_highest_fragments=lib_settings['output_tsv'][
                 'keep_higest_k_peaks'
             ],
             min_frag_intensity=lib_settings['output_tsv'][
                 'min_relative_intensity'
             ],
@@ -141,29 +141,29 @@
                 'max_fragment_mz'
             ],
             batch_size=lib_settings['output_tsv'][
                 'translate_batch_size'
             ],
             translate_mod_dict=translate_mod_dict,
         )
-    
-    def translate_library(self, 
+
+    def translate_library(self,
         translate_mod_dict:dict=None
     )->pd.DataFrame:
-        """Translate predicted DataFrames into 
+        """Translate predicted DataFrames into
         a single DataFrame in SWATH library format
         """
         logging.info("Translating library for DiaNN/Spectronaut...")
         lib_settings = global_settings['library']
 
         if 'proteins' not in self.spec_lib._precursor_df.columns:
             self.spec_lib.append_protein_name()
-        
+
         return speclib_to_single_df(
-            self.spec_lib, 
+            self.spec_lib,
             translate_mod_dict=translate_mod_dict,
             keep_k_highest_fragments=lib_settings['output_tsv'][
                 'keep_higest_k_peaks'
             ],
             min_frag_intensity=lib_settings['output_tsv'][
                 'min_relative_intensity'
             ],
@@ -172,15 +172,15 @@
             ],
             max_frag_mz=lib_settings['output_tsv'][
                 'max_fragment_mz'
             ],
         )
 
 def load_dfs(infiles):
-    if isinstance(infiles,str): infiles = [infiles] 
+    if isinstance(infiles,str): infiles = [infiles]
     df_list = []
     for file_path in infiles:
         df_list.append(read_peptide_table(file_path))
     return pd.concat(df_list, ignore_index=True)
 
 class PSMReaderLibraryMaker(PredictLibraryMakerBase):
     def _input(self, psm_type_infiles:Tuple[str,Union[str,list]]):
@@ -212,22 +212,22 @@
             df = load_dfs(infiles)
         if 'charge' not in df.columns:
             raise KeyError('`precursor_table` must contain the "charge" column.')
         df.drop_duplicates(["sequence","mods","mod_sites","charge"],inplace=True)
         self.spec_lib._precursor_df = df
         self.spec_lib.add_peptide_labeling()
         self.spec_lib.append_decoy_sequence()
-    
+
     def _check_df(self):
         (
             self.spec_lib.precursor_df['charge']
         ) = self.spec_lib.precursor_df['charge'].astype(np.int8)
 
         if (
-            'mods' not in self.spec_lib.precursor_df.columns or 
+            'mods' not in self.spec_lib.precursor_df.columns or
             'mod_sites' not in self.spec_lib.precursor_df.columns
         ):
             self.spec_lib.precursor_df['mods'] = ''
             self.spec_lib.precursor_df['mod_sites'] = ''
         else:
             (
                 self.spec_lib.precursor_df['mods']
@@ -303,8 +303,8 @@
 library_maker_provider.register_maker('precursor_table', PrecursorLibraryMaker)
 library_maker_provider.register_maker('precursor_library', PrecursorLibraryMaker)
 library_maker_provider.register_maker('peptide_table', PeptideLibraryMaker)
 library_maker_provider.register_maker('peptide_library', PeptideLibraryMaker)
 library_maker_provider.register_maker('sequence_table', SequenceLibraryMaker)
 library_maker_provider.register_maker('sequence_library', SequenceLibraryMaker)
 library_maker_provider.register_maker('fasta', FastaLibraryMaker)
-library_maker_provider.register_maker('fasta_library', FastaLibraryMaker)
+library_maker_provider.register_maker('fasta_library', FastaLibraryMaker)
```

### Comparing `peptdeep-1.1.9/peptdeep/spec_lib/predict_lib.py` & `peptdeep-1.2.0/peptdeep/spec_lib/predict_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 model_mgr_settings = global_settings['model_mgr']
 
 class PredictSpecLib(SpecLibBase):
     def __init__(self,
         model_manager: ModelManager = None,
         charged_frag_types = ['b_z1','b_z2','y_z1','y_z2'],
-        precursor_mz_min:float = 400.0, 
+        precursor_mz_min:float = 400.0,
         precursor_mz_max:float = 2000.0,
         decoy:str = 'pseudo_reverse',
         rt_to_irt:bool = False,
         generate_precursor_isotope:bool = False,
     ):
         """
         Parameters
@@ -41,15 +41,15 @@
         precursor_mz_min : float, optional
             precursor_mz_min, by default 400.0
 
         precursor_mz_max : float, optional
             precursor_mz_max, by default 2000.0
 
         decoy : str, optional
-            Decoy choice, see `alphabase.spec_lib.decoy_library`, 
+            Decoy choice, see `alphabase.spec_lib.decoy_library`,
             by default 'pseudo_reverse'
 
         rt_to_irt : bool, optional
             Convert predicted RT to iRT values, by default False
 
         generate_precursor_isotope : bool, optional
             Generate precursor isotopes, defaults to False
@@ -77,38 +77,38 @@
         fragment_intensity_df: pd.DataFrame,
     ):
         self._precursor_df = precursor_df
         self._fragment_intensity_df = fragment_intensity_df
         self._fragment_mz_df = fragment_mz_df
 
         self._fragment_mz_df.drop(columns=[
-            col for col in self._fragment_mz_df.columns 
+            col for col in self._fragment_mz_df.columns
             if col not in self.charged_frag_types
         ], inplace=True)
 
         self._fragment_intensity_df.drop(columns=[
-            col for col in self._fragment_intensity_df.columns 
+            col for col in self._fragment_intensity_df.columns
             if col not in self.charged_frag_types
         ], inplace=True)
 
     def translate_rt_to_irt_pred(self, irt_pep_df:pd.DataFrame = None):
         """ Add 'irt_pred' into columns based on 'rt_pred' """
         return self.model_manager.rt_model.add_irt_column_to_precursor_df(
             self._precursor_df, irt_pep_df=irt_pep_df
         )
 
-    def predict_all(self, 
+    def predict_all(self,
         min_required_precursor_num_for_mp:int=2000,
         predict_items:list = ['rt','mobility','ms2'],
     ):
         """
         1. Predict RT/IM/MS2 for self._precursor_df
         2. Calculate isotope information in self._precursor_df
         """
-        if 'precursor_mz' not in self.precursor_df.columns: 
+        if 'precursor_mz' not in self.precursor_df.columns:
             self.calc_precursor_mz()
             self.clip_by_precursor_mz_()
         if self.generate_precursor_isotope:
             if self.model_manager.verbose:
                 logging.info('Calculating precursor isotope distributions ...')
             if len(self.precursor_df) < min_required_precursor_num_for_mp:
                 self._precursor_df = calc_precursor_isotope(
@@ -130,44 +130,44 @@
             process_num=global_settings['thread_num'],
         )
         self.set_precursor_and_fragment(**res)
         if self.rt_to_irt and 'rt_pred' in self._precursor_df.columns:
             self.translate_rt_to_irt_pred()
         if self.model_manager.verbose:
             logging.info('End predicting RT/IM/MS2')
-        
+
 
 class PredictSpecLibFlat(SpecLibFlat):
-    """ 
-    Flatten the predicted spectral library, the key feature is to 
+    """
+    Flatten the predicted spectral library, the key feature is to
     predict and flatten fragments in batch with `predict_and_parse_lib_in_batch()`
 
     Parameters
     ----------
     min_fragment_intensity : float, optional
         minimal intensity to keep, by default 0.001
     keep_top_k_fragments : int, optional
         top k highest peaks to keep, by default 1000
     """
-    def __init__(self, 
+    def __init__(self,
         min_fragment_intensity:float = 0.001,
         keep_top_k_fragments:int = 1000,
         custom_fragment_df_columns:list = [
             'type','number','position','charge','loss_type'
         ],
         **kwargs,
     ):
         super().__init__(
             min_fragment_intensity=min_fragment_intensity,
             keep_top_k_fragments=keep_top_k_fragments,
             custom_fragment_df_columns=custom_fragment_df_columns
         )
 
-    def predict_and_parse_lib_in_batch(self, 
-        predict_lib:PredictSpecLib, 
+    def predict_and_parse_lib_in_batch(self,
+        predict_lib:PredictSpecLib,
         batch_size:int = 200000
     ):
         """Predict and flatten fragments in batch
 
         Parameters
         ----------
         predict_lib : PredictSpecLib
@@ -198,9 +198,7 @@
                 )
                 precursor_df_list.append(flat_df)
                 fragment_df_list.append(frag_df)
             predict_lib._precursor_df = df
             self._precursor_df, self._fragment_df = concat_precursor_fragment_dataframes(
                 precursor_df_list, fragment_df_list
             )
-
-
```

### Comparing `peptdeep-1.1.9/peptdeep/utils/__init__.py` & `peptdeep-1.2.0/peptdeep/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     return df
 
 _special_raw_suffices = [
     '.ms_data.hdf',
     '_hcdft.mgf',
     '.mzml'
     '.mgf'
-]   
+]
 
 def parse_ms_file_names_to_dict(
     ms_file_list:list
 )->dict:
     """
     Load spectrum file paths into a dict:
         "/Users/xxx/raw_name.raw" -> {"raw_name":"/Users/xxx/raw_name.raw"}
@@ -86,8 +86,7 @@
     except ValueError:
         # pandas <= 1.2.x?
         logging.warn(f'pandas=={pd.__version__} cannot explode multiple columns')
         ret_df = df.explode(columns[0])
         for col in columns[1:]:
             ret_df[col] = _flatten(df[col].values)
         return ret_df
-
```

### Comparing `peptdeep-1.1.9/peptdeep/utils/_pyinstaller_hooks.py` & `peptdeep-1.2.0/peptdeep/utils/_pyinstaller_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from transformers.dependency_versions_check import pkgs_to_check_at_runtime
 
 def get_peptdeep_datas():
     """
-    Huggingface has some dependencies those are not included in pyinstaller, 
+    Huggingface has some dependencies those are not included in pyinstaller,
     so we need to add them manually.
     Usages:
-    In pyinstaller's *.spec file, add `datas += get_peptdeep_datas()` before 
+    In pyinstaller's *.spec file, add `datas += get_peptdeep_datas()` before
     `.. = Analysis(..., datas=datas,...)`.
     """
     from PyInstaller.utils.hooks import copy_metadata
     for _pkg in ["python","accelerate"]:
         if _pkg in pkgs_to_check_at_runtime:
             pkgs_to_check_at_runtime.remove(_pkg)
     datas = []
     for _pkg in pkgs_to_check_at_runtime:
         datas += copy_metadata(_pkg)
-    return datas
+    return datas
```

### Comparing `peptdeep-1.1.9/peptdeep/utils/device_utils.py` & `peptdeep-1.2.0/peptdeep/utils/device_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     try:
         return torch.backends.mps.is_available()
     except AttributeError:
         return False
 
 torch_devices:dict = {
     'gpu': {
-        'is_available': torch.cuda.is_available, 
+        'is_available': torch.cuda.is_available,
         'device': 'cuda',
     },
     'cuda': {
-        'is_available': torch.cuda.is_available, 
+        'is_available': torch.cuda.is_available,
         'device': 'cuda',
     },
     'mps': {
-        'is_available': _is_mps_available, 
+        'is_available': _is_mps_available,
         'device': 'mps',
     },
     'm1': {
-        'is_available': _is_mps_available, 
+        'is_available': _is_mps_available,
         'device': 'mps',
     }
 }
 
 def get_device(device:str, device_ids:list=[])->tuple:
     """Device name to torch.device
 
@@ -42,26 +42,25 @@
         torch.device
         str: device name
     """
     device = device.lower()
     if device in torch_devices:
         if torch_devices[device]['is_available']():
             if (
-                torch_devices[device]['device'] == 'cuda' 
+                torch_devices[device]['device'] == 'cuda'
                 and len(device_ids) > 0
             ):
                 return torch.device(
                     f'cuda:{",".join(str(_id) for _id in device_ids)}'
                 ), 'cuda'
             else:
                 return (
-                    torch.device(torch_devices[device]['device']), 
+                    torch.device(torch_devices[device]['device']),
                     device
                 )
     return torch.device('cpu'), 'cpu'
 
 def get_available_device()->tuple:
     for name, item in torch_devices.items():
         if item['is_available']():
             return torch.device(item['device']), name
     return torch.device('cpu'), 'cpu'
-
```

### Comparing `peptdeep-1.1.9/peptdeep/utils/logger.py` & `peptdeep-1.2.0/peptdeep/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         If False, no log data is sent to stream.
         If True, all logging can be tracked with stdout stream.
         Default is True.
 
     log_level : str or int
         The logging level. Usable values are defined in Python's "logging"
         module. Could be: 'debug', 'info', 'warning', 'error', 'critical'.
-        See `log_level_dict`. 
+        See `log_level_dict`.
         Default is 'info'.
 
     overwrite : bool
         If True, overwrite the log_file if one exists.
         If False, append to this log file.
         Default is False.
 
@@ -64,15 +64,15 @@
         The file name to where the log is written.
     """
     if isinstance(log_level, str):
         if log_level.lower() in log_level_dict:
             log_level = log_level_dict[log_level.lower()]
         else:
             log_level = logging.INFO
-    
+
     root = logging.getLogger()
     formatter = logging.Formatter(
         '%(asctime)s> %(message)s', "%Y-%m-%d %H:%M:%S"
     )
     root.setLevel(log_level)
     while root.hasHandlers():
         root.removeHandler(root.handlers[0])
@@ -183,8 +183,8 @@
         except importlib.metadata.PackageNotFoundError:
             module_version = ""
         module_versions[module_name] = module_version
     max_len = max(len(key) for key in module_versions)
     logging.info("Python information:")
     for key, value in sorted(module_versions.items()):
         logging.info(f"{key:<{max_len}} - {value}")
-    logging.info("")
+    logging.info("")
```

### Comparing `peptdeep-1.1.9/peptdeep/utils/regression.py` & `peptdeep-1.2.0/peptdeep/utils/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         Dataframe of PSMs.
 
     target : str, optional
         Target columns to sample.
         Defaults to 'rt_norm'.
 
     n_train : int, optional
-        The number of training PSMs to sample. 
+        The number of training PSMs to sample.
         Defaults to 1000.
 
     return_test_df : bool, optional
         If also return `test_df`.
         `test_df` contains the PSMs that are not sampled.
         Defaults to False.
 
@@ -83,34 +83,34 @@
         R_square=[R_square],
         R=[np.sqrt(R_square)],
         slope=[w],
         intercept=[b],
     )
 
 def evaluate_linear_regression(
-    df:pd.DataFrame, x='rt_pred', y='rt_norm', 
+    df:pd.DataFrame, x='rt_pred', y='rt_norm',
     ci=95, n_sample=10000000
 ):
     if len(df) > n_sample:
         df = df.sample(n_sample, replace=False)
 
     regs = linear_regression(df[x].values, df[y].values)
     regs["test_num"] = len(df)
 
     return pd.DataFrame(regs)
 
 def evaluate_linear_regression_plot(
-    df:pd.DataFrame, x='rt_pred', y='rt_norm', 
+    df:pd.DataFrame, x='rt_pred', y='rt_norm',
     ci=95, n_sample=100000
 ):
     import seaborn as sns
     if len(df) > n_sample:
         df = df.sample(n_sample)
     alpha = 0.05
     if len(df) < 5000:
         alpha = 1
     elif len(df) < 50000:
         alpha = 5000.0/len(df)
     return sns.regplot(
-        data=df, x=x, y=y, color='r', ci=ci, 
+        data=df, x=x, y=y, color='r', ci=ci,
         scatter_kws={'s':0.05, 'alpha':alpha, 'color':'b'}
-    )
+    )
```

### Comparing `peptdeep-1.1.9/peptdeep/webui/library_ui.py` & `peptdeep-1.2.0/peptdeep/webui/library_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,31 +43,31 @@
             'modloss_composition','modloss','modloss_importance'
         ]], hide_index=True)
 
     varmod_range()
 
 def varmod_range():
     min_varmod = st.number_input(label='Min number of variable modifications',
-        value = global_ui_settings['library']['min_var_mod_num'], 
+        value = global_ui_settings['library']['min_var_mod_num'],
         min_value = 0, step = 1,
     )
     max_varmod = st.number_input(label='Max number of variable modifications',
-        value = global_ui_settings['library']['max_var_mod_num'], 
+        value = global_ui_settings['library']['max_var_mod_num'],
         min_value = 0, step = 1,
     )
     global_ui_settings['library']['min_var_mod_num'] = min_varmod
     global_ui_settings['library']['max_var_mod_num'] = max_varmod
 
 def specialmod_options():
     st.write('#### Special modificatins')
     st.write('*Useful for Phospho@S/T or GlyGly@K*')
     st.write('- For Phospho@S/T or HexNAc@S, as a sequence may generate many peptidoforms, this can control the overall number.')
     st.write('- For GlyGly@K or GG@K, it will not occur at C-term Lys/K, using `special modifications` to enable this feature.')
     specialmod_expander = st.expander(
-        label='Special modificatins', 
+        label='Special modificatins',
         expanded=len(global_ui_settings['library']['special_mods'])>0,
     )
     with specialmod_expander:
         with st.form(key="Select special modifications"):
             global_ui_settings['library']['special_mods'] = st.multiselect(
                 label='Please select special modifications',
                 options=MOD_DF.index.values,
@@ -83,38 +83,38 @@
                 ]
             ], hide_index=True)
 
         specialmod_range()
 
 def specialmod_range():
     min_specialmod = st.number_input(label='Min number of special modifications',
-        value = global_ui_settings['library']['min_special_mod_num'], 
+        value = global_ui_settings['library']['min_special_mod_num'],
         min_value = 0, step = 1
     )
     max_specialmod = st.number_input(label='Max number of special modifications',
-        value = global_ui_settings['library']['max_special_mod_num'], 
+        value = global_ui_settings['library']['max_special_mod_num'],
         min_value = 0, step = 1
     )
     global_ui_settings['library']['min_special_mod_num'] = min_specialmod
     global_ui_settings['library']['max_special_mod_num'] = max_specialmod
 
     st.write("Special modifications cannot modify AAs at:")
     st.write("*e.g. GlyGly@K will not occur at C-term Lys/K*")
     global_ui_settings['library'][
         'special_mods_cannot_modify_pep_n_term'
     ] = bool(
-        st.checkbox(label='N-term', 
+        st.checkbox(label='N-term',
         value=global_ui_settings['library'][
             'special_mods_cannot_modify_pep_n_term'
         ])
     )
     global_ui_settings['library'][
         'special_mods_cannot_modify_pep_c_term'
     ] = bool(
-        st.checkbox(label='C-term', 
+        st.checkbox(label='C-term',
         value=global_ui_settings['library'][
             'special_mods_cannot_modify_pep_c_term'
         ])
     )
 
 def labeling_options():
     def _concat_df_dict(d):
@@ -185,19 +185,19 @@
             global_ui_settings['library']['decoy']
         )
     )
 
 def choose_protease():
     def on_custom_protease():
         if (
-            len(st.session_state['custom_protease_text']) <= 1 
+            len(st.session_state['custom_protease_text']) <= 1
             or st.session_state['custom_protease_text'] in protease_dict
             or (
-                '(' in st.session_state['custom_protease_text'] and 
-                ')' in st.session_state['custom_protease_text'] and 
+                '(' in st.session_state['custom_protease_text'] and
+                ')' in st.session_state['custom_protease_text'] and
                 len(st.session_state['custom_protease_text']) >= 3
             )
         ):
             return
         else:
             st.session_state['custom_protease_text'] = ''
 
@@ -244,22 +244,22 @@
 
 def output_tsv():
     min_fragment_mz = st.number_input(label='Min fragment mz:', value = global_ui_settings['library']['output_tsv']['min_fragment_mz'])
     global_ui_settings['library']['output_tsv']['min_fragment_mz'] = min_fragment_mz
     max_fragment_mz = st.number_input(label='Max fragment mz:', min_value = min_fragment_mz, value = global_ui_settings['library']['output_tsv']['max_fragment_mz'])
     global_ui_settings['library']['output_tsv']['max_fragment_mz'] = max_fragment_mz
     min_relative_intensity = st.number_input(
-        label='Min relative intensity:', 
+        label='Min relative intensity:',
         value = global_ui_settings['library']['output_tsv']['min_relative_intensity'],
         step=0.0001,
         format='%0.4f'
     )
     global_ui_settings['library']['output_tsv']['min_relative_intensity'] = min_relative_intensity
     keep_higest_k_peaks = st.number_input(
-        label='Number of highest peaks to keep:', 
+        label='Number of highest peaks to keep:',
         value = global_ui_settings['library']['output_tsv']['keep_higest_k_peaks']
     )
     global_ui_settings['library']['output_tsv']['keep_higest_k_peaks'] = keep_higest_k_peaks
     global_ui_settings['library']['output_tsv']['translate_mod_to_unimod_id']=bool(
         st.checkbox(label='Translate modifications to Unimod ids',
         value=global_ui_settings['library']['output_tsv']['translate_mod_to_unimod_id']
     ))
@@ -270,15 +270,15 @@
     st.write('### Input')
 
     infile_type = file_type_selectbox(
         ui_label='Input file type',
         st_key='lib_input_type',
         default_type=global_ui_settings['library']['infile_type'],
         monitor_files=global_ui_settings['library']['infiles'],
-        choices=global_ui_settings['library']['infile_type_choices'], 
+        choices=global_ui_settings['library']['infile_type_choices'],
         index=global_ui_settings['library']['infile_type_choices'].index(
             global_ui_settings['library']['infile_type']
         )
     )
     global_ui_settings['library']['infile_type'] = infile_type
 
     if infile_type != 'fasta':
@@ -302,15 +302,15 @@
         'sequence_table': ['tsv','txt','csv'],
         'peptide_table': ['tsv','txt','csv'],
         'precursor_table': ['tsv','txt','csv'],
     }
 
     if infile_type == 'fasta':
         global_ui_settings['library']['fasta']['add_contaminants'] = bool(st.checkbox(
-            label='Add fasta of contaminants', 
+            label='Add fasta of contaminants',
             value=global_ui_settings['library']['fasta']['add_contaminants']
         ))
     select_files(
         global_ui_settings['library']['infiles'],
         infile_ext_dict[infile_type],
         'Input sequence files',
     )
@@ -322,52 +322,52 @@
         choose_protease()
         mod_options()
         specialmod_options()
 
     elif infile_type == 'sequence_table':
         mod_options()
         specialmod_options()
-    
+
     labeling_options()
 
     st.write("#### Common peptide settings")
-    
+
     if infile_type == 'fasta':
         choose_peptide_len()
 
     if infile_type in ['fasta','sequence_table','peptide_table']:
         choose_precursor_charge()
-    
+
     choose_precursor_mz()
     choose_frag_types()
 
     st.write("### Output")
 
     output_folder = st.text_input(
-        label="Output folder", 
+        label="Output folder",
         value=global_ui_settings['library']['output_folder'].format(
             PEPTDEEP_HOME=global_ui_settings['PEPTDEEP_HOME']
         )
     )
     output_folder = os.path.expanduser(output_folder)
     output_folder = get_posix(output_folder)
     global_ui_settings['library']['output_folder'] = output_folder
 
     global_ui_settings['library']['rt_to_irt'] = bool(st.checkbox(
-        label='Convert predicted RT to iRT', 
+        label='Convert predicted RT to iRT',
         value=global_ui_settings['library']['rt_to_irt']
     ))
 
     global_ui_settings['library']['generate_precursor_isotope'] = bool(st.checkbox(
-        label="Generate precursor isotopes (don't check this for DiaNN/Spectronaut search)", 
+        label="Generate precursor isotopes (don't check this for DiaNN/Spectronaut search)",
         value=global_ui_settings['library']['generate_precursor_isotope']
     ))
 
     tsv_enabled = bool(st.checkbox(
-        label='Output TSV (for DiaNN/Spectronaut)', 
+        label='Output TSV (for DiaNN/Spectronaut)',
         value=global_ui_settings['library']['output_tsv']['enabled']
     ))
     global_ui_settings['library']['output_tsv']['enabled'] = tsv_enabled
     st.warning("Writing the TSV file for a big library is very slow")
     if tsv_enabled:
         output_tsv()
 
@@ -383,13 +383,13 @@
 
         yaml_path = f'{queue_folder}/{task_name}.yaml'
         save_yaml(
             yaml_path, global_ui_settings
         )
         save_yaml(
             os.path.join(
-                output_folder, 
+                output_folder,
                 f'{task_name}.yaml'
-            ), 
+            ),
             global_ui_settings
         )
         st.write(f'`library` task saved as `{os.path.expanduser(yaml_path)}`')
```

### Comparing `peptdeep-1.1.9/peptdeep/webui/logos/peptdeep.ico` & `peptdeep-1.2.0/peptdeep/webui/logos/peptdeep.ico`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.9/peptdeep/webui/logos/peptdeep.png` & `peptdeep-1.2.0/peptdeep/webui/logos/peptdeep.png`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.9/peptdeep/webui/main_ui.py` & `peptdeep-1.2.0/peptdeep/webui/main_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from PIL import Image
 import os
 import socket
 import peptdeep
 
 from peptdeep.webui import (
-    model_ui, startpage, rescore_ui, 
+    model_ui, startpage, rescore_ui,
     library_ui, transfer_ui,
     settings_ui, server_ui,
 )
 
 _this_file = __file__
 _this_directory = os.path.dirname(_this_file)
 LOGO_PATH = os.path.join(_this_directory, 'logos', 'peptdeep.png')
@@ -51,8 +51,8 @@
 
 menu = st.sidebar.radio("", list(sidebar.keys()))
 
 if menu:
     sidebar[menu]()
 
 link = f'[PeptDeep on GitHub]({peptdeep.__github__})'
-st.sidebar.markdown(link, unsafe_allow_html=True)
+st.sidebar.markdown(link, unsafe_allow_html=True)
```

### Comparing `peptdeep-1.1.9/peptdeep/webui/model_ui.py` & `peptdeep-1.2.0/peptdeep/webui/model_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.9/peptdeep/webui/rescore_ui.py` & `peptdeep-1.2.0/peptdeep/webui/rescore_ui.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
         result_files = files_in_folder_pandas(result_folder,psm_type)
 
         st.dataframe(result_files)
 
     st.warning("We are still working on Rescore GUI panel.")
     st.warning("For command line users, please use `peptdeep rescore` for rescoring.")
-    st.warning("For Python users, please use `peptdeep.pipeline_api.rescore()` for rescoring.")
+    st.warning("For Python users, please use `peptdeep.pipeline_api.rescore()` for rescoring.")
```

### Comparing `peptdeep-1.1.9/peptdeep/webui/server.py` & `peptdeep-1.2.0/peptdeep/webui/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 import os
 import sys
 import shutil
 import multiprocessing as mp
 
 from peptdeep.pipeline_api import (
-    generate_library, 
-    transfer_learn, 
+    generate_library,
+    transfer_learn,
     # rescore
 )
 from peptdeep.settings import global_settings, load_global_settings
 from peptdeep.utils import logging
 
 def get_yamls(folder):
     ymls = []
@@ -40,15 +40,15 @@
     files = []
     echo_waiting = True
     while True:
         files = get_yamls(queue_folder)
         if len(files) > 0:
             yaml_file = files.pop(0)
             print(f"[PeptDeep] Starting a new job '{yaml_file}'...")
-            
+
             running_txt = f'{home_folder}/tasks/running.txt'
             with open(running_txt,'w') as f:
                 f.write(yaml_file)
 
             try:
                 load_global_settings(yaml_file)
                 if global_settings['task_workflow'][0] == 'train':
@@ -61,25 +61,25 @@
                 #     print("[PeptDeep] Rescoring PSMs ... ")
                 #     rescore()
                 else:
                     logging.warning(f"[PeptDeep] Unknown task type `{global_settings['task_workflow']}`, skip ... ")
                     continue
                 if os.path.isfile(yaml_file):
                     shutil.move(
-                        yaml_file, 
+                        yaml_file,
                         os.path.join(done_folder, os.path.basename(yaml_file))
                     )
             except KeyboardInterrupt as e:
                 with open(running_txt,'w') as f:
                     f.write("")
                 raise e
             except Exception as e:
                 if os.path.isfile(yaml_file):
                     shutil.move(
-                        yaml_file, 
+                        yaml_file,
                         os.path.join(failed_folder, os.path.basename(yaml_file)),
                     )
                 print(e)
             with open(running_txt,'w') as f:
                 f.write("")
             echo_waiting=True
         else:
@@ -91,16 +91,16 @@
 
         time.sleep(3)
 
 class PeptDeepServer:
     def __init__(self):
         self.process:mp.Process = None
         self._process_file = os.path.join(
-            global_settings['PEPTDEEP_HOME'], 
-            'tasks/serve_pid.txt', 
+            global_settings['PEPTDEEP_HOME'],
+            'tasks/serve_pid.txt',
         )
 
     def start(self):
         if self.process is None:
             self.process = mp.Process(target=serve)
             self.process.start()
 
@@ -113,9 +113,9 @@
             self.process.kill()
             self.process = None
 
         os.replace(self._process_file, self._process_file[:-3]+'prev.txt')
 
     def __del__(self):
         self.terminate()
-    
+
 _server = PeptDeepServer()
```

### Comparing `peptdeep-1.1.9/peptdeep/webui/server_ui.py` & `peptdeep-1.2.0/peptdeep/webui/server_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.9/peptdeep/webui/settings_ui.py` & `peptdeep-1.2.0/peptdeep/webui/settings_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         def _clear_user_mods():
             global_ui_settings['common']['user_defined_modifications'] = {}
             st.session_state.user_mod_name = ''
             st.session_state.user_mod_comp = ''
             st.session_state.user_mod_loss = ''
 
-        st.button(label='Clear all user modifications', 
+        st.button(label='Clear all user modifications',
             on_click=_clear_user_mods
         )
 
         if st.button(label='Add user modifications into AlphaBase'):
             add_user_defined_modifications()
             st.write("Check last n+2 modifications:")
             st.dataframe(MOD_DF.tail(
@@ -66,59 +66,59 @@
             ), hide_index=True)
 
 def show():
     load_settings_gui()
     save_settings_gui()
 
     st.write("### Common settings")
-    
+
     add_user_mods()
 
     ms2_ppm = st.checkbox(label='MS2 ppm (otherwise Da)', value=global_ui_settings['peak_matching']['ms2_ppm'])
     global_ui_settings['peak_matching']['ms2_ppm'] = ms2_ppm
     ms2_tol_value = st.number_input(label='MS2 tolerance', value = global_ui_settings['peak_matching']['ms2_tol_value'], step = 1.0)
     global_ui_settings['peak_matching']['ms2_tol_value'] = ms2_tol_value
 
     ms1_ppm = st.checkbox(label='MS1 ppm (otherwise Da)', value=global_ui_settings['peak_matching']['ms1_ppm'])
     global_ui_settings['peak_matching']['ms1_ppm'] = ms1_ppm
     ms1_tol_value = st.number_input(label='MS1 tolerance', value = global_ui_settings['peak_matching']['ms1_tol_value'], step = 1.0)
     global_ui_settings['peak_matching']['ms1_tol_value'] = ms1_tol_value
-    
+
     cpu_count = multiprocessing.cpu_count()
-    thread_num = st.number_input(label='Thread number', 
+    thread_num = st.number_input(label='Thread number',
         value=min(
-            global_ui_settings['thread_num'], 
-            cpu_count, 
+            global_ui_settings['thread_num'],
+            cpu_count,
             global_settings['MAX_THREADS']
-        ), 
+        ),
         max_value=min(
             cpu_count, global_settings['MAX_THREADS']
-        ), 
+        ),
         step=1
     )
     global_ui_settings['thread_num'] = thread_num
 
     global_ui_settings['torch_device']['device_type'] = st.selectbox(
         label='Computing devices',
         options=global_ui_settings['torch_device']['device_type_choices'],
         index = global_ui_settings['torch_device']['device_type_choices'].index(
             global_ui_settings['torch_device']['device_type']
         )
     )
 
     global_ui_settings['log_level'] = st.selectbox(
-        label='Log level', 
-        options=global_ui_settings['log_level_choices'], 
+        label='Log level',
+        options=global_ui_settings['log_level_choices'],
         index = global_ui_settings['log_level_choices'].index(
             global_ui_settings['log_level']
         )
     )
 
     global_ui_settings['common']['modloss_importance_level'] = st.number_input(
-        'Modification loss importance level (for a PTM, fragment modloss mz=0 if modloss_importance<modloss_importance_level)', 
+        'Modification loss importance level (for a PTM, fragment modloss mz=0 if modloss_importance<modloss_importance_level)',
         value=global_ui_settings['common']['modloss_importance_level'], step=1.0,
     )
     keep_modloss_by_importance(global_ui_settings['common']['modloss_importance_level'])
 
     st.write("Modification modloss example (check the `modloss` column):")
     st.dataframe(MOD_DF.loc[
         ['Carbamidomethyl@C','Oxidation@M','Phospho@S'],
@@ -151,8 +151,8 @@
     f = StringIO()
     yaml.dump(global_ui_settings, f)
 
     st.download_button(
         label="Download settings as yaml",
         data=f.getvalue(),
         file_name='peptdeep_settings.yaml',
-    )
+    )
```

### Comparing `peptdeep-1.1.9/peptdeep/webui/startpage.py` & `peptdeep-1.2.0/peptdeep/webui/startpage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
             "When starting PeptDeep you launch a server that can be closed when closing the terminal window."
         )
         st.write(
             "If your firewall policy allows external access, this page can also be accessed from other computers in the network."
         )
         st.write(
             "The server starts an PeptDeep process in the background that will process new experiments once they are submitted."
-        )
+        )
```

### Comparing `peptdeep-1.1.9/peptdeep/webui/transfer_ui.py` & `peptdeep-1.2.0/peptdeep/webui/transfer_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     grid_nce_last = st.number_input(label='End NCE for grid NCE search',min_value = grid_nce_first, value = global_ui_settings['model_mgr']['transfer']['grid_nce_last']*1.0,step = 1.0)
     global_ui_settings['model_mgr']['transfer']['grid_nce_last'] = grid_nce_last
     grid_nce_step = st.number_input(label='Step NCE for grid NCE search', value = global_ui_settings['model_mgr']['transfer']['grid_nce_step']*1.0,step = 1.0)
     global_ui_settings['model_mgr']['transfer']['grid_nce_step'] = grid_nce_step
 
     grid_instrument = st.multiselect(label='Instruments for grid NCE search',
         options=global_ui_settings['model_mgr']['instrument_group'],
-        default = global_ui_settings['model_mgr']['transfer']['grid_instrument']) 
+        default = global_ui_settings['model_mgr']['transfer']['grid_instrument'])
     global_ui_settings['model_mgr']['transfer']['grid_instrument'] = grid_instrument
 
 def fine_tune():
     st.write("#### Epochs and learning rates")
     epoch_ms2 = st.number_input(label='Epoch to train MS2 model', value = global_ui_settings['model_mgr']['transfer']['epoch_ms2'])
     global_ui_settings['model_mgr']['transfer']['epoch_ms2'] = epoch_ms2
     warmup_epoch_ms2 = st.number_input(label='Warmup epoch to train MS2 model', value = global_ui_settings['model_mgr']['transfer']['warmup_epoch_ms2'], max_value=epoch_ms2)
     global_ui_settings['model_mgr']['transfer']['warmup_epoch_ms2'] = warmup_epoch_ms2
     batch_size_ms2 = st.number_input(label='Mini-batch size to train MS2 model', value = global_ui_settings['model_mgr']['transfer']['batch_size_ms2'])
     global_ui_settings['model_mgr']['transfer']['batch_size_ms2'] = batch_size_ms2
     lr_ms2 = st.number_input(label='Learning rate to train MS2 model', value = global_ui_settings['model_mgr']['transfer']['lr_ms2'], format='%e', step=1e-5)
     global_ui_settings['model_mgr']['transfer']['lr_ms2'] = lr_ms2
-    
+
     epoch_rt_ccs = st.number_input(label='Epoch to train RT and CCS models', value = global_ui_settings['model_mgr']['transfer']['epoch_rt_ccs'])
     global_ui_settings['model_mgr']['transfer']['epoch_rt_ccs'] = epoch_rt_ccs
     warmup_epoch_rt_ccs = st.number_input(label='Warmup epoch to train RT and CCS model', value = global_ui_settings['model_mgr']['transfer']['warmup_epoch_rt_ccs'], max_value=epoch_rt_ccs)
     global_ui_settings['model_mgr']['transfer']['warmup_epoch_rt_ccs'] = warmup_epoch_rt_ccs
     batch_size_rt_ccs = st.number_input(label='Mini-batch size to train RT and CCS model', value = global_ui_settings['model_mgr']['transfer']['batch_size_rt_ccs'])
     global_ui_settings['model_mgr']['transfer']['batch_size_rt_ccs'] = batch_size_rt_ccs
     lr_rt_ccs = st.number_input(label='Learning rate to train RT and CCS model', value = global_ui_settings['model_mgr']['transfer']['lr_rt_ccs'], format='%e', step=1e-5)
@@ -78,23 +78,23 @@
 
         def _clear_user_mods():
             global_ui_settings['model_mgr']['transfer'][
                 'psm_modification_mapping'
             ] = {}
             st.session_state.other_reader_mods = ''
 
-        st.button(label='Clear all other modification mapping', 
+        st.button(label='Clear all other modification mapping',
             on_click=_clear_user_mods
         )
 
 def show():
     st.write("# Transfer learning")
 
     model_output_folder = st.text_input(
-        label='Model output folder', 
+        label='Model output folder',
         value=global_ui_settings['model_mgr']['transfer']['model_output_folder'].format(
             PEPTDEEP_HOME=global_ui_settings['PEPTDEEP_HOME']
         )
     )
     model_output_folder = get_posix(
         model_output_folder
     )
@@ -118,138 +118,138 @@
         "pfind": ".spectra",
         "maxquant": "msms.txt",
         "diann": "tsv",
         "speclib_tsv": "tsv",
     }
     global_ui_settings['model_mgr']['transfer']['psm_type'] = psm_type
     select_files(
-        global_ui_settings['model_mgr']['transfer']['psm_files'], 
-        psm_type_to_ext_dict[psm_type], 
+        global_ui_settings['model_mgr']['transfer']['psm_files'],
+        psm_type_to_ext_dict[psm_type],
         "Input PSM files"
     )
     add_other_psm_reader_mods()
 
     st.write("### MS files for training")
     ms_file_type = file_type_selectbox(
         ui_label='MS file type',
         st_key='select_ms_file_type',
         default_type=global_ui_settings['model_mgr']['transfer']['ms_file_type'],
         monitor_files=global_ui_settings['model_mgr']['transfer']['ms_files'],
-        choices=global_ui_settings['model_mgr']['transfer']['ms_file_type_choices'], 
+        choices=global_ui_settings['model_mgr']['transfer']['ms_file_type_choices'],
         index=global_ui_settings['model_mgr']['transfer']['ms_file_type_choices'].index(
             global_ui_settings['model_mgr']['transfer']['ms_file_type']
         )
     )
     ms_type_to_ext_dict = {
         "alphapept_hdf": ".ms_data.hdf",
         "thermo_raw": ".raw",
         "mgf": ".mgf",
         "mzml": ".mzml",
         "speclib_tsv": [".tsv", ".csv"]
     }
     global_ui_settings['model_mgr']['transfer']['ms_file_type'] = ms_file_type
     select_files(
-        global_ui_settings['model_mgr']['transfer']['ms_files'], 
-        ms_type_to_ext_dict[ms_file_type], 
+        global_ui_settings['model_mgr']['transfer']['ms_files'],
+        ms_type_to_ext_dict[ms_file_type],
         "Input MS files"
     )
 
     st.write("### Training settings")
 
     training_expander = st.expander("Training hyper-parameters")
     with training_expander:
         fine_tune()
 
         st.write('#### PSM numbers for training and testing')
         global_ui_settings['model_mgr']['transfer'][
             'psm_num_to_train_ms2'
         ] = st.number_input(
-            label='PSM num to refine MS2 model', 
+            label='PSM num to refine MS2 model',
             value = int(global_ui_settings['model_mgr']['transfer'][
                 'psm_num_to_train_ms2'
             ]), step = 1
         )
         global_ui_settings['model_mgr']['transfer'][
             'psm_num_per_mod_to_train_ms2'
         ] = st.number_input(
-            label='PSM num per mod to refine MS2 model', 
+            label='PSM num per mod to refine MS2 model',
             value = int(global_ui_settings['model_mgr']['transfer'][
                 'psm_num_per_mod_to_train_ms2'
             ]), step = 1
         )
         global_ui_settings['model_mgr']['transfer'][
             'psm_num_to_test_ms2'
         ] = st.number_input(
-            label='PSM num to test MS2 model', 
+            label='PSM num to test MS2 model',
             value = int(global_ui_settings['model_mgr']['transfer'][
                 'psm_num_to_test_ms2'
             ]), step = 1
         )
 
         global_ui_settings['model_mgr']['transfer'][
             'psm_num_to_train_rt_ccs'
         ] = st.number_input(
-            label='PSM num to refine RT and CCS model', 
+            label='PSM num to refine RT and CCS model',
             value = int(global_ui_settings['model_mgr']['transfer'][
                 'psm_num_to_train_rt_ccs'
             ]), step = 1
         )
         global_ui_settings['model_mgr']['transfer'][
             'psm_num_per_mod_to_train_rt_ccs'
         ] = st.number_input(
-            label='PSM num per mod to refine RT and CCS model', 
+            label='PSM num per mod to refine RT and CCS model',
             value = int(global_ui_settings['model_mgr']['transfer'][
                 'psm_num_per_mod_to_train_rt_ccs'
             ]), step = 1
         )
-        
+
         global_ui_settings['model_mgr']['transfer'][
             'psm_num_to_test_rt_ccs'
         ] = st.number_input(
-            label='PSM num to test RT and CCS model', 
+            label='PSM num to test RT and CCS model',
             value = int(global_ui_settings['model_mgr']['transfer'][
                 'psm_num_to_test_rt_ccs'
             ]), step = 1
         )
-        
+
         st.write("#### Other hyper-parameters")
         global_ui_settings['model_mgr']['transfer'][
             'top_n_mods_to_train'
         ] = st.number_input(
-            label='Top n mods to refine models', 
+            label='Top n mods to refine models',
             value = int(global_ui_settings['model_mgr']['transfer'][
                 'top_n_mods_to_train'
             ]), step = 1
         )
 
     st.write('#### Grid search for NCEs and instruments')
     st.write('If NCE and instrument are unknown, grid search will look for the best NCE and instrument)')
-    grid_nce_search = bool(st.checkbox(label='Enabled', 
+    grid_nce_search = bool(st.checkbox(label='Enabled',
         value=global_ui_settings['model_mgr']['transfer']['grid_nce_search']
     ))
     global_ui_settings['model_mgr']['transfer']['grid_nce_search'] = grid_nce_search
     if grid_nce_search is True:
         nce_search()
 
     now = datetime.now()
     current_time = now.strftime("%Y-%m-%d--%H-%M-%S.%f")
     task_name = st.text_input(label="Task name", value=f"peptdeep_transfer_{current_time}")
-    
+
     if st.button(label='Submit for transfer learning'):
         global_ui_settings['task_workflow'] = ['train']
 
         if not os.path.exists(model_output_folder):
             os.makedirs(model_output_folder)
 
         yaml_path = f'{queue_folder}/{task_name}.yaml'
         save_yaml(
             yaml_path, global_ui_settings
         )
         save_yaml(
             os.path.join(
-                model_output_folder, 
+                model_output_folder,
                 f'{task_name}.yaml'
-            ), 
+            ),
             global_ui_settings
         )
-        
-        st.write(f'`train` task saved as "{os.path.expanduser(yaml_path)}" in the task queue')
+
+        st.write(f'`train` task saved as "{os.path.expanduser(yaml_path)}" in the task queue')
```

### Comparing `peptdeep-1.1.9/peptdeep/webui/ui_utils.py` & `peptdeep-1.2.0/peptdeep/webui/ui_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     sizes = [os.path.getsize(_) / 1024 ** 2 for _ in files]
     df = pd.DataFrame(files, columns=["File Path"])
     df["Created Time"] = created
     df["File Size (Mb)"] = sizes
 
     return df
 
-def file_type_selectbox( 
+def file_type_selectbox(
     ui_label:str,
-    st_key:str, 
+    st_key:str,
     default_type:str,
     monitor_files:list,
     choices:list,
     index=0,
 )->str:
     def on_type_change():
         if len(monitor_files)>0:
@@ -56,16 +56,16 @@
         _ for _ in file_list
         if os.path.isfile(_)
     ]
     file_list.clear()
     file_list.extend(_list)
 
 def select_files(
-    file_list:list, 
-    file_exts:list, 
+    file_list:list,
+    file_exts:list,
     ui_label="File"
 ):
     if isinstance(file_exts, str):
         file_exts = [file_exts.lower()]
     else:
         file_exts = [ext.lower() for ext in file_exts]
     st.write('##### ' + ui_label)
@@ -156,15 +156,15 @@
         pd.DataFrame: PandasDataFrame.
     """
     if file_type is None:
         files = os.listdir(folder)
     else:
         file_type = file_type.lower()
         files = [
-            file for file in os.listdir(folder) 
+            file for file in os.listdir(folder)
             if file.lower().endswith(f".{file_type}") or file.lower() == file_type
         ]
     created = [time.ctime(os.path.getctime(os.path.join(folder, _))) for _ in files]
     sizes = [os.path.getsize(os.path.join(folder, _)) / 1024 ** 2 for _ in files]
     df = pd.DataFrame(files, columns=["File"])
     df["Created"] = created
     df["Filesize (Mb)"] = sizes
@@ -269,8 +269,8 @@
             p["init"] = True
             for _ in kwargs:
                 p[_] = kwargs[_]
             with open(process_path, "w") as file:
                 yaml.dump(p, file, sort_keys=False)
             break
         else:
-            time.sleep(1)
+            time.sleep(1)
```

### Comparing `peptdeep-1.1.9/peptdeep.egg-info/PKG-INFO` & `peptdeep-1.2.0/peptdeep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptdeep
-Version: 1.1.9
+Version: 1.2.0
 Summary: The AlphaX deep learning framework for Proteomics
 Home-page: https://github.com/MannLabs/peptdeep
 Author: Mann Labs
 Author-email: jalew.zwf@qq.com
 License: Apache 2.0
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
@@ -45,15 +45,14 @@
 Requires-Dist: jupyter; extra == "development-stable"
 Requires-Dist: twine; extra == "development-stable"
 Requires-Dist: bumpversion; extra == "development-stable"
 Requires-Dist: pipdeptree; extra == "development-stable"
 Requires-Dist: ipykernel; extra == "development-stable"
 Requires-Dist: tqdm; extra == "development-stable"
 Requires-Dist: wget; extra == "development-stable"
-Requires-Dist: nbdev; extra == "development-stable"
 Requires-Dist: pyinstaller; extra == "development-stable"
 Requires-Dist: click; extra == "development-stable"
 Requires-Dist: pandas; extra == "development-stable"
 Requires-Dist: numpy; extra == "development-stable"
 Requires-Dist: seaborn; extra == "development-stable"
 Requires-Dist: matplotlib; extra == "development-stable"
 Requires-Dist: numba; extra == "development-stable"
@@ -70,25 +69,27 @@
 Requires-Dist: jinja2; extra == "development-stable"
 Requires-Dist: contextfilter; extra == "development-stable"
 Requires-Dist: furo; extra == "development-stable"
 Requires-Dist: torch; extra == "development-stable"
 Requires-Dist: streamlit>=1.23.0; extra == "development-stable"
 Requires-Dist: alphabase>=1.1.0; extra == "development-stable"
 Requires-Dist: alpharaw>=0.2.0; extra == "development-stable"
+Requires-Dist: pytest; extra == "development-stable"
+Requires-Dist: pre-commit==3.7.0; extra == "development-stable"
+Requires-Dist: nbmake==1.5.3; extra == "development-stable"
 Provides-Extra: development
 Requires-Dist: pywin32; sys_platform == "win32" and extra == "development"
 Requires-Dist: pythonnet; sys_platform == "win32" and extra == "development"
 Requires-Dist: jupyter; extra == "development"
 Requires-Dist: twine; extra == "development"
 Requires-Dist: bumpversion; extra == "development"
 Requires-Dist: pipdeptree; extra == "development"
 Requires-Dist: ipykernel; extra == "development"
 Requires-Dist: tqdm; extra == "development"
 Requires-Dist: wget; extra == "development"
-Requires-Dist: nbdev; extra == "development"
 Requires-Dist: pyinstaller; extra == "development"
 Requires-Dist: click; extra == "development"
 Requires-Dist: pandas; extra == "development"
 Requires-Dist: numpy; extra == "development"
 Requires-Dist: seaborn; extra == "development"
 Requires-Dist: matplotlib; extra == "development"
 Requires-Dist: numba; extra == "development"
@@ -105,14 +106,17 @@
 Requires-Dist: jinja2; extra == "development"
 Requires-Dist: contextfilter; extra == "development"
 Requires-Dist: furo; extra == "development"
 Requires-Dist: torch; extra == "development"
 Requires-Dist: streamlit; extra == "development"
 Requires-Dist: alphabase; extra == "development"
 Requires-Dist: alpharaw; extra == "development"
+Requires-Dist: pytest; extra == "development"
+Requires-Dist: pre-commit; extra == "development"
+Requires-Dist: nbmake; extra == "development"
 Provides-Extra: gui-stable
 Requires-Dist: pywin32; sys_platform == "win32" and extra == "gui-stable"
 Requires-Dist: pythonnet; sys_platform == "win32" and extra == "gui-stable"
 Requires-Dist: click; extra == "gui-stable"
 Requires-Dist: pandas; extra == "gui-stable"
 Requires-Dist: numpy; extra == "gui-stable"
 Requires-Dist: torch; extra == "gui-stable"
@@ -429,28 +433,14 @@
 ***By using the editable flag `-e`, all modifications to the [peptdeep
 source code folder](peptdeep) are directly reflected when running
 peptdeep. Note that the peptdeep folder cannot be moved and/or renamed
 if an editable version is installed. In case of confusion, you can
 always retrieve the location of any Python module with e.g. the command
 `import module` followed by `module.__file__`.***
 
-We used [nbdev v2](https://nbdev.fast.ai/) for developers to build
-Python source code and docs smoothly from Python notebooks, so please do
-not edit .py files directly, edit .ipynb in `nbdev_nbs` folder instead.
-After installing nbdev, cd to alphapeptdeep project folder and run:
-
-``` bash
-nbdev_install_hooks
-```
-
-to init gitconfig for nbdev. After editing the source code in .ipynb
-files, using `nbdev_export` to build python source code and `nbdev_test`
-to run all .ipynb files in `nbdev_nbs` for testing. Check [nbdev
-docs](https://nbdev.fast.ai/) for more information.
-
 ------------------------------------------------------------------------
 
 ## Usage
 
 There are three ways to use peptdeep:
 
 - [**GUI**](#gui)
@@ -527,15 +517,15 @@
 ```
 
 This command will export the default settings into the `settings.yaml`
 as a template, users can edit the yaml file to run other commands.
 
 Here is a section of the yaml file which controls global parameters for
 different tasks:
-  
+
 ```
 model_url: "https://github.com/MannLabs/alphapeptdeep/releases/download/pre-trained-models/pretrained_models.zip"
 
 task_type: library
 task_type_choices:
   - library
   - train
@@ -558,15 +548,15 @@
   - critical
 
 common:
   modloss_importance_level: 1.0
   user_defined_modifications: {}
   # For example,
   # user_defined_modifications:
-  #   "Dimethyl2@Any N-term": 
+  #   "Dimethyl2@Any N-term":
   #     composition: "H(2)2H(2)C(2)"
   #     modloss_composition: "H(0)" # can be without if no modloss
   #   "Dimethyl2@K":
   #     composition: "H(2)2H(2)C(2)"
   #   "Dimethyl6@Any N-term":
   #     composition: "2H(4)13C(2)"
   #   "Dimethyl6@K":
@@ -626,15 +616,15 @@
 ``` bash
 peptdeep cmd-flow ...
 ```
 
 Support CLI parameters to control `global_settings` for CLI users. It supports three workflows: `train`, `library` or `train library`, controlled by CLI parameter `--task_workflow`, for example, `--task_workflow train library`. All settings in [global_settings](peptdeep/constants/default_settings.yaml) are converted to CLI parameters using `--` as the dict level indicator, for example, `global_settings["library"]["var_mods"]` corresponds to `--library--var_mods`. See [test_cmd_flow.sh](tests/test_cmd_flow.sh) for example.
 
 There are three kinds of parameter types:
-  1. value type (int, float, bool, str): The CLI parameter only has a single value, for instance: `--model_mgr--default_instrument 30.0`. 
+  1. value type (int, float, bool, str): The CLI parameter only has a single value, for instance: `--model_mgr--default_instrument 30.0`.
   2. list type (list): The CLI parameter has a list of values seperated by a space, for instance `--library--var_mods "Oxidation@M" "Acetyl@Protein_N-term"`.
   3. dict type (dict): Only three parameters are `dict type`, `--library--labeling_channels`, `--model_mgr--transfer--psm_modification_mapping`, and `--common--user_defined_modifications`. Here are the examples:
     - `--library--labeling_channels`: labeling channels for the library. Example: `--library--labeling_channels "0:Dimethyl@Any_N-term;Dimethyl@K" "4:xx@Any_N-term;xx@K"`
     - `--model_mgr--transfer--psm_modification_mapping`: converting other search engines' modification names to alphabase modifications for transfer learning. Example: `--model_mgr--transfer--psm_modification_mapping "Dimethyl@Any_N-term:_(Dimethyl-n-0);_(Dimethyl)" "Dimethyl@K:K(Dimethyl-K-0);K(Dimethyl)"`. Note that `X(UniMod:id)` format can directly be recognized by alphabase.
     - `--common--user_defined_modification`: user defined modifications. Example:`--common--user_defined_modification "NewMod1@Any_N-term:H(2)2H(2)C(2)" "NewMod2@K:H(100)O(2)C(2)"`
 
 #### library
@@ -652,15 +642,15 @@
 library:
   infile_type: fasta
   infile_type_choices:
   - fasta
   - sequence_table
   - peptide_table # sequence with mods and mod_sites
   - precursor_table # peptide with charge state
-  infiles: 
+  infiles:
   - xxx.fasta
   fasta:
     protease: 'trypsin'
     protease_choices:
     - 'trypsin'
     - '([KR])'
     - 'trypsin_not_P'
@@ -670,15 +660,15 @@
     - 'lys-n'
     - '\w(?=K)'
     - 'chymotrypsin'
     - 'asp-n'
     - 'glu-c'
     max_miss_cleave: 2
     add_contaminants: False
-  fix_mods: 
+  fix_mods:
   - Carbamidomethyl@C
   var_mods:
   - Acetyl@Protein N-term
   - Oxidation@M
   special_mods: [] # normally for Phospho or GlyGly@K
   special_mods_cannot_modify_pep_n_term: False
   special_mods_cannot_modify_pep_c_term: False
@@ -781,15 +771,15 @@
 
 ``` python
 df
 ```
 
 |  | sequence | mods | mod_sites | charge |
 | --- | --- | --- | --- | --- |
-| 0 | ACDEFGHIK | Carbamidomethyl@C | 2 | 2 | 
+| 0 | ACDEFGHIK | Carbamidomethyl@C | 2 | 2 |
 | 1 | LMNPQRSTVK | Acetyl@Protein N-term;Phospho@S | 0;7 | 3 |
 | 2 | WYVSTR | | | 1 |
 
 > Columns of `proteins` and `genes` are optional for these txt/tsv/csv
 > files.
 
 peptdeep supports multiple files for library prediction, for example (in
@@ -859,22 +849,22 @@
     psm_num_to_train_ms2: 100000000
     psm_num_per_mod_to_train_ms2: 50
     psm_num_to_test_ms2: 0
     psm_num_to_train_rt_ccs: 100000000
     psm_num_per_mod_to_train_rt_ccs: 50
     psm_num_to_test_rt_ccs: 0
     top_n_mods_to_train: 10
-    psm_modification_mapping: {} 
+    psm_modification_mapping: {}
     # alphabase modification to modifications of other search engines
     # For example,
     # psm_modification_mapping:
-    #   Dimethyl@Any N-term: 
+    #   Dimethyl@Any N-term:
     #     - _(Dimethyl-n-0)
     #     - _(Dimethyl)
-    #   Dimethyl:2H(2)@K: 
+    #   Dimethyl:2H(2)@K:
     #     - K(Dimethyl-K-2)
     #   ...
 ```
 For DDA data, peptdeep can also extract MS2 intensities from the
 spectrum files from `model_mgr:transfer:ms_files` and
 `model_mgr:transfer:ms_file_type` for all PSMs. This will enable the
 transfer learning of the MS2 model.
@@ -941,15 +931,15 @@
   percolator_model_choices:
     pytorch_as_backend:
       - linear # not fully tested, performance may be unstable
       - mlp # not implemented yet
     sklearn_as_backend:
       - linear # logistic regression
       - random_forest
-  lr_percolator_torch_model: 0.1 # learning rate, only used when percolator_backend==pytorch 
+  lr_percolator_torch_model: 0.1 # learning rate, only used when percolator_backend==pytorch
   percolator_iter_num: 5 # percolator iteration number
   cv_fold: 1
   fdr: 0.01
   fdr_level: psm
   fdr_level_choices:
     - psm
     - precursor
@@ -968,15 +958,15 @@
       - alphapept_hdf
       - thermo_raw # if alpharaw is installed
       - mgf
       - mzml
     ms_files: []
     other_score_column_mapping:
       alphapept: {}
-      pfind: 
+      pfind:
         raw_score: Raw_Score
       msfragger:
         hyperscore: hyperscore
         nextscore: nextscore
       maxquant: {}
   output_folder: "{PEPTDEEP_HOME}/rescore"
 ```
@@ -1040,15 +1030,15 @@
 Pipeline APIs provides the same functionalities with [CLI](#cli),
 including [library prediction](#library), [transfer
 learning](#transfer), and [rescoring](#rescore).
 
 ``` python
 from peptdeep.pipeline_api import (
     generate_library,
-    transfer_learn, 
+    transfer_learn,
     rescore,
 )
 ```
 
 All these functionalities take a `settings_dict` as the inputs, the dict
 structure is the same as the settings yaml file. See the documatation of `generate_library`, `transfer_learn`, `rescore` in https://alphapeptdeep.readthedocs.io/en/latest/module_pipeline_api.html.
```

### Comparing `peptdeep-1.1.9/peptdeep.egg-info/SOURCES.txt` & `peptdeep-1.2.0/peptdeep.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 peptdeep/__init__.py
 peptdeep/_modidx.py
 peptdeep/cli.py
 peptdeep/cli_argparse.py
 peptdeep/gui.py
 peptdeep/pipeline_api.py
```

### Comparing `peptdeep-1.1.9/peptdeep.egg-info/requires.txt` & `peptdeep-1.2.0/peptdeep.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 jupyter
 twine
 bumpversion
 pipdeptree
 ipykernel
 tqdm
 wget
-nbdev
 pyinstaller
 click
 pandas
 numpy
 seaborn
 matplotlib
 numba
@@ -48,24 +47,26 @@
 jinja2
 contextfilter
 furo
 torch
 streamlit
 alphabase
 alpharaw
+pytest
+pre-commit
+nbmake
 
 [development-stable]
 jupyter
 twine
 bumpversion
 pipdeptree
 ipykernel
 tqdm
 wget
-nbdev
 pyinstaller
 click
 pandas
 numpy
 seaborn
 matplotlib
 numba
@@ -82,14 +83,17 @@
 jinja2
 contextfilter
 furo
 torch
 streamlit>=1.23.0
 alphabase>=1.1.0
 alpharaw>=0.2.0
+pytest
+pre-commit==3.7.0
+nbmake==1.5.3
 
 [development-stable:sys_platform == "win32"]
 pywin32
 pythonnet
 
 [development:sys_platform == "win32"]
 pywin32
```

### Comparing `peptdeep-1.1.9/setup.py` & `peptdeep-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,14 @@
 
 
 def get_long_description():
     with open("README.md", "r") as readme_file:
         long_description = readme_file.read()
     return long_description
 
-#nbdev2
-# from configparser import ConfigParser
-# nbdev_config = ConfigParser(delimiters=['='])
-# nbdev_config.read('settings.ini')
-# nbdev_cfg = nbdev_config['DEFAULT']
-
 def get_requirements():
     extra_requirements = {}
     requirement_file_names = package2install.__extra_requirements__
     requirement_file_names[""] = "requirements.txt"
     for extra, requirement_file_name in requirement_file_names.items():
         full_requirement_file_name = os.path.join(
             "requirements",
@@ -62,15 +56,14 @@
         project_urls=package2install.__urls__,
         keywords=package2install.__keywords__,
         classifiers=package2install.__classifiers__,
         packages=[package2install.__project__],
         include_package_data=True,
         entry_points={
             "console_scripts": package2install.__console_scripts__,
-            # 'nbdev': [f'{nb.ydev_cfg.get("lib_path")}={nbdev_cfg.get("lib_path")}._modidx:d'],
         },
         install_requires=requirements,
         extras_require=extra_requirements,
         python_requires=package2install.__python_version__,
     )
```

