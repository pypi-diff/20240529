# Comparing `tmp/alphadia-1.6.0.tar.gz` & `tmp/alphadia-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphadia-1.6.0.tar", last modified: Tue May 28 15:28:47 2024, max compression
+gzip compressed data, was "alphadia-1.6.1.tar", last modified: Wed May 29 17:24:54 2024, max compression
```

## Comparing `alphadia-1.6.0.tar` & `alphadia-1.6.1.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.235388 alphadia-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-28 15:28:06.000000 alphadia-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 15:28:06.000000 alphadia-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-05-28 15:28:47.235388 alphadia-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-28 15:28:06.000000 alphadia-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.231388 alphadia-1.6.0/alphaDIA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-05-28 15:28:47.000000 alphadia-1.6.0/alphaDIA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-28 15:28:47.000000 alphadia-1.6.0/alphaDIA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:28:47.000000 alphadia-1.6.0/alphaDIA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 15:28:47.000000 alphadia-1.6.0/alphaDIA.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-28 15:28:47.000000 alphadia-1.6.0/alphaDIA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 15:28:47.000000 alphadia-1.6.0/alphaDIA.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.223388 alphadia-1.6.0/alphadia/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.223388 alphadia-1.6.0/alphadia/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/calibration/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/calibration/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.223388 alphadia-1.6.0/alphadia/constants/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.227388 alphadia-1.6.0/alphadia/constants/classifier/
--rw-r--r--   0 runner    (1001) docker     (127)    51796 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/constants/classifier/fa9945ae23db872d.pth
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/constants/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.227388 alphadia-1.6.0/alphadia/data/
--rw-r--r--   0 runner    (1001) docker     (127)    29633 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/data/alpharaw.py
--rw-r--r--   0 runner    (1001) docker     (127)    32847 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/data/bruker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/fdr.py
--rw-r--r--   0 runner    (1001) docker     (127)    38795 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/fdrexperimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    45476 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/fragcomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/libtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.227388 alphadia-1.6.0/alphadia/numba/
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/numba/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/numba/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/numba/fragments.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/numba/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)    19948 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/outputaccumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    34716 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/outputtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.227388 alphadia-1.6.0/alphadia/peakgroup/
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/peakgroup/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    36386 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/peakgroup/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/peakgroup/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/planning.py
--rw-r--r--   0 runner    (1001) docker     (127)    62836 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/plexscoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.227388 alphadia-1.6.0/alphadia/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/plotting/cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/plotting/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/plotting/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/quadrupole.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/test_data_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.227388 alphadia-1.6.0/alphadia/transferlearning/
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/transferlearning/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/transferlearning/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.227388 alphadia-1.6.0/alphadia/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20173 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/workflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23098 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/workflow/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    43905 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/workflow/peptidecentric.py
--rw-r--r--   0 runner    (1001) docker     (127)    18414 2024-05-28 15:28:06.000000 alphadia-1.6.0/alphadia/workflow/reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.231388 alphadia-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-28 15:28:06.000000 alphadia-1.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-28 15:28:06.000000 alphadia-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.219388 alphadia-1.6.0/release/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.231388 alphadia-1.6.0/release/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-28 15:28:06.000000 alphadia-1.6.0/release/pyinstaller/cli_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.231388 alphadia-1.6.0/release/pyinstaller/hookdir/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 15:28:06.000000 alphadia-1.6.0/release/pyinstaller/hookdir/hook-huggingface_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-28 15:28:06.000000 alphadia-1.6.0/release/pyinstaller/hookdir/hook-rocket_fft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:28:47.231388 alphadia-1.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 15:28:06.000000 alphadia-1.6.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 15:28:06.000000 alphadia-1.6.0/requirements/requirements_development.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-28 15:28:06.000000 alphadia-1.6.0/requirements/requirements_loose.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-28 15:28:06.000000 alphadia-1.6.0/requirements/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:28:47.235388 alphadia-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.642790 alphadia-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-29 17:24:20.000000 alphadia-1.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 17:24:20.000000 alphadia-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24606 2024-05-29 17:24:54.642790 alphadia-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-29 17:24:20.000000 alphadia-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.638790 alphadia-1.6.1/alphaDIA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24606 2024-05-29 17:24:54.000000 alphadia-1.6.1/alphaDIA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-29 17:24:54.000000 alphadia-1.6.1/alphaDIA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:24:54.000000 alphadia-1.6.1/alphaDIA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 17:24:54.000000 alphadia-1.6.1/alphaDIA.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-29 17:24:54.000000 alphadia-1.6.1/alphaDIA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 17:24:54.000000 alphadia-1.6.1/alphaDIA.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.630790 alphadia-1.6.1/alphadia/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.630790 alphadia-1.6.1/alphadia/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/calibration/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/calibration/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.630790 alphadia-1.6.1/alphadia/constants/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.630790 alphadia-1.6.1/alphadia/constants/classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)    51796 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/constants/classifier/fa9945ae23db872d.pth
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/constants/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/alphadia/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    29633 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/data/alpharaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32847 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/data/bruker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38795 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/fdrexperimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45476 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/fragcomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/libtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/alphadia/numba/
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/numba/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/numba/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/numba/fragments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/numba/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19948 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/outputaccumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34824 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/outputtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/alphadia/peakgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/peakgroup/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36386 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/peakgroup/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/peakgroup/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/planning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62836 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/plexscoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/alphadia/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/plotting/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/plotting/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/plotting/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/quadrupole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/test_data_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/alphadia/transferlearning/
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/transferlearning/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/transferlearning/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/alphadia/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20173 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/workflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23098 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/workflow/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43996 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/workflow/peptidecentric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18414 2024-05-29 17:24:20.000000 alphadia-1.6.1/alphadia/workflow/reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-29 17:24:20.000000 alphadia-1.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-29 17:24:20.000000 alphadia-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.626790 alphadia-1.6.1/release/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/release/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-29 17:24:20.000000 alphadia-1.6.1/release/pyinstaller/cli_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.634791 alphadia-1.6.1/release/pyinstaller/hookdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 17:24:20.000000 alphadia-1.6.1/release/pyinstaller/hookdir/hook-huggingface_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 17:24:20.000000 alphadia-1.6.1/release/pyinstaller/hookdir/hook-rocket_fft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:54.638790 alphadia-1.6.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-29 17:24:20.000000 alphadia-1.6.1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-29 17:24:20.000000 alphadia-1.6.1/requirements/requirements_development.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 17:24:20.000000 alphadia-1.6.1/requirements/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-29 17:24:20.000000 alphadia-1.6.1/requirements/requirements_loose.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 17:24:20.000000 alphadia-1.6.1/requirements/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:24:54.642790 alphadia-1.6.1/setup.cfg
```

### Comparing `alphadia-1.6.0/LICENSE.txt` & `alphadia-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/PKG-INFO` & `alphadia-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphaDIA
-Version: 1.6.0
+Version: 1.6.1
 Summary: A novel proteomics search engine for DIA data based on end-to-end transfer learning.
 Author-email: Mann Labs <wallmann@biochem.mpg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -227,14 +227,15 @@
 Requires-Dist: peptdeep
 Requires-Dist: progressbar
 Requires-Dist: neptune
 Requires-Dist: seaborn
 Requires-Dist: rocket_fft
 Requires-Dist: xxhash
 Requires-Dist: torchmetrics
