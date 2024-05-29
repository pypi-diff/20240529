# Comparing `tmp/CellDetection-0.4.5.tar.gz` & `tmp/celldetection-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CellDetection-0.4.5.tar", last modified: Wed Nov 15 13:30:53 2023, max compression
+gzip compressed data, was "celldetection-0.4.8.tar", last modified: Wed May 29 14:36:53 2024, max compression
```

## Comparing `CellDetection-0.4.5.tar` & `celldetection-0.4.8.tar`

### file list

```diff
@@ -1,77 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.862284 CellDetection-0.4.5/CellDetection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23781 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-15 13:30:53.000000 CellDetection-0.4.5/CellDetection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-15 13:30:44.000000 CellDetection-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-15 13:30:44.000000 CellDetection-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23781 2023-11-15 13:30:53.870283 CellDetection-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22662 2023-11-15 13:30:44.000000 CellDetection-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.862284 CellDetection-0.4.5/celldetection/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/__meta__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.862284 CellDetection-0.4.5/celldetection/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/callbacks/dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.862284 CellDetection-0.4.5/celldetection/data/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21356 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/cpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.866284 CellDetection-0.4.5/celldetection/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/bbbc038.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/bbbc039.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/bbbc041.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/datasets/synth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/instance_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    14850 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/data/toydata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.866284 CellDetection-0.4.5/celldetection/models/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27393 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    78316 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/cpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    16641 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    17291 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/manet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/mobilenetv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/ppm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18173 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/smp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/timmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    37241 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/models/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.866284 CellDetection-0.4.5/celldetection/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/mpi/mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/celldetection/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/cpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/ops/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/celldetection/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/optim/lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/celldetection/util/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/util/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/util/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    47790 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:30:53.870283 CellDetection-0.4.5/celldetection/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/visualization/cmaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2023-11-15 13:30:44.000000 CellDetection-0.4.5/celldetection/visualization/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-15 13:30:44.000000 CellDetection-0.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 13:30:53.870283 CellDetection-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-11-15 13:30:44.000000 CellDetection-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.620405 celldetection-0.4.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.616405 celldetection-0.4.8/CellDetection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25859 2024-05-29 14:36:53.000000 celldetection-0.4.8/CellDetection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-29 14:36:53.000000 celldetection-0.4.8/CellDetection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:36:53.000000 celldetection-0.4.8/CellDetection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 14:36:53.000000 celldetection-0.4.8/CellDetection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-29 14:36:53.000000 celldetection-0.4.8/CellDetection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 14:36:53.000000 celldetection-0.4.8/CellDetection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 14:36:49.000000 celldetection-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 14:36:49.000000 celldetection-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25859 2024-05-29 14:36:53.620405 celldetection-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24693 2024-05-29 14:36:49.000000 celldetection-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.608405 celldetection-0.4.8/celldetection/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/__meta__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.608405 celldetection-0.4.8/celldetection/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/callbacks/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/callbacks/keepalive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.608405 celldetection-0.4.8/celldetection/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25987 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/cpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.608405 celldetection-0.4.8/celldetection/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/datasets/bbbc038.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/datasets/bbbc039.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/datasets/bbbc041.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/datasets/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/datasets/synth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18816 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/instance_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/toydata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.612405 celldetection-0.4.8/celldetection/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29810 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15832 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19165 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/convnextv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78316 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/cpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17946 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/lightning_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/lightning_cpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/mamba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/manet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/mobilenetv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/ppm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/smp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/timmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37678 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/models/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.612405 celldetection-0.4.8/celldetection/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/mpi/mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.616405 celldetection-0.4.8/celldetection/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/ops/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/ops/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/ops/cpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/ops/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/ops/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/ops/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.616405 celldetection-0.4.8/celldetection/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/optim/lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.616405 celldetection-0.4.8/celldetection/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/util/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/util/shm_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/util/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66941 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.616405 celldetection-0.4.8/celldetection/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/visualization/cmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection/visualization/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:53.616405 celldetection-0.4.8/celldetection_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38427 2024-05-29 14:36:49.000000 celldetection-0.4.8/celldetection_scripts/cpn_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-29 14:36:49.000000 celldetection-0.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:36:53.620405 celldetection-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-29 14:36:49.000000 celldetection-0.4.8/setup.py
```

### Comparing `CellDetection-0.4.5/CellDetection.egg-info/PKG-INFO` & `celldetection-0.4.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: CellDetection
-Version: 0.4.5
-Summary: Cell Detection with PyTorch.
-Home-page: https://celldetection.org
-Author: Eric Upschulte
-Author-email: e.upschulte@fz-juelich.de
-License: Apache License, Version 2.0
-Keywords: cell,detection,object,segmentation,pytorch,cpn,contour,proposal,network,deep,learning,unet,fzj,julich,juelich,ai
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-Requires-Dist: scikit-image
-Requires-Dist: opencv-python
-Requires-Dist: torch>=2.0.0
-Requires-Dist: torchvision
-Requires-Dist: seaborn
-Requires-Dist: tqdm
-Requires-Dist: h5py
-Requires-Dist: pillow
-Requires-Dist: pynvml>=11.0.0
-Requires-Dist: albumentations>=1.3.0
-Requires-Dist: timm
-Requires-Dist: segmentation-models-pytorch
-Requires-Dist: pandas
-Requires-Dist: pytorch_lightning
-
 # Cell Detection
 
 [![Downloads](https://static.pepy.tech/badge/celldetection?l)](https://pepy.tech/project/celldetection)
 [![Test](https://github.com/FZJ-INM1-BDA/celldetection/workflows/Test/badge.svg)](https://github.com/FZJ-INM1-BDA/celldetection/actions?query=workflow%3ATest)
 [![PyPI](https://img.shields.io/pypi/v/celldetection?l)](https://pypi.org/project/celldetection/)
 [![Documentation Status](https://readthedocs.org/projects/celldetection/badge/?version=latest)](https://celldetection.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/349111085.svg)](https://zenodo.org/badge/latestdoi/349111085)
@@ -363,48 +330,106 @@
 ```
 
 
 ## 🤗 Hugging Face Spaces
 
 Find us on Hugging Face and upload your own images for segmentation: https://huggingface.co/spaces/ericup/celldetection
 
+There's also an API (Python & JavaScript), allowing you to utilize community GPUs (currently Nvidia A100) remotely!
+
 <details>
     <summary style="font-weight: bold; color: #888888">Hugging Face API</summary>
 
 ### Python
 
 ```python
-import requests
+from gradio_client import Client
+
+# Define inputs (local filename or URL)
+inputs = 'https://raw.githubusercontent.com/scikit-image/scikit-image/main/skimage/data/coins.png'
+
+# Set up client
+client = Client("ericup/celldetection")
+
+# Predict
+overlay_filename, img_filename, h5_filename, csv_filename = client.predict(
+    inputs,  # str: Local filepath or URL of your input image
+    
+    # Model name
+    'ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c',
+    
+    # Custom Score Threshold (numeric value between 0 and 1)
+    False, .9,  # bool: Whether to use custom setting; float: Custom setting
+    
+    # Custom NMS Threshold
+    False, .3142,  # bool: Whether to use custom setting; float: Custom setting
+    
+    # Custom Number of Sample Points
+    False, 128,  # bool: Whether to use custom setting; int: Custom setting
+    
+    # Overlapping objects
+    True,  # bool: Whether to allow overlapping objects
+    
+    # API name (keep as is)
+    api_name="/predict"
+)
 
-response = requests.post("https://ericup-celldetection.hf.space/run/predict", json={
-    "data": [
-        "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAACklEQVR4nGMAAQAABQABDQottAAAAABJRU5ErkJggg==",
-        "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
-    ]
-}).json()
 
-data = response["data"]
+# Example usage: Code below only shows how to use the results
+from matplotlib import pyplot as plt
+import celldetection as cd
+import pandas as pd
+
+# Read results from local temporary files
+img = imread(img_filename)
+overlay = imread(overlay_filename)  # random colors per instance; transparent overlap
+properties = pd.read_csv(csv_filename)
+contours, scores, label_image = cd.from_h5(h5_filename, 'contours', 'scores', 'labels')
+
+# Optionally display overlay
+cd.imshow_row(img, img, figsize=(16, 9))
+cd.imshow(overlay)
+plt.show()
+
+# Optionally display contours with text
+cd.imshow_row(img, img, figsize=(16, 9))
+cd.plot_contours(contours, texts=['score: %d%%\narea: %d' % s for s in zip((scores * 100).round(), properties.area)])
+plt.show()
 ```
 
 ### Javascript
 
 ```javascript
-const response = await fetch("https://ericup-celldetection.hf.space/run/predict", {
-    method: "POST",
-    headers: {"Content-Type": "application/json"},
-    body: JSON.stringify({
-        data: [
-            "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAACklEQVR4nGMAAQAABQABDQottAAAAABJRU5ErkJggg==",
-            "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
-        ]
-    })
-});
-
-const data = await response.json();
+import { client } from "@gradio/client";
 
+const response_0 = await fetch("https://raw.githubusercontent.com/scikit-image/scikit-image/main/skimage/data/coins.png");
+const exampleImage = await response_0.blob();
+						
+const app = await client("ericup/celldetection");
+const result = await app.predict("/predict", [
+    exampleImage,  // blob: Your input image
+    
+    // Model name (hosted model or URL)
+    "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
+    
+    // Custom Score Threshold (numeric value between 0 and 1)
+    false, .9,  // bool: Whether to use custom setting; float: Custom setting
+    
+    // Custom NMS Threshold
+    false, .3142,  // bool: Whether to use custom setting; float: Custom setting
+    
+    // Custom Number of Sample Points
+    false, 128,  // bool: Whether to use custom setting; int: Custom setting
+    
+    // Overlapping objects
+    true,  // bool: Whether to allow overlapping objects
+    
+    // API name (keep as is)
+    api_name="/predict"
+]);
 ```
 
 </details>
 
 ## 🧑‍💻 Napari Plugin
 
 Find our Napari Plugin here: https://github.com/FZJ-INM1-BDA/celldetection-napari </br>
@@ -443,9 +468,9 @@
 - [Article (sciencedirect)](https://www.sciencedirect.com/science/article/pii/S136184152200024X "Contour Proposal Networks for Biomedical Instance Segmentation")
 - [PDF (sciencedirect)](https://www.sciencedirect.com/sdfe/reader/pii/S136184152200024X/pdf "Contour Proposal Networks for Biomedical Instance Segmentation")
 - [PyPI](https://pypi.org/project/celldetection/ "CellDetection")
 - [Documentation](https://docs.celldetection.org "Documentation")
 
 ## 🧑‍🔬 Thanks!
 
-[![Stargazers repo roster for @FZJ-INM1-BDA/celldetection](https://reporoster.com/stars/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/stargazers)
-[![Forkers repo roster for @FZJ-INM1-BDA/celldetection](https://reporoster.com/forks/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/network/members)
+[![Stargazers repo roster for @FZJ-INM1-BDA/celldetection](http://reporoster.com/stars/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/stargazers)
+[![Forkers repo roster for @FZJ-INM1-BDA/celldetection](http://reporoster.com/forks/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/network/members)
```

### Comparing `CellDetection-0.4.5/CellDetection.egg-info/SOURCES.txt` & `celldetection-0.4.8/CellDetection.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,42 +2,49 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 CellDetection.egg-info/PKG-INFO
 CellDetection.egg-info/SOURCES.txt
 CellDetection.egg-info/dependency_links.txt
+CellDetection.egg-info/entry_points.txt
 CellDetection.egg-info/requires.txt
 CellDetection.egg-info/top_level.txt
 celldetection/__init__.py
 celldetection/__meta__.py
 celldetection/callbacks/__init__.py
 celldetection/callbacks/dropout.py
+celldetection/callbacks/keepalive.py
 celldetection/data/__init__.py
 celldetection/data/cpn.py
 celldetection/data/instance_eval.py
 celldetection/data/misc.py
 celldetection/data/segmentation.py
 celldetection/data/toydata.py
+celldetection/data/transforms.py
 celldetection/data/datasets/__init__.py
 celldetection/data/datasets/bbbc038.py
 celldetection/data/datasets/bbbc039.py
 celldetection/data/datasets/bbbc041.py
 celldetection/data/datasets/generic.py
 celldetection/data/datasets/synth.py
 celldetection/models/__init__.py
 celldetection/models/commons.py
 celldetection/models/convnext.py
+celldetection/models/convnextv2.py
 celldetection/models/cpn.py
+celldetection/models/densenet.py
 celldetection/models/features.py
 celldetection/models/filters.py
 celldetection/models/fpn.py
 celldetection/models/inference.py
-celldetection/models/lightning.py
+celldetection/models/lightning_base.py
+celldetection/models/lightning_cpn.py
 celldetection/models/loss.py
+celldetection/models/mamba.py
 celldetection/models/manet.py
 celldetection/models/mobilenetv3.py
 celldetection/models/normalization.py
 celldetection/models/ppm.py
 celldetection/models/resnet.py
 celldetection/models/smp.py
 celldetection/models/timmodels.py
@@ -51,13 +58,17 @@
 celldetection/ops/draw.py
 celldetection/ops/features.py
 celldetection/ops/loss.py
 celldetection/ops/normalization.py
 celldetection/optim/__init__.py
 celldetection/optim/lr_scheduler.py
 celldetection/util/__init__.py
+celldetection/util/logging.py
 celldetection/util/schedule.py
+celldetection/util/shm_cache.py
 celldetection/util/timer.py
 celldetection/util/util.py
 celldetection/visualization/__init__.py
 celldetection/visualization/cmaps.py
-celldetection/visualization/images.py
+celldetection/visualization/images.py
+celldetection_scripts/__init__.py
+celldetection_scripts/cpn_inference.py
```

### Comparing `CellDetection-0.4.5/LICENSE` & `celldetection-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/PKG-INFO` & `celldetection-0.4.8/CellDetection.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CellDetection
-Version: 0.4.5
+Version: 0.4.8
 Summary: Cell Detection with PyTorch.
 Home-page: https://celldetection.org
 Author: Eric Upschulte
 Author-email: e.upschulte@fz-juelich.de
 License: Apache License, Version 2.0
 Keywords: cell,detection,object,segmentation,pytorch,cpn,contour,proposal,network,deep,learning,unet,fzj,julich,juelich,ai
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -16,24 +16,26 @@
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: scikit-image
 Requires-Dist: opencv-python
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision
+Requires-Dist: tensorboard
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: h5py
 Requires-Dist: pillow
-Requires-Dist: pynvml>=11.0.0
+Requires-Dist: nvidia-ml-py
 Requires-Dist: albumentations>=1.3.0
 Requires-Dist: timm
 Requires-Dist: segmentation-models-pytorch
 Requires-Dist: pandas
 Requires-Dist: pytorch_lightning
+Requires-Dist: pyyaml
 
 # Cell Detection
 
 [![Downloads](https://static.pepy.tech/badge/celldetection?l)](https://pepy.tech/project/celldetection)
 [![Test](https://github.com/FZJ-INM1-BDA/celldetection/workflows/Test/badge.svg)](https://github.com/FZJ-INM1-BDA/celldetection/actions?query=workflow%3ATest)
 [![PyPI](https://img.shields.io/pypi/v/celldetection?l)](https://pypi.org/project/celldetection/)
 [![Documentation Status](https://readthedocs.org/projects/celldetection/badge/?version=latest)](https://celldetection.readthedocs.io/en/latest/?badge=latest)
@@ -363,48 +365,106 @@
 ```
 
 
 ## 🤗 Hugging Face Spaces
 
 Find us on Hugging Face and upload your own images for segmentation: https://huggingface.co/spaces/ericup/celldetection
 
+There's also an API (Python & JavaScript), allowing you to utilize community GPUs (currently Nvidia A100) remotely!
+
 <details>
     <summary style="font-weight: bold; color: #888888">Hugging Face API</summary>
 
 ### Python
 
 ```python
-import requests
+from gradio_client import Client
+
+# Define inputs (local filename or URL)
+inputs = 'https://raw.githubusercontent.com/scikit-image/scikit-image/main/skimage/data/coins.png'
+
+# Set up client
+client = Client("ericup/celldetection")
+
+# Predict
+overlay_filename, img_filename, h5_filename, csv_filename = client.predict(
+    inputs,  # str: Local filepath or URL of your input image
+    
+    # Model name
+    'ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c',
+    
+    # Custom Score Threshold (numeric value between 0 and 1)
+    False, .9,  # bool: Whether to use custom setting; float: Custom setting
+    
+    # Custom NMS Threshold
+    False, .3142,  # bool: Whether to use custom setting; float: Custom setting
+    
+    # Custom Number of Sample Points
+    False, 128,  # bool: Whether to use custom setting; int: Custom setting
+    
+    # Overlapping objects
+    True,  # bool: Whether to allow overlapping objects
+    
+    # API name (keep as is)
+    api_name="/predict"
+)
 
-response = requests.post("https://ericup-celldetection.hf.space/run/predict", json={
-    "data": [
-        "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAACklEQVR4nGMAAQAABQABDQottAAAAABJRU5ErkJggg==",
-        "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
-    ]
-}).json()
 
-data = response["data"]
+# Example usage: Code below only shows how to use the results
+from matplotlib import pyplot as plt
+import celldetection as cd
+import pandas as pd
+
+# Read results from local temporary files
+img = imread(img_filename)
+overlay = imread(overlay_filename)  # random colors per instance; transparent overlap
+properties = pd.read_csv(csv_filename)
+contours, scores, label_image = cd.from_h5(h5_filename, 'contours', 'scores', 'labels')
+
+# Optionally display overlay
+cd.imshow_row(img, img, figsize=(16, 9))
+cd.imshow(overlay)
+plt.show()
+
+# Optionally display contours with text
+cd.imshow_row(img, img, figsize=(16, 9))
+cd.plot_contours(contours, texts=['score: %d%%\narea: %d' % s for s in zip((scores * 100).round(), properties.area)])
+plt.show()
 ```
 
 ### Javascript
 
 ```javascript
-const response = await fetch("https://ericup-celldetection.hf.space/run/predict", {
-    method: "POST",
-    headers: {"Content-Type": "application/json"},
-    body: JSON.stringify({
-        data: [
-            "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAACklEQVR4nGMAAQAABQABDQottAAAAABJRU5ErkJggg==",
-            "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
-        ]
-    })
-});
-
-const data = await response.json();
+import { client } from "@gradio/client";
 
+const response_0 = await fetch("https://raw.githubusercontent.com/scikit-image/scikit-image/main/skimage/data/coins.png");
+const exampleImage = await response_0.blob();
+						
+const app = await client("ericup/celldetection");
+const result = await app.predict("/predict", [
+    exampleImage,  // blob: Your input image
+    
+    // Model name (hosted model or URL)
+    "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
+    
+    // Custom Score Threshold (numeric value between 0 and 1)
+    false, .9,  // bool: Whether to use custom setting; float: Custom setting
+    
+    // Custom NMS Threshold
+    false, .3142,  // bool: Whether to use custom setting; float: Custom setting
+    
+    // Custom Number of Sample Points
+    false, 128,  // bool: Whether to use custom setting; int: Custom setting
+    
+    // Overlapping objects
+    true,  // bool: Whether to allow overlapping objects
+    
+    // API name (keep as is)
+    api_name="/predict"
+]);
 ```
 
 </details>
 
 ## 🧑‍💻 Napari Plugin
 
 Find our Napari Plugin here: https://github.com/FZJ-INM1-BDA/celldetection-napari </br>
@@ -443,9 +503,9 @@
 - [Article (sciencedirect)](https://www.sciencedirect.com/science/article/pii/S136184152200024X "Contour Proposal Networks for Biomedical Instance Segmentation")
 - [PDF (sciencedirect)](https://www.sciencedirect.com/sdfe/reader/pii/S136184152200024X/pdf "Contour Proposal Networks for Biomedical Instance Segmentation")
 - [PyPI](https://pypi.org/project/celldetection/ "CellDetection")
 - [Documentation](https://docs.celldetection.org "Documentation")
 
 ## 🧑‍🔬 Thanks!
 
-[![Stargazers repo roster for @FZJ-INM1-BDA/celldetection](https://reporoster.com/stars/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/stargazers)
-[![Forkers repo roster for @FZJ-INM1-BDA/celldetection](https://reporoster.com/forks/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/network/members)
+[![Stargazers repo roster for @FZJ-INM1-BDA/celldetection](http://reporoster.com/stars/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/stargazers)
+[![Forkers repo roster for @FZJ-INM1-BDA/celldetection](http://reporoster.com/forks/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/network/members)
```

### Comparing `CellDetection-0.4.5/README.md` & `celldetection-0.4.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: CellDetection
+Version: 0.4.8
+Summary: Cell Detection with PyTorch.
+Home-page: https://celldetection.org
+Author: Eric Upschulte
+Author-email: e.upschulte@fz-juelich.de
+License: Apache License, Version 2.0
+Keywords: cell,detection,object,segmentation,pytorch,cpn,contour,proposal,network,deep,learning,unet,fzj,julich,juelich,ai
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+Requires-Dist: scikit-image
+Requires-Dist: opencv-python
+Requires-Dist: torch>=2.0.0
+Requires-Dist: torchvision
+Requires-Dist: tensorboard
+Requires-Dist: seaborn
+Requires-Dist: tqdm
+Requires-Dist: h5py
+Requires-Dist: pillow
+Requires-Dist: nvidia-ml-py
+Requires-Dist: albumentations>=1.3.0
+Requires-Dist: timm
+Requires-Dist: segmentation-models-pytorch
+Requires-Dist: pandas
+Requires-Dist: pytorch_lightning
+Requires-Dist: pyyaml
+
 # Cell Detection
 
 [![Downloads](https://static.pepy.tech/badge/celldetection?l)](https://pepy.tech/project/celldetection)
 [![Test](https://github.com/FZJ-INM1-BDA/celldetection/workflows/Test/badge.svg)](https://github.com/FZJ-INM1-BDA/celldetection/actions?query=workflow%3ATest)
 [![PyPI](https://img.shields.io/pypi/v/celldetection?l)](https://pypi.org/project/celldetection/)
 [![Documentation Status](https://readthedocs.org/projects/celldetection/badge/?version=latest)](https://celldetection.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/349111085.svg)](https://zenodo.org/badge/latestdoi/349111085)
@@ -330,48 +365,106 @@
 ```
 
 
 ## 🤗 Hugging Face Spaces
 
 Find us on Hugging Face and upload your own images for segmentation: https://huggingface.co/spaces/ericup/celldetection
 
+There's also an API (Python & JavaScript), allowing you to utilize community GPUs (currently Nvidia A100) remotely!
+
 <details>
     <summary style="font-weight: bold; color: #888888">Hugging Face API</summary>
 
 ### Python
 
 ```python
-import requests
+from gradio_client import Client
+
+# Define inputs (local filename or URL)
+inputs = 'https://raw.githubusercontent.com/scikit-image/scikit-image/main/skimage/data/coins.png'
+
+# Set up client
+client = Client("ericup/celldetection")
+
+# Predict
+overlay_filename, img_filename, h5_filename, csv_filename = client.predict(
+    inputs,  # str: Local filepath or URL of your input image
+    
+    # Model name
+    'ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c',
+    
+    # Custom Score Threshold (numeric value between 0 and 1)
+    False, .9,  # bool: Whether to use custom setting; float: Custom setting
+    
+    # Custom NMS Threshold
+    False, .3142,  # bool: Whether to use custom setting; float: Custom setting
+    
+    # Custom Number of Sample Points
+    False, 128,  # bool: Whether to use custom setting; int: Custom setting
+    
+    # Overlapping objects
+    True,  # bool: Whether to allow overlapping objects
+    
+    # API name (keep as is)
+    api_name="/predict"
+)
 
-response = requests.post("https://ericup-celldetection.hf.space/run/predict", json={
-    "data": [
-        "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAACklEQVR4nGMAAQAABQABDQottAAAAABJRU5ErkJggg==",
-        "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
-    ]
-}).json()
 
-data = response["data"]
+# Example usage: Code below only shows how to use the results
+from matplotlib import pyplot as plt
+import celldetection as cd
+import pandas as pd
+
+# Read results from local temporary files
+img = imread(img_filename)
+overlay = imread(overlay_filename)  # random colors per instance; transparent overlap
+properties = pd.read_csv(csv_filename)
+contours, scores, label_image = cd.from_h5(h5_filename, 'contours', 'scores', 'labels')
+
+# Optionally display overlay
+cd.imshow_row(img, img, figsize=(16, 9))
+cd.imshow(overlay)
+plt.show()
+
+# Optionally display contours with text
+cd.imshow_row(img, img, figsize=(16, 9))
+cd.plot_contours(contours, texts=['score: %d%%\narea: %d' % s for s in zip((scores * 100).round(), properties.area)])
+plt.show()
 ```
 
 ### Javascript
 
 ```javascript
-const response = await fetch("https://ericup-celldetection.hf.space/run/predict", {
-    method: "POST",
-    headers: {"Content-Type": "application/json"},
-    body: JSON.stringify({
-        data: [
-            "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAACklEQVR4nGMAAQAABQABDQottAAAAABJRU5ErkJggg==",
-            "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
-        ]
-    })
-});
-
-const data = await response.json();
+import { client } from "@gradio/client";
 
+const response_0 = await fetch("https://raw.githubusercontent.com/scikit-image/scikit-image/main/skimage/data/coins.png");
+const exampleImage = await response_0.blob();
+						
+const app = await client("ericup/celldetection");
+const result = await app.predict("/predict", [
+    exampleImage,  // blob: Your input image
+    
+    // Model name (hosted model or URL)
+    "ginoro_CpnResNeXt101UNet-fbe875f1a3e5ce2c",
+    
+    // Custom Score Threshold (numeric value between 0 and 1)
+    false, .9,  // bool: Whether to use custom setting; float: Custom setting
+    
+    // Custom NMS Threshold
+    false, .3142,  // bool: Whether to use custom setting; float: Custom setting
+    
+    // Custom Number of Sample Points
+    false, 128,  // bool: Whether to use custom setting; int: Custom setting
+    
+    // Overlapping objects
+    true,  // bool: Whether to allow overlapping objects
+    
+    // API name (keep as is)
+    api_name="/predict"
+]);
 ```
 
 </details>
 
 ## 🧑‍💻 Napari Plugin
 
 Find our Napari Plugin here: https://github.com/FZJ-INM1-BDA/celldetection-napari </br>
@@ -410,9 +503,9 @@
 - [Article (sciencedirect)](https://www.sciencedirect.com/science/article/pii/S136184152200024X "Contour Proposal Networks for Biomedical Instance Segmentation")
 - [PDF (sciencedirect)](https://www.sciencedirect.com/sdfe/reader/pii/S136184152200024X/pdf "Contour Proposal Networks for Biomedical Instance Segmentation")
 - [PyPI](https://pypi.org/project/celldetection/ "CellDetection")
 - [Documentation](https://docs.celldetection.org "Documentation")
 
 ## 🧑‍🔬 Thanks!
 
-[![Stargazers repo roster for @FZJ-INM1-BDA/celldetection](https://reporoster.com/stars/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/stargazers)
-[![Forkers repo roster for @FZJ-INM1-BDA/celldetection](https://reporoster.com/forks/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/network/members)
+[![Stargazers repo roster for @FZJ-INM1-BDA/celldetection](http://reporoster.com/stars/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/stargazers)
+[![Forkers repo roster for @FZJ-INM1-BDA/celldetection](http://reporoster.com/forks/FZJ-INM1-BDA/celldetection)](https://github.com/FZJ-INM1-BDA/celldetection/network/members)
```

### Comparing `CellDetection-0.4.5/celldetection/callbacks/dropout.py` & `celldetection-0.4.8/celldetection/callbacks/dropout.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/data/cpn.py` & `celldetection-0.4.8/celldetection/data/cpn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import numpy as np
 import cv2
+import torch
 from skimage.measure import regionprops
+from skimage import img_as_ubyte
 from collections import OrderedDict
 from .segmentation import filter_instances_
-from .misc import labels2properties
-
+from .misc import labels2properties, resample_contours
+from ..util.util import asnumpy
 
 __all__ = [
     'CPNTargetGenerator', 'contours2labels', 'render_contour', 'clip_contour_', 'masks2labels',
     'contours2boxes', 'contours2properties', 'resolve_label_channels',
-    'filter_contours_by_intensity'
+    'filter_contours_by_intensity', 'draw_contours', 'contours2overlay'
 ]
 
 
 def efd(contour, order=10, epsilon=1e-6):
     """Elliptic fourier descriptor.
 
     Computes elliptic fourier descriptors from contour data.
@@ -236,14 +238,26 @@
     if round:
         contour = contour.round()
     a = cv2.drawContours(a, [np.array(contour, dtype=np.int32).reshape((-1, 1, 2))], 0, val, -1,
                          offset=(-xmin, -ymin))
     return a, (xmin, xmax), (ymin, ymax)
 
 
+def draw_contours(canvas, contours, val=(51, 255, 51), round=True, contour_idx=-1, thickness=2, **kwargs):
+    if isinstance(contours, torch.Tensor):
+        contours = asnumpy(contours)
+    if canvas.ndim == 2 and isinstance(val, (list, tuple, np.ndarray)) and len(val) == 3:
+        canvas = cv2.cvtColor(canvas, cv2.COLOR_GRAY2RGB)
+    if contours.dtype.kind == 'f':
+        if round:
+            contours = contours.round()
+        contours = contours.astype(int)
+    return cv2.drawContours(canvas, contours, contour_idx, val, thickness, **kwargs)
+
+
 def filter_contours_by_intensity(img, contours, min_intensity=None, max_intensity=200, aggregate='mean'):
     keep = np.ones(len(contours), dtype=bool)
     for idx, con in enumerate(contours):
         m, (xmin, xmax), (ymin, ymax) = render_contour(con, dtype='uint8')
         img_crop = img[ymin:ymin + m.shape[0], xmin:xmin + m.shape[1]]
         m = m[:img_crop.shape[0], :img_crop.shape[1]]
         assert m.dtype == np.uint8
@@ -257,15 +271,16 @@
 
 
 def clip_contour_(contour, size):
     np.clip(contour[..., 0], 0, size[1], out=contour[..., 0])
     np.clip(contour[..., 1], 0, size[0], out=contour[..., 1])
 
 
-def contours2labels(contours, size, rounded=True, clip=True, initial_depth=1, gap=3, dtype='int32'):
+def contours2labels(contours, size, rounded=True, clip=True, initial_depth=1, gap=3, dtype='int32', ioa_thresh=None,
+                    sort_by=None, sort_descending=True, return_indices=False):
     """Contours to labels.
 
     Convert contours to label image.
 
     Notes:
         - ~137 ms for contours.shape=(1284, 128, 2), size=(1000, 1000).
         - Label images come with channels, as contours may assign pixels to multiple objects.
@@ -276,34 +291,60 @@
         contours: Contours of a single image. Array[num_contours, num_points, 2] or List[Array[num_points, 2]].
         size: Label image size. (height, width).
         rounded: Whether to round contour coordinates.
         clip: Whether to clip contour coordinates to given `size`.
         initial_depth: Initial number of channels. More channels are used if necessary.
         gap: Gap between instances.
         dtype: Data type of label image.
+        ioa_thresh: Intersection over area threshold. Skip contours that have an intersection over own area
+            (i.e. area of contour that already contains a label vs. area of contour) greater `ioa_thresh`,
+            compared to the union of all contours painted before. Note that the order of `contours` is
+            relevant, as contours are processed iteratively. IoA of 0 means no labels present so far, IoA of 1. means
+            the entire contour area is already covered by other contours.
+        sort_by: Optional Array used to sort contours. Note, that if this option is used, labels and contour indices no
+            longer correspond.
+        sort_descending: Whether to sort by descending.
+        return_indices: Whether to return indices.
 
     Returns:
         Array[height, width, channels]. Since contours may assign pixels to multiple objects, the label image comes
         with channels. To remove channels refer to `resolve_label_channels`.
     """
+    contours_ = contours
+    if sort_by is not None:
+        indices = np.argsort(sort_by)
+        if sort_descending:
+            indices = reversed(indices)
+        contours_ = (contours[i] for i in indices)
     labels = np.zeros(tuple(size) + (initial_depth,), dtype=dtype)
     lbl = 1
-    for contour in contours:
+    keep = []
+    for idx, contour in enumerate(contours_):
         if rounded:
             contour = np.round(contour)
         if clip:
             clip_contour_(contour, np.array(size) - 1)
         a, (xmin, xmax), (ymin, ymax) = render_contour(contour, val=lbl, dtype=dtype)
+        if ioa_thresh is not None:
+            m = a > 0
+            crp = (labels[ymin:ymin + a.shape[0], xmin:xmin + a.shape[1]] > 0).any(-1)
+            ioa = crp[m].sum() / m.sum()
+            if ioa > ioa_thresh:
+                continue
+            else:
+                keep.append(idx)
         lbl += 1
         s = (labels[np.maximum(0, ymin - gap): gap + ymin + a.shape[0],
              np.maximum(0, xmin - gap): gap + xmin + a.shape[1]] > 0).sum((0, 1))
         i = next(i for i in range(labels.shape[2] + 1) if ~ (i < labels.shape[2] and np.any(s[i])))
         if i >= labels.shape[2]:
             labels = np.concatenate((labels, np.zeros(size, dtype=dtype)[..., None]), axis=-1)
         labels[ymin:ymin + a.shape[0], xmin:xmin + a.shape[1], i] += a
+    if return_indices:
+        return labels, keep
     return labels
 
 
 def resolve_label_channels(labels, method='dilation', max_iter=999, kernel=(3, 3)):
     """Resolve label channels.
 
     Remove channels from a label image.
@@ -382,28 +423,32 @@
         for p in regionprops(labels):
             c = p.coords
             indices = (c[:, 0], c[:, 1])
             dist[indices] /= np.maximum(dist[indices].max(), .000001)
     return dist
 
 
-def _labels2distances_instance(labels, fg_mask_wo_overlap, distance_type):
+def _labels2distances_instance(labels, fg_mask_wo_overlap, distance_type, protected_size=6 * 6):
     dist = np.zeros_like(fg_mask_wo_overlap, dtype='float32')
     if labels.size > 0:
         for p in regionprops(labels):
             y0, x0, _, y1, x1, _ = p.bbox
             box_slices = (slice(y0, y1), slice(x0, x1))
             mask = np.any(p.image, 2) & fg_mask_wo_overlap[box_slices]
             d_ = cv2.distanceTransform(np.pad(mask.astype('uint8'), 1), distance_type, 3)[1:-1, 1:-1]
-            d_ /= np.maximum(d_.max(), .000001)
+            if mask.sum() > protected_size:
+                d_max = d_.max()
+                if d_max > 0:
+                    d_ /= d_max
+            d_ = d_.clip(0., 1.)
             dist[box_slices][mask] = d_[mask]
     return dist
 
 
-def labels2distances(labels, distance_type=cv2.DIST_L2, overlap_zero=True, per_instance=True):
+def labels2distances(labels, distance_type=cv2.DIST_L2, overlap_zero=True, per_instance=True, **kwargs):
     """Label stacks to distances.
 
     Measures distances from pixel to closest border, relative to largest distance.
     Values as percentage. Overlap is zero.
 
     Notes:
         54.9 ms ± 3.41 ms (shape (576, 576, 3); 762 instances in three channels)
@@ -427,17 +472,17 @@
         labels[overlap_mask] = -1
         fg_mask_wo_overlap = np.sum(mask, 2) == 1
     else:
         fg_mask_wo_overlap = np.any(mask, 2)
 
     # Fg mask
     if per_instance:
-        dist = _labels2distances_instance(labels, fg_mask_wo_overlap, distance_type)
+        dist = _labels2distances_instance(labels, fg_mask_wo_overlap, distance_type, **kwargs)
     else:
-        dist = _labels2distances_fg(labels, fg_mask_wo_overlap, distance_type)
+        dist = _labels2distances_fg(labels, fg_mask_wo_overlap, distance_type, **kwargs)
 
     return dist.clip(0., 1.), labels  # 332 µs ± 24.5 µs for (576, 576)
 
 
 class CPNTargetGenerator:
     def __init__(self, samples, order, random_sampling=True, remove_partials=False, min_fg_dist=.75, max_bg_dist=.5,
                  flag_fragmented=True, flag_fragmented_constant=-1):
@@ -447,59 +492,61 @@
         self.remove_partials = remove_partials
         self.min_fg_dist = min_fg_dist
         self.max_bg_dist = max_bg_dist
         self.flag_fragmented = flag_fragmented
         self.flag_fragmented_constant = flag_fragmented_constant
 
         self.labels = None
+        self.labels_red = None
         self.distances = None
         self.partials_mask = None
         self._sampling = self._contours = self._fourier = self._locations = self._sampled_contours = None
         self._sampled_sizes = None
+        self._resampled_contours = None
         self._reset()
 
     def _reset(self):
         self._sampling = None
         self._contours = None
         self._fourier = None
         self._locations = None
         self._sampled_contours = None
         self._sampled_sizes = None
+        self._resampled_contours = None
 
-    def feed(self, labels, border=1, min_area=1, max_area=None):
+    def feed(self, labels, border=1, min_area=1, max_area=None, **kwargs):
         """
 
         Notes:
             - May apply inplace changes to ``labels``.
 
         Args:
             labels: Single label image. E.g. of shape (height, width, channels).
             border:
             min_area:
             max_area:
         """
+        self._reset()
         if labels.ndim == 2:
             labels = labels[..., None]
 
         filter_instances_(labels, partials=self.remove_partials, partials_border=border,
                           min_area=min_area, max_area=max_area, constant=-1, continuous=True)
 
         self.labels = labels
         _ = self.contours  # compute contours
 
-        self.distances, labels = labels2distances(labels)
-        mask_labels_by_distance_(labels, self.distances, self.max_bg_dist, self.min_fg_dist)
-
-        self._reset()
+        self.distances, self.labels_red = labels2distances(labels, **kwargs)
+        mask_labels_by_distance_(self.labels_red, self.distances, self.max_bg_dist, self.min_fg_dist)
 
     @property
     def reduced_labels(self):
         if self.flag_fragmented:
             _ = self.contours  # Since labels2contours may filter instances, it has to be done before returning labels
-        return self.labels.max(2)
+        return self.labels_red.max(2)
 
     @property
     def sampling(self):
         if self._sampling is None:
             if self.random_sampling:
                 self._sampling = np.random.uniform(0., 1., self.samples)
 
@@ -535,19 +582,69 @@
         """
         if self._sampled_contours is None:
             self._sampled_contours = fourier2contour(self.fourier, self.locations, samples=self.samples,
                                                      sampling=self.sampling)
         return self._sampled_contours
 
     @property
+    def resampled_contours(self):
+        """
+        Returns:
+            Tensor[num_contours, num_points, 2]
+        """
+        if self._resampled_contours is None:
+            contours: dict = self.contours
+
+            if len(contours) > 0:
+                max_label = np.max(list(contours.keys()))
+            else:
+                max_label = 0
+
+            resampled = np.zeros((max_label, self.samples, 2))
+            for key, contour in contours.items():
+                if contour.ndim == 3:
+                    contour = contour.squeeze(1)
+
+                # Resample contour (would be done sequentially anyway because of different shapes)
+                resampled[key - 1] = resample_contours(contour, self.samples)
+
+            self._resampled_contours = resampled
+
+            assert (self._resampled_contours.shape == self._sampled_contours.shape), (
+                f'Shape mismatch: {self._resampled_contours.shape, self._sampled_contours.shape}')
+
+            # self._resampled_contours = OrderedDict({k: v for k, v in zip(keys, _resampled_contours)})
+        return self._resampled_contours
+
+    @property
     def sampled_sizes(self):
         """
         Notes:
             The quality of `sizes` depends on how accurate `sampled_contours` represents the actual contours.
 
         Returns:
             Tensor[num_contours, 2]. Contains height and width for each contour.
         """
         if self._sampled_sizes is None:
             c = self.sampled_contours
             self._sampled_sizes = c.max(1) - c.min(1)
         return self._sampled_sizes
+
+
+def contours2overlay(contours, size, hue_range=(0, 180), saturation_range=(60, 133), value_range=(180, 256),
+                     rounded=True, clip=True, intermediate_dtype='float16'):
+    from ..visualization.cmaps import random_colors_hsv
+    overlay = np.zeros(tuple(size) + (4,), dtype=intermediate_dtype)
+    counter = np.zeros(tuple(size), dtype=intermediate_dtype)
+    for idx, contour in enumerate(contours):
+        if rounded:
+            contour = np.round(contour)
+        if clip:
+            clip_contour_(contour, np.array(size) - 1)
+        a, (xmin, xmax), (ymin, ymax) = render_contour(contour, val=1, dtype='uint8')
+        c = random_colors_hsv(1, hue_range=hue_range, saturation_range=saturation_range, value_range=value_range)
+        counter[ymin:ymin + a.shape[0], xmin:xmin + a.shape[1]] += a
+        overlay[ymin:ymin + a.shape[0], xmin:xmin + a.shape[1]] += (list(c[0]) + [1.]) * a[..., None]
+    m = counter > 1
+    overlay[m] /= counter[m][..., None]
+    overlay = img_as_ubyte(overlay)
+    return overlay
```

### Comparing `CellDetection-0.4.5/celldetection/data/datasets/bbbc038.py` & `celldetection-0.4.8/celldetection/data/datasets/bbbc038.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/data/datasets/bbbc039.py` & `celldetection-0.4.8/celldetection/data/datasets/bbbc039.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/data/datasets/bbbc041.py` & `celldetection-0.4.8/celldetection/data/datasets/bbbc041.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/data/datasets/generic.py` & `celldetection-0.4.8/celldetection/data/datasets/generic.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/data/datasets/synth.py` & `celldetection-0.4.8/celldetection/data/datasets/synth.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/data/misc.py` & `celldetection-0.4.8/celldetection/data/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import torch
 from collections import OrderedDict
 from skimage import img_as_ubyte
 from ..util.util import get_device
 import cv2
 from skimage import measure
 import pandas as pd
+import traceback
 
 __all__ = ['to_tensor', 'transpose_spatial', 'universal_dict_collate_fn', 'normalize_percentile', 'random_crop',
            'channels_last2channels_first', 'channels_first2channels_last', 'ensure_tensor', 'rgb_to_scalar',
            'padding_stack', 'labels2crops', 'labels2properties', 'rle2mask', 'resample_contours',
-           'labels2property_table', 'pad_to_size', 'pad_to_div']
+           'labels2property_table', 'pad_to_size', 'pad_to_div', 'regionprops2d', 'split']
 
 
 def transpose_spatial(inputs: np.ndarray, inputs_channels_last=True, spatial_dims=2, has_batch=False):
     if spatial_dims == 0:
         return inputs
     has_batch = bool(has_batch)
     a = ([0] * has_batch)
@@ -118,14 +119,16 @@
     Args:
         *images: Images.
         axis: Axis used for stacking.
 
     Returns:
         Array
     """
+    if len(images) == 1 and isinstance(images[0], (list, tuple)):
+        images, = images
     shapes = np.array([i.shape for i in images])
     pad = np.any([np.unique(shapes[:, col].size > 1 for col in range(shapes.shape[1]))])
     if pad:
         target_shape = np.max(shapes, 0)
         images = [np.pad(i, [(0, ts - s) for s, ts in zip(i.shape, target_shape)]) for i in images]
     return np.stack(images, axis=axis)
 
@@ -154,15 +157,15 @@
     if not isinstance(percentile, (list, tuple)):
         percentile = (100 - percentile, percentile)
     low, high = np.percentile(image, percentile)
     img = (np.clip(image, low, high) - low) / (high - low)
     return img_as_ubyte(img) if to_uint8 else img
 
 
-def random_crop(*arrays, height, width=None):
+def _legacy_random_crop(*arrays, height, width=None):
     """Random crop.
 
     Args:
         *arrays: Input arrays that are to be cropped. None values accepted.
             The shape of the first element is used as reference.
         height: Output height.
         width: Output width. Default is same as height.
@@ -183,14 +186,38 @@
     )
     results = [(None if v is None else v[slices]) for v in arrays]
     if len(results) == 1:
         results, = results
     return results
 
 
+def random_crop(inputs, size=None, *args, return_coords=False, return_slices=False, **kwargs):
+    if 'height' in kwargs or 'width' in kwargs:
+        if size is None:
+            return _legacy_random_crop(inputs, *args, **kwargs)
+        else:
+            return _legacy_random_crop(inputs, size, *args, **kwargs)
+    assert size is not None, 'Specify a targeted size for cropping.'
+    reference_size = (inputs[0] if isinstance(inputs, (tuple, list)) else inputs).shape[:len(size)]
+    size = [(np.random.randint(*i) if isinstance(i, tuple) else i) for i in size]
+    diffs = [a - b for a, b in zip(reference_size, size)]
+    coords = [(np.random.randint(0, d) if d > 0 else 0) for d in diffs]
+    slices = tuple(slice(a, a + s) for a, s in zip(coords, size))
+
+    if isinstance(inputs, (list, tuple)):
+        res = tuple((None if i is None else i[slices]) for i in inputs)
+    else:
+        res = inputs[slices]
+
+    meta = tuple(i for i, c in ((coords, return_coords), (slices, return_slices)) if c)
+    if len(meta):
+        return res, meta
+    return res
+
+
 def random_pad(*arrays, size, mode='constant', **kwargs):
     if len(arrays) <= 0:
         return None
     reference = arrays[0].shape[:len(size)]
     padding = [max(size[i] - reference[i], 0) for i in range(len(size))]
     start = [int(np.random.uniform() * p) for p in padding]
     end = [p - s for p, s in zip(padding, start)]
@@ -415,7 +442,100 @@
     Returns:
         Padded Array.
     """
     if not isinstance(div, (tuple, list)):
         div = (div,) * nd
     size = [(i // d + bool(i % d)) * d for i, d in zip(v.shape, div)]
     return pad_to_size(v, size, **kwargs)
+
+
+def regionprops2d(
+        label_image,
+        intensity_image=None,
+        cache=True,
+        *,
+        extra_properties=None,
+        spacing=None,
+        offset=None,
+):
+    """Regionprops 2d.
+
+    Helper function that allows to use `skimage.measure.regionprops` with label images that have channels.
+
+    Note:
+        Labels may not yield in order!
+
+    Args:
+        label_image: Array[h, w] or Array[h, w, c].
+        intensity_image:
+        cache:
+        extra_properties:
+        spacing:
+        offset:
+
+    Returns:
+
+    """
+    assert label_image.ndim in (2, 3)
+    if label_image.ndim == 2:
+        label_image = label_image[..., None]
+    for z in range(label_image.shape[2]):
+        label_image_ = label_image[..., z]
+        for p in measure.regionprops(label_image_, intensity_image=intensity_image, cache=cache,
+                                     extra_properties=extra_properties,
+                                     spacing=spacing, offset=offset):
+            yield p
+
+
+def split(n: int, *splits, shuffle=True, seed=None):
+    """Split.
+
+    Splits a range of indices into multiple sets based on the given fractions.
+
+    Args:
+        n: The total number of indices.
+        *splits: Variable length list of floats representing the fraction of the dataset for each split.
+        shuffle: Whether to shuffle the indices before splitting.
+        seed: Seed for the random number generator.
+
+    Returns:
+        Split indices.
+    """
+    if sum(splits) != 1:
+        raise ValueError("The sum of splits must be equal to 1.")
+
+    indices = np.arange(n)
+
+    if shuffle:
+        if seed is not None:
+            np.random.seed(seed)
+        np.random.shuffle(indices)
+
+    split_indices = []
+    start = 0
+    for i, sp in enumerate(splits):
+        end = n if (i == len(splits) - 1) else start + int(round(n * sp))
+        split_indices.append(indices[start:end])
+        start = end
+
+    assert sum([len(i) for i in split_indices]) == n
+    assert np.unique(np.concatenate(split_indices)).size == n
+
+    return split_indices
+
+
+def pad_arrays(arrays):
+    if not arrays:
+        return []
+
+    # Finding the maximum shape
+    max_shape = np.max([np.array(a.shape) for a in arrays], axis=0)
+
+    # Padding each array
+    padded_arrays = []
+    for a in arrays:
+        # Calculate the padding needed for each dimension
+        padding = [(0, max_s - s) for s, max_s in zip(a.shape, max_shape)]
+        padded_a = np.pad(a, padding, mode='constant')
+        padded_arrays.append(padded_a)
+
+    return padded_arrays
```

### Comparing `CellDetection-0.4.5/celldetection/data/segmentation.py` & `celldetection-0.4.8/celldetection/data/segmentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,24 +36,30 @@
     uniques = list(set(uni) - set(uni[uni <= 0]))  # ignore zeros and negative values
     uniques.sort()
     gaps = list(set(range(1, len(uniques) + 1)) - set(uniques))
     while len(gaps) > 0:
         labels[labels == uniques.pop()] = gaps.pop()
 
 
-def fill_padding_(inputs, padding: int, constant=-1):
+def fill_padding_(inputs, padding: int, constant=-1, preserve_existing=True, axes=(0, 1)):
     if padding <= 0:
         return None
     if isinstance(inputs, (list, tuple)):
         [fill_padding_(i, padding, constant) for i in inputs]
         return
-    inputs[:padding] = constant
-    inputs[-padding:] = constant
-    inputs[:, :padding] = constant
-    inputs[:, -padding:] = constant
+    for ax in axes:
+        if ax < 0:
+            ax = ax + inputs.ndim
+        for sl in (slice(0, padding), slice(-padding, None)):  # , (slice(None), slice(0, padding)), (slice(None), slice(-padding, None))
+            sl = (slice(None),) * ax + (sl,)
+            if preserve_existing:
+                mask = ~inputs[sl].any(-1)
+            else:
+                mask = slice(None)
+            inputs[sl][mask] = constant
 
 
 def remove_padding(inputs, padding: int):
     if isinstance(inputs, (list, tuple)):
         return [remove_padding(i, padding) for i in inputs]
     return inputs[padding:-padding, padding:-padding]
```

### Comparing `CellDetection-0.4.5/celldetection/data/toydata.py` & `celldetection-0.4.8/celldetection/data/toydata.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/commons.py` & `celldetection-0.4.8/celldetection/models/commons.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor, tanh, sigmoid
 from torchvision import transforms as trans
+from torch.nn.common_types import _size_2_t
 from ..util.util import lookup_nn, tensor_to, ensure_num_tuple, get_nd_conv
 from ..ops.commons import split_spatially, minibatch_std_layer
-from typing import Type
+from typing import Type, Union
 from functools import partial
 
 __all__ = []
 
 
 def register(obj):
     __all__.append(obj.__name__)
@@ -426,37 +427,49 @@
             activation='relu',
             norm='batchnorm2d',
             final_activation=None,
             dropout=0.1,
             channels_mid=None,
             stride=1,
             nd=2,
+            attention=None,
     ):
         super().__init__()
         Conv = get_nd_conv(nd)
         Norm = lookup_nn(norm, nd=nd, call=False)
         Dropout = lookup_nn(nn.Dropout2d, nd=nd, call=False)
         self.channels_out = channels_out
         if channels_mid is None:
             channels_mid = channels_in
 
+        self.attention = None
+        if attention is not None:
+            if isinstance(attention, dict):
+                attention_kwargs, = list(attention.values())
+                attention, = list(attention.keys())
+            else:
+                attention_kwargs = {}
+            self.attention = lookup_nn(attention, nd=nd, call=False)(channels_in, **attention_kwargs)
+
         self.block = nn.Sequential(
             Conv(channels_in, channels_mid, kernel_size, padding=padding, stride=stride),
             Norm(channels_mid),
             lookup_nn(activation),
             Dropout(p=dropout) if dropout else nn.Identity(),
             Conv(channels_mid, channels_out, 1),
         )
 
         if final_activation is ...:
             self.activation = lookup_nn(activation)
         else:
             self.activation = lookup_nn(final_activation)
 
     def forward(self, x):
+        if self.attention is not None:
+            x = self.attention(x)
         out = self.block(x)
         return self.activation(out)
 
 
 @register
 class SpatialSplit(nn.Module):
     def __init__(self, height, width=None):
@@ -541,22 +554,22 @@
         if getattr(self, 'constant', False):
             s += ', constant=True'
         return s
 
 
 @register
 class AdditiveNoise2d(_AdditiveNoise):
-    def __init__(self, in_channels, noise_channels=1, weighted=True):
-        super().__init__(in_channels=in_channels, noise_channels=noise_channels, weighted=weighted, nd=2)
+    def __init__(self, in_channels, noise_channels=1, weighted=True, **kwargs):
+        super().__init__(in_channels=in_channels, noise_channels=noise_channels, weighted=weighted, nd=2, **kwargs)
 
 
 @register
 class AdditiveNoise3d(_AdditiveNoise):
-    def __init__(self, in_channels, noise_channels=1, weighted=True):
-        super().__init__(in_channels=in_channels, noise_channels=noise_channels, weighted=weighted, nd=3)
+    def __init__(self, in_channels, noise_channels=1, weighted=True, **kwargs):
+        super().__init__(in_channels=in_channels, noise_channels=noise_channels, weighted=weighted, nd=3, **kwargs)
 
 
 class _Stride(nn.Module):
     def __init__(self, stride, start=0, nd=2):
         super().__init__()
         self.stride = ensure_num_tuple(stride, nd)
         self.start = start
@@ -674,14 +687,58 @@
         scale = super().forward(inputs)
         scaled = inputs * scale
         if self.residual:
             return inputs + scaled
         return scaled
 
 
+@register
+class SelfAttention(nn.Module):
+    def __init__(self, in_channels, out_channels=None, mid_channels=None, kernel_size=1, padding=0, beta=True, nd=2):
+        """Self-Attention.
+
+        References:
+            - https://arxiv.org/pdf/1805.08318.pdf
+
+        Args:
+            in_channels:
+            out_channels: Equal to `in_channels` by default.
+            mid_channels: Set to `in_channels // 8` by default.
+            kernel_size:
+            padding:
+            beta:
+            nd:
+        """
+        super().__init__()
+        if mid_channels is None:
+            mid_channels = in_channels // 8
+        if out_channels is None:
+            out_channels = in_channels
+        Conv = lookup_nn('Conv2d', nd=nd, call=False)
+        self.beta = nn.Parameter(torch.zeros(1)) if beta else 1.
+        if in_channels != out_channels:
+            self.in_conv = Conv(in_channels, out_channels, kernel_size=3, padding=1)
+        else:
+            self.in_conv = None
+        self.proj_b, self.proj_a = [Conv(out_channels, mid_channels, kernel_size=1) for _ in range(2)]
+        self.proj = Conv(out_channels, out_channels, kernel_size=kernel_size, padding=padding)
+        self.out_conv = Conv(out_channels, out_channels, kernel_size=kernel_size, padding=padding)
+
+    def forward(self, inputs):
+        x = inputs if self.in_conv is None else self.in_conv(inputs)
+        a = self.proj_a(x).flatten(2)
+        b = self.proj_b(x).flatten(2)  # Tensor[n, c', hw]
+        p = torch.matmul(a.permute(0, 2, 1), b)  # Tensor[n, hw, hw]
+        p = F.softmax(p, dim=1)  # Tensor[n, hw, hw]
+        c = self.proj(x).flatten(2)  # Tensor[n, c, hw]
+        out = torch.matmul(p, c.permute(0, 2, 1)).view(*c.shape[:2], *inputs.shape[2:])  # T[n, c, hw] -> T[n, c, h, w]
+        out = self.out_conv(self.beta * out + x)
+        return out
+
+
 def channels_last_permute(nd):
     return (0,) + tuple(range(2, nd + 2)) + (1,)
 
 
 def channels_first_permute(nd):
     return (0, nd + 1,) + tuple(range(1, nd + 1))
```

### Comparing `CellDetection-0.4.5/celldetection/models/convnext.py` & `celldetection-0.4.8/celldetection/models/convnext.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 from typing import List, Optional, Callable, Sequence
 import torch
 from torch import Tensor, nn
 import torch.nn.functional as F
 from functools import partial
 from torchvision.ops import misc, Permute
 from torchvision.ops.stochastic_depth import StochasticDepth
-from ..util.util import lookup_nn
+from ..util.util import lookup_nn, get_nn
+from .ppm import append_pyramid_pooling_
 from .commons import LayerNorm1d, LayerNorm2d, LayerNorm3d, channels_last_permute, channels_first_permute
 from torch.hub import load_state_dict_from_url
+from pytorch_lightning.core.mixins import HyperparametersMixin
 
-__all__ = ['ConvNeXtBase', 'ConvNeXtTiny', 'ConvNeXtSmall', 'ConvNeXtLarge', 'ConvNeXt']
+
+__all__ = ['ConvNeXtBase', 'ConvNeXtTiny', 'ConvNeXtSmall', 'ConvNeXtLarge', 'ConvNeXt', 'CNBlock']
 
 default_model_urls = dict(
     ConvNeXtLarge=cnx.ConvNeXt_Large_Weights.IMAGENET1K_V1.url,
     ConvNeXtBase=cnx.ConvNeXt_Base_Weights.IMAGENET1K_V1.url,
     ConvNeXtSmall=cnx.ConvNeXt_Small_Weights.IMAGENET1K_V1.url,
     ConvNeXtTiny=cnx.ConvNeXt_Tiny_Weights.IMAGENET1K_V1.url,
 )
@@ -93,46 +96,56 @@
             Permute(list(channels_last_permute(nd))),
             norm_layer(out_channels),
             nn.Linear(in_features=out_channels, out_features=4 * out_channels, bias=True),
             lookup_nn(activation),
             nn.Linear(in_features=4 * out_channels, out_features=out_channels, bias=True),
             Permute(list(channels_first_permute(nd))),
         )
-        self.layer_scale = nn.Parameter(torch.ones(out_channels, *(1,) * nd) * layer_scale)
+        if layer_scale is None:
+            self.layer_scale = 1
+        else:
+            self.layer_scale = nn.Parameter(torch.ones(out_channels, *(1,) * nd) * layer_scale)
         self.stochastic_depth = StochasticDepth(stochastic_depth_prob, "row")
 
     def forward(self, inputs: Tensor) -> Tensor:
         identity = inputs if self.identity is None else self.identity(inputs)
         result = self.layer_scale * self.block(inputs)
         result = self.stochastic_depth(result)
         result += identity
         return result
 
 
-class ConvNeXt(nn.Sequential):
+class ConvNeXt(nn.Sequential, HyperparametersMixin):
     def __init__(
             self,
             in_channels: int,
             out_channels: int,
             block_setting: List[CNBlockConfig],
             stochastic_depth_prob: float = 0.0,
             layer_scale: float = 1e-6,
             block: Optional[Callable[..., nn.Module]] = None,
             block_kwargs: dict = None,
             norm_layer: Optional[Callable[..., nn.Module]] = None,
             pretrained=False,
             fused_initial=True,
             final_layer=None,
+            pyramid_pooling=False,
+            pyramid_pooling_channels=64,
+            pyramid_pooling_kwargs=None,
+            secondary_block=None,
             nd=2,
     ):
         if not block_setting:
             raise ValueError("The block_setting should not be empty")
         elif not (isinstance(block_setting, Sequence) and all([isinstance(s, CNBlockConfig) for s in block_setting])):
             raise TypeError("The block_setting should be List[CNBlockConfig]")
 
+        if secondary_block is not None:
+            secondary_block = get_nn(secondary_block, nd=nd)
+
         block_kwargs = {} if block_kwargs is None else block_kwargs
         if block is None:
             block = partial(CNBlock, nd=nd)
 
         if norm_layer is None:
             norm_layer = partial([LayerNorm1d, LayerNorm2d, LayerNorm3d][nd - 1], eps=1e-6)
 
@@ -172,14 +185,16 @@
             if down is not None:
                 stage += [down]  # downsampling is part of the stage
             for _ in range(cnf.num_layers):
                 sd_prob = stochastic_depth_prob * stage_block_id / (total_stage_blocks - 1.0)
                 stage.append(block(cnf.input_channels, layer_scale=layer_scale, stochastic_depth_prob=sd_prob,
                                    **block_kwargs))
                 stage_block_id += 1
+            if secondary_block is not None:
+                stage.append(secondary_block(cnf.input_channels, nd=nd))
             layers.append(nn.Sequential(*stage))
             if cnf.out_channels is not None:
                 # Downsampling
                 down = nn.Sequential(
                     norm_layer(cnf.input_channels),
                     Conv(cnf.input_channels, cnf.out_channels, kernel_size=2, stride=2),
                 )
@@ -203,14 +218,17 @@
                 if '.pytorch.org' in pretrained:
                     state_dict = map_state_dict(in_channels, self.state_dict(), state_dict, nd=nd,
                                                 fused_initial=fused_initial)
                 self.load_state_dict(state_dict)
             else:
                 raise ValueError('There is no default set of weights for this model. '
                                  'Please specify a URL using the `pretrained` argument.')
+        if pyramid_pooling:
+            pyramid_pooling_kwargs = {} if pyramid_pooling_kwargs is None else pyramid_pooling_kwargs
+            append_pyramid_pooling_(self, pyramid_pooling_channels, nd=nd, **pyramid_pooling_kwargs)
 
 
 class ConvNeXtTiny(ConvNeXt):
     def __init__(
             self,
             in_channels: int = 3,
             out_channels: int = 0,
@@ -230,14 +248,15 @@
             stochastic_depth_prob: Stochastic depth probability.
                 Base probability of randomly dropping residual connections. Actual probability in blocks is given by
                 ``stochastic_depth_prob * stage_block_id / (total_stage_blocks - 1.0)``.
             pretrained: Whether to use pretrained weights. By default, weights from ``torchvision`` are used.
             nd: Number of spatial dimensions.
             **kwargs: Additional keyword arguments.
         """
+        self.save_hyperparameters()
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ConvNeXtTiny']
         super().__init__(
             in_channels=in_channels,
             out_channels=out_channels,
             block_setting=[
                 CNBlockConfig(96, 192, 3),
@@ -258,14 +277,15 @@
             in_channels: int = 3,
             out_channels: int = 0,
             stochastic_depth_prob: float = .1,
             pretrained: bool = False,
             nd: int = 2,
             **kwargs
     ):
+        self.save_hyperparameters()
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ConvNeXtSmall']
         super().__init__(
             in_channels=in_channels,
             out_channels=out_channels,
             block_setting=[
                 CNBlockConfig(96, 192, 3),
@@ -300,14 +320,15 @@
             stochastic_depth_prob: Stochastic depth probability.
                 Base probability of randomly dropping residual connections. Actual probability in blocks is given by
                 ``stochastic_depth_prob * stage_block_id / (total_stage_blocks - 1.0)``.
             pretrained: Whether to use pretrained weights. By default, weights from ``torchvision`` are used.
             nd: Number of spatial dimensions.
             **kwargs: Additional keyword arguments.
         """
+        self.save_hyperparameters()
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ConvNeXtBase']
         super().__init__(
             in_channels=in_channels,
             out_channels=out_channels,
             block_setting=[
                 CNBlockConfig(128, 256, 3),
@@ -342,14 +363,15 @@
             stochastic_depth_prob: Stochastic depth probability.
                 Base probability of randomly dropping residual connections. Actual probability in blocks is given by
                 ``stochastic_depth_prob * stage_block_id / (total_stage_blocks - 1.0)``.
             pretrained: Whether to use pretrained weights. By default, weights from ``torchvision`` are used.
             nd: Number of spatial dimensions.
             **kwargs: Additional keyword arguments.
         """
+        self.save_hyperparameters()
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ConvNeXtLarge']
         super().__init__(
             in_channels=in_channels,
             out_channels=out_channels,
             block_setting=[
                 CNBlockConfig(192, 384, 3),
```

### Comparing `CellDetection-0.4.5/celldetection/models/cpn.py` & `celldetection-0.4.8/celldetection/models/cpn.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/features.py` & `celldetection-0.4.8/celldetection/models/features.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/filters.py` & `celldetection-0.4.8/celldetection/models/filters.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/fpn.py` & `celldetection-0.4.8/celldetection/models/fpn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,73 @@
 import torch
 from torch import nn
 from torch import Tensor
 from torch.nn import functional as F
 from torchvision.models.detection import backbone_utils
 from torchvision.models._utils import IntermediateLayerGetter
 from torchvision.ops import feature_pyramid_network
-from torchvision.ops.feature_pyramid_network import ExtraFPNBlock
-from ..util.util import lookup_nn
-from .commons import ConvNorm, _ni_3d
+from torchvision.ops.feature_pyramid_network import ExtraFPNBlock as _ExtraFPNBlock
+from ..util.util import lookup_nn, dict2model, update_model_hparams_, resolve_model
+from .commons import ConvNorm, _ni_3d, Normalize
 from .resnet import ResNet18, ResNet34, ResNet50, ResNet101, ResNet152, ResNeXt50_32x4d, ResNeXt101_32x8d, \
     ResNeXt152_32x8d, WideResNet50_2, WideResNet101_2
 from .mobilenetv3 import MobileNetV3Large, MobileNetV3Small
 from typing import Optional, Callable, List, Tuple, Dict
 from functools import partial
+from pytorch_lightning.core.mixins import HyperparametersMixin
 from .smp import SmpEncoder
 from .timmodels import TimmEncoder
 from .convnext import ConvNeXtLarge, ConvNeXtSmall, ConvNeXtBase, ConvNeXtTiny
+import copy
 
 __all__ = []
 
 
 def register(obj):
     __all__.append(obj.__name__)
     return obj
 
 
+class ExtraFPNBlock(_ExtraFPNBlock):
+    """
+    Base class for the extra block in the FPN.
+
+    Args:
+        results (List[Tensor]): the result of the FPN
+        x (List[Tensor]): the original feature maps
+        names (List[str]): the names for each one of the
+            original feature maps
+
+    Returns:
+        results (List[Tensor]): the extended set of results
+            of the FPN
+        names (List[str]): the extended set of names for the results
+    """
+
+    def adapt_out_channel_list(self, channel_list):  # must be implemented if extra block changes channels
+        return channel_list
+
+
 class LastLevelMaxPool(ExtraFPNBlock):
     def __init__(self, nd=2):
         """
         This is an adapted class from torchvision to support n-dimensional data.
 
         References:
             https://github.com/pytorch/vision/blob/d2d448c71b4cb054d160000a0f63eecad7867bdb/torchvision/ops/feature_pyramid_network.py#L207
 
         Notes:
             This class just applies stride 2 to spatial dimensions, and uses pytorch's max_pool function to do it.
         """
         super().__init__()
         self._fn = lookup_nn('max_pool2d', nd=nd, call=False, src=F)
 
+    def adapt_out_channel_list(self, channel_list):  # must be implemented if extra block changes channels
+        return channel_list + channel_list[-1:]
+
     def forward(
             self,
             x: List[Tensor],
             y: List[Tensor],
             names: List[str],
     ) -> Tuple[List[Tensor], List[str]]:
         names.append("pool")
@@ -58,15 +83,32 @@
             out_channels: int,
             block_cls=None,
             block_kwargs: dict = None,
             extra_blocks: Optional['ExtraFPNBlock'] = None,
             norm_layer: Optional[Callable[..., nn.Module]] = None,
             nd: int = 2,
     ):
+        """Feature Pyramid Network
+
+        Note:
+            Model uses output convolutions, mapping decoder features to the returned output.
+            If output features are not used (e.g. by prediction heads), the parameters of the output convolutions
+            will not contribute to the loss, which is to be avoided and may lead to a `RuntimeError`.
+
+        Args:
+            in_channels_list:
+            out_channels:
+            block_cls:
+            block_kwargs:
+            extra_blocks:
+            norm_layer:
+            nd:
+        """
         super(feature_pyramid_network.FeaturePyramidNetwork, self).__init__()
+
         block = partial(ConvNorm, nd=nd) if block_cls is None else block_cls
         block_kwargs = {} if block_kwargs is None else block_kwargs
         self.inner_blocks = nn.ModuleList()
         self.layer_blocks = nn.ModuleList()
         for in_channels in in_channels_list:
             if in_channels == 0:
                 raise ValueError("in_channels=0 is currently not supported")
@@ -95,34 +137,60 @@
 class BackboneWithFPN(backbone_utils.BackboneWithFPN):
     def __init__(
             self,
             backbone: nn.Module,
             return_layers: Dict[str, str],
             in_channels_list: List[int],
             out_channels: int,
+            out_channel_list: List[int],
             extra_blocks: Optional['ExtraFPNBlock'] = None,
             norm_layer: Optional[Callable[..., nn.Module]] = None,
+            ilg=None,
+            nd: int = 2,
+            **kwargs
     ) -> None:
         super(backbone_utils.BackboneWithFPN, self).__init__()
-
+        if ilg is None:
+            ilg = isinstance(backbone, nn.Sequential)
         if extra_blocks is None:
-            extra_blocks = backbone_utils.LastLevelMaxPool()
-
-        self.body = IntermediateLayerGetter(backbone, return_layers=return_layers)
+            extra_blocks = LastLevelMaxPool(nd=nd)
+            if hasattr(extra_blocks, 'adapt_out_channel_list'):
+                out_channel_list = extra_blocks.adapt_out_channel_list(out_channel_list)
+
+        pretrained_cfg = backbone.__dict__.get('pretrained_cfg', {})
+        if not len(pretrained_cfg) and hasattr(backbone, 'hparams') and isinstance(backbone.hparams, dict):
+            pretrained_cfg = backbone.hparams.get('pretrained_cfg', pretrained_cfg)
+
+        if kwargs.pop('normalize', True):
+            self.normalize = Normalize(mean=kwargs.get('inputs_mean', pretrained_cfg.get('mean', 0.)),
+                                       std=kwargs.get('inputs_std', pretrained_cfg.get('std', 1.)),
+                                       assert_range=kwargs.get('assert_range', (0., 1.)))
+        else:
+            self.normalize = None
+        self.body = IntermediateLayerGetter(backbone, return_layers=return_layers) if ilg else backbone
         self.fpn = FeaturePyramidNetwork(
             in_channels_list=in_channels_list,
             out_channels=out_channels,
             extra_blocks=extra_blocks,
             norm_layer=norm_layer,
+            nd=nd
         )
-        self.out_channels = out_channels
+        # self.out_channels = out_channels
+        self.out_channels = out_channel_list
+
+    def forward(self, x: Tensor) -> Dict[str, Tensor]:
+        if self.normalize is not None:
+            x = self.normalize(x)
+        x = self.body(x)
+        x = self.fpn(x)
+        return x
 
 
 @register
-class FPN(BackboneWithFPN):
+class FPN(BackboneWithFPN, HyperparametersMixin):
     def __init__(self, backbone, channels=256, return_layers: dict = None, **kwargs):
         """
 
         Examples:
             >>> from celldetection.models import ResNet18, FPN
             ... import torch
             >>> model = FPN(ResNet18(in_channels=1))
@@ -138,23 +206,30 @@
             backbone: Backbone module
                 Note that `backbone.out_channels` must be defined.
             channels: Channels in the upsampling branch.
             return_layers: Dictionary like `{backbone_layer_name: out_name}`.
                 Note that this influences how outputs are computed, as the input for the upsampling
                 is gathered by `IntermediateLayerGetter` based on given dict keys.
         """
+        self.save_hyperparameters(ignore=['backbone'])
+        update_model_hparams_(self, resolve=kwargs.pop('resolve_model_hparam', True), backbone=backbone)
+        backbone = resolve_model(backbone, **kwargs.pop('backbone_kwargs', {}))
         names = [name for name, _ in backbone.named_children()]  # assuming ordered
         if return_layers is None:
             return_layers = {n: str(i) for i, n in enumerate(names)}
+            out_channel_list = [channels] * len(list(backbone.out_channels))
+        else:
+            out_channel_list = [channels] * len(return_layers)
         layers = {str(k): (str(names[v]) if isinstance(v, int) else str(v)) for k, v in return_layers.items()}
         super(FPN, self).__init__(
             backbone=backbone,
             return_layers=layers,
             in_channels_list=list(backbone.out_channels),
             out_channels=channels,
+            out_channel_list=out_channel_list,  # [channels] * len(layers),
             **kwargs
         )
 
 
 def _default_res_kwargs(backbone_kwargs, pretrained=False):
     kw = dict(fused_initial=False, pretrained=pretrained)
     kw.update({} if backbone_kwargs is None else backbone_kwargs)
```

### Comparing `CellDetection-0.4.5/celldetection/models/inference.py` & `celldetection-0.4.8/celldetection/models/inference.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/lightning.py` & `celldetection-0.4.8/celldetection/util/schedule.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,395 +1,574 @@
-import matplotlib.pyplot as plt
-import pytorch_lightning as pl
-import torch
-from typing import Any, Optional, Dict, List, Tuple, Union, Sequence, Callable
-from ..util.schedule import Config, conf2scheduler, conf2optimizer
-from ..util.util import asnumpy, get_tiling_slices, fetch_model, load_model
-from torch import optim, Tensor, nn
-from collections import OrderedDict, ChainMap
-from ..data.instance_eval import LabelMatcher, LabelMatcherList
-from ..data.cpn import contours2labels
-from ..data.misc import channels_first2channels_last
-from ..ops.cpn import remove_border_contours
-from . import cpn
-from ..visualization.images import show_detection, imshow_row
-from torch.distributed import is_available, all_gather_object, get_world_size, is_initialized, get_rank
-from itertools import chain
-import numpy as np
-from os.path import isfile
-from torchvision.ops.boxes import remove_small_boxes, nms
-from torch.optim.lr_scheduler import SequentialLR
-from ..optim.lr_scheduler import WarmUp
-from ..util.util import GpuStats, to_device, dict2model, model2dict
-
-STEP_OUTPUT = Union[Tensor, Dict[str, Any]]
-EPOCH_OUTPUT = List[STEP_OUTPUT]
-
-GPU_STATS = GpuStats() if torch.cuda.is_available() else None
-
-
-class LitCpn(pl.LightningModule):
-    def __init__(
-            self,
-            model: Union[str, nn.Module],
-            losses_prog_bar=True,
-            optimizer=None,
-            scheduler=None,
-            scheduler_conf=None,
-            warmup_steps=512,
-            **kwargs
-    ):
-        super().__init__()
-        self.save_hyperparameters()
-        if isinstance(model, str):
-            model = self.build_model(model, **kwargs)
-            if kwargs.pop('resolve_model_hparam', True):
-                self.hparams['model'] = model2dict(model)
-        elif isinstance(model, dict):
-            model = dict2model(model)
-        self.model = model
-        self.inputs_key = 'inputs'
-        self.targets_key = 'targets'
-        self.val_iou_thresholds = kwargs.get('val_iou_thresholds', (.5, .6, .7, .8, .9))
-        self.test_iou_thresholds = kwargs.get('test_iou_thresholds', (.5, .6, .7, .8, .9))
-        self.losses_prog_bar = losses_prog_bar
-        self.warmup_steps = warmup_steps
-        self._optimizer = optimizer
-        self._scheduler = scheduler
-        self._scheduler_conf = scheduler_conf
-        self._lr_multiplier = kwargs.get('lr_multiplier')
-        self._weight_decay_multiplier = kwargs.get('weight_decay_multiplier')
-        self.figsize = kwargs.get('figsize', (32, 18))
-        self._log_figures = kwargs.get('log_figures', True)
-        self._eval_zero_division = kwargs.get('eval_zero_division', 0.)
-        self._validation_outputs = None
-        self._test_outputs = None
-        self._predict_outputs = None
-        self._val_mean_keys = (
-            'f1',
-
-            'f1_np',
-            'jaccard_np',
-            'fowlkes_mallows_np',
-            'recall',
-            'precision',
-
-            'avg_recall',
-            'avg_precision',
-            'avg_f1',
-            'avg_jaccard',
-            'avg_fowlkes_mallows',
+from .util import dict_hash, Dict, tweak_module_, lookup_nn, print_to_file
+from ..optim import lr_scheduler
+import json
+from itertools import product
+from collections import OrderedDict
+from torch.nn import Module
+from torch import optim
+import inspect
+from typing import Callable, Union
+import albumentations as A
+from os.path import splitext
+import yaml
+
+__all__ = ['Config', 'Schedule', 'conf2optimizer', 'conf2scheduler', 'conf2augmentation', 'conf2tweaks_', 'conf2call']
+
+
+def conf2call(settings: Union[dict, str], origin, **kwargs):
+    """Config to call.
+
+    Examples:
+        >>> import celldetection as cd
+        >>> model = cd.conf2call('ResNet18', cd.models, in_channels=1)
+        >>> model = cd.conf2call({'ResNet18': dict(in_channels=1)}, cd.models)
+
+    Args:
+        settings: Name or dictionary as ``{name: kwargs}``. Name must be the symbol's name that is to be retrieved
+            from ``origin``.
+        origin: Origin.
+        **kwargs: Additional keyword arguments for the call of retrieved symbol.
+
+    Returns:
+        Return value of the call of retrieved symbol.
+    """
+    assert len(settings) == 1 or isinstance(settings, str)
+    if not isinstance(origin, (tuple, list)):
+        origin = origin,
+    if isinstance(settings, str):
+        key = settings
+        kw = {}
+    else:
+        key = next(iter(settings.keys()))
+        kw = next(iter(settings.values()))
+    try:
+        fn = next(iter(getattr(o, key) for o in origin if hasattr(o, key)))
+    except StopIteration:
+        raise ValueError(f'No such function: {key} in {origin}')
+    return fn(**kw, **kwargs)
+
+
+def conf2optimizer(settings: dict, params):
+    """Config to optimizer.
+
+    Examples:
+        >>> import celldetection as cd
+        >>> module = nn.Conv2d(1, 2, 3)
+        >>> optimizer = cd.conf2optimizer({'Adam': dict(lr=.0002, betas=(0.5, 0.999))}, module.parameters())
+        ... optimizer
+        Adam (
+            Parameter Group 0
+                amsgrad: False
+                betas: (0.5, 0.999)
+                eps: 1e-08
+                lr: 0.0002
+                weight_decay: 0
         )
-        self._val_sum_keys = ('true_positives', 'false_negatives', 'false_positives')
-        self._test_mean_keys = tuple(self._val_mean_keys)
-        self._test_sum_keys = tuple(self._val_sum_keys)
-        self.max_imsize = kwargs.get('max_imsize', 2048)
+
+    Args:
+        settings:
+        params:
+
+    Returns:
+
+    """
+    return conf2call(settings, optim, params=params)
+
+
+def conf2scheduler(settings: dict, optimizer, origins=None):
+    if origins is None:
+        origins = (lr_scheduler, optim.lr_scheduler)
+    return conf2call(settings, origins, optimizer=optimizer)
+
+
+def conf2augmentation(settings: dict) -> A.Compose:
+    """Config to augmentation.
+
+    Maps settings to composed augmentation workflow using ``albumentations``.
+
+    Examples:
+        >>> import celldetection as cd
+        >>> cd.conf2augmentation({
+        ...     'RandomRotate90': dict(p=.5),
+        ...     'Transpose': dict(p=.5),
+        ... })
+        Compose([
+          RandomRotate90(always_apply=False, p=0.5),
+          Transpose(always_apply=False, p=0.5),
+        ], p=1.0, bbox_params=None, keypoint_params=None, additional_targets={})
+
+    Args:
+        settings: Settings dictionary as ``{name: kwargs}``.
+
+    Returns:
+        ``A.Compose`` object.
+    """
+    return A.Compose([getattr(A, k)(**v) for k, v in settings.items()])
+
+
+def conf2tweaks_(settings: dict, module: Module):
+    """Config to tweaks.
+
+    Apply tweaks to module.
+
+    Notes:
+        - If module does not contain specified objects, nothing happens.
+
+    Examples:
+        >>> import celldetection as cd, torch.nn as nn
+        >>> model = cd.models.ResNet18(in_channels=3)
+        >>> cd.conf2tweaks_({nn.BatchNorm2d: dict(momentum=0.05)}, model)  # sets momentum to 0.05
+        >>> cd.conf2tweaks_({'BatchNorm2d': dict(momentum=0.42)}, model)  # sets momentum to 0.42
+        >>> cd.conf2tweaks_({'LeakyReLU': dict(negative_slope=0.2)}, model)  # sets negative_slope to 0.2
+
+    Args:
+        settings: Settings dictionary as ``{name: kwargs}``.
+        module: Module that is to be tweaked.
+
+    """
+    for key, kwargs in settings.items():
+        tweak_module_(module, lookup_nn(key, call=False), **kwargs)
+
+
+class Config(Dict):
+    def __init__(self, **kwargs):
+        """Config.
+
+        Just a ``dict`` with benefits.
+
+        ``Config`` objects treat values as attributes, print nicely, and can be saved and loaded to/from json files.
+        The ``hash`` method also offers a unique and compact string representation of the ``Config`` content.
+
+        Examples:
+            >>> import celldetection as cd, torch.nn as nn
+            >>> conf = cd.Config(optimizer={'Adam': dict(lr=.001)}, epochs=100)
+            >>> conf
+            Config(
+              (optimizer): {'Adam': {'lr': 0.001}}
+              (epochs): 100
+            )
+            >>> conf.to_json('config.json')
+            >>> conf.hash()
+            'cf647b987ca37eb954d8bd01df01809e'
+            >>> conf.epochs = 200
+            ... conf.epochs
+            200
+            >>> module = nn.Conv2d(1, 2, 3)
+            >>> optimizer = cd.conf2optimizer(conf.optimizer, module.parameters())
+            ... optimizer
+            Adam (
+                Parameter Group 0
+                    amsgrad: False
+                    betas: (0.9, 0.999)
+                    eps: 1e-08
+                    lr: 0.001
+                    weight_decay: 0
+            )
+
+        Args:
+            **kwargs: Items.
+        """
+        super().__init__(**kwargs)
+
+    def hash(self) -> str:
+        return dict_hash(self.to_dict())
 
     @staticmethod
-    def build_model(model: str, *args, **kwargs):
-        if model in dir(cpn):
-            assert 'cpn' in model.lower()
-            return getattr(cpn, model)(*args, **kwargs)
-        elif isfile(model):
-            return load_model(model, **kwargs)
-        else:
-            return fetch_model(model, **kwargs)
+    def from_json(filename):
+        c = Config()
+        c.load(filename, backend='json')
+        return c
 
-    def training_step(self, batch: dict, batch_idx: int) -> STEP_OUTPUT:
-        inputs = batch[self.inputs_key]
-        if batch_idx == 0:
-            logger = None if self.logger is None else self.logger.experiment
-            if logger is not None:
-                logger.add_images('inputs', inputs, self.global_step)
-        outputs: dict = self.model(inputs, targets=batch)
-        log_d = {} if GPU_STATS is None else GPU_STATS.dict(prefix='gpus/gpu')
-        losses = outputs.get('losses')
-        losses['loss'] = losses.get('loss', outputs['loss'])
-        if losses is not None and isinstance(losses, dict):
-            log_d.update({f'losses/{k}': v for k, v in losses.items() if v is not None})
-            self.log_dict(log_d, prog_bar=self.losses_prog_bar, logger=True, on_step=True)
-        return outputs
-
-    def training_step_end(self, training_step_outputs):
-        return training_step_outputs['loss']
-
-    def configure_optimizers(self):
-        if isinstance(self._optimizer, (dict, str, type(None))):
-            optimizer = dict(AdamW=dict()) if self._optimizer is None else self._optimizer
-            optimizer = conf2optimizer(optimizer, filter(lambda p: p.requires_grad, self.parameters()))
-        else:
-            optimizer = self._optimizer
+    @staticmethod
+    def from_yaml(filename):
+        c = Config()
+        c.load(filename, backend='yaml')
+        return c
 
-        if self._lr_multiplier is not None:
-            for gr in optimizer.param_groups:
-                print('Update learning rate from', gr['lr'], end='')
-                gr['lr'] *= self._lr_multiplier
-                print('to', gr['lr'], flush=True)
-        if self._weight_decay_multiplier is not None:
-            for gr in optimizer.param_groups:
-                if 'weight_decay' in gr:
-                    print('Update learning rate from', gr['weight_decay'], end='')
-                    gr['weight_decay'] *= self._weight_decay_multiplier
-                    print('to', gr['weight_decay'], flush=True)
+    @staticmethod
+    def from_file(filename):
+        c = Config()
+        c.load(filename)
+        return c
+
+    @staticmethod
+    def from_files(filenames, reverse=True):
+        """From files.
 
-        if self._scheduler is None:
-            return optimizer
+        Args:
+            filenames: Filenames
+            reverse: Whether to reverse filenames. True by default. If reversed, the leftmost elements
+                are dominant.
 
-        if isinstance(self._scheduler, (dict, str)):
-            scheduler = conf2scheduler(self._scheduler, optimizer)
+        Returns:
+            Config.
+        """
+        if isinstance(filenames, str):
+            return Config.from_file(filenames)
+        if reverse:
+            filenames = filenames[::-1]
+        c = Config.from_file(filenames[0])
+        for f in filenames[1:]:
+            c.update(Config.from_file(f))
+        return c
+
+    def load(self, filename, backend=None):
+        ext = splitext(filename)[1]
+        if backend == 'yaml' or ext in ('.yml', '.yaml'):
+            with open(filename, 'r') as fp:
+                config = yaml.safe_load(fp)
         else:
-            scheduler = self._scheduler
+            with open(filename, 'r') as fp:
+                config = json.load(fp)
+        if config is not None:
+            self.update(config)
+
+    def to_dict(self) -> dict:
+        return {k: (v.to_dict() if isinstance(v, Config) else v) for k, v in dict(self).items() if
+                not k.startswith('_')}
+
+    def to_json(self, filename):
+        with open(filename, 'w') as fp:
+            json.dump(self.to_dict(), fp)
+
+    def to_yaml(self, filename):  # cannot preserve types
+        with open(filename, 'w') as fp:
+            yaml.safe_dump(self.to_dict(), fp)
+
+    def to_txt(self, filename, mode='w', **kwargs):
+        print_to_file(self, filename=filename, mode=mode, **kwargs)
+
+    def __str__(self):
+        return repr(self)
+
+    def _get_name(self):
+        return 'Config'
+
+    def extra_repr(self) -> str:
+        return ''
+
+    def __repr__(self):
+        if '_modules' in self:
+            return str(self.to_dict())
+        self._modules = self.to_dict()
+        r = Module.__repr__(self)
+        del self._modules
+        return r
 
-        if self.warmup_steps and scheduler is not None:
-            scheduler = SequentialLR(optimizer, [WarmUp(optimizer, self.warmup_steps), scheduler],
-                                     milestones=[self.warmup_steps])
-
-        scheduler = {
-            **dict(
-                interval='step',
-                frequency=1,
-                scheduler=scheduler,
-                strict=True,
-                name=None,
-            ),
-            **self._scheduler_conf
-        }
-
-        return [optimizer], [scheduler]
-
-    def log_figures(self, tag, inputs, contours, close=True):
-        logger = None if self.logger is None else self.logger.experiment
-        if logger is not None:
-            figures = []
-            for i in range(len(inputs)):
-                img = channels_first2channels_last(asnumpy(inputs[i]))
-                cons = asnumpy(contours[i])
-                imshow_row(img, img, figsize=self.figsize)
-                figures.append(plt.gcf())
-                show_detection(contours=cons)
-            logger.add_figure(
-                tag=tag,
-                figure=figures,
-                global_step=self.global_step,
-                close=close
-            )
-            plt.close('all')  # should be done above
+    def args(self, fn: Callable):
+        """
+
+        Examples:
+            >>> conf = cd.Config(a=1, b=2, c=42)
+            >>> def f(a, b):
+            ...     return a + b
+            >>> f(*conf.args(f))
+            3
+
+        Args:
+            fn:
+
+        Returns:
 
-    def evaluation_step(self, batch: dict, batch_idx: int, prefix: str):
-        inputs = batch[self.inputs_key]
-        indices = asnumpy(batch['indices'])
-        outputs: dict = self(inputs)  # TODO: Add val loss
-        contours = asnumpy(outputs['contours'])
-        targets = asnumpy(batch[self.targets_key])
-        if self._log_figures:
-            self.log_figures(tag=f'{prefix}/batch{batch_idx}', inputs=inputs, contours=contours)
-        matches = {}
-        for i, (cons, target, index) in enumerate(zip(contours, targets, indices)):
-            prediction = contours2labels(cons, size=inputs[i].shape[-2:], initial_depth=3)
-            target = channels_first2channels_last(target)
-            matches[index] = LabelMatcher(prediction, target, zero_division=0.)
-        return matches
+        """
+        r = []
+        for k in inspect.signature(fn).parameters.keys():
+            if k == 'args' or k == 'kwargs':
+                break
+            r.append(self[k])
+        return r
 
-    def evaluation_epoch_end(self, outputs, prefix, iou_thresholds, mean_keys, sum_keys) -> None:
+    def kwargs(self, fn: Callable):
         """
 
-        Note:
-            `outputs` is a nested sequence of dictionaries, mapping data_index to data_item. Use of dictionary prevents
-            double calculations of examples during evaluation. Note that double calculations are the default
-            behaviour in PyTorch's DistributedSampler and example omission the only provided
-            alternative (drop_last). Both would give wrong evaluation results.
-            The use of dictionaries prevents this, yielding correct evaluation results.
+        Examples:
+            >>> conf = cd.Config(a=1, b=2, c=42)
+            >>> def f(a, b):
+            ...     return a + b
+            >>> f(**conf.kwargs(f))
+            3
 
         Args:
-            outputs:
-            prefix:
-            iou_thresholds:
-            mean_keys:
-            sum_keys:
+            fn:
 
         Returns:
 
         """
-        if isinstance(outputs, list):
-            if is_available() and is_initialized():
-                o = ([None] * get_world_size())
-                all_gather_object(obj=outputs, object_list=o)  # give every rank access to results
-                outputs = o
-            if outputs is not None:
-                while len(outputs) and isinstance(outputs[0], list):
-                    outputs = list(chain.from_iterable(outputs))
-                assert isinstance(outputs[0], dict)
-                outputs = ChainMap(*outputs)
+        r = dict()
+        for k in inspect.signature(fn).parameters.keys():
+            if k == 'args' or k == 'kwargs':
+                continue
+            v = self.get(k, None)
+            if v is not None:
+                r[k] = v
+        return r
+
+    def __getstate__(self):
+        return self.to_dict()
+
+    def __setstate__(self, d: dict):
+        self.update(d)
+
+
+class Schedule:
+    def __init__(self, **kwargs):
+        """Schedule.
+
+        Provides an easy interface to the cross product of different configurations.
+
+        Examples:
+            >>> s = cd.Schedule(
+            ...     lr=(0.001, 0.0005),
+            ...     net=('resnet34', 'resnet50'),
+            ...     epochs=100
+            ... )
+            ... len(s)
+            4
+            >>> s[:]
+            [Config(
+              (epochs): 100
+              (lr): 0.001
+              (net): 'resnet34'
+            ), Config(
+              (epochs): 100
+              (lr): 0.001
+              (net): 'resnet50'
+            ), Config(
+              (epochs): 100
+              (lr): 0.0005
+              (net): 'resnet34'
+            ), Config(
+              (epochs): 100
+              (lr): 0.0005
+              (net): 'resnet50'
+            )]
+            >>> for config in s:
+            ...     print(config.lr, config.net, config.epoch)
+            0.001 resnet34 100
+            0.001 resnet50 100
+            0.0005 resnet34 100
+            0.0005 resnet50 100
+
+        Args:
+            **kwargs: Configurations. Possible item layouts:
+                ``<name>: <static setting>``,
+                ``<name>: (<option1>, ..., <optionN>)``,
+                ``<name>: [<option1>, ..., <optionN>]``,
+                ``<name>: {<option1>, ..., <optionN>}``.
+        """
+        self.values = OrderedDict({})
+        self.conditions = []
+        self.conditioned_values = []
+        self.add(kwargs)
+        self._iter_conf = None
+        self._iter_i = None
+
+    def get_multiples(self, num=2):
+        return {k: v for k, v in self.values.items() if (isinstance(v, (list, tuple, set)) and len(v) >= num)}
+
+    def add(self, d: dict = None, conditions: dict = None, **kwargs):
+        """Add setting to schedule.
+
+        Examples:
+            >>> schedule = cd.Schedule(model=('resnet18', 'resnet50'), batch_size=8)
+            ... schedule.add(batch_size=(16, 32), conditions={'model': 'resnet18'})
+            ... schedule[:]
+            [Config(
+               (batch_size): 16,
+               (model): resnet18,
+             ),
+             Config(
+               (batch_size): 32,
+               (model): resnet18,
+             ),
+             Config(
+               (batch_size): 8,
+               (model): resnet50,
+             )]
+
+            >>> schedule = cd.Schedule(model=('resnet18', 'resnet50'))
+            ... schedule.add(batch_size=(16, 32), conditions={'model': 'resnet18'})
+            ... schedule[:]
+            [Config(
+               (model): resnet18,
+               (batch_size): 16,
+             ),
+             Config(
+               (model): resnet18,
+               (batch_size): 32,
+             ),
+             Config(
+               (model): resnet50,
+             )]
+
+            >>> schedule = cd.Schedule(model=('resnet18', 'resnet50'), batch_size=(64, 128, 256))
+            ... schedule.add(batch_size=(16, 32), conditions={'model': 'resnet50'})
+            ... schedule[:]
+            [Config(
+               (batch_size): 64
+               (model): 'resnet18'
+             ),
+             Config(
+               (batch_size): 16
+               (model): 'resnet50'
+             ),
+             Config(
+               (batch_size): 32
+               (model): 'resnet50'
+             ),
+             Config(
+               (batch_size): 128
+               (model): 'resnet18'
+             ),
+             Config(
+               (batch_size): 256
+               (model): 'resnet18'
+             )]
+
+        Args:
+            d: Dictionary of settings.
+            conditions: If set, added settings are only applied if conditions are met.
+                Note: Conditioned settings replace/override existing settings if conditions are met.
+            **kwargs: Configurations. Possible item layouts:
+                <name>: <static setting>
+                <name>: (<option1>, ..., <optionN>)
+                <name>: [<option1>, ..., <optionN>]
+                <name>: {<option1>, ..., <optionN>}
+
+        """
+        if d is not None:
+            if isinstance(d, Schedule):
+                d = d.to_dict()
+            else:
+                assert isinstance(d, dict)
+            d.update(kwargs)
+            kwargs = d
+        if conditions is None:
+            dst = self.values
         else:
-            raise ValueError(type(outputs))
+            self.conditions.append(OrderedDict(conditions))
+            dst = OrderedDict()
+            self.conditioned_values.append(dst)
+        for key, val in kwargs.items():
+            if not isinstance(val, (tuple, list, set)):
+                val = (val,)
+            dst[key] = val
 
-        if outputs is not None:
-            res = LabelMatcherList(list(outputs.values()))
+    @staticmethod
+    def _product(v):
+        keys = list(v.keys())
+        keys.sort()
+        vals = list(product(*[v[k] for k in keys]))
+        return [{k: v for k, v in zip(keys, va)} for va in vals]
+
+    @property
+    def product(self):
+        initials = finals = self._product(self.values)
+        for conditions, conditioned_values in zip(self.conditions, self.conditioned_values):
+            finals = []
+            for i in initials:
+                if all(((i[ck] in conditions[ck]) if isinstance(conditions[ck], tuple) else (conditions[ck] == i[ck])
+                        for ck in conditions.keys())):
+                    extra = self._product(conditioned_values)
+                    for j in extra:
+                        extra_i = dict(i)
+                        extra_i.update(j)
+                        finals.append(extra_i)
+                else:
+                    finals.append(i)
+            initials = finals
+        return finals
+
+    @property
+    def configs(self):
+        return list({c.hash(): c for c in [Config(**p) for p in self.product]}.values())
+
+    def __str__(self):
+        return Module.__repr__(Dict(_get_name=lambda: 'Schedule', extra_repr=lambda: '', _modules=dict(self.values)))
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __getitem__(self, item):
+        return self.configs[item]
+
+    def __len__(self):
+        return len(self.configs)
+
+    def to_json(self, filename):
+        with open(filename, 'w') as fp:
+            json.dump(self.values, fp)
+
+    def to_yaml(self, filename):  # cannot preserve types
+        with open(filename, 'w') as fp:
+            yaml.safe_dump(self.to_dict(), fp)
 
-            # Gather results for different IoU thresholds
-            primary = {k: [] for k in mean_keys + sum_keys}
-            primary['score_thresh'] = self.model.__dict__.get('score_thresh')
-            primary['nms_thresh'] = self.model.__dict__.get('nms_thresh')
-            primary['num_examples'] = len(res)
-            secondary = {}
-            for res.iou_thresh in iou_thresholds:
-                for k in mean_keys + sum_keys:
-                    v = getattr(res, k)
-                    primary[k].append(v)
-                    secondary[f'{k}_{int(res.iou_thresh * 100)}'] = v
-
-            # Reduce results
-            for k in mean_keys:
-                primary[k] = np.mean(primary[k])
-            for k in sum_keys:
-                primary[k] = np.sum(primary[k])
-
-            self.log_dict({f'{prefix}/{k}': float(v) for k, v in primary.items()}, logger=True, sync_dist=True,
-                          reduce_fx='max')  # ranks are assumed to have same results
-            self.log_dict({f'{prefix}_detail/{k}': float(v) for k, v in secondary.items()}, logger=True, sync_dist=True,
-                          reduce_fx='max')
-
-    def on_validation_epoch_start(self) -> None:
-        self._validation_outputs = []
-
-    def validation_step(self, batch: dict, batch_idx: int):
-        outputs = self.evaluation_step(batch, batch_idx, 'val')
-        self._validation_outputs.append(outputs)
-        return outputs
-
-    def on_validation_epoch_end(self) -> None:
-        assert self._validation_outputs is not None
-        outputs = self._validation_outputs
-        self.evaluation_epoch_end(outputs, 'val', iou_thresholds=self.val_iou_thresholds,
-                                  sum_keys=self._val_sum_keys, mean_keys=self._val_mean_keys)
-
-    def on_test_epoch_start(self) -> None:
-        self._test_outputs = []
-
-    def test_step(self, batch: dict, batch_idx: int):
-        outputs = self.evaluation_step(batch, batch_idx, 'test')
-        self._test_outputs.append(outputs)
-
-    def on_test_epoch_end(self) -> None:
-        outputs = self._test_outputs
-        self.evaluation_epoch_end(outputs, 'test', iou_thresholds=self.test_iou_thresholds,
-                                  sum_keys=self._test_sum_keys, mean_keys=self._test_mean_keys)
-
-    def on_predict_epoch_start(self) -> None:
-        self._predict_outputs = []
-
-    def predict_step(self, batch: Any, batch_idx: int, dataloader_idx: int = 0) -> Any:
-        if isinstance(batch, Tensor):
-            return super().predict_step(batch, batch_idx, dataloader_idx)
-        assert isinstance(batch, dict)
-        inputs = batch.pop(self.inputs_key)
-        assert inputs is not None
-        out = OrderedDict(batch)
-        out.update(self(inputs, **batch))
-        self._predict_outputs.append(out)
-        return out
-
-    def on_predict_epoch_end(self) -> None:
-        outputs = self._predict_outputs
-        return outputs
-
-    def forward(
-            self,
-            inputs: Tensor,
-            targets: Optional[Dict[str, Tensor]] = None,
-            max_imsize: Optional[int] = None,
-            **kwargs
-    ) -> Dict[str, Union[Tensor, List[Tensor]]]:
-        max_imsize = self.max_imsize if max_imsize is None else max_imsize
-        if max_imsize and max(inputs.shape[2:]) > max_imsize:
-            return self.forward_tiled(inputs, targets=targets, **kwargs)
-
-        device = self.device
-        if inputs.device != device:
-            inputs = inputs.to(device)
-
-        return self.model(inputs, targets=targets, **kwargs)
-
-    def forward_tiled(
-            self,
-            inputs: Tensor,
-            crop_size: Union[int, Sequence[int]] = 768,
-            stride: Union[int, Sequence[int]] = 384,
-            **kwargs
-    ) -> Dict[str, List[Tensor]]:
-        assert np.array(crop_size) <= np.array(stride) * 2
-        slices, slices_by_dim = get_tiling_slices(inputs.shape[2:], crop_size, stride)  # ordered
-        prod = np.prod(slices_by_dim)
-        results: List[List[Dict[str, Tensor]]] = [[None] * prod for _ in torch.arange(0, inputs.shape[0])]
-        h_tiles, w_tiles = slices_by_dim
-        device = self.device
-        extra_keys = kwargs.get('extra_keys', ())  # extra output keys
-        extra_nms = kwargs.get('extra_nms', {})  # specify which extra outputs need to be filtered by nms
-        border_removal = kwargs.get('border_removal', 6)
-        box_min_size = kwargs.get('min_box_size', 1.)
-        nms_thresh = kwargs.get('nms_thresh', self.model.__dict__.get('nms_thresh', None))
-        inputs_mask = kwargs.get('inputs_mask')
-        assert nms_thresh is not None, 'Could not retrieve nms_thresh from model. Please specify it in forward method.'
-        for i, slices_ in enumerate(slices):
-            crop = inputs[(...,) + tuple(slices_)].to(device)
-            if inputs_mask is not None:
-                crop_m = inputs_mask[(...,) + tuple(slices_)].to(device)
-                if not torch.any(crop_m):
-                    continue  # skip masked out tile
-            outputs = self.forward(crop, targets=kwargs.get('targets'), max_imsize=False)
-            h_i, w_i = np.unravel_index(i, slices_by_dim)
-            h_start, w_start = [s.start for s in slices_]
-
-            top, bottom = h_i > 0, h_i < (h_tiles - 1)
-            right, left = w_i < (w_tiles - 1), w_i > 0
-            for j in torch.arange(0, inputs.shape[0]):
-                contours = outputs['contours'][j]
-                boxes = outputs['boxes'][j]
-                scores = outputs['scores'][j]
-                extra = [outputs[k][j] for k in extra_keys]
-
-                # Remove small boxes (default min_size: 1.)
-                keep = remove_small_boxes(boxes, box_min_size)
-                contours, scores, boxes = (c[keep] for c in (contours, scores, boxes))
-                extra = [e[keep] for e in extra]
-
-                # Remove partial detections to avoid tiling artifacts
-                keep = remove_border_contours(contours, crop.shape[2:], border_removal,
-                                              top=top, right=right, bottom=bottom, left=left)
-                contours, scores, boxes = (c[keep] for c in (contours, scores, boxes))
-                extra = [e[keep] for e in extra]
-
-                # Add offset  # TODO: Replace with cpn internal offsets
-                contours[..., 1] += h_start
-                contours[..., 0] += w_start
-                boxes[..., [0, 2]] += w_start
-                boxes[..., [1, 3]] += h_start
-
-                results[j][i] = dict(
-                    contours=contours,
-                    boxes=boxes,
-                    scores=scores,
-                    extra=extra,  # list
-                    keep=torch.ones(contours.shape[0], dtype=torch.bool)
-                )
-
-        final = OrderedDict(
-            contours=[torch.cat([res_['contours'] for res_ in res if res_ is not None]) for res in results],
-            scores=[torch.cat([res_['scores'] for res_ in res if res_ is not None]) for res in results],
-            boxes=[torch.cat([res_['boxes'] for res_ in res if res_ is not None]) for res in results],
-            **{k: [torch.cat([res_['extra'][i] for res_ in res if res_ is not None]) for res in results] for i, k in
-               enumerate(extra_keys)}
-        )
+    @staticmethod
+    def from_json(filename):
+        c = Schedule()
+        c.load(filename, backend='json')
+        return c
 
-        if not self.training:
-            for n in torch.arange(inputs.shape[0]):  # TODO
-                boxes = final['boxes'][n]
-                reference = boxes.shape[0]
-                keep = nms(boxes, final['scores'][n], iou_threshold=nms_thresh)
-                for k in final:
-                    v = final[k][n]
-                    if extra_nms.get(k, True):
-                        assert v.shape[0] == reference, f'Output `{k}` is not compatible with nms. ' \
-                                                        f'Specify extra_nms=dict({k}=False) when calling ' \
-                                                        f'forward method.'
-                        final[k][n] = v[keep]
-        return final
+    @staticmethod
+    def from_yaml(filename):
+        c = Schedule()
+        c.load(filename, backend='yaml')
+        return c
+
+    @staticmethod
+    def from_file(filename):
+        c = Schedule()
+        c.load(filename)
+        return c
+
+    @staticmethod
+    def from_files(filenames, reverse=True):
+        """From files.
+
+        Args:
+            filenames: Filenames
+            reverse: Whether to reverse filenames. True by default. If reversed, the leftmost elements
+                are dominant.
+
+        Returns:
+            Schedule.
+        """
+        if isinstance(filenames, str):
+            return Schedule.from_file(filenames)
+        if reverse:
+            filenames = filenames[::-1]
+        c = Schedule.from_file(filenames[0])
+        for f in filenames[1:]:
+            c.add(Schedule.from_file(f))
+        return c
+
+    def load(self, filename, backend=None):
+        ext = splitext(filename)[1]
+        if backend == 'yaml' or ext in ('.yml', '.yaml'):
+            with open(filename, 'r') as fp:
+                self.values = yaml.safe_load(fp)
+        else:
+            with open(filename, 'r') as fp:
+                self.values = json.load(fp)
+
+    def to_dict(self):
+        return dict(self.values)
+
+    def to_dict_list(self):
+        return [c.to_dict() for c in self]
+
+    def __eq__(self, other):
+        assert isinstance(other, Schedule)
+        return self.values.__eq__(other.to_dict())
+
+    def __iter__(self):
+        self._iter_conf = self.configs
+        self._iter_i = 0
+        return self
+
+    def __next__(self):
+        if self._iter_i < len(self._iter_conf):
+            res = self._iter_conf[self._iter_i]
+            self._iter_i += 1
+            return res
+        else:
+            raise StopIteration
```

### Comparing `CellDetection-0.4.5/celldetection/models/loss.py` & `celldetection-0.4.8/celldetection/models/loss.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/manet.py` & `celldetection-0.4.8/celldetection/models/manet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import torch.nn as nn
 from torch.nn.functional import softmax
 from typing import Optional, Union, List, Type, Dict
 from torch import Tensor
 from torch.nn import functional as F
 from functools import partial
-from ..util.util import lookup_nn
+from ..util.util import lookup_nn, dict2model
 from .unet import UNet, IntermediateUNetBlock
 from .commons import ConvNormRelu, SqueezeExcitation as SE, _ni_3d
 from .smp import SmpEncoder
 from .timmodels import TimmEncoder
 
 __all__ = [
     'MaNet', 'MultiscaleFusionAttention', 'PositionWiseAttention',
@@ -110,15 +110,15 @@
             b = self.se_low(x2)  # lateral
             x = x * (a + b)  # scaled x
             x = torch.cat((x, x2), 1)
         return self.out_block(x)
 
 
 class MaNet(UNet):
-    def __init__(self, backbone, out_channels: int, pab_channels=64,
+    def __init__(self, backbone, out_channels: int = 0, pab_channels=64,
                  block: Type[nn.Module] = None, block_kwargs: dict = None, final_activation=None,
                  interpolate='nearest', nd=2, **kwargs):
         """Multi-Scale Attention Network.
 
         A U-Net variant using a generic encoder and a special decoder that includes a
         Position-wise Attention Block (PAB) and several Multi-scale Fusion Attention Blocks (MFAB).
 
@@ -132,14 +132,17 @@
             block: Main block. Default: Multi-scale Fusion Attention Block (MFAB).
             block_kwargs: Block keyword arguments.
             final_activation: Final activation function.
             interpolate: Interpolation.
             nd: Spatial dimensions.
             **kwargs: Additional keyword arguments.
         """
+        if isinstance(backbone, dict):
+            backbone = dict2model(backbone)
+
         oc = backbone.out_channels
         intermediate_blocks = None
         if pab_channels:
             intermediate_blocks = PAB(oc[-1], oc[-1], mid_channels=pab_channels, nd=nd,
                                       replace=True, **kwargs.get('pwa_kwargs', {}))
         kwargs['block_interpolate'] = block_interpolate = kwargs.get('block_interpolate', True)
         if block is None:
```

### Comparing `CellDetection-0.4.5/celldetection/models/mobilenetv3.py` & `celldetection-0.4.8/celldetection/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/normalization.py` & `celldetection-0.4.8/celldetection/models/normalization.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/ppm.py` & `celldetection-0.4.8/celldetection/models/ppm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from typing import Union
 from torchvision.models.segmentation.deeplabv3 import ASPP
-from ..util.util import lookup_nn
+from ..util.util import lookup_nn, get_nd_conv
 
 __all__ = ['Ppm']
 
 
 class Ppm(nn.Module):
     def __init__(
             self,
             in_channels, out_channels,
             scales: Union[list, tuple] = (1, 2, 3, 6),
             kernel_size=1,
             norm='BatchNorm2d',
             activation='relu',
             concatenate=True,
+            nd=2,
             **kwargs
     ):
         """Pyramid Pooling Module.
 
         References:
             - https://ieeexplore.ieee.org/document/8100143
 
@@ -34,41 +35,47 @@
             concatenate: Whether to concatenate module inputs to pyramid pooling output before returning results.
             **kwargs: Keyword arguments for ``nn.Conv2d``.
         """
         super().__init__()
         self.blocks = nn.ModuleList()
         self.concatenate = concatenate
         self.out_channels = out_channels * len(scales) + in_channels * int(concatenate)
-        norm = lookup_nn(norm, call=False)
-        activation = lookup_nn(activation, call=False)
+        Conv = get_nd_conv(nd)
+        AdaptiveAvgPool = lookup_nn(nn.AdaptiveAvgPool2d, call=False, nd=nd)
+        norm = lookup_nn(norm, call=False, nd=nd)
+        activation = lookup_nn(activation, call=False, nd=nd)
         for scale in scales:
             self.blocks.append(nn.Sequential(
-                nn.AdaptiveAvgPool2d(output_size=scale),
-                nn.Conv2d(in_channels, out_channels, kernel_size, **kwargs),
+                AdaptiveAvgPool(output_size=scale),
+                Conv(in_channels, out_channels, kernel_size, **kwargs),
                 norm(out_channels),
                 activation(),
             ))
 
     def forward(self, x):
         prefix = [x] if self.concatenate else []
         return torch.cat(prefix + [
-            F.interpolate(m(x), x.shape[-2:], mode='bilinear', align_corners=False) for m in self.blocks
+            F.interpolate(m(x), x.shape[2:], mode='bilinear', align_corners=False) for m in self.blocks
         ], 1)
 
 
 def append_pyramid_pooling_(module: nn.Sequential, out_channels, scales=(1, 2, 3, 6), method='ppm', in_channels=None,
                             **kwargs):
     if in_channels is None:
         in_channels = module.out_channels[-1]
     method = method.lower()
     if method == 'ppm':
         assert (out_channels % len(scales)) == 0
         p = Ppm(in_channels, out_channels, scales=scales, **kwargs)
         out_channels = p.out_channels
     elif method == 'aspp':
         scales = sorted(tuple(set(scales) - {1}))
+        nd = kwargs.pop('nd', 2)
+        assert nd == 2, NotImplementedError('Only nd=2 supported.')
         p = ASPP(in_channels, scales, out_channels, **kwargs)
     else:
         raise ValueError
     module.append(p)
     if hasattr(module, 'out_channels'):
         module.out_channels += (out_channels,)
+    if hasattr(module, 'out_strides'):
+        module.out_strides += module.out_strides[-1:]
```

### Comparing `CellDetection-0.4.5/celldetection/models/resnet.py` & `celldetection-0.4.8/celldetection/models/resnet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import torch
 from torch import nn
 from torch.nn import functional as F
 from torchvision.models import resnet as tvr
-from ..util.util import Dict, lookup_nn, get_nd_conv
+from os.path import isfile
+from ..util.util import Dict, lookup_nn, get_nd_conv, get_nn, resolve_pretrained
 from torch.hub import load_state_dict_from_url
 from .ppm import append_pyramid_pooling_
 from typing import Type, Union, Optional
+from pytorch_lightning.core.mixins import HyperparametersMixin
 
 __all__ = ['get_resnet', 'ResNet50', 'ResNet34', 'ResNet18', 'ResNet152', 'ResNet101', 'WideResNet101_2',
            'WideResNet50_2', 'ResNeXt152_32x8d', 'ResNeXt101_32x8d', 'ResNeXt50_32x4d']
 
 default_model_urls = {
     'ResNet18': 'https://download.pytorch.org/models/resnet18-f37072fd.pth',  # IMAGENET1K_V1
     'ResNet34': 'https://download.pytorch.org/models/resnet34-b627a593.pth',  # IMAGENET1K_V1
@@ -18,23 +21,31 @@
     'ResNeXt50_32x4d': 'https://download.pytorch.org/models/resnext50_32x4d-1a0047aa.pth',  # IMAGENET1K_V2
     'ResNeXt101_32x8d': 'https://download.pytorch.org/models/resnext101_32x8d-8ba56ff5.pth',  # IMAGENET1K_V2
     'WideResNet50_2': 'https://download.pytorch.org/models/wide_resnet50_2-9ba9bcbe.pth',  # IMAGENET1K_V2
     'WideResNet101_2': 'https://download.pytorch.org/models/wide_resnet101_2-d733dc28.pth',  # IMAGENET1K_V2
 }
 
 
-def conv3x3(in_planes: int, out_planes: int, stride: int = 1, groups: int = 1, dilation: int = 1,
+def conv3x3(in_planes: int, out_planes: int, stride: int = 1, groups: int = 1, dilation: int = 1, kernel_size=3,
             nd=2) -> nn.Conv2d:
     """3x3 convolution with padding"""
+    if isinstance(kernel_size, int):
+        kernel_size = (kernel_size,) * nd
+    if isinstance(dilation, int):
+        dilation = (dilation,) * nd
+
+    # Calculate padding for 'same' padding
+    padding = tuple((ks - 1) * dil // 2 for ks, dil in zip(kernel_size, dilation))
+
     return get_nd_conv(nd)(
         in_planes,
         out_planes,
-        kernel_size=3,
+        kernel_size=kernel_size,
         stride=stride,
-        padding=dilation,
+        padding=padding,
         groups=groups,
         bias=False,
         dilation=dilation,
     )
 
 
 def conv1x1(in_planes: int, out_planes: int, stride: int = 1, nd=2) -> nn.Conv2d:
@@ -52,23 +63,24 @@
             planes: int,
             stride: int = 1,
             downsample: Optional[nn.Module] = None,
             groups: int = 1,
             base_width: int = 64,
             dilation: int = 1,
             norm_layer='batchnorm2d',
+            kernel_size=3,
             nd=2
     ) -> None:
         super().__init__()
         norm_layer = lookup_nn(norm_layer, call=False, nd=nd)
         if groups != 1 or base_width != 64:
             raise ValueError("BasicBlock only supports groups=1 and base_width=64")
         if dilation > 1:
             raise NotImplementedError("Dilation > 1 not supported in BasicBlock")
-        self.conv1 = conv3x3(inplanes, planes, stride, nd=nd)
+        self.conv1 = conv3x3(inplanes, planes, stride, nd=nd, kernel_size=kernel_size)
         self.bn1 = norm_layer(planes)
         self.relu = nn.ReLU(inplace=True)
         self.conv2 = conv3x3(planes, planes, nd=nd)
         self.bn2 = norm_layer(planes)
         self.downsample = downsample
         self.stride = stride
 
@@ -83,22 +95,23 @@
             planes: int,
             stride: int = 1,
             downsample: Optional[nn.Module] = None,
             groups: int = 1,
             base_width: int = 64,
             dilation: int = 1,
             norm_layer='batchnorm2d',
+            kernel_size=3,
             nd=2
     ) -> None:
         super().__init__()
         norm_layer = lookup_nn(norm_layer, call=False, nd=nd)
         width = int(planes * (base_width / 64.0)) * groups
         self.conv1 = conv1x1(inplanes, width, nd=nd)
         self.bn1 = norm_layer(width)
-        self.conv2 = conv3x3(width, width, stride, groups, dilation, nd=nd)
+        self.conv2 = conv3x3(width, width, stride, groups, dilation, kernel_size=kernel_size, nd=nd)
         self.bn2 = norm_layer(width)
         self.conv3 = conv1x1(width, planes * self.expansion, nd=nd)
         self.bn3 = norm_layer(planes * self.expansion)
         self.relu = nn.ReLU(inplace=True)
         self.downsample = downsample
         self.stride = stride
 
@@ -106,70 +119,115 @@
 def _make_layer(  # Port from torchvision (to support 3d)
         self,
         block: Type[Union[BasicBlock, Bottleneck]],
         planes: int,
         blocks: int,
         stride: int = 1,
         dilate: bool = False,
+        kernel_size: int = 3,
         nd=2,
+        secondary_block=None,
+        downsample_method=None,
 ) -> nn.Sequential:
+    """
+
+    References:
+        - [1] https://arxiv.org/abs/1812.01187.pdf
+
+    Args:
+        self:
+        block:
+        planes:
+        blocks:
+        stride:
+        dilate:
+        kernel_size:
+        nd:
+        secondary_block:
+        downsample_method: Downsample method. None: 1x1Conv with stride, Norm (standard ResNet),
+            'avg': AvgPool, 1x1Conv, Norm (ResNet-D in [1])
+
+    Returns:
+
+    """
+    if secondary_block is not None:
+        secondary_block = get_nn(secondary_block, nd=nd)
     norm_layer = self._norm_layer
     downsample = None
     previous_dilation = self.dilation
     if dilate:
         self.dilation *= stride
         stride = 1
     if stride != 1 or self.inplanes != planes * block.expansion:
-        downsample = nn.Sequential(
-            conv1x1(self.inplanes, planes * block.expansion, stride, nd=nd),
-            norm_layer(planes * block.expansion),
-        )
+        if downsample_method is None or stride <= 1:
+            downsample = nn.Sequential(
+                conv1x1(self.inplanes, planes * block.expansion, stride, nd=nd),
+                norm_layer(planes * block.expansion),
+            )
+        elif downsample_method == 'avg':
+            downsample = nn.Sequential(
+                get_nn(nn.AvgPool2d, nd=nd)(2, stride=stride),
+                conv1x1(self.inplanes, planes * block.expansion, nd=nd),
+                norm_layer(planes * block.expansion),
+            )
+        else:
+            raise ValueError(f'Unknown downsample_method: {downsample_method}')
 
     layers = []
     layers.append(
         block(self.inplanes, planes, stride, downsample, self.groups, self.base_width, previous_dilation, norm_layer,
-              nd=nd))
+              kernel_size=kernel_size, nd=nd))
     self.inplanes = planes * block.expansion
     for _ in range(1, blocks):
         layers.append(block(
             self.inplanes,
             planes,
             groups=self.groups,
             base_width=self.base_width,
             dilation=self.dilation,
             norm_layer=norm_layer,
+            kernel_size=kernel_size,
             nd=nd,
         ))
+    if secondary_block is not None:
+        layers.append(secondary_block(self.inplanes, nd=nd))  # must be preconfigured and not change channels
     return nn.Sequential(*layers)
 
 
 def make_res_layer(block, inplanes, planes, blocks, norm_layer=nn.BatchNorm2d, base_width=64, groups=1, stride=1,
-                   dilation=1, dilate=False, nd=2, **kwargs) -> nn.Module:
+                   dilation=1, dilate=False, nd=2, secondary_block=None, downsample_method=None, kernel_size=3,
+                   **kwargs) -> nn.Module:
     """
 
     Args:
         block: Module class. For example `BasicBlock` or `Bottleneck`.
         inplanes: Number of in planes
         planes: Number of planes
         blocks: Number of blocks
         norm_layer: Norm Module class
         base_width: Base width. Acts as a factor of the bottleneck size of the Bottleneck block and is used with groups.
         groups:
         stride:
         dilation:
         dilate:
+        nd:
+        secondary_block:
+        downsample_method:
+        kernel_size:
+        kwargs:
 
     Returns:
 
     """
     norm_layer = lookup_nn(norm_layer, nd=nd, call=False)
     d = Dict(inplanes=inplanes, _norm_layer=norm_layer, base_width=base_width,
              groups=groups, dilation=dilation)  # almost a ResNet
 
-    return _make_layer(self=d, block=block, planes=planes, blocks=blocks, stride=stride, dilate=dilate, nd=nd)
+    return _make_layer(self=d, block=block, planes=planes, blocks=blocks, stride=stride, dilate=dilate, nd=nd,
+                       secondary_block=secondary_block, downsample_method=downsample_method, kernel_size=kernel_size)
 
 
 def _apply_mapping_rules(key, rules: dict):
     for prefix, repl in rules.items():
         if key.startswith(prefix):
             key = key.replace(prefix, repl, 1)
     return key
@@ -200,15 +258,15 @@
         else:
             rules = {'conv1.': '0.0.', 'bn1.': '0.1.', 'layer1.': '1.1.', 'layer2.': '2.', 'layer3.': '3.',
                      'layer4.': '4.', 'layer5.': '5.'}
         mapping[_apply_mapping_rules(k, rules)] = v
     return mapping
 
 
-class ResNet(nn.Sequential):
+class ResNet(nn.Sequential, HyperparametersMixin):
     def __init__(self, in_channels, *body: nn.Module, initial_strides=2, base_channel=64, initial_pooling=True,
                  final_layer=None, final_activation=None, fused_initial=True, pretrained=False,
                  pyramid_pooling=False, pyramid_pooling_channels=64, pyramid_pooling_kwargs=None, nd=2, **kwargs):
         assert len(body) > 0
         body = list(body)
         Conv = get_nd_conv(nd)
         Norm = lookup_nn(nn.BatchNorm2d, nd=nd, call=False)
@@ -227,40 +285,45 @@
         components = [initial] + list(body[1:] if fused_initial else body)
         if final_layer is not None:
             components += [final_layer]
         if final_activation is not None:
             components += [lookup_nn(final_activation)]
         super(ResNet, self).__init__(*components)
         if pretrained:
-            if isinstance(pretrained, str):
-                state_dict = load_state_dict_from_url(pretrained)
-                if '.pytorch.org' in pretrained:
-                    state_dict = map_state_dict(in_channels, state_dict, fused_initial=fused_initial)
-                self.load_state_dict(state_dict)
-            else:
-                raise ValueError('There is no default set of weights for this model. '
-                                 'Please specify a URL using the `pretrained` argument.')
+            state_dict = resolve_pretrained(pretrained, in_channels=in_channels, fused_initial=fused_initial,
+                                            state_dict_mapper=map_state_dict)
+            self.load_state_dict(state_dict, strict=kwargs.get('pretrained_strict', True))
         if pyramid_pooling:
             pyramid_pooling_kwargs = {} if pyramid_pooling_kwargs is None else pyramid_pooling_kwargs
-            append_pyramid_pooling_(self, pyramid_pooling_channels, **pyramid_pooling_kwargs)
+            append_pyramid_pooling_(self, pyramid_pooling_channels, nd=nd, **pyramid_pooling_kwargs)
 
 
 class VanillaResNet(ResNet):
-    def __init__(self, in_channels, out_channels=0, layers=(2, 2, 2, 2), base_channel=64, fused_initial=True, nd=2,
-                 **kwargs):
+    def __init__(self, in_channels, out_channels=0, layers=(2, 2, 2, 2), base_channel=64, fused_initial=True,
+                 kernel_size=3, per_layer_kernel_sizes: dict = None, nd=2, **kwargs):
+        if per_layer_kernel_sizes is None:
+            per_layer_kernel_sizes = {}
+        if isinstance(per_layer_kernel_sizes, (tuple, list)):
+            per_layer_kernel_sizes = {i: v for i, v in enumerate(per_layer_kernel_sizes)}
+        self.save_hyperparameters()
         self.out_channels = oc = (base_channel, base_channel * 2, base_channel * 4, base_channel * 8)
         self.out_strides = (4, 8, 16, 32)
         if out_channels and 'final_layer' not in kwargs.keys():
             kwargs['final_layer'] = get_nd_conv(nd)(self.out_channels[-1], out_channels, 1)
+
         super(VanillaResNet, self).__init__(
             in_channels,
-            make_res_layer(BasicBlock, base_channel, oc[0], layers[0], stride=1, nd=nd, **kwargs),
-            make_res_layer(BasicBlock, oc[0], oc[1], layers[1], stride=2, nd=nd, **kwargs),
-            make_res_layer(BasicBlock, oc[1], oc[2], layers[2], stride=2, nd=nd, **kwargs),
-            make_res_layer(BasicBlock, oc[2], oc[3], layers[3], stride=2, nd=nd, **kwargs),
+            make_res_layer(BasicBlock, base_channel, oc[0], layers[0], stride=1, nd=nd,
+                           kernel_size=per_layer_kernel_sizes.get(0, kernel_size), **kwargs),
+            make_res_layer(BasicBlock, oc[0], oc[1], layers[1], stride=2, nd=nd,
+                           kernel_size=per_layer_kernel_sizes.get(1, kernel_size), **kwargs),
+            make_res_layer(BasicBlock, oc[1], oc[2], layers[2], stride=2, nd=nd,
+                           kernel_size=per_layer_kernel_sizes.get(2, kernel_size), **kwargs),
+            make_res_layer(BasicBlock, oc[2], oc[3], layers[3], stride=2, nd=nd,
+                           kernel_size=per_layer_kernel_sizes.get(3, kernel_size), **kwargs),
             base_channel=base_channel, fused_initial=fused_initial, nd=nd, **kwargs
         )
         if not fused_initial:
             self.out_channels = (base_channel,) + self.out_channels
             self.out_strides = (2,) + self.out_strides
 
 
@@ -279,121 +342,150 @@
                 Alternatively, ``pretrained`` can be a URL of a ``state_dict`` that is hosted online.
             **kwargs: Additional keyword arguments.
         """
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ResNet18']
         super(ResNet18, self).__init__(in_channels, out_channels=out_channels, layers=(2, 2, 2, 2),
                                        pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
 
 class ResNet34(VanillaResNet):
     def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ResNet34']
         super(ResNet34, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 6, 3),
                                        pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNet 34')
 
 
 class BottleResNet(ResNet):
-    def __init__(self, in_channels, out_channels=0, layers=(3, 4, 6, 3), base_channel=64, fused_initial=True, nd=2,
-                 **kwargs):
+    def __init__(self, in_channels, out_channels=0, layers=(3, 4, 6, 3), base_channel=64, fused_initial=True,
+                 kernel_size=3, per_layer_kernel_sizes: dict = None, nd=2, **kwargs):
+        if per_layer_kernel_sizes is None:
+            per_layer_kernel_sizes = {}
+        if isinstance(per_layer_kernel_sizes, (tuple, list)):
+            per_layer_kernel_sizes = {i: v for i, v in enumerate(per_layer_kernel_sizes)}
+        self.save_hyperparameters()
         ex = Bottleneck.expansion
         self.out_channels = oc = (base_channel * 4, base_channel * 8, base_channel * 16, base_channel * 32)
         self.out_strides = (4, 8, 16, 32)
         if out_channels and 'final_layer' not in kwargs.keys():
             kwargs['final_layer'] = nn.Conv2d(self.out_channels[-1], out_channels, 1)
         super(BottleResNet, self).__init__(
             in_channels,
-            make_res_layer(Bottleneck, base_channel, oc[0] // ex, layers[0], stride=1, nd=nd, **kwargs),
-            make_res_layer(Bottleneck, base_channel * 4, oc[1] // ex, layers[1], stride=2, nd=nd, **kwargs),
-            make_res_layer(Bottleneck, base_channel * 8, oc[2] // ex, layers[2], stride=2, nd=nd, **kwargs),
-            make_res_layer(Bottleneck, base_channel * 16, oc[3] // ex, layers[3], stride=2, nd=nd, **kwargs),
+            make_res_layer(Bottleneck, base_channel, oc[0] // ex, layers[0], stride=1, nd=nd,
+                           kernel_size=per_layer_kernel_sizes.get(0, kernel_size), **kwargs),
+            make_res_layer(Bottleneck, base_channel * 4, oc[1] // ex, layers[1], stride=2, nd=nd,
+                           kernel_size=per_layer_kernel_sizes.get(1, kernel_size), **kwargs),
+            make_res_layer(Bottleneck, base_channel * 8, oc[2] // ex, layers[2], stride=2, nd=nd,
+                           kernel_size=per_layer_kernel_sizes.get(2, kernel_size), **kwargs),
+            make_res_layer(Bottleneck, base_channel * 16, oc[3] // ex, layers[3], stride=2, nd=nd,
+                           kernel_size=per_layer_kernel_sizes.get(3, kernel_size), **kwargs),
             base_channel=base_channel, fused_initial=fused_initial, nd=nd, **kwargs
         )
         if not fused_initial:
             self.out_channels = (base_channel,) + self.out_channels
             self.out_strides = (2,) + self.out_strides
 
 
 class ResNet50(BottleResNet):
     def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ResNet50']
         super(ResNet50, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 6, 3),
                                        pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNet 50')
 
 
 class ResNet101(BottleResNet):
     def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ResNet101']
         super(ResNet101, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 23, 3),
                                         pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNet 101')
 
 
 class ResNet152(BottleResNet):
     def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ResNet152']
         super(ResNet152, self).__init__(in_channels, out_channels=out_channels, layers=(3, 8, 36, 3),
                                         pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNet 152')
 
 
 class ResNeXt50_32x4d(BottleResNet):
     def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ResNeXt50_32x4d']
         super(ResNeXt50_32x4d, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 6, 3), groups=32,
                                               base_width=4, pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNeXt 50')
 
 
 class ResNeXt101_32x8d(BottleResNet):
     def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['ResNeXt101_32x8d']
         super(ResNeXt101_32x8d, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 23, 3), groups=32,
                                                base_width=8, pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNeXt 101')
 
 
 class ResNeXt152_32x8d(BottleResNet):
     def __init__(self, in_channels, out_channels=0, nd=2, **kwargs):
         super(ResNeXt152_32x8d, self).__init__(in_channels, out_channels=out_channels, layers=(3, 8, 36, 3), groups=32,
                                                base_width=8, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNeXt 152')
 
 
 class WideResNet50_2(BottleResNet):
     def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['WideResNet50_2']
         super(WideResNet50_2, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 6, 3),
                                              base_width=64 * 2, pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'Wide ResNet 50')
 
 
 class WideResNet101_2(BottleResNet):
     def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
         if pretrained is True and nd == 2:
             pretrained = default_model_urls['WideResNet101_2']
         super(WideResNet101_2, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 23, 3),
                                               base_width=64 * 2, pretrained=pretrained, nd=nd, **kwargs)
+        self.hparams.clear()
+        self.save_hyperparameters()
 
     __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'Wide ResNet 101')
 
 
 models_by_name = {
     'resnet18': ResNet18,
     'resnet34': ResNet34,
```

### Comparing `CellDetection-0.4.5/celldetection/models/smp.py` & `celldetection-0.4.8/celldetection/models/smp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import segmentation_models_pytorch as smp
 from torch import nn
 from collections import OrderedDict
 from typing import List, Callable
+from pytorch_lightning.core.mixins import HyperparametersMixin
 
 __all__ = ['SmpEncoder']
 
 
 class ExternBase(nn.Module):
     def __init__(self, model_name: str):
         super().__init__()
@@ -22,15 +23,15 @@
                                       ] + model_list_callback())
             raise ValueError(msg)
 
     def _get_name(self):
         return self.model_name.title()
 
 
-class SmpEncoder(ExternBase):
+class SmpEncoder(ExternBase, HyperparametersMixin):
     def __init__(self, model_name: str, in_channels: int = 3, depth: int = 5, pretrained=False,
                  output_stride: int = 32, **kwargs):
         """Smp Encoder.
 
         A wrapper that provides compatibility with "segmentation_models_pytorch (smp)".
 
         References:
@@ -44,14 +45,15 @@
             depth: Encoder dpeth.
             pretrained: Encoder weights. Find available weights here: https://smp.readthedocs.io/en/latest/encoders.html
             output_stride: Output stride.
             **kwargs:
         """
         self.check_model_name(model_name, smp.encoders.get_encoder_names)
         super().__init__(model_name)
+        self.save_hyperparameters()
 
         # Map pretrained for consistency
         if pretrained is True:
             pretrained = 'imagenet'  # best guess
         elif pretrained is False:
             pretrained = None
         if 'weights' in kwargs:
```

### Comparing `CellDetection-0.4.5/celldetection/models/timmodels.py` & `celldetection-0.4.8/celldetection/models/timmodels.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/models/unet.py` & `celldetection-0.4.8/celldetection/models/unet.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
             interpolate='nearest',
             final_interpolate=None,
             initialize=True,
             keep_features=True,
             bridge_strides=True,
             bridge_block_cls: 'nn.Module' = None,
             bridge_block_kwargs: dict = None,
+            secondary_block: 'nn.Module' = None,
             in_strides_list: Union[List[int], Tuple[int]] = None,
             out_channels_list: Union[List[int], Tuple[int]] = None,
             nd=2,
             **kwargs
     ):
         super().__init__([], 0, extra_blocks=kwargs.get('extra_blocks'))
         block_kwargs = {} if block_kwargs is None else block_kwargs
@@ -144,15 +145,18 @@
                     cls, kw = bridge_block_cls, bridge_block_kwargs
                     inp = inc,
                 elif self.block_cat:  # block_cls handles merging
                     inp = inc, lat
                 else:  # normal cat
                     self.apply_cat[i] = True
                     inp = inc + lat,
-                self.layer_blocks.append(cls(*inp, ouc, nd=nd, **kw))
+                layer_block = cls(*inp, ouc, nd=nd, **kw)
+                if secondary_block is not None:  # must be preconfigured and not change channels
+                    layer_block = nn.Sequential(layer_block, secondary_block(ouc, nd=nd))
+                self.layer_blocks.append(layer_block)
 
         self.depth = len(self.layer_blocks)
         self.interpolate = interpolate
 
         self.keep_features = keep_features
         self.features_prefix = 'encoder'
         self.out_layer = Conv(out_channels_list[0], out_channels, 1) if out_channels > 0 else None
@@ -254,17 +258,20 @@
             ilg = isinstance(backbone, nn.Sequential)
         if block is None:
             block = TwoConvNormRelu  # it's called with nd
         else:
             block = get_nn(block, nd=nd)
         self.nd = nd
         pretrained_cfg = backbone.__dict__.get('pretrained_cfg', {})
-        self.normalize = Normalize(mean=kwargs.get('inputs_mean', pretrained_cfg.get('mean', 0.)),
-                                   std=kwargs.get('inputs_std', pretrained_cfg.get('std', 1.)),
-                                   assert_range=kwargs.get('assert_range', (0., 1.)))
+        if kwargs.pop('normalize', True):
+            self.normalize = Normalize(mean=kwargs.get('inputs_mean', pretrained_cfg.get('mean', 0.)),
+                                       std=kwargs.get('inputs_std', pretrained_cfg.get('std', 1.)),
+                                       assert_range=kwargs.get('assert_range', (0., 1.)))
+        else:
+            self.normalize = None
         self.body = IntermediateLayerGetter(backbone, return_layers=return_layers) if ilg else backbone
 
         self.intermediate_blocks = kwargs.get('intermediate_blocks')
         if self.intermediate_blocks is not None:
             in_channels_list = in_channels_list + type(in_channels_list)(self.intermediate_blocks.out_channels)
             if in_strides_list is not None:
                 in_strides_list = in_strides_list + type(in_strides_list)(
@@ -283,15 +290,17 @@
             **kwargs
         )
         self.out_channels = list(self.unet.out_channels_list)  # list(in_channels_list)
         # self.out_strides = kwargs.get('in_stride_list')
         self.nd = nd
 
     def forward(self, inputs):
-        x = self.normalize(inputs)
+        x = inputs
+        if self.normalize is not None:
+            x = self.normalize(x)
         x = self.body(x)
         if self.intermediate_blocks is not None:
             x = self.intermediate_blocks(x)
         x = self.unet(x, size=inputs.shape[-self.nd:])
         return x
```

### Comparing `CellDetection-0.4.5/celldetection/mpi/mpi.py` & `celldetection-0.4.8/celldetection/mpi/mpi.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,41 +81,56 @@
     ANY_SOURCE = MPI.ANY_SOURCE
 except (ModuleNotFoundError, ImportError) as e:
     _ERR = e
     MPI = False
     ANY_TAG = -1
     ANY_SOURCE = -2  # may differ depending on MPI implementation
 
-__all__ = ['recv', 'send', 'sink', 'query', 'serve', 'all_filter', 'get_local_comm', 'get_hosts', 'get_comm']
+__all__ = ['recv', 'send', 'sink', 'query', 'serve', 'all_filter', 'get_local_comm', 'get_hosts', 'get_comm', 'has_mpi',
+           'get_num_nodes']
 
 
 def assert_mpi(func):
     def func_wrapper(*a, **k):
         if not MPI:
             raise ModuleNotFoundError(
                 f'In order to use mpi functions, MPI must be installed. Could not import mpi4py.\n\n'
                 f'Check out: https://mpi4py.readthedocs.io/en/stable/install.html\n\n{str(_ERR)}')
         return func(*a, **k)
 
     func_wrapper.__doc__ = func.__doc__
     return func_wrapper
 
 
+def has_mpi(check_initialized=True):
+    v = bool(MPI)
+    if v and check_initialized:
+        return v and MPI.Is_initialized()
+    return v
+
+
 @assert_mpi
 def get_hosts(comm, return_ranks=False):
     host = MPI.Get_processor_name()
     hosts = list(np.sort(np.unique(comm.allgather(host))))
     res = host, hosts
     if return_ranks:
         node_rank = next(i for i, h in enumerate(hosts) if h == host)
         node_ranks = len(list(hosts))
         res += (node_rank, node_ranks)
     return res
 
 
+@assert_mpi
+def get_num_nodes():
+    comm = MPI.COMM_WORLD
+    host, hosts, node_rank, node_ranks = get_hosts(comm, return_ranks=True)
+    return node_ranks
+
+
 if MPI:
     @assert_mpi
     def get_comm(comm=None, return_ranks=True):
         comm = comm or MPI.COMM_WORLD
         res = comm,
         if return_ranks:
             rank = comm.Get_rank()
```

### Comparing `CellDetection-0.4.5/celldetection/ops/boxes.py` & `celldetection-0.4.8/celldetection/ops/boxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from os import name
 
 WINDOWS = name == 'nt'
 
 __all__ = ['nms', 'contours2boxes', 'pairwise_box_iou', 'pairwise_generalized_box_iou', 'filter_by_box_voting']
 
 
-def no_decorator(*args, **kwargs):
+def torch_compile(*args, **kwargs):
     def decorator(func):
-        return func
+        if WINDOWS:
+            return func  # compile not supported on Windows, yet
+        else:
+            return torch.compile(func, *args, **kwargs)
 
     return decorator
 
 
-torch_compile = (no_decorator if WINDOWS else torch.compile)  # TODO: Remove when torch.compile is supports on Windows
-
-
 @torch_compile(dynamic=True)
 def nms(boxes, scores, thresh=.5) -> torch.Tensor:
     """Non-maximum suppression.
 
     Perform non-maximum suppression (NMS) on the boxes according to their intersection-over-union (IoU).
 
     Notes:
```

### Comparing `CellDetection-0.4.5/celldetection/ops/commons.py` & `celldetection-0.4.8/celldetection/ops/commons.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,55 @@
 import torch
 from torch import Tensor
 import torch.nn.functional as F
 from typing import List
 
 __all__ = ['downsample_labels', 'padded_stack2d', 'split_spatially', 'minibatch_std_layer', 'strided_upsampling2d',
-           'interpolate_vector', 'pad_to_div', 'pad_to_size']
+           'interpolate_vector', 'pad_to_div', 'pad_to_size', 'spatial_mean', 'process_scores', 'equal_size']
+
+
+def equal_size(x, reference, mode='bilinear', align_corners=False):
+    if reference.shape[2:] != x.shape[2:]:  # 337 ns
+        # bilinear: 3.79 ms for (128, 128) to (512, 512)
+        # bicubic: 11.5 ms for (128, 128) to (512, 512)
+        x = F.interpolate(x, reference.shape[2:],
+                          mode=mode, align_corners=align_corners)
+    return x
+
+
+def _apply_score_bounds(scores, scores_lower_bound, scores_upper_bound):
+    if scores_upper_bound is not None:
+        assert scores_upper_bound.ndim >= 4, (f'Please make sure scores_upper_bound comes in NCHW format: '
+                                              f'{scores_upper_bound.shape}')
+        assert scores_upper_bound.dtype.is_floating_point, (f'Please make sure to pass scores_upper_bound as float '
+                                                            f'instead of {scores_upper_bound.dtype}')
+        scores = torch.minimum(scores, equal_size(scores_upper_bound, scores))
+    if scores_lower_bound is not None:
+        assert scores_lower_bound.ndim >= 4, (f'Please make sure scores_upper_bound comes in NCHW format: '
+                                              f'{scores_lower_bound.shape}')
+        assert scores_lower_bound.dtype.is_floating_point, (f'Please make sure to pass scores_upper_bound as float '
+                                                            f'instead of {scores_lower_bound.dtype}')
+        scores = torch.maximum(scores, equal_size(scores_lower_bound, scores))
+    return scores
+
+
+def process_scores(scores, score_channels, score_thresh, scores_lower_bound, scores_upper_bound):
+    score_bounds = scores_lower_bound, scores_upper_bound
+    if score_channels == 1:
+        scores = _apply_score_bounds(torch.sigmoid(scores), *score_bounds)
+        classes = torch.squeeze((scores > score_thresh).long(), 1)
+    elif score_channels == 2:
+        scores = _apply_score_bounds(F.softmax(scores, dim=1)[:, 1:2], *score_bounds)
+        classes = torch.squeeze((scores > score_thresh).long(), 1)
+    elif score_channels > 2:
+        scores = _apply_score_bounds(F.softmax(scores, dim=1), *score_bounds)
+        classes = torch.argmax(scores, dim=1).long()
+    else:
+        raise ValueError
+    return scores, classes
 
 
 def downsample_labels(inputs, size: List[int]):
     """
 
     Down-sample via max-pooling and interpolation
 
@@ -183,7 +224,12 @@
     Returns:
         Padded Tensor.
     """
     if not isinstance(div, (tuple, list)):
         div = (div,) * nd
     size = [(i // d + bool(i % d)) * d for i, d in zip(v.shape[-len(div):], div)]
     return pad_to_size(v, size, return_pad=return_pad, **kwargs)
+
+
+def spatial_mean(x, keepdim=False):
+    spatial = tuple(range(2, x.ndim))
+    return torch.mean(x, spatial, keepdim=keepdim)
```

### Comparing `CellDetection-0.4.5/celldetection/ops/cpn.py` & `celldetection-0.4.8/celldetection/ops/cpn.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/ops/draw.py` & `celldetection-0.4.8/celldetection/ops/draw.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/ops/features.py` & `celldetection-0.4.8/celldetection/ops/features.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/ops/loss.py` & `celldetection-0.4.8/celldetection/ops/loss.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/ops/normalization.py` & `celldetection-0.4.8/celldetection/ops/normalization.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/util/timer.py` & `celldetection-0.4.8/celldetection/util/timer.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.4.5/celldetection/util/util.py` & `celldetection-0.4.8/celldetection/util/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import warnings
 import numpy as np
 import inspect
+import copy
 import torch
 import torch.nn as nn
 import torch.nn.init as init
 from typing import Union, List, Tuple, Any, Dict as TDict, Iterator, Type, Callable, Iterable, Sequence
 from torch import Tensor
 from torch.hub import load_state_dict_from_url
 import hashlib
@@ -14,31 +16,35 @@
 import pynvml as nv
 from cv2 import getGaussianKernel
 import h5py
 from collections import OrderedDict
 import re
 import sys
 from itertools import product
-from inspect import currentframe
+from inspect import currentframe, signature
 from shutil import copy2
 from PIL import Image
 from io import BytesIO
 from base64 import b64encode, b64decode
+from glob import glob
 
 __all__ = ['Dict', 'lookup_nn', 'reduce_loss_dict', 'tensor_to', 'to_device', 'asnumpy', 'fetch_model',
            'random_code_name', 'dict_hash', 'fetch_image', 'random_seed', 'tweak_module_', 'add_to_loss_dict',
            'random_code_name_dir', 'get_device', 'num_params', 'count_submodules', 'train_epoch', 'Bytes', 'Percent',
            'GpuStats', 'trainable_params', 'frozen_params', 'Tiling', 'load_image', 'gaussian_kernel',
            'iter_submodules', 'replace_module_', 'wrap_module_', 'spectral_norm_', 'to_h5', 'to_tiff',
            'to_json', 'from_json', 'exponential_moving_average_', 'weight_norm_', 'inject_extra_repr_',
            'ensure_num_tuple', 'get_nd_conv', 'get_nd_linear', 'get_nd_dropout', 'get_nd_max_pool', 'get_nd_batchnorm',
            'get_warmup_factor', 'print_to_file', 'NormProxy', 'num_bytes', 'from_h5', 'update_dict_',
            'get_tiling_slices', 'get_nn', 'copy_script', 'hash_file', 'append_hash_to_filename', 'save_fetchable_model',
            'load_model', 'freeze_', 'unfreeze_', 'freeze_submodules_', 'unfreeze_submodules_',
-           'image_to_base64', 'base64_to_image', 'model2dict', 'dict2model']
+           'image_to_base64', 'base64_to_image', 'model2dict', 'dict2model', 'is_ipython', 'grouped_glob',
+           'tweak_attribute_', 'to_batched_h5', 'compare_file_hashes', 'import_file', 'load_imagej_rois',
+           'glob_h5_split', 'say_goodbye', 'parse_url_params', 'save_requirements', 'get_installed_packages',
+           'resolve_model', 'is_package_installed', 'has_argument', 'dict_to_json_string', 'resolve_pretrained']
 
 
 def copy_script(dst, no_script_okay=True, frame=None, verbose=False):
     """Copy current script.
 
     Copies the script from where this function is called to ``dst``.
     By default, nothing happens if this function is not called from within a script.
@@ -197,28 +203,35 @@
     elif isinstance(item, nn.Module):
         return item
     elif isinstance(item, dict):
         assert len(item) == 1
         key, = item
         val = item[key]
         assert isinstance(val, dict)
-        v = lookup_nn(key, src=src, call=False, inplace=inplace, nd=nd)(**val)
+        cls = lookup_nn(key, src=src, call=False, inplace=inplace, nd=nd)
+        if issubclass(cls, nn.modules.loss._WeightedLoss):  # allows weight to be passed as lists (common use case)
+            if 'weight' in val and not isinstance(val['weight'], Tensor):
+                val['weight'] = torch.as_tensor(val['weight'])
+        v = cls(**val)
     elif isinstance(item, type) and nd is not None:
         v = replace_ndim(item, nd)
     else:
         v = item
     if call:
         kwargs = {'inplace': inplace} if 'inplace' in inspect.getfullargspec(v).args else {}
         kwargs.update(kw)
         v = v(*a, **kwargs)
     return v
 
 
-def get_nn(item: Union[str, 'nn.Module', Type['nn.Module']], src=None, nd=None):
-    return lookup_nn(item, src=src, nd=nd, call=False)
+def get_nn(item: Union[str, 'nn.Module', Type['nn.Module']], src=None, nd=None, call_if_type=False):
+    ret = lookup_nn(item, src=src, nd=nd, call=False)
+    if call_if_type and type(ret) is type:
+        ret = ret()
+    return ret
 
 
 class NormProxy:
     def __init__(self, norm, **kwargs):
         """Norm Proxy.
 
         Examples:
@@ -254,20 +267,22 @@
 
     def __repr__(self):
         return f'NormProxy({self.norm}, kwargs={self.kwargs})'
 
     __str__ = __repr__
 
 
-def reduce_loss_dict(losses: dict, divisor):
-    return sum((i for i in losses.values() if i is not None)) / divisor
+def reduce_loss_dict(losses: dict, divisor, ignore_prefix='_'):
+    return sum((i for k, i in losses.items() if (i is not None and not k.startswith(ignore_prefix)))) / divisor
 
 
 def add_to_loss_dict(d: dict, key: str, loss: torch.Tensor, weight=None):
-    dk = d[key]
+    if loss is None:
+        return
+    dk = d.get(key, None)
     torch.nan_to_num_(loss, 0., 0., 0.)
     if weight is not None:
         loss = loss * weight
     d[key] = loss if dk is None else dk + loss
 
 
 def tensor_to(inputs: Union[list, tuple, dict, Tensor], *args, **kwargs):
@@ -350,25 +365,34 @@
     else:
         raise ValueError(f'Type not supported: {type(v)}')
 
 
 def dict2model(conf, **kwargs):
     from .. import models
 
+    if len(conf) == 1:  # alternative format: {'class_name': kwargs}
+        key, = conf.keys()
+        if key != 'model':
+            m = getattr(models, key, None)
+            if m is not None:
+                return m(**conf[key])
+
+    # Format: {'model': class_name, 'kwargs': kwargs}
     kw = {**conf.get('kwargs', conf.get('kw', {})), **kwargs}
     m = getattr(models, conf['model'])(*conf.get('args', conf.get('a', ())), **kw)
     return m
 
 
-def _load_cd_format(m, **kwargs):
+def _load_cd_format(m, pretrained=True, **kwargs):
     assert isinstance(m, dict) and 'cd.models' in m.keys()
     state_dict = m['state_dict']
     conf = m['cd.models']
     m = dict2model(conf, **kwargs)
-    m.load_state_dict(state_dict)
+    if pretrained:
+        m.load_state_dict(state_dict, strict=kwargs.get('pretrained_strict', True))
     return m
 
 
 def load_model(filename, map_location=None, **kwargs):
     assert isfile(filename), f'Could not find file: {filename}'
     m = torch.load(filename, map_location=map_location, **kwargs.pop('load_kwargs', {}))
     if isinstance(m, dict) and 'cd.models' in m.keys():
@@ -400,22 +424,14 @@
     # url = name if name.startswith('http') else f'https://celldetection.org/torch/models/{name}.pt'
     m = load_state_dict_from_url(url, map_location=map_location, **load_state_dict_kwargs)
     if isinstance(m, dict) and 'cd.models' in m.keys():
         m = _load_cd_format(m, **kwargs)
     return m
 
 
-def hash_file(filename):
-    import hashlib
-
-    with open(filename, 'rb') as f:
-        sha256 = hashlib.sha256(f.read()).hexdigest()
-    return sha256
-
-
 def append_hash_to_filename(filename, num=None, ext=True):
     from os import rename
     prefix = filename
     postfix = ''
     if ext:
         sp = prefix.split('.')
         prefix = '.'.join(sp[:-1])
@@ -426,26 +442,29 @@
     dst = prefix + f'-{sha256}' + postfix
     rename(filename, dst)
 
 
 def model2dict(model: 'nn.Module'):
     return dict(
         model=model.__class__.__name__,
-        kwargs=model.hparams,
+        kwargs=dict(model.hparams),
     )
 
 
-def save_fetchable_model(model: 'nn.Module', filename, append_hash=16):
+def save_fetchable_model(model: 'nn.Module', filename, append_hash=16, **kwargs):
+    from ..__meta__ import __version__
     if not len(splitext(filename)[1]):
         filename += '.pt'
     model.eval()
     model = model.to('cpu')
     torch.save({
+        'cd.__version__': __version__,
         'cd.models': model2dict(model),
         'state_dict': model.state_dict(),
+        **kwargs
     }, filename)
     if append_hash:
         if append_hash is True:
             append_hash = None
         append_hash_to_filename(filename, num=append_hash)
 
 
@@ -677,14 +696,35 @@
     for handle, key, mod in iter_submodules(module, class_or_tuple, recursive=recursive):
         for k, v in kwargs.items():
             if must_exist:
                 getattr(mod, k)
             setattr(mod, k, v)
 
 
+def tweak_attribute_(module: nn.Module, require_existence=True, **kwargs):
+    """Tweak attribute.
+
+    Allows to change attributes of a module.
+
+    Args:
+        module: Module.
+        **kwargs: Key value pairs. Keys specify the attribute (e.g. `submodule.attribute_name`) and value
+            the respective new value.
+
+    """
+    for k, v in kwargs.items():
+        x = module
+        sp = k.split('.')
+        for k_ in sp[:-1]:
+            x = getattr(x, k_)
+        if require_existence:
+            assert hasattr(x, sp[-1]), f'Could not find {sp[-1]} attribute in {x}.'
+        setattr(x, sp[-1], v)
+
+
 def replace_module_(module: nn.Module, class_or_tuple, substitute: Union[Type[nn.Module], nn.Module], recursive=True,
                     inherit_attr: Union[list, str, dict] = None, **kwargs):
     """Replace module.
 
     Replace all occurrences of `class_or_tuple` in `module` with `substitute`.
 
     Examples:
@@ -1004,39 +1044,88 @@
         except Exception:
             self.num = 0
         self.delimiter = delimiter
 
     def __len__(self):
         return self.num
 
+    @staticmethod
+    def _is_mig_enabled(h):
+        # https://docs.nvidia.com/deploy/nvml-api/group__nvmlMultiInstanceGPU.html#group__nvmlMultiInstanceGPU_1g1fa0acf9076404ef28c3c6976eb96f2b
+        try:
+            mode, pending_mode = nv.nvmlDeviceGetMigMode(h)
+            is_mig_enabled = mode == nv.NVML_DEVICE_MIG_ENABLE
+        except nv.NVMLError:  # if device doesn't support MIG mode
+            is_mig_enabled = False
+        return is_mig_enabled
+
+    @staticmethod
+    def _get_mig_info(h, idx):
+        # https://docs.nvidia.com/deploy/nvml-api/group__nvmlMultiInstanceGPU.html#group__nvmlMultiInstanceGPU_1g15e07cc6230a2d90c5bc85de85261ef7
+        mig_device_count = nv.nvmlDeviceGetMaxMigDeviceCount(h)
+        mig_infos = []
+        for i in range(mig_device_count):
+            try:
+                # Get MIG device handle for the given index under its parent NVML device
+                mig_h = nv.nvmlDeviceGetMigDeviceHandleByIndex(h, i)
+
+                # Per-instance information can be queried by using specific MIG device handles
+                mem = nv.nvmlDeviceGetMemoryInfo(mig_h)
+
+                # Utilization rates are not available for MIG devices
+                # https://docs.nvidia.com/deploy/nvml-api/group__nvmlDeviceQueries.html#group__nvmlDeviceQueries_1g540824faa6cef45500e0d1dc2f50b321
+
+                mig_infos.append((f'{idx}-{i}', {
+                    'free': Bytes(mem.free),
+                    'used': Bytes(mem.used)
+                }))
+            except nv.NVMLError as e:
+                warnings.warn(str(e))
+        return mig_infos
+
+    @staticmethod
+    def _get_nonmig_info(h, idx):
+        info = idx, None
+        try:
+            mem = nv.nvmlDeviceGetMemoryInfo(h)
+            uti = nv.nvmlDeviceGetUtilizationRates(h)
+            info = idx, dict(
+                free=Bytes(mem.free),
+                used=Bytes(mem.used),
+                util=Percent(uti.gpu)
+            )
+        except nv.NVMLError as e:
+            warnings.warn(str(e))
+        return info
+
     def __getitem__(self, item: int):
         if item >= len(self):
             raise IndexError
         h = nv.nvmlDeviceGetHandleByIndex(item)
         idx = nv.nvmlDeviceGetIndex(h)
-        mem = nv.nvmlDeviceGetMemoryInfo(h)
-        uti = nv.nvmlDeviceGetUtilizationRates(h)
-        return idx, dict(
-            free=Bytes(mem.free),
-            used=Bytes(mem.used),
-            util=Percent(uti.gpu)
-        )
+        return (self._get_mig_info if self._is_mig_enabled(h) else self._get_nonmig_info)(h, idx)
 
     def dict(self, byte_lvl=3, prefix='gpu'):
         d = {}
-        for i, stat in self:
-            for k, v in stat.items():
-                if isinstance(v, Bytes):
-                    v = np.round(float(v) / (2 ** (10 * byte_lvl)), 2)
-                d[f'{prefix}{i}-{k}'] = float(v)
+        for r in self:
+            for i, stat in (r if isinstance(r, list) else [r]):
+                if stat is not None:
+                    for k, v in stat.items():
+                        if isinstance(v, Bytes):
+                            v = np.round(float(v) / (2 ** (10 * byte_lvl)), 2)
+                        d[f'{prefix}{i}-{k}'] = float(v)
         return d
 
     def __str__(self):
-        deli = self.delimiter
-        return deli.join([f'gpu{i}({deli.join([f"{k}: {v}" for k, v in stat.items()])})' for i, stat in self])
+        s = []
+        for r in self:
+            for i, stat in (r if isinstance(r, list) else [r]):
+                if stat is not None:
+                    s.append(f'gpu{i}({self.delimiter.join([f"{k}: {v}" for k, v in stat.items()])})')
+        return self.delimiter.join(s)
 
     __repr__ = __str__
 
 
 class Tiling:
     def __init__(self, tile_size: tuple, context_shape: tuple, overlap=0):
         self.overlap = overlap
@@ -1121,58 +1210,125 @@
         slices.append(axis_slices), shape.append(len(starts)), overlaps.append(axis_overlaps)
     slices = product(*slices)
     if return_overlaps:
         return slices, product(*overlaps), shape
     return slices, shape
 
 
-def to_h5(filename, mode='w', chunks=None, compression=None, overwrite=False, create_dataset_kw: dict = None,
-          **kwargs):
+def to_h5(filename, mode='w', chunks=None, compression=None, overwrite=False, driver=None,
+          create_dataset_kw: dict = None, attributes: dict = None, **kwargs):
     """To hdf5 file.
 
     Write data to hdf5 file.
 
     Args:
         filename: File name.
         mode: Mode.
         chunks: Chunks setting for created datasets. Chunk shape, or True to enable auto-chunking.
+            Can be dictionary, if each dataset needs a different chunking.
+            Individual chunks can be integer. Then each dimension is chunked to that integer
+            or the dimension, whichever is smaller.
         compression: Compression setting for created datasets. Legal values are 'gzip', 'szip', 'lzf'. If an integer
             in range(10), this indicates gzip compression level. Otherwise, an integer indicates the number of a
             dynamically loaded compression filter.
-        overwrite: Whether to overwrite existing dataset.
+        overwrite: Whether to overwrite existing dataset. If False, attempt to replace the contents of the existing
+            dataset, without creating a new dataset.
+        driver: Hdf5 driver.
         create_dataset_kw: Additional keyword arguments for ``h5py.File().create_dataset``.
+        attributes: Attributes. Format: `dict(dataset_name=dict(attribute0=value0))`.
+            Note that only specific attributes are supported by h5py (e.g. not None).
         **kwargs: Data as ``{dataset_name: data}``.
-
     """
+    attributes = {} if attributes is None else attributes
     create_dataset_kw = {} if create_dataset_kw is None else create_dataset_kw
-    with h5py.File(filename, mode) as h:
+    with h5py.File(filename, mode, **({} if driver is None else dict(driver=driver))) as h:
         for k, v in kwargs.items():
+            chunks_ = chunks[k] if isinstance(chunks, dict) else chunks
+            if isinstance(chunks_, int) and v.ndim > 1:
+                chunks_ = tuple(np.minimum((256,) * v.ndim, v.shape))
             exists = k in h
             if overwrite and exists:
                 del h[k]
-            elif exists:
-                h[k][:] = v
+            if exists:
+                ds = h[k]
+                ds[:] = v
             else:
-                h.create_dataset(k, data=v, compression=compression, chunks=chunks, **create_dataset_kw)
+                ds = h.create_dataset(k, data=v, compression=compression, chunks=chunks_, **create_dataset_kw)
+            attrs = attributes.get(k)
+            if attrs:
+                assert isinstance(attrs, dict)
+                ds.attrs.update(attrs)
+
+
+def to_batched_h5(filename, index, batch_size=256, mode='a', chunks=None, compression=None, overwrite=False,
+                  driver=None, create_dataset_kw: dict = None, file_digits=6, item_digits=6, **kwargs):
+    """To batched hdf5 file.
+
+    Write data to batched hdf5 file.
+    When called for multiple data inputs (with different indices), this function creates possibly multiple hdf5 files,
+    each containing up to `batch_size` items.
+    Each call creates exactly one item (or item group).
+
+    Content is assigned to a `batch_id` and an `item_id`, based on `index` and `batch_size`.
+    The filename is changed from `filename.h5` to `filename_000001.h5`, to include the `batch_id`.
+    Dataset keys are changed from `key` to `key_000001`, to include the `item_id`.
+
+    Args:
+        filename: File name.
+        index: Batch index (int).
+        batch_size: Batch size (int).
+        mode: Mode.
+        chunks: Chunks setting for created datasets. Chunk shape, or True to enable auto-chunking.
+            Can be dictionary, if each dataset needs a different chunking.
+            Individual chunks can be integer. Then each dimension is chunked to that integer
+            or the dimension, whichever is smaller.
+        compression: Compression setting for created datasets. Legal values are 'gzip', 'szip', 'lzf'. If an integer
+            in range(10), this indicates gzip compression level. Otherwise, an integer indicates the number of a
+            dynamically loaded compression filter.
+        overwrite: Whether to overwrite existing dataset. If False, attempt to replace the contents of the existing
+            dataset, without creating a new dataset.
+        driver: Hdf5 driver.
+        create_dataset_kw: Additional keyword arguments for ``h5py.File().create_dataset``.
+        file_digits: Number of digits to display batch index.
+        item_digits: Number of digits to display item index.
+        **kwargs: Data as ``{dataset_name: data}``.
+
+    """
+    batch_id = index // batch_size
+    item_id = index % batch_size
+    pre, ext = splitext(filename)
+    if isinstance(chunks, dict):
+        chunks = {f'{k}_%0{item_digits}d' % item_id: v for k, v in chunks.items()}
+    to_h5(
+        filename=f'{pre}_%0{file_digits}d{ext}' % batch_id,
+        mode=mode,
+        chunks=chunks,
+        compression=compression,
+        overwrite=overwrite,
+        driver=driver,
+        create_dataset_kw=create_dataset_kw,
+        **{f'{k}_%0{item_digits}d' % item_id: v for k, v in kwargs.items()}
+    )
 
 
-def from_h5(filename, *keys, **keys_slices):
+def from_h5(filename, *keys, file_kwargs=None, **keys_slices):
     """From h5.
 
     Reads data from hdf5 file.
 
     Args:
         filename: Filename.
         *keys: Keys to read.
+        file_kwargs: File keyword arguments.
         **keys_slices: Keys with indices or slices. E.g. `from_h5('file.h5', 'key0', key=slice(0, 42))`.
 
     Returns:
         Data from hdf5 file. As tuple if multiple keys are provided.
     """
-    with h5py.File(filename, 'r') as h:
+    with h5py.File(filename, 'r', **(file_kwargs or {})) as h:
         if len(keys) == 0 and len(keys_slices) == 0:
             print('Available keys:', list(h.keys()), flush=True)
         res = tuple(h[k][:] for k in keys) + tuple(h[k][v] for k, v in keys_slices.items())
     if len(res) == 1:
         res, = res
     return res
 
@@ -1396,24 +1552,393 @@
     if len(names) == 1 and isinstance(names[0], (tuple, list)):
         names, = names
     for n in names:
         unfreeze_(module.get_submodule(n), recurse=recurse)
 
 
 def image_to_base64(img: 'np.ndarray', ext='png', as_url=True, url_template=None):
+    """Image to base64.
+
+    Converts image to base64 code.
+
+    Args:
+        img: Image as numpy array.
+        ext: Image format.
+        as_url: Whether to format result as URL.
+        url_template: Optional URL template containing `ext` and `code` placeholders.
+
+    Returns:
+        Base64 code.
+    """
     pi = Image.fromarray(img)
     buff = BytesIO()
     pi.save(buff, format='png')
     code = b64encode(buff.getvalue()).decode('utf-8')
     if as_url:
         if url_template is None:
             url_template = 'data:image/{ext};base64,{code}'
         return url_template.format(ext=ext, code=code)
     return code
 
 
 def base64_to_image(code, as_numpy=True):
+    """Base64 to image.
+
+    Converts base64 code to image.
+
+    Args:
+        code: Base 64 code.
+        as_numpy: Whether to convert results to numpy instead of `PIL.Image`.
+
+    Returns:
+        Image.
+    """
     base64_decoded = b64decode(code)
     img = Image.open(BytesIO(base64_decoded))
     if as_numpy:
         return np.array(img)
     return img
+
+
+def is_ipython() -> bool:
+    """Is IPython.
+
+    Checks whether function is called via IPython.
+
+    Returns:
+        True/False.
+    """
+    import builtins
+    return getattr(builtins, '__IPYTHON__', False)
+
+
+def grouped_glob(pathname, group_pattern, *, sort=True, keep_unmatched=True, sub_kwargs=None, substitute='', **kwargs):
+    """Grouped glob.
+
+    A glob helper that groups search results by `group_pattern`.
+
+    Args:
+        pathname: Glob pattern.
+        group_pattern: Group pattern for `re.sub`. Matches are substituted with `substitute` for each filename.
+            The resulting string is used as the group handle. All files with the same handle belong to the same group.
+        sort: Whether to sort results.
+        keep_unmatched: Whether to keep files that do not match the `group_pattern`.
+        sub_kwargs: Keyword arguments for `re.sub`.
+        substitute: Substitute for creation of the group handle (see `group_pattern`).
+        **kwargs: Keyword arguments for glob.
+
+    Returns:
+        Dictionary of glob results.
+    """
+    files = glob(pathname, **kwargs)
+    if sort:
+        files = sorted(files)
+
+    grouped = {}
+    for f in files:
+        try:
+            next(re.finditer(group_pattern, f))
+            key = re.sub(group_pattern, substitute, f, **({} if sub_kwargs is None else sub_kwargs))
+        except StopIteration:
+            if keep_unmatched:
+                key = f
+            else:
+                continue
+        grouped[key] = li = grouped.get(key, [])
+        li.append(f)
+    return grouped
+
+
+def hash_file(filename, method='sha256', buffer_size=8192) -> str:
+    """Hash file.
+
+    Computes a hash for the given file.
+
+    Args:
+        filename: Filename.
+        method: Hashing method.
+        buffer_size: Buffer size (file is hashed in chunks).
+
+    Returns:
+        Hash.
+    """
+    import hashlib
+
+    hasher = getattr(hashlib, method)()
+    with open(filename, 'rb') as file:
+        buffer = file.read(buffer_size)
+        while buffer:
+            hasher.update(buffer)
+            buffer = file.read(buffer_size)
+    return hasher.hexdigest()
+
+
+def compare_file_hashes(*filenames, method='sha256') -> bool:
+    """Compare file hashes.
+
+    Computes file hashes for provided files.
+    Returns True if all hashes are equal, False otherwise.
+
+    Args:
+        *filenames: Filenames.
+        method: Hashing method.
+
+    Returns:
+        True/False.
+    """
+    assert len(filenames)
+    if len(filenames) == 1:
+        return True
+    reference_hash = hash_file(filenames[0], method=method)
+    return all(hash_file(f, method=method) == reference_hash for f in filenames[1:])
+
+
+def import_file(filename):
+    """Import Python file.
+
+    Args:
+        filename: Python filename.
+
+    Returns:
+        Loaded module.
+    """
+    from os.path import abspath, basename
+    import importlib
+
+    filename = abspath(filename)
+    name = splitext(basename(filename))[0]
+    spec = importlib.util.spec_from_file_location(name, filename)
+    mod = importlib.util.module_from_spec(spec)
+    sys.modules[name] = mod
+    spec.loader.exec_module(mod)
+    return mod
+
+
+def load_imagej_rois(filename, *keys):
+    """Load ImageJ ROIs.
+
+    Args:
+        filename: Filename.
+        *keys: Specific keys to load from the ROIs.
+
+    Returns:
+        (boxes, contours) if no keys provided. (boxes, contours, meta) if keys provided.
+    """
+    try:
+        import roifile as rf
+    except ModuleNotFoundError as e:
+        print('Please install the `roifile` package to use this function: "pip install roifile" '
+              '(https://pypi.org/project/roifile/)')
+        raise e
+
+    rois = rf.ImagejRoi.fromfile(filename)
+    boxes = []
+    contours = []
+    meta = {k: [] for k in keys}
+    for r in rois:
+        y0, y1 = r.top, r.bottom
+        x0, x1 = r.left, r.right
+        contour = r.integer_coordinates + [x0, y0]
+        contours.append(contour)
+        boxes.append([x0, y0, x1, y1])
+
+    res = np.array(boxes), contours
+    if len(meta):
+        return res + (meta,)
+    return res
+
+
+def glob_h5_split(pathname, ext='-r.h5', **kwargs):
+    """Glob for split HDF5 files.
+
+    This is a helper function for finding split h5 files via glob.
+    Filenames are searched with appendix and returned without appendix, as this is what `h5py` expects.
+
+    Args:
+        pathname: Glob pattern.
+        ext: Split h5 appendix.
+        **kwargs: Keyword arguments for glob.
+
+    Returns:
+        Modified glob results. Each filename has its appendix (`ext`) removed.
+    """
+    return [f[:-len(ext)] for f in glob(pathname=pathname if pathname.endswith(ext) else pathname + ext, **kwargs)]
+
+
+def say_goodbye():
+    a = ('All done,Task complete,Script finalized,Operation successful,All set,Execution concluded,Work finished,Proces'
+         's ended,All clear,Routine complete,Job done,Sequence finalized,Task accomplished,Chores completed,Duty conclu'
+         'ded,Activity finished,Assignment completed,Undertaking achieved,Procedure closed,Milestone reached')
+    b = ('have a magnificent day,enjoy your splendid day,hope your day is extraordinary,have a delightful day,may your '
+         'day be as bright as your smile,wishing you a day full of joy,have an awesome day ahead,enjoy your amazing day'
+         ',hope your day is as fantastic as you,have a superb day,may your day be filled with happiness,wishing you a d'
+         'ay of peace and joy,have a wonderful adventure today,may your day be as productive as you are,have a day as w'
+         'onderful as your achievements')
+    print(', '.join((np.random.choice(i.split(',')) for i in (a, b))) + '!')
+
+
+def parse_url_params(url, sep='?', param_sep=';'):
+    """Parse url params.
+
+    Examples:
+        ```Python
+        cd.parse_url_params('file.py?a=42;b=43')
+        ('file.py', {'a': 42, 'b': 43))
+        ```
+
+    Args:
+        url: URL.
+        sep: Separator between URL and params.
+        param_sep: Separator between params.
+
+    Returns:
+        Tuple of URL and parameter dict.
+    """
+    ar = url.split(sep)
+    if len(ar) > 1:
+        url = sep.join(url.split(sep)[:-1])
+    ar = dict([(tuple(i.split('=')) if '=' in i else (i, True)) for i in ar[-1].split(param_sep)]) if len(
+        ar) > 1 else None
+    return url, ar
+
+
+def get_installed_packages(template='{name}=={version}'):
+    """Get installed packages.
+
+    Returns a list of all installed packages.
+
+    Returns:
+        List of installed packages.
+    """
+    import importlib.metadata
+
+    return [package for package in sorted([
+        template.format(name=dist.metadata['Name'], version=dist.version) for dist in importlib.metadata.distributions()
+    ])]
+
+
+def save_requirements(filename, **kwargs):
+    """Save requirements.
+
+    Writes all installed packages with specified versions to `filename`.
+
+    Args:
+        filename: Filename.
+        **kwargs: Additional keyword arguments for `cd.print_to_file`.
+    """
+    print_to_file('\n'.join(get_installed_packages()), filename=filename, **kwargs)
+
+
+def update_model_hparams_(obj, resolve=True, **kwargs):
+    assert hasattr(obj, '_set_hparams')
+    assert hasattr(obj, '_hparams_initial')
+    assert hasattr(obj, '_hparams')
+    changes = {}
+    for key, value in kwargs.items():
+        if isinstance(value, nn.Module):
+            if resolve:
+                value = model2dict(value)
+        changes[key] = value
+
+    if len(changes):
+        # Override hparams
+        obj._set_hparams(changes)
+        obj._hparams_initial = copy.deepcopy(obj._hparams)
+
+
+def resolve_model(value, src=None, map_location='cpu', check_hash=None, **kwargs) -> 'nn.Module':
+    """Resolve model.
+
+    Args:
+        value: Model description. Either `nn.Module`, `str` (URL (leading http), filename, hosted model name,
+            class name, or dict).
+        src: Class name source. (cd.models is default).
+        map_location: Map location for loaded models. (cpu is default).
+        check_hash: Whether to check hash. Only relevant for downloads. Hash must be postfix in filename.
+        **kwargs: Keyword arguments for respective handler.
+
+    Returns:
+        Module.
+    """
+    if isinstance(value, nn.Module):
+        return value
+    elif isinstance(value, str):
+        if src is None:
+            from .. import models as src
+
+        # Model name
+        if value in dir(src):
+            item = getattr(src, value)
+            assert issubclass(item, nn.Module), (f'Model variable must describe a torch.nn.Module, '
+                                                 f'but found {value, item}')
+            return item(**kwargs)
+
+        # URL or hosted model
+        elif value.startswith('http') or value.startswith('cd://') or (not isfile(value) and not splitext(value)[1]):
+            if check_hash is None:
+                check_hash = value.startswith('cd://') or (not isfile(value) and not splitext(value)[1])
+            return fetch_model(value, map_location=map_location, check_hash=check_hash, **kwargs)
+
+        # Filename
+        elif isfile(value):
+            return load_model(value, map_location=map_location, **kwargs)
+    elif isinstance(value, dict):
+        return dict2model(value, **kwargs)
+    else:
+        raise ValueError(f'Could not handle type of `value`: {type(value)}')
+
+
+def resolve_pretrained(pretrained, state_dict_mapper=None, **kwargs):
+    if isinstance(pretrained, str):
+        if isfile(pretrained):
+            state_dict = torch.load(pretrained)
+        else:
+            state_dict = load_state_dict_from_url(pretrained)
+        if 'state_dict' in state_dict:
+            state_dict = state_dict['state_dict']
+        if '.pytorch.org' in pretrained:
+            if state_dict_mapper is not None:
+                state_dict = state_dict_mapper(state_dict=state_dict, **kwargs)
+    else:
+        raise ValueError('There is no default set of weights for this model. '
+                         'Please specify a URL or filename using the `pretrained` argument.')
+    return state_dict
+
+
+def is_package_installed(name) -> bool:
+    """Is package installed.
+
+    Checks if package called `name` is installed by attempting to retrieve its version via `importlib.metadata.version`.
+
+    Args:
+        name: Package name.
+
+    Returns:
+        Bool.
+    """
+    import importlib.metadata
+    try:
+        importlib.metadata.version(name)
+        return True
+    except importlib.metadata.PackageNotFoundError:
+        return False
+
+
+def has_argument(fn, *args, mode='any'):
+    sig = signature(fn)
+    gen = ((a in sig.parameters) for a in args)
+    if mode == 'any':
+        return any(gen)
+    elif mode == 'all':
+        return all(gen)
+    raise ValueError(f'Unknown mode: {mode}')
+
+
+def dict_to_json_string(input_dict):
+    serializable_dict = {}
+    for k, v in input_dict.items():
+        try:
+            json.dumps(v)
+            serializable_dict[k] = v
+        except TypeError:
+            pass  # skip
+    return json.dumps(serializable_dict)
```

### Comparing `CellDetection-0.4.5/celldetection/visualization/cmaps.py` & `celldetection-0.4.8/celldetection/visualization/cmaps.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,26 +13,27 @@
         np.random.randint(*saturation_range, num),
         np.random.randint(*value_range, num),
     ), 1).astype('uint8')[None], cv2.COLOR_HSV2RGB) / 255
     return colors
 
 
 def label_cmap(labels: ndarray, colors: Union[str, ndarray] = 'rand', zero_val: Union[float, tuple, list] = 0.,
-               rgba: bool = True, alpha: float = None):
+               rgba: bool = True, alpha: float = None, reduce_axis=2):
     """Label colormap.
 
     Applies a colormap to a label image.
 
     Args:
         labels: Label image. Typically Array[h, w].
         colors: Either 'rand' or one of ['Pastel1', 'Pastel2', 'Paired', 'Accent', 'Dark2', 'Set1', 'Set2', 'Set3',
             'tab10', 'tab20', 'tab20b', 'tab20c'] (see matplotlib's qualitative colormaps) or Array[n, c].
         zero_val: Special color for the zero label (usually background).
         rgba: Whether to add an alpha channel to rgb colors.
         alpha: Specific alpha value.
+        reduce_axis: Axis to be reduced with alpha compositing (e.g. channel axis).
 
     Returns:
         Mapped labels. E.g. rgba mapping Array[h, w] -> Array[h, w, 4].
     """
     assert issubclass(labels.dtype.type, np.integer), 'Pass labels as an integer array.'
     if isinstance(colors, str):
         if colors == 'rand':
@@ -46,8 +47,17 @@
     if alpha is not None and colors.shape[1] == 4:
         colors[:, -1] = alpha
     if zero_val is not None:
         labels = np.copy(labels)
         m = labels != 0
         labels[m] = labels[m] % len(colors) + 1
         colors = np.concatenate((np.ones_like(colors[:1]) * zero_val, colors))
-    return colors[labels]
+    res = colors[labels]
+
+    if reduce_axis and labels.ndim > 2:  # reduce label channels by alpha weighted average
+        weight = res[..., -1]
+        weight = weight / (weight.sum(reduce_axis, keepdims=True) + 1e-12)
+        if reduce_axis < 0:
+            reduce_axis = labels.ndim + reduce_axis
+        res = (weight[..., None] * res).sum(reduce_axis)
+
+    return res
```

### Comparing `CellDetection-0.4.5/setup.py` & `celldetection-0.4.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,27 @@
     version=m['__version__'],
     description=m['__summary__'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url=m['__url__'],
     packages=['celldetection', 'celldetection.data', 'celldetection.callbacks', 'celldetection.optim',
               'celldetection.data.datasets', 'celldetection.models', 'celldetection.mpi', 'celldetection.ops',
-              'celldetection.util', 'celldetection.visualization'],
+              'celldetection.util', 'celldetection.visualization', 'celldetection_scripts'],
     package_data={'': ['LICENSE', 'requirements.txt', 'README.md']},
     include_package_data=True,
     install_requires=requirements,
     license=m['__license__'],
     keywords=['cell', 'detection', 'object', 'segmentation', 'pytorch', 'cpn', 'contour', 'proposal', 'network', 'deep',
               'learning', 'unet', 'fzj', 'julich', 'juelich', 'ai'],
     classifiers=[
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
-    ]
+    ],
+    entry_points={
+        'console_scripts': [
+            'cd-inference-cpn=celldetection_scripts.cpn_inference:main',
+            # 'cd-train=celldetection_scripts.train:main'
+         ]
+    }
 )
```

