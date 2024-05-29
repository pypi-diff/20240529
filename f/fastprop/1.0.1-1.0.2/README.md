# Comparing `tmp/fastprop-1.0.1.tar.gz` & `tmp/fastprop-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastprop-1.0.1.tar", last modified: Sun Apr 28 02:16:26 2024, max compression
+gzip compressed data, was "fastprop-1.0.2.tar", last modified: Wed May 29 17:02:30 2024, max compression
```

## Comparing `fastprop-1.0.1.tar` & `fastprop-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-28 02:16:23.000000 fastprop-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13813 2024-04-28 02:16:26.712403 fastprop-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-04-28 02:16:23.000000 fastprop-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/fastprop/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/fastprop/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/shap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/cli/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    39676 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-04-28 02:16:23.000000 fastprop-1.0.1/fastprop/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/fastprop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13813 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 02:16:26.000000 fastprop-1.0.1/fastprop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-28 02:16:23.000000 fastprop-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:16:26.712403 fastprop-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:26.712403 fastprop-1.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-28 02:16:23.000000 fastprop-1.0.1/test/test_fastprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.194127 fastprop-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-29 17:02:26.000000 fastprop-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-29 17:02:30.194127 fastprop-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-29 17:02:26.000000 fastprop-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.190127 fastprop-1.0.2/fastprop/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.194127 fastprop-1.0.2/fastprop/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39676 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.194127 fastprop-1.0.2/fastprop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-29 17:02:26.000000 fastprop-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:02:30.194127 fastprop-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.194127 fastprop-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-29 17:02:26.000000 fastprop-1.0.2/test/test_fastprop.py
```

### Comparing `fastprop-1.0.1/LICENSE` & `fastprop-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.1/PKG-INFO` & `fastprop-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastprop
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fast Molecular Property Prediction with mordredcommunity
 Author: Jackson Burns
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,14 +12,17 @@
 Requires-Dist: pyyaml
 Requires-Dist: lightning
 Requires-Dist: torch>=1.13
 Requires-Dist: mordredcommunity
 Requires-Dist: astartes[molecules]
 Requires-Dist: tensorboard
 Requires-Dist: psutil
+Requires-Dist: polars
+Requires-Dist: pandas
+Requires-Dist: pyarrow
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: hopt
 Requires-Dist: ray[train]; extra == "hopt"
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: fastprop Version: 1.0.1 Summary: Fast Molecular
+Metadata-Version: 2.1 Name: fastprop Version: 1.0.2 Summary: Fast Molecular
 Property Prediction with mordredcommunity Author: Jackson Burns License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pyyaml Requires-Dist:
 lightning Requires-Dist: torch>=1.13 Requires-Dist: mordredcommunity Requires-
 Dist: astartes[molecules] Requires-Dist: tensorboard Requires-Dist: psutil
-Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist: isort;
-extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov;
-extra == "dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra == "hopt"
-Requires-Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-Dist:
-shap<0.45; extra == "shap" Requires-Dist: matplotlib; extra == "shap" Provides-
-Extra: bmark Requires-Dist: py2opsin; extra == "bmark"
+Requires-Dist: polars Requires-Dist: pandas Requires-Dist: pyarrow Provides-
+Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist: isort; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
+"dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra == "hopt" Requires-
+Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-Dist: shap<0.45;
+extra == "shap" Requires-Dist: matplotlib; extra == "shap" Provides-Extra:
+bmark Requires-Dist: py2opsin; extra == "bmark"
                                 [fastprop Logo]
         ********** MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
                     ******** FFaasstt,, SSccaallaabbllee,, aanndd <<550000 LLOOCC ********
           [GitHub Repo Stars][PyPI - Downloads][PyPI][PyPI - License]
 # Announcements ## alphaXiv The `fastprop` paper is freely available online at
 [arxiv.org/abs/2404.02058](https://arxiv.org/abs/2404.02058) and we are
 conducting open source peer review on [alphaXiv](https://alphaxiv.org/abs/
```

### Comparing `fastprop-1.0.1/README.md` & `fastprop-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.1/fastprop/cli/base.py` & `fastprop-1.0.2/fastprop/cli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,22 @@
     train_subparser = subparsers.add_parser("train")
     train_subparser.add_argument("config_file", nargs="?", help="YAML configuration file")
     train_subparser.add_argument("-od", "--output-directory", help="directory for fastprop output")
     # featurization
     train_subparser.add_argument("-if", "--input-file", help="csv of SMILES and targets")
     train_subparser.add_argument("-tc", "--target-columns", nargs="+", help="column name(s) for target(s)")
     train_subparser.add_argument("-sc", "--smiles-column", help="column name for SMILES")
-    train_subparser.add_argument("-d", "--descriptors", help="descriptors to calculate (one of all, optimized, or debug)")
+    train_subparser.add_argument("-ds", "--descriptor-set", help="descriptors to calculate (one of all, optimized, or debug)")
     train_subparser.add_argument("-ec", "--enable-cache", type=bool, help="allow saving and loading of cached descriptors")
     train_subparser.add_argument("-p", "--precomputed", help="precomputed descriptors from fastprop or mordred")
 
     # training
     train_subparser.add_argument("-op", "--optimize", action="store_true", help="run hyperparameter optimization", default=False)
     train_subparser.add_argument("-fl", "--fnn-layers", type=int, help="number of fnn layers")
+    train_subparser.add_argument("-hs", "--hidden-size", type=int, help="hidden size of fnn layers")
     train_subparser.add_argument("-lr", "--learning-rate", type=float, help="learning rate")
     train_subparser.add_argument("-bs", "--batch-size", type=int, help="batch size")
     train_subparser.add_argument("-ne", "--number-epochs", type=int, help="number of epochs")
     train_subparser.add_argument("-nr", "--number-repeats", type=int, help="number of repeats")
     train_subparser.add_argument("-pt", "--problem-type", help="problem type (regression or a type of classification)")
     train_subparser.add_argument("-ns", "--train-size", type=float, help="train size")
     train_subparser.add_argument("-vs", "--val-size", type=float, help="val size")
```

### Comparing `fastprop-1.0.1/fastprop/cli/predict.py` & `fastprop-1.0.2/fastprop/cli/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     if smiles_file is not None:
         if smiles_strings:
             raise RuntimeError("Specify either smiles_strings or smiles_file, not both.")
         smiles_strings = [s.strip() for s in open(smiles_file, "r").readlines()]
 
     # load the models
     if precomputed_descriptors is None:
-        _, rdkit_mols = clean_dataset(np.zeros((1, len(smiles_strings))), np.array(smiles_strings))
+        _, rdkit_mols, _ = clean_dataset(np.zeros((1, len(smiles_strings))), np.array(smiles_strings))
         descs = get_descriptors(cache_filepath=False, descriptors=DESCRIPTOR_SET_LOOKUP[descriptor_set], rdkit_mols=rdkit_mols)
         descs = descs.to_numpy(dtype=float)
     else:
         descs = load_saved_descriptors(precomputed_descriptors)
 
     all_models = []
     for checkpoint in os.listdir(checkpoints_dir):
```

### Comparing `fastprop-1.0.1/fastprop/cli/shap.py` & `fastprop-1.0.2/fastprop/cli/shap.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.1/fastprop/cli/train.py` & `fastprop-1.0.2/fastprop/cli/train.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 import datetime
 import logging
 import os
 from pathlib import Path
 from typing import Dict, List
 
 import pandas as pd
+import psutil
 import torch
 from lightning.pytorch import seed_everything
+from lightning.pytorch.utilities.rank_zero import rank_zero_only
 from scipy.stats import ttest_ind
 
 from fastprop.data import (
     clean_dataset,
     fastpropDataLoader,
     fastpropDataset,
     split,
     standard_scale,
 )
 from fastprop.defaults import DESCRIPTOR_SET_LOOKUP, _init_loggers, init_logger
 from fastprop.descriptors import get_descriptors
 from fastprop.io import load_saved_descriptors, read_input_csv
 from fastprop.model import fastprop, train_and_test
 
-logger = init_logger(__name__)
-
 
 tune, OptunaSearch = None, None
 try:
     import ray
     from ray import tune
     from ray.train.torch import enable_reproducibility
     from ray.tune.search.optuna import OptunaSearch
 except ImportError as ie:
     hopt_error = ie
 
 logger = init_logger(__name__)
 
 
-MODELS_PER_GPU, NUM_HOPT_TRIALS = 4, 16
+NUM_HOPT_TRIALS = 16
+
+
+@rank_zero_only
+def _get_out_subdir_name(output_directory: str):
+    return os.path.join(output_directory, f"fastprop_{int(datetime.datetime.utcnow().timestamp())}")
 
 
 def train_fastprop(
     output_directory: str,
     input_file: str,
     smiles_column: str,
     target_columns: List[str],
@@ -63,15 +68,15 @@
     hopt: bool = False,
 ):
     if hopt and (tune is None or OptunaSearch is None):
         raise RuntimeError(
             "Unable to import hyperparameter optimization dependencies, please install fastprop[hopt].\nOriginal error: " + str(hopt_error)
         )
     # setup logging and output directories
-    output_subdirectory = os.path.join(output_directory, f"fastprop_{int(datetime.datetime.utcnow().timestamp())}")
+    output_subdirectory = _get_out_subdir_name(output_directory)
     os.makedirs(output_directory, exist_ok=True)
     os.makedirs(output_subdirectory, exist_ok=True)
     os.makedirs(os.path.join(output_subdirectory, "checkpoints"), exist_ok=True)
     _init_loggers(output_subdirectory)
     logging.getLogger("pytorch_lightning").setLevel(logging.INFO)
     seed_everything(random_seed)
 
@@ -83,30 +88,30 @@
         cache_file = os.path.join(
             output_directory, "cached_" + Path(input_file).stem + "_" + descriptor_set + "_" + str(int(os.stat(input_file).st_ctime)) + ".csv"
         )
         if os.path.exists(cache_file) and enable_cache:
             logger.info(f"Found cached descriptor data at {cache_file}, loading instead of recalculating.")
             descriptors = load_saved_descriptors(cache_file)
         else:
-            targets, rdkit_mols = clean_dataset(targets, smiles)
+            targets, rdkit_mols, smiles = clean_dataset(targets, smiles)
             descriptors = get_descriptors(enable_cache and cache_file, DESCRIPTOR_SET_LOOKUP[descriptor_set], rdkit_mols)
             descriptors = descriptors.to_numpy(dtype=float)
 
     descriptors = torch.tensor(descriptors, dtype=torch.float32)
     targets = torch.tensor(targets, dtype=torch.float32)
 
     if problem_type == "multiclass" and not (targets.size(dim=1) > 1):
         logger.info("One-hot encoding targets.")
         targets = torch.nn.functional.one_hot(targets.long()).squeeze()
 
     input_size = descriptors.shape[1]
     readout_size = targets.shape[1]
     n_tasks = 1 if problem_type in {"binary", "multiclass"} else readout_size
 
-    logger.info(f"Run 'tensorboard --logdir {os.path.join(output_directory, 'tensorboard_logs')}' to track training progress.")
+    logger.info(f"Run 'tensorboard --logdir {os.path.join(output_subdirectory, 'tensorboard_logs')}' to track training progress.")
     if not hopt:
         return _replicates(
             number_repeats,
             smiles,
             train_size,
             val_size,
             test_size,
@@ -160,23 +165,21 @@
                     fnn_layers,
                     batch_size,
                     number_epochs,
                     patience,
                     target_columns,
                     output_subdirectory,
                 ),
-                # run n_parallel models at the same time (leave 20% for system)
-                # don't specify cpus, and just let pl figure it out
-                resources={"gpu": (1 - 0.20) / MODELS_PER_GPU},
+                resources={"gpu": 1, "cpu": psutil.cpu_count()},
             ),
             tune_config=tune.TuneConfig(
                 metric=metric,
                 mode="min",
                 search_alg=algo,
-                max_concurrent_trials=MODELS_PER_GPU,
+                max_concurrent_trials=1,
                 num_samples=NUM_HOPT_TRIALS,
             ),
             param_space=search_space,
         )
         results = tuner.fit()
         best = results.get_best_result().config
         logger.info(f"Best hyperparameters identified: {', '.join([key + ': ' + str(val) for key, val in best.items()])}")