+Requires-Dist: transformers<=4.40.2
 Requires-Dist: directlfq
 Requires-Dist: pythonnet
 Requires-Dist: zstandard
 Requires-Dist: scipy>=1.12.0
 Provides-Extra: stable
 Requires-Dist: numba==0.59.1; extra == "stable"
 Requires-Dist: argparse==1.4.0; extra == "stable"
@@ -244,42 +245,43 @@
 Requires-Dist: peptdeep==1.1.9; extra == "stable"
 Requires-Dist: progressbar==2.5; extra == "stable"
 Requires-Dist: neptune==1.10.4; extra == "stable"
 Requires-Dist: seaborn==0.13.2; extra == "stable"
 Requires-Dist: rocket_fft==0.2.5; extra == "stable"
 Requires-Dist: xxhash==3.4.1; extra == "stable"
 Requires-Dist: torchmetrics==1.4.0.post0; extra == "stable"
+Requires-Dist: transformers==4.40.2; extra == "stable"
 Requires-Dist: directlfq==0.2.19; extra == "stable"
 Requires-Dist: pythonnet==3.0.3; extra == "stable"
 Requires-Dist: zstandard==0.22.0; extra == "stable"
 Requires-Dist: scipy==1.12.0; extra == "stable"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: coverage-badge; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: development
 Requires-Dist: jupyter; extra == "development"
 Requires-Dist: jupyter_contrib_nbextensions; extra == "development"
 Requires-Dist: pyinstaller; extra == "development"
