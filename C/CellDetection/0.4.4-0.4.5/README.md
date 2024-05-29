# Comparing `tmp/CellDetection-0.4.4.tar.gz` & `tmp/CellDetection-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CellDetection-0.4.4.tar", last modified: Tue Nov 14 17:05:27 2023, max compression
+gzip compressed data, was "CellDetection-0.4.5.tar", last modified: Wed Nov 15 13:30:53 2023, max compression
```

## Comparing `CellDetection-0.4.4.tar` & `CellDetection-0.4.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.233843 CellDetection-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.221843 CellDetection-0.4.4/CellDetection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23781 2023-11-14 17:05:27.000000 CellDetection-0.4.4/CellDetection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-11-14 17:05:27.000000 CellDetection-0.4.4/CellDetection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 17:05:27.000000 CellDetection-0.4.4/CellDetection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-14 17:05:27.000000 CellDetection-0.4.4/CellDetection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-14 17:05:27.000000 CellDetection-0.4.4/CellDetection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-14 17:05:17.000000 CellDetection-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-14 17:05:17.000000 CellDetection-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23781 2023-11-14 17:05:27.229843 CellDetection-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22662 2023-11-14 17:05:17.000000 CellDetection-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.221843 CellDetection-0.4.4/celldetection/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/__meta__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.221843 CellDetection-0.4.4/celldetection/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/callbacks/dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.225844 CellDetection-0.4.4/celldetection/data/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21356 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/cpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.225844 CellDetection-0.4.4/celldetection/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/datasets/bbbc038.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/datasets/bbbc039.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/datasets/bbbc041.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/datasets/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/datasets/synth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/instance_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    14850 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/data/toydata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.229843 CellDetection-0.4.4/celldetection/models/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27393 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    78316 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/cpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    16641 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    17291 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/manet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/mobilenetv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/ppm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18173 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/smp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/timmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    37241 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/models/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.229843 CellDetection-0.4.4/celldetection/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/mpi/mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.229843 CellDetection-0.4.4/celldetection/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/ops/boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/ops/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/ops/cpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/ops/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/ops/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/ops/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.229843 CellDetection-0.4.4/celldetection/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/optim/lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.229843 CellDetection-0.4.4/celldetection/util/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/util/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/util/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    47790 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:05:27.229843 CellDetection-0.4.4/celldetection/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/visualization/cmaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2023-11-14 17:05:17.000000 CellDetection-0.4.4/celldetection/visualization/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-14 17:05:17.000000 CellDetection-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 17:05:27.233843 CellDetection-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-11-14 17:05:17.000000 CellDetection-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.862284 CellDetection-0.4.5/CellDetection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23781 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-15 13:30:44.000000 CellDetection-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-15 13:30:44.000000 CellDetection-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23781 2023-11-15 13:30:53.870283 CellDetection-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22662 2023-11-15 13:30:44.000000 CellDetection-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.862284 CellDetection-0.4.5/celldetection/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/__meta__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.862284 CellDetection-0.4.5/celldetection/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/callbacks/dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.862284 CellDetection-0.4.5/celldetection/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21356 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/cpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.866284 CellDetection-0.4.5/celldetection/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/bbbc038.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/bbbc039.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/bbbc041.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/synth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/instance_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14850 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/toydata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.866284 CellDetection-0.4.5/celldetection/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27393 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78316 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/cpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16641 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17291 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/manet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/mobilenetv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/ppm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18173 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/smp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/timmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37241 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.866284 CellDetection-0.4.5/celldetection/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/mpi/mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/celldetection/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/cpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/celldetection/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/optim/lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/celldetection/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/util/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/util/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47790 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/celldetection/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/visualization/cmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/visualization/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-15 13:30:44.000000 CellDetection-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 13:30:53.870283 CellDetection-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-11-15 13:30:44.000000 CellDetection-0.4.5/setup.py
```

### Comparing `CellDetection-0.4.4/CellDetection.egg-info/PKG-INFO` & `CellDetection-0.4.5/CellDetection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CellDetection
-Version: 0.4.4
+Version: 0.4.5
 Summary: Cell Detection with PyTorch.
 Home-page: https://celldetection.org
 Author: Eric Upschulte
 Author-email: e.upschulte@fz-juelich.de
 License: Apache License, Version 2.0
 Keywords: cell,detection,object,segmentation,pytorch,cpn,contour,proposal,network,deep,learning,unet,fzj,julich,juelich,ai
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `CellDetection-0.4.4/CellDetection.egg-info/SOURCES.txt` & `CellDetection-0.4.5/CellDetection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/LICENSE` & `CellDetection-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/PKG-INFO` & `CellDetection-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CellDetection
-Version: 0.4.4
+Version: 0.4.5
 Summary: Cell Detection with PyTorch.
 Home-page: https://celldetection.org
 Author: Eric Upschulte
 Author-email: e.upschulte@fz-juelich.de
 License: Apache License, Version 2.0
 Keywords: cell,detection,object,segmentation,pytorch,cpn,contour,proposal,network,deep,learning,unet,fzj,julich,juelich,ai
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `CellDetection-0.4.4/README.md` & `CellDetection-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/callbacks/dropout.py` & `CellDetection-0.4.5/celldetection/callbacks/dropout.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/cpn.py` & `CellDetection-0.4.5/celldetection/data/cpn.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/datasets/bbbc038.py` & `CellDetection-0.4.5/celldetection/data/datasets/bbbc038.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/datasets/bbbc039.py` & `CellDetection-0.4.5/celldetection/data/datasets/bbbc039.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/datasets/bbbc041.py` & `CellDetection-0.4.5/celldetection/data/datasets/bbbc041.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/datasets/generic.py` & `CellDetection-0.4.5/celldetection/data/datasets/generic.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/datasets/synth.py` & `CellDetection-0.4.5/celldetection/data/datasets/synth.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/instance_eval.py` & `CellDetection-0.4.5/celldetection/data/instance_eval.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/misc.py` & `CellDetection-0.4.5/celldetection/data/misc.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/segmentation.py` & `CellDetection-0.4.5/celldetection/data/segmentation.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/data/toydata.py` & `CellDetection-0.4.5/celldetection/data/toydata.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/commons.py` & `CellDetection-0.4.5/celldetection/models/commons.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/convnext.py` & `CellDetection-0.4.5/celldetection/models/convnext.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/cpn.py` & `CellDetection-0.4.5/celldetection/models/cpn.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/features.py` & `CellDetection-0.4.5/celldetection/models/features.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/filters.py` & `CellDetection-0.4.5/celldetection/models/filters.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/fpn.py` & `CellDetection-0.4.5/celldetection/models/fpn.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/inference.py` & `CellDetection-0.4.5/celldetection/models/inference.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/lightning.py` & `CellDetection-0.4.5/celldetection/models/lightning.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/loss.py` & `CellDetection-0.4.5/celldetection/models/loss.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/manet.py` & `CellDetection-0.4.5/celldetection/models/manet.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/mobilenetv3.py` & `CellDetection-0.4.5/celldetection/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/normalization.py` & `CellDetection-0.4.5/celldetection/models/normalization.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/ppm.py` & `CellDetection-0.4.5/celldetection/models/ppm.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/resnet.py` & `CellDetection-0.4.5/celldetection/models/resnet.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/smp.py` & `CellDetection-0.4.5/celldetection/models/smp.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/timmodels.py` & `CellDetection-0.4.5/celldetection/models/timmodels.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/models/unet.py` & `CellDetection-0.4.5/celldetection/models/unet.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/mpi/mpi.py` & `CellDetection-0.4.5/celldetection/mpi/mpi.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/ops/boxes.py` & `CellDetection-0.4.5/celldetection/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/ops/commons.py` & `CellDetection-0.4.5/celldetection/ops/commons.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/ops/cpn.py` & `CellDetection-0.4.5/celldetection/ops/cpn.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/ops/draw.py` & `CellDetection-0.4.5/celldetection/ops/draw.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/ops/features.py` & `CellDetection-0.4.5/celldetection/ops/features.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/ops/loss.py` & `CellDetection-0.4.5/celldetection/ops/loss.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/ops/normalization.py` & `CellDetection-0.4.5/celldetection/ops/normalization.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/optim/lr_scheduler.py` & `CellDetection-0.4.5/celldetection/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/util/schedule.py` & `CellDetection-0.4.5/celldetection/util/schedule.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/util/timer.py` & `CellDetection-0.4.5/celldetection/util/timer.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/util/util.py` & `CellDetection-0.4.5/celldetection/util/util.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/visualization/cmaps.py` & `CellDetection-0.4.5/celldetection/visualization/cmaps.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/celldetection/visualization/images.py` & `CellDetection-0.4.5/celldetection/visualization/images.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.4/setup.py` & `CellDetection-0.4.5/setup.py`

 * *Files identical despite different names*