@@ -206,39 +209,41 @@
     target_columns,
     output_subdirectory,
 ):
     all_test_results, all_validation_results = [], []
     for replicate_number in range(number_repeats):
         logger.info(f"Training model {replicate_number+1} of {number_repeats} ({random_seed=})")
 
+        descriptors_copy = descriptors.detach().clone()
+        targets_copy = targets.detach().clone()
         # prepare the dataloaders
         train_indexes, val_indexes, test_indexes = split(smiles, random_seed, train_size, val_size, test_size, sampler)
-        descriptors[train_indexes], feature_means, feature_vars = standard_scale(descriptors[train_indexes])
-        descriptors[val_indexes] = standard_scale(descriptors[val_indexes], feature_means, feature_vars)
-        descriptors[test_indexes] = standard_scale(descriptors[test_indexes], feature_means, feature_vars)
+        descriptors_copy[train_indexes], feature_means, feature_vars = standard_scale(descriptors_copy[train_indexes])
+        descriptors_copy[val_indexes] = standard_scale(descriptors_copy[val_indexes], feature_means, feature_vars)
+        descriptors_copy[test_indexes] = standard_scale(descriptors_copy[test_indexes], feature_means, feature_vars)
 
         if problem_type == "regression":
-            targets[train_indexes], target_means, target_vars = standard_scale(targets[train_indexes, :])
-            targets[val_indexes] = standard_scale(targets[val_indexes, :], target_means, target_vars)
-            targets[test_indexes] = standard_scale(targets[test_indexes, :], target_means, target_vars)
+            targets_copy[train_indexes], target_means, target_vars = standard_scale(targets_copy[train_indexes, :])
+            targets_copy[val_indexes] = standard_scale(targets_copy[val_indexes, :], target_means, target_vars)
+            targets_copy[test_indexes] = standard_scale(targets_copy[test_indexes, :], target_means, target_vars)
         else:
             target_means = None
             target_vars = None
 
         train_dataloader = fastpropDataLoader(
-            fastpropDataset(descriptors[train_indexes], targets[train_indexes]),
+            fastpropDataset(descriptors_copy[train_indexes], targets_copy[train_indexes]),
             shuffle=True,
             batch_size=batch_size,
         )
         val_dataloader = fastpropDataLoader(
-            fastpropDataset(descriptors[val_indexes], targets[val_indexes]),
+            fastpropDataset(descriptors_copy[val_indexes], targets_copy[val_indexes]),
             batch_size=batch_size,
         )
         test_dataloader = fastpropDataLoader(
-            fastpropDataset(descriptors[test_indexes], targets[test_indexes]),
+            fastpropDataset(descriptors_copy[test_indexes], targets_copy[test_indexes]),
             batch_size=batch_size,
         )
 
         # initialize the model and train/test
         model = fastprop(
             input_size,
             hidden_size,
@@ -274,27 +279,27 @@
     logger.info("Displaying validation results:\n%s", validation_results_df.describe().transpose().to_string())
     test_results_df = pd.DataFrame.from_records(all_test_results)
     logger.info("Displaying testing results:\n%s", test_results_df.describe().transpose().to_string())
 
     if number_repeats > 1:
         metric = fastprop.get_metric(problem_type)
         ttest_result = ttest_ind(
-            test_results_df[f"test_{metric}_loss"].to_numpy(),
-            validation_results_df[f"validation_{metric}_loss"].to_numpy(),
+            test_results_df[f"test_{metric}_scaled_loss"].to_numpy(),
+            validation_results_df[f"validation_{metric}_scaled_loss"].to_numpy(),
         )
         if (p := ttest_result.pvalue) < 0.05:
             logger.warn(
                 "Detected possible over/underfitting! 2-sided T-test between validation and testing"
                 f" {metric} yielded {p=:.3f}<0.05. Consider changing patience."
             )
         else:
             logger.info(f"2-sided T-test between validation and testing {metric} yielded p value of {p=:.3f}>0.05.")
     else:
         logger.info("fastprop is unable to generate statistics to check for overfitting, consider increasing 'num_repeats' to at least 2.")
-    return test_results_df
+    return validation_results_df, test_results_df
 
 
 def _hopt_objective(
     trial,
     smiles_ref,
     targets_ref,
     descriptors_ref,
@@ -317,15 +322,15 @@
     target_columns,
     output_subdirectory,
 ) -> Dict[str, float]:
     descriptors = ray.get(descriptors_ref)
     targets = ray.get(targets_ref)
     smiles = ray.get(smiles_ref)
     enable_reproducibility(random_seed)
-    test_results_df = _replicates(
+    validation_results_df, test_results_df = _replicates(
         number_repeats,
         smiles,
         train_size,
         val_size,
         test_size,
         descriptors,
         targets,
@@ -341,8 +346,8 @@
         batch_size,
         number_epochs,
         patience,
         target_columns,
         output_subdirectory,
     )
     metric = fastprop.get_metric(problem_type)
-    return {metric: test_results_df.describe().at["mean", f"test_{metric}_loss"]}
+    return {metric: validation_results_df.describe().at["mean", f"validation_{metric}_scaled_loss"]}
```

### Comparing `fastprop-1.0.1/fastprop/data.py` & `fastprop-1.0.2/fastprop/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,26 +139,26 @@
         logger.warn(f"Removed {len(error_mols_idxs)} entries from the dataset ({100*len(error_mols_idxs)/starting_length:.2f}% of the data).")
         targets = np.delete(targets, error_mols_idxs, axis=0)
         rdkit_mols = np.delete(rdkit_mols, error_mols_idxs, axis=0)
         smiles = np.delete(smiles, error_mols_idxs)
 
     # also remove dataset entries where the target is missing
     # TODO: weight masking instead of removal?
-    error_target_idxs = [idx for idx, arr in enumerate(targets) if any(np.isnan(arr))]
+    error_target_idxs = [idx for idx, arr in enumerate(targets) if np.any(np.isnan(arr))]
     for idx in error_target_idxs:
         logger.warn(
             f"Missing target value (target={targets[idx]}) for SMILES {smiles[idx]}. Both the molecule and the target will be removed from the data."
         )
     if len(error_target_idxs) > 0:
         # specify axis=0 to avoid changing dimensions (flattening)
         logger.warn(f"Removed {len(error_target_idxs)} entries from the dataset ({100*len(error_target_idxs)/starting_length:.2f}% of the data).")
         targets = np.delete(targets, error_target_idxs, axis=0)
         rdkit_mols = np.delete(rdkit_mols, error_target_idxs, axis=0)
         smiles = np.delete(smiles, error_target_idxs)
-    return targets, rdkit_mols
+    return targets, rdkit_mols, smiles
 
 
 # wrap the basic pytorch Dataset and Dataloader to set some arguments in a convenient way
 
 
 class fastpropDataset(TorchDataset):
     def __init__(
```

### Comparing `fastprop-1.0.1/fastprop/defaults.py` & `fastprop-1.0.2/fastprop/defaults.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.1/fastprop/descriptors.py` & `fastprop-1.0.2/fastprop/descriptors.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.1/fastprop/io.py` & `fastprop-1.0.2/fastprop/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
+import polars as pl
 
 from fastprop.defaults import init_logger
 
 logger = init_logger(__name__)
 
 
 def read_input_csv(filepath: str, smiles_column: str, target_columns: List[str]) -> Tuple[np.ndarray, np.ndarray]:
@@ -18,15 +19,15 @@
 
     Raises:
         RuntimeError: Missing columns name(s).
 
     Returns:
         tuple[np.ndarray, np.ndarray]: Targets and SMILES strings.
     """
-    src = pd.read_csv(filepath)
+    src = pl.read_csv(filepath).to_pandas()
     try:
         targets = pd.concat([src.pop(x) for x in target_columns], axis=1).to_numpy()
         smiles = src.pop(smiles_column).to_numpy()
     except KeyError as ke:
         raise RuntimeError(f"Unable to find column(s) inside file {filepath}. Check spelling and file contents.") from ke
 
     # keep everything 2D
@@ -41,11 +42,11 @@
 
     Args:
         fpath (str): Filepath to CSV.
 
     Returns:
         np.ndarray: Loaded descriptors.
     """
-    d = pd.read_csv(fpath, low_memory=False)
+    d = pl.read_csv(fpath, ignore_errors=True).to_pandas()
     d = d.apply(pd.to_numeric, errors="coerce")
     descs = d[d.columns[1:]].to_numpy(dtype=float)
     return descs
```

### Comparing `fastprop-1.0.1/fastprop/metrics.py` & `fastprop-1.0.2/fastprop/metrics.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.1/fastprop/model.py` & `fastprop-1.0.2/fastprop/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import glob
 import os
 from time import perf_counter
 from typing import List, Literal, Optional, OrderedDict, Tuple
 
 import pandas as pd
 import pytorch_lightning as pl
 import torch
@@ -59,23 +58,19 @@
         self.register_buffer("target_vars", target_vars)
         self.problem_type = problem_type
         self.training_metric = fastprop.get_metric(problem_type)
         self.learning_rate = learning_rate
         self.target_names = target_names
 
         # fully-connected nn
-        layers = OrderedDict(
-            [
-                ("lin1", torch.nn.Linear(input_size, hidden_size)),
-                ("act1", torch.nn.ReLU()),
-            ]
-        )
-        for i in range(fnn_layers - 1):
-            layers[f"lin{i+2}"] = torch.nn.Linear(hidden_size, hidden_size)
-            layers[f"act{i+2}"] = torch.nn.ReLU()
+        layers = OrderedDict()
+        for i in range(fnn_layers):
+            layers[f"lin{i+1}"] = torch.nn.Linear(input_size if i == 0 else hidden_size, hidden_size)
+            if fnn_layers == 1 or i < (fnn_layers - 1):  # no output activation, unless single layer
+                layers[f"act{i+1}"] = torch.nn.ReLU()
         self.fnn = torch.nn.Sequential(layers)
         self.readout = torch.nn.Linear(hidden_size, readout_size)
 
         self.save_hyperparameters()
 
     def configure_optimizers(self):
         """See https://lightning.ai/docs/pytorch/stable/common/optimization.html
@@ -131,26 +126,26 @@
 
     def log(self, name, value, **kwargs):
         """Wrap the parent PyTorch Lightning log function to automatically detect DDP."""
         return super().log(name, value, sync_dist=distributed.is_initialized(), **kwargs)
 
     def training_step(self, batch, batch_idx):
         loss, _ = self._machine_loss(batch)
-        self.log(f"train_{self.training_metric}_loss", loss)
+        self.log(f"train_{self.training_metric}_scaled_loss", loss)
         return loss
 
     def validation_step(self, batch, batch_idx):
         loss, y_hat = self._machine_loss(batch)
-        self.log(f"validation_{self.training_metric}_loss", loss)
+        self.log(f"validation_{self.training_metric}_scaled_loss", loss)
         self._human_loss(y_hat, batch, "validation")
         return loss
 
     def test_step(self, batch, batch_idx):
         loss, y_hat = self._machine_loss(batch)
-        self.log(f"test_{self.training_metric}_loss", loss)
+        self.log(f"test_{self.training_metric}_scaled_loss", loss)
         self._human_loss(y_hat, batch, "test")
         return loss
 
     def predict_step(self, batch: Tuple[torch.Tensor]):
         """Applies feature scaling and appropriate activation function to a Tensor of descriptors.
 
         Args:
@@ -215,75 +210,76 @@
     output_directory: str,
     fastprop_model: fastprop,
     train_dataloader: fastpropDataLoader,
     val_dataloader: fastpropDataLoader,
     test_dataloader: fastpropDataLoader,
     number_epochs: int = 30,
     patience: int = 5,
+    quiet: bool = False
 ):
     """Run a single train/validate and test iteration.
 
     Args:
         output_directory (str): Filepath to write logs and checkpoints.
         fastprop_model (fastprop): fastprop LightningModule instance.
         train_dataloader (fastpropDataLoader): Training data.
         val_dataloader (fastpropDataLoader): Validation data.
         test_dataloader (fastpropDataLoader): Testing data.
         number_epochs (int, optional): Maximum number of epochs for training. Defaults to 30.
         patience (int, optional): Number of epochs for early stopping. Defaults to 5.
+        quiet (bool, optional): Set True to disable some printing. Default to False.
 
     Returns:
-        _type_: _description_
+        list[dict]: Lightning model output.
     """
     try:
         repetition_number = len(os.listdir(os.path.join(output_directory, "tensorboard_logs"))) + 1
     except FileNotFoundError:
         repetition_number = 1
     tensorboard_logger = TensorBoardLogger(
         output_directory,
         name="tensorboard_logs",
         version=f"repetition_{repetition_number}",
         default_hp_metric=False,
     )
 
     callbacks = [
         EarlyStopping(
-            monitor=f"validation_{fastprop_model.training_metric}_loss",
+            monitor=f"validation_{fastprop_model.training_metric}_scaled_loss",
             mode="min",
             verbose=False,
             patience=patience,
         ),
         ModelCheckpoint(
-            monitor=f"validation_{fastprop_model.training_metric}_loss",
+            monitor=f"validation_{fastprop_model.training_metric}_scaled_loss",
             dirpath=os.path.join(output_directory, "checkpoints"),
             filename=f"repetition-{repetition_number}" + "-{epoch:02d}-{val_loss:.2f}",
             save_top_k=1,
             mode="min",
         ),
     ]
 
     trainer = pl.Trainer(
         max_epochs=number_epochs,
-        enable_progress_bar=True,
-        enable_model_summary=True,
+        enable_progress_bar=not quiet,
+        enable_model_summary=not quiet,
         logger=tensorboard_logger,
         log_every_n_steps=1,
         enable_checkpointing=True,
         check_val_every_n_epoch=1,
         callbacks=callbacks,
     )
 
     t1_start = perf_counter()
     trainer.fit(fastprop_model, train_dataloader, val_dataloader)
     t1_stop = perf_counter()
     logger.info("Elapsed time during training: " + str(datetime.timedelta(seconds=t1_stop - t1_start)))
-    checkpoints_list = glob.glob(os.path.join(output_directory, "checkpoints", "*.ckpt"))
-    latest_file = max(checkpoints_list, key=os.path.getctime)
-    logger.info(f"Reloading best model from checkpoint file: {latest_file}")
-    fastprop_model = fastprop.load_from_checkpoint(latest_file)
+    ckpt_path = trainer.checkpoint_callback.best_model_path
+    logger.info(f"Reloading best model from checkpoint file: {ckpt_path}")
+    fastprop_model = fastprop_model.__class__.load_from_checkpoint(ckpt_path)
     validation_results = trainer.validate(fastprop_model, val_dataloader, verbose=False)
     test_results = trainer.test(fastprop_model, test_dataloader, verbose=False)
     validation_results_df = pd.DataFrame.from_records(validation_results, index=("value",))
     logger.info("Displaying validation results for repetition %d:\n%s", repetition_number, validation_results_df.transpose().to_string())
     test_results_df = pd.DataFrame.from_records(test_results, index=("value",))
     logger.info("Displaying validation results for repetition %d:\n%s", repetition_number, test_results_df.transpose().to_string())
     return test_results, validation_results
```

### Comparing `fastprop-1.0.1/fastprop.egg-info/PKG-INFO` & `fastprop-1.0.2/fastprop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastprop
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fast Molecular Property Prediction with mordredcommunity
 Author: Jackson Burns
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,14 +12,17 @@
 Requires-Dist: pyyaml
 Requires-Dist: lightning
 Requires-Dist: torch>=1.13
 Requires-Dist: mordredcommunity
 Requires-Dist: astartes[molecules]
 Requires-Dist: tensorboard
 Requires-Dist: psutil
+Requires-Dist: polars
+Requires-Dist: pandas
+Requires-Dist: pyarrow
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: hopt
 Requires-Dist: ray[train]; extra == "hopt"
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: fastprop Version: 1.0.1 Summary: Fast Molecular
+Metadata-Version: 2.1 Name: fastprop Version: 1.0.2 Summary: Fast Molecular
 Property Prediction with mordredcommunity Author: Jackson Burns License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pyyaml Requires-Dist:
 lightning Requires-Dist: torch>=1.13 Requires-Dist: mordredcommunity Requires-
 Dist: astartes[molecules] Requires-Dist: tensorboard Requires-Dist: psutil
-Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist: isort;
-extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov;
-extra == "dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra == "hopt"
-Requires-Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-Dist:
-shap<0.45; extra == "shap" Requires-Dist: matplotlib; extra == "shap" Provides-
-Extra: bmark Requires-Dist: py2opsin; extra == "bmark"
+Requires-Dist: polars Requires-Dist: pandas Requires-Dist: pyarrow Provides-
+Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist: isort; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
+"dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra == "hopt" Requires-
+Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-Dist: shap<0.45;
+extra == "shap" Requires-Dist: matplotlib; extra == "shap" Provides-Extra:
+bmark Requires-Dist: py2opsin; extra == "bmark"
                                 [fastprop Logo]
         ********** MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
                     ******** FFaasstt,, SSccaallaabbllee,, aanndd <<550000 LLOOCC ********
           [GitHub Repo Stars][PyPI - Downloads][PyPI][PyPI - License]
 # Announcements ## alphaXiv The `fastprop` paper is freely available online at
 [arxiv.org/abs/2404.02058](https://arxiv.org/abs/2404.02058) and we are
 conducting open source peer review on [alphaXiv](https://alphaxiv.org/abs/
```

### Comparing `fastprop-1.0.1/pyproject.toml` & `fastprop-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastprop"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "Jackson Burns" },
 ]
 license = { text = "MIT" }
 description = "Fast Molecular Property Prediction with mordredcommunity"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 urls = { Homepage = "https://github.com/JacksonBurns/fastprop" }
 requires-python = ">=3.8"
-dependencies = ["pyyaml", "lightning", "torch>=1.13", "mordredcommunity", "astartes[molecules]", "tensorboard", "psutil"]
+dependencies = ["pyyaml", "lightning", "torch>=1.13", "mordredcommunity", "astartes[molecules]", "tensorboard", "psutil", "polars", "pandas", "pyarrow"]
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pytest", "pytest-cov"]
 hopt = ["ray[train]", "optuna"]
 shap = ["shap<0.45", "matplotlib"]
 bmark = ["py2opsin"]
```

### Comparing `fastprop-1.0.1/test/test_fastprop.py` & `fastprop-1.0.2/test/test_fastprop.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         train_args = dict(DEFAULT_TRAINING_CONFIG)
         with open(self.config_file, "r") as f:
             fastprop_args = yaml.safe_load(f)
             fastprop_args["target_columns"] = fastprop_args["target_columns"].split(" ")
             fastprop_args["output_directory"] = self.temp_dirname
             fastprop_args["input_file"] = os.path.join(self.benchmark_dir, "pah", "arockiaraj_pah_data.csv")
             train_args.update(fastprop_args)
-            res = train_fastprop(**train_args)
+            _, res = train_fastprop(**train_args)
             assert res.describe().loc["mean", "test_r2_score"] > 0.90
 
     @classmethod
     def tearDownClass(cls):
         shutil.rmtree(cls.temp_dirname, ignore_errors=True)
```