-Requires-Dist: autodocsumm; extra == "development"
-Requires-Dist: sphinx-rtd-theme; extra == "development"
-Requires-Dist: nbsphinx; extra == "development"
-Requires-Dist: myst_parser; extra == "development"
-Requires-Dist: sphinx_design; extra == "development"
-Requires-Dist: furo; extra == "development"
 Requires-Dist: twine; extra == "development"
 Requires-Dist: bumpversion; extra == "development"
 Requires-Dist: pipdeptree; extra == "development"
 Requires-Dist: ipykernel; extra == "development"
 Requires-Dist: psutil; extra == "development"
 Requires-Dist: pre-commit==3.7.0; extra == "development"
 Requires-Dist: pywin32; sys_platform == "win32" and extra == "development"
 Requires-Dist: coverage; extra == "development"
 Requires-Dist: coverage-badge; extra == "development"
 Requires-Dist: pytest; extra == "development"
+Requires-Dist: autodocsumm; extra == "development"
+Requires-Dist: sphinx-rtd-theme; extra == "development"
+Requires-Dist: nbsphinx; extra == "development"
+Requires-Dist: myst_parser; extra == "development"
+Requires-Dist: sphinx_design; extra == "development"
+Requires-Dist: furo; extra == "development"
 
 ![Release](https://img.shields.io/badge/release-v1.6.0-brightgreen)
 ![License](https://img.shields.io/badge/License-Apache-brightgreen)
 ![Tests](https://github.com/MannLabs/alphadia/workflows/Default%20installation%20and%20tests/badge.svg)
 ![Deployment](https://github.com/MannLabs/alphadia/workflows/Publish%20on%20PyPi%20and%20release%20on%20GitHub/badge.svg)
 ![Coverage](https://github.com/MannLabs/alphadia/blob/main/coverage.svg)
 
@@ -418,21 +420,23 @@
 
 * [Issues](https://github.com/MannLabs/alphadia/issues): Try a few different search terms to find out if a similar problem has been encountered before
 * [Discussions](https://github.com/MannLabs/alphadia/discussions): Check if your problem or feature requests has been discussed before.
 
 ---
 ## Citations
 
-There are currently only vague plans to draft a manuscript.
+A manuscript has been submitted to bioRxiv.
 
 ---
 ## How to contribute
 
 If you like this software, you can give us a [star](https://github.com/MannLabs/alphadia/stargazers) to boost our visibility! All direct contributions are also welcome. Feel free to post a new [issue](https://github.com/MannLabs/alphadia/issues) or clone the repository and create a [pull request](https://github.com/MannLabs/alphadia/pulls) with a new branch. For an even more interactive participation, check out the [discussions](https://github.com/MannLabs/alphadia/discussions) and the [the Contributors License Agreement](misc/CLA.md).
 
+Further information on the development process can be found [here](docs/installation.md).
+
 ---
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made in each version.
 
 ---
 ## About
```

### Comparing `alphadia-1.6.0/README.md` & `alphadia-1.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -139,21 +139,23 @@
 
 * [Issues](https://github.com/MannLabs/alphadia/issues): Try a few different search terms to find out if a similar problem has been encountered before
 * [Discussions](https://github.com/MannLabs/alphadia/discussions): Check if your problem or feature requests has been discussed before.
 
 ---
 ## Citations
 
-There are currently only vague plans to draft a manuscript.
+A manuscript has been submitted to bioRxiv.
 
 ---
 ## How to contribute
 
 If you like this software, you can give us a [star](https://github.com/MannLabs/alphadia/stargazers) to boost our visibility! All direct contributions are also welcome. Feel free to post a new [issue](https://github.com/MannLabs/alphadia/issues) or clone the repository and create a [pull request](https://github.com/MannLabs/alphadia/pulls) with a new branch. For an even more interactive participation, check out the [discussions](https://github.com/MannLabs/alphadia/discussions) and the [the Contributors License Agreement](misc/CLA.md).
 
+Further information on the development process can be found [here](docs/installation.md).
+
 ---
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made in each version.
 
 ---
 ## About
```

#### html2text {}

```diff
@@ -78,24 +78,25 @@
 files Select an output folder where the search progress and the final results
 should be saved. ### 4. Run the search Click *Run Workflow* to start the search
 and see the progress. --- ## Troubleshooting In case of issues, check out the
 following: * [Issues](https://github.com/MannLabs/alphadia/issues): Try a few
 different search terms to find out if a similar problem has been encountered
 before * [Discussions](https://github.com/MannLabs/alphadia/discussions): Check
 if your problem or feature requests has been discussed before. --- ## Citations
-There are currently only vague plans to draft a manuscript. --- ## How to
-contribute If you like this software, you can give us a [star](https://
-github.com/MannLabs/alphadia/stargazers) to boost our visibility! All direct
-contributions are also welcome. Feel free to post a new [issue](https://
-github.com/MannLabs/alphadia/issues) or clone the repository and create a [pull
-request](https://github.com/MannLabs/alphadia/pulls) with a new branch. For an
-even more interactive participation, check out the [discussions](https://
-github.com/MannLabs/alphadia/discussions) and the [the Contributors License
-Agreement](misc/CLA.md). --- ## Changelog See the [HISTORY.md](HISTORY.md) for
-a full overview of the changes made in each version. --- ## About An open-
-source Python package of the AlphaPept ecosystem from the [Mann Labs at the Max
-Planck Institute of Biochemistry](https://www.biochem.mpg.de/mann). --- ##
-License AlphaDIA was developed by the [Mann Labs at the Max Planck Institute of
+A manuscript has been submitted to bioRxiv. --- ## How to contribute If you
+like this software, you can give us a [star](https://github.com/MannLabs/
+alphadia/stargazers) to boost our visibility! All direct contributions are also
+welcome. Feel free to post a new [issue](https://github.com/MannLabs/alphadia/
+issues) or clone the repository and create a [pull request](https://github.com/
+MannLabs/alphadia/pulls) with a new branch. For an even more interactive
+participation, check out the [discussions](https://github.com/MannLabs/
+alphadia/discussions) and the [the Contributors License Agreement](misc/
+CLA.md). Further information on the development process can be found [here]
+(docs/installation.md). --- ## Changelog See the [HISTORY.md](HISTORY.md) for a
+full overview of the changes made in each version. --- ## About An open-source
+Python package of the AlphaPept ecosystem from the [Mann Labs at the Max Planck
+Institute of Biochemistry](https://www.biochem.mpg.de/mann). --- ## License
+AlphaDIA was developed by the [Mann Labs at the Max Planck Institute of
 Biochemistry](https://www.biochem.mpg.de/mann) and is freely available with an
 [Apache License](LICENSE.txt). External Python packages (available in the
 [requirements](requirements) folder) have their own licenses, which can be
 consulted on their respective websites. ---
```

### Comparing `alphadia-1.6.0/alphaDIA.egg-info/PKG-INFO` & `alphadia-1.6.1/alphaDIA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphaDIA
-Version: 1.6.0
+Version: 1.6.1
 Summary: A novel proteomics search engine for DIA data based on end-to-end transfer learning.
 Author-email: Mann Labs <wallmann@biochem.mpg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -227,14 +227,15 @@
 Requires-Dist: peptdeep
 Requires-Dist: progressbar
 Requires-Dist: neptune
 Requires-Dist: seaborn
 Requires-Dist: rocket_fft
 Requires-Dist: xxhash
 Requires-Dist: torchmetrics
+Requires-Dist: transformers<=4.40.2
 Requires-Dist: directlfq
 Requires-Dist: pythonnet
 Requires-Dist: zstandard
 Requires-Dist: scipy>=1.12.0
 Provides-Extra: stable
 Requires-Dist: numba==0.59.1; extra == "stable"
 Requires-Dist: argparse==1.4.0; extra == "stable"
@@ -244,42 +245,43 @@
 Requires-Dist: peptdeep==1.1.9; extra == "stable"
 Requires-Dist: progressbar==2.5; extra == "stable"
 Requires-Dist: neptune==1.10.4; extra == "stable"
 Requires-Dist: seaborn==0.13.2; extra == "stable"
 Requires-Dist: rocket_fft==0.2.5; extra == "stable"
 Requires-Dist: xxhash==3.4.1; extra == "stable"
 Requires-Dist: torchmetrics==1.4.0.post0; extra == "stable"
+Requires-Dist: transformers==4.40.2; extra == "stable"
 Requires-Dist: directlfq==0.2.19; extra == "stable"
 Requires-Dist: pythonnet==3.0.3; extra == "stable"
 Requires-Dist: zstandard==0.22.0; extra == "stable"
 Requires-Dist: scipy==1.12.0; extra == "stable"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: coverage-badge; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: development
 Requires-Dist: jupyter; extra == "development"
 Requires-Dist: jupyter_contrib_nbextensions; extra == "development"
 Requires-Dist: pyinstaller; extra == "development"
-Requires-Dist: autodocsumm; extra == "development"
-Requires-Dist: sphinx-rtd-theme; extra == "development"
-Requires-Dist: nbsphinx; extra == "development"
-Requires-Dist: myst_parser; extra == "development"
-Requires-Dist: sphinx_design; extra == "development"
-Requires-Dist: furo; extra == "development"
 Requires-Dist: twine; extra == "development"
 Requires-Dist: bumpversion; extra == "development"
 Requires-Dist: pipdeptree; extra == "development"
 Requires-Dist: ipykernel; extra == "development"
 Requires-Dist: psutil; extra == "development"
 Requires-Dist: pre-commit==3.7.0; extra == "development"
 Requires-Dist: pywin32; sys_platform == "win32" and extra == "development"
 Requires-Dist: coverage; extra == "development"
 Requires-Dist: coverage-badge; extra == "development"
 Requires-Dist: pytest; extra == "development"
+Requires-Dist: autodocsumm; extra == "development"
+Requires-Dist: sphinx-rtd-theme; extra == "development"
+Requires-Dist: nbsphinx; extra == "development"
+Requires-Dist: myst_parser; extra == "development"
+Requires-Dist: sphinx_design; extra == "development"
+Requires-Dist: furo; extra == "development"
 
 ![Release](https://img.shields.io/badge/release-v1.6.0-brightgreen)
 ![License](https://img.shields.io/badge/License-Apache-brightgreen)
 ![Tests](https://github.com/MannLabs/alphadia/workflows/Default%20installation%20and%20tests/badge.svg)
 ![Deployment](https://github.com/MannLabs/alphadia/workflows/Publish%20on%20PyPi%20and%20release%20on%20GitHub/badge.svg)
 ![Coverage](https://github.com/MannLabs/alphadia/blob/main/coverage.svg)
 
@@ -418,21 +420,23 @@
 
 * [Issues](https://github.com/MannLabs/alphadia/issues): Try a few different search terms to find out if a similar problem has been encountered before
 * [Discussions](https://github.com/MannLabs/alphadia/discussions): Check if your problem or feature requests has been discussed before.
 
 ---
 ## Citations
 
-There are currently only vague plans to draft a manuscript.
+A manuscript has been submitted to bioRxiv.
 
 ---
 ## How to contribute
 
 If you like this software, you can give us a [star](https://github.com/MannLabs/alphadia/stargazers) to boost our visibility! All direct contributions are also welcome. Feel free to post a new [issue](https://github.com/MannLabs/alphadia/issues) or clone the repository and create a [pull request](https://github.com/MannLabs/alphadia/pulls) with a new branch. For an even more interactive participation, check out the [discussions](https://github.com/MannLabs/alphadia/discussions) and the [the Contributors License Agreement](misc/CLA.md).
 
+Further information on the development process can be found [here](docs/installation.md).
+
 ---
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made in each version.
 
 ---
 ## About
```

### Comparing `alphadia-1.6.0/alphaDIA.egg-info/SOURCES.txt` & `alphadia-1.6.1/alphaDIA.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -49,9 +49,10 @@
 alphadia/workflow/reporting.py
 docs/conf.py
 release/pyinstaller/cli_hook.py
 release/pyinstaller/hookdir/hook-huggingface_hub.py
 release/pyinstaller/hookdir/hook-rocket_fft.py
 requirements/requirements.txt
 requirements/requirements_development.txt
+requirements/requirements_docs.txt
 requirements/requirements_loose.txt
 requirements/requirements_test.txt
```

### Comparing `alphadia-1.6.0/alphaDIA.egg-info/requires.txt` & `alphadia-1.6.1/alphaDIA.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,38 +6,39 @@
 peptdeep
 progressbar
 neptune
 seaborn
 rocket_fft
 xxhash
 torchmetrics
+transformers<=4.40.2
 directlfq
 pythonnet
 zstandard
 scipy>=1.12.0
 
 [development]
 jupyter
 jupyter_contrib_nbextensions
 pyinstaller
-autodocsumm
-sphinx-rtd-theme
-nbsphinx
-myst_parser
-sphinx_design
-furo
 twine
 bumpversion
 pipdeptree
 ipykernel
 psutil
 pre-commit==3.7.0
 coverage
 coverage-badge
 pytest
+autodocsumm
+sphinx-rtd-theme
+nbsphinx
+myst_parser
+sphinx_design
+furo
 
 [development:sys_platform == "win32"]
 pywin32
 
 [stable]
 numba==0.59.1
 argparse==1.4.0
@@ -47,14 +48,15 @@
 peptdeep==1.1.9
 progressbar==2.5
 neptune==1.10.4
 seaborn==0.13.2
 rocket_fft==0.2.5
 xxhash==3.4.1
 torchmetrics==1.4.0.post0
+transformers==4.40.2
 directlfq==0.2.19
 pythonnet==3.0.3
 zstandard==0.22.0
 scipy==1.12.0
 
 [test]
 coverage
```

### Comparing `alphadia-1.6.0/alphadia/calibration/models.py` & `alphadia-1.6.1/alphadia/calibration/models.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/calibration/property.py` & `alphadia-1.6.1/alphadia/calibration/property.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/cli.py` & `alphadia-1.6.1/alphadia/cli.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/constants/classifier/fa9945ae23db872d.pth` & `alphadia-1.6.1/alphadia/constants/classifier/fa9945ae23db872d.pth`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/constants/default.yaml` & `alphadia-1.6.1/alphadia/constants/default.yaml`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/data/alpharaw.py` & `alphadia-1.6.1/alphadia/data/alpharaw.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/data/bruker.py` & `alphadia-1.6.1/alphadia/data/bruker.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/fdr.py` & `alphadia-1.6.1/alphadia/fdr.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/fdrexperimental.py` & `alphadia-1.6.1/alphadia/fdrexperimental.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/features.py` & `alphadia-1.6.1/alphadia/features.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/fragcomp.py` & `alphadia-1.6.1/alphadia/fragcomp.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/grouping.py` & `alphadia-1.6.1/alphadia/grouping.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/libtransform.py` & `alphadia-1.6.1/alphadia/libtransform.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/numba/config.py` & `alphadia-1.6.1/alphadia/numba/config.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/numba/fft.py` & `alphadia-1.6.1/alphadia/numba/fft.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/numba/fragments.py` & `alphadia-1.6.1/alphadia/numba/fragments.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/numba/numeric.py` & `alphadia-1.6.1/alphadia/numba/numeric.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/outputaccumulator.py` & `alphadia-1.6.1/alphadia/outputaccumulator.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/outputtransform.py` & `alphadia-1.6.1/alphadia/outputtransform.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,19 @@
         -------
 
         stat_df: pd.DataFrame
             Precursor table
         """
         logger.progress("Building search statistics")
 
-        all_channels = set(self.config["search"]["channel_filter"].split(","))
+        if self.config["search"]["channel_filter"] == "":
+            all_channels = {0}
+        else:
+            all_channels = set(self.config["search"]["channel_filter"].split(","))
+
         if self.config["multiplexing"]["enabled"]:
             all_channels &= set(
                 self.config["multiplexing"]["target_channels"].split(",")
             )
         all_channels = sorted([int(c) for c in all_channels])
 
         if psm_df is None:
```

### Comparing `alphadia-1.6.0/alphadia/peakgroup/kernel.py` & `alphadia-1.6.1/alphadia/peakgroup/kernel.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/peakgroup/search.py` & `alphadia-1.6.1/alphadia/peakgroup/search.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/peakgroup/utils.py` & `alphadia-1.6.1/alphadia/peakgroup/utils.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/planning.py` & `alphadia-1.6.1/alphadia/planning.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,40 +327,51 @@
                 psm_df.to_csv(psm_location, sep="\t", index=False)
                 frag_df.to_csv(frag_location, sep="\t", index=False)
 
                 workflow.reporter.log_string(f"Finished workflow for {raw_name}")
                 workflow.reporter.context.__exit__(None, None, None)
                 del workflow
 
-            except Exception as e:
+            except peptidecentric.CalibrationError as e:
                 # get full traceback
-                import traceback
-
-                traceback.print_exc()
-
-                print(e)
-                logger.error(f"Workflow failed for {raw_name} with error {e}")
+                logger.error(
+                    f"Search for {raw_name} failed as not enough precursors were found for calibration"
+                )
+                logger.error(f"This can have the following reasons:")
+                logger.error(
+                    f"   1. The sample was empty and therefore nor precursors were found"
+                )
+                logger.error(f"   2. The sample contains only very few precursors.")
+                logger.error(
+                    f"      For small libraries, try to set recalibration_target to a lower value"
+                )
+                logger.error(
+                    f"      For large libraries, try to reduce the library size and reduce the calibration MS1 and MS2 tolerance"
+                )
+                logger.error(
+                    f"   3. There was a fundamental issue with search parameters"
+                )
                 continue
+            except Exception as e:
+                logger.error(
+                    f"Search for {raw_name} failed with error {e}", exc_info=True
+                )
+                raise e
 
         try:
             base_spec_lib = SpecLibBase()
             base_spec_lib.load_hdf(
                 os.path.join(self.output_folder, "speclib.hdf"), load_mod_seq=True
             )
 
             output = outputtransform.SearchPlanOutput(self.config, self.output_folder)
             output.build(workflow_folder_list, base_spec_lib)
 
         except Exception as e:
-            # get full traceback
-            import traceback
-
-            traceback.print_exc()
-            print(e)
-            logger.error(f"Output failed with error {e}")
+            logger.error(f"Output failed with error {e}", exc_info=True)
             return
 
         logger.progress("=================== Search Finished ===================")
 
     def clean(self):
         if not self.config["library_loading"]["save_hdf"]:
             os.remove(os.path.join(self.output_folder, "speclib.hdf"))
```

### Comparing `alphadia-1.6.0/alphadia/plexscoring.py` & `alphadia-1.6.1/alphadia/plexscoring.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/plotting/cycle.py` & `alphadia-1.6.1/alphadia/plotting/cycle.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/plotting/debug.py` & `alphadia-1.6.1/alphadia/plotting/debug.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/plotting/utils.py` & `alphadia-1.6.1/alphadia/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/quadrupole.py` & `alphadia-1.6.1/alphadia/quadrupole.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/test_data_downloader.py` & `alphadia-1.6.1/alphadia/test_data_downloader.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/transferlearning/metrics.py` & `alphadia-1.6.1/alphadia/transferlearning/metrics.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/transferlearning/train.py` & `alphadia-1.6.1/alphadia/transferlearning/train.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/utils.py` & `alphadia-1.6.1/alphadia/utils.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/validate.py` & `alphadia-1.6.1/alphadia/validate.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/workflow/base.py` & `alphadia-1.6.1/alphadia/workflow/base.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/workflow/config.py` & `alphadia-1.6.1/alphadia/workflow/config.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/workflow/manager.py` & `alphadia-1.6.1/alphadia/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/alphadia/workflow/peptidecentric.py` & `alphadia-1.6.1/alphadia/workflow/peptidecentric.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,20 @@
 ]
 
 classifier_base = fdrx.BinaryClassifierLegacyNewBatching(
     test_size=0.001, batch_size=5000, learning_rate=0.001, epochs=10
 )
 
 
+class CalibrationError(Exception):
+    """Raised when calibration fails"""
+
+    pass
+
+
 class PeptideCentricWorkflow(base.WorkflowBase):
     def __init__(
         self,
         instance_name: str,
         config: dict,
     ) -> None:
         super().__init__(
@@ -485,15 +491,15 @@
                 else:
                     # check if last step has been reached
                     if current_step == len(self.batch_plan) - 1:
                         self.reporter.log_string(
                             "Searched all data without finding recalibration target",
                             verbosity="error",
                         )
-                        raise RuntimeError(
+                        raise CalibrationError(
                             "Searched all data without finding recalibration target"
                         )
 
             self.end_of_epoch()
 
         if "final_full_calibration" in self.config["calibration"]:
             if self.config["calibration"]["final_full_calibration"]:
```

### Comparing `alphadia-1.6.0/alphadia/workflow/reporting.py` & `alphadia-1.6.1/alphadia/workflow/reporting.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/docs/conf.py` & `alphadia-1.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/pyproject.toml` & `alphadia-1.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -48,13 +48,13 @@
 find = {}
 
 [tool.setuptools.dynamic]
 # https://stackoverflow.com/a/73600610
 dependencies = {file = ["requirements/requirements_loose.txt"]}
 optional-dependencies = { stable = { file = ["requirements/requirements.txt",
 ] }, test = { file = [ "requirements/requirements_test.txt",
-] }, development = { file = ["requirements/requirements_development.txt", "requirements/requirements_test.txt"
+] }, development = { file = ["requirements/requirements_development.txt", "requirements/requirements_test.txt", "requirements/requirements_docs.txt"
 ] }}
 version = {attr = "alphadia.__version__"}
 
 [project.scripts]
 alphadia = "alphadia.cli:run"
```

### Comparing `alphadia-1.6.0/release/pyinstaller/cli_hook.py` & `alphadia-1.6.1/release/pyinstaller/cli_hook.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/release/pyinstaller/hookdir/hook-rocket_fft.py` & `alphadia-1.6.1/release/pyinstaller/hookdir/hook-rocket_fft.py`

 * *Files identical despite different names*

### Comparing `alphadia-1.6.0/requirements/requirements.txt` & `alphadia-1.6.1/requirements/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 peptdeep==1.1.9
 progressbar==2.5
 neptune==1.10.4
 seaborn==0.13.2
 rocket_fft==0.2.5
 xxhash==3.4.1
 torchmetrics==1.4.0.post0
+transformers==4.40.2
 directlfq==0.2.19
 pythonnet==3.0.3
 zstandard==0.22.0
 # not direct dependencies but we have to restrict the versions
 scipy==1.12.0
```

