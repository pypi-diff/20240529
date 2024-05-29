# Comparing `tmp/falcon_challenge-0.3.8.tar.gz` & `tmp/falcon_challenge-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.3.8.tar", last modified: Fri May 17 03:52:31 2024, max compression
+gzip compressed data, was "falcon_challenge-0.3.9.tar", last modified: Tue May 28 21:26:28 2024, max compression
```

## Comparing `falcon_challenge-0.3.8.tar` & `falcon_challenge-0.3.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.674625 falcon_challenge-0.3.8/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.674625 falcon_challenge-0.3.8/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    28438 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:28.386132 falcon_challenge-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-28 21:26:28.386132 falcon_challenge-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:28.382132 falcon_challenge-0.3.9/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:28.382132 falcon_challenge-0.3.9/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:28.386132 falcon_challenge-0.3.9/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-28 21:26:28.000000 falcon_challenge-0.3.9/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-28 21:26:28.000000 falcon_challenge-0.3.9/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:26:28.000000 falcon_challenge-0.3.9/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 21:26:28.000000 falcon_challenge-0.3.9/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 21:26:28.000000 falcon_challenge-0.3.9/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:28.386132 falcon_challenge-0.3.9/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:26:28.386132 falcon_challenge-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-28 21:26:21.000000 falcon_challenge-0.3.9/setup.py
```

### Comparing `falcon_challenge-0.3.8/LICENSE` & `falcon_challenge-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/PKG-INFO` & `falcon_challenge-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.8
+Version: 0.3.9
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.8/README.md` & `falcon_challenge-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/decoder_demos/decoding_utils.py` & `falcon_challenge-0.3.9/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/decoder_demos/filtering.py` & `falcon_challenge-0.3.9/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.3.9/decoder_demos/ndt2_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/decoder_demos/random_decoder.py` & `falcon_challenge-0.3.9/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.3.9/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.3.9/decoder_demos/sklearn_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,16 +263,18 @@
     else:
         day_unique = set([f.stem.split('_')[1] for f in all_datafiles])
     all_decoders = {}
     x_means = {}
     x_stds = {}
     for day in sorted(day_unique): # separate decoder
         print(f"Training on day {day}")
-        fit_datafiles = [d for d in all_datafiles if day == task_config.hash_dataset(d).split('_set_')[0]]
-
+        if task_config.task == FalconTask.h1:
+            fit_datafiles = [d for d in all_datafiles if day == task_config.hash_dataset(d).split('_set_')[0]]
+        else:
+            fit_datafiles = [d for d in all_datafiles if day == d.stem.split('_')[1]]
         (
             neural_data,
             covariates,
             trial_change,
             eval_mask
         ) = zip(*[load_nwb(fn, task_config.task) for fn in fit_datafiles])
         neural_data = np.concatenate(neural_data)
```

### Comparing `falcon_challenge-0.3.8/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.3.9/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/falcon_challenge/config.py` & `falcon_challenge-0.3.9/falcon_challenge/config.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/falcon_challenge/dataloaders.py` & `falcon_challenge-0.3.9/falcon_challenge/dataloaders.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/falcon_challenge/evaluator.py` & `falcon_challenge-0.3.9/falcon_challenge/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,16 @@
 # Used to label test server data file names to look for
 # These act as a _reduction_ set of the full list of datafiles considered, to specific sessions. Relevant for H1/M2.
 def reduce_key(key):
     if key.startswith('Run'):
         return key.split('_')[1]
     if key.startswith('L_'):
         return key
+    if key.startswith('S'):
+        return key.split('_')[0]    
     return key
 
 HELD_IN_KEYS = {
     FalconTask.h1: ['S0_', 'S1_', 'S2_', 'S3_', 'S4_', 'S5_'],
     FalconTask.m1: ['L_20120924', 'L_20120926', 'L_20120927', 'L_20120928'],
     FalconTask.m2: ['20201019', '20201020', '20201027', '20201028'],
     FalconTask.h2: DATASET_HELDINOUT_MAP['h2']['held_in'],
@@ -194,28 +196,42 @@
         split_result["Normalized Latency"] = user_submission[datasplit]["normalized_latency"]
         del user_submission[datasplit]["normalized_latency"]
         pred_dict = defaultdict(list)
         tgt_dict = defaultdict(list)
         mask_dict = defaultdict(list)
         if 'h2' not in datasplit:
             dset_len_dict = defaultdict(lambda: defaultdict(list))
-        for dataset in user_submission[datasplit]:
+        if 'm2' in datasplit:
+            grouped = {}
+            for set_name in user_submission[datasplit]:
+                run, date = set_name.split('_')
+                if date not in grouped:
+                    grouped[date] = []
+                grouped[date].append(set_name)
+            for date in grouped:
+                grouped[date].sort()
+            all_datasets = [run for runs in grouped.values() for run in runs]
+        else:
+            all_datasets = user_submission[datasplit]
+        for dataset in all_datasets:
             dataset_pred = user_submission[datasplit][dataset]
             dataset_tgt = split_annotations[dataset]['data']
             dataset_mask = split_annotations[dataset]['mask']
             dataset_pred = dataset_pred[:dataset_mask.shape[0]] # In case excess timesteps are predicted due to batching, reduce
             if dataset in DATASET_HELDINOUT_MAP[datasplit]['held_in']:
                 if 'h2' not in datasplit:
+                    # For splits with multiple datasets per session (H1 and M2), we need to map predictions, targets, and masks for each dataset to the session ID 
                     session_id = reduce_key(dataset)
                     dset_len_dict['held_in'][session_id].append(dataset_mask.shape[0])
                 pred_dict['held_in'].append(dataset_pred)
                 tgt_dict['held_in'].append(dataset_tgt)
                 mask_dict['held_in'].append(dataset_mask)
             elif dataset in DATASET_HELDINOUT_MAP[datasplit]['held_out']:
                 if not 'h2' in datasplit:
+                    # For splits with multiple datasets per session (H1 and M2), we need to map predictions, targets, and masks for each dataset to the session ID 
                     session_id = reduce_key(dataset)
                     dset_len_dict['held_out'][session_id].append(dataset_mask.shape[0])
                 pred_dict['held_out'].append(dataset_pred)
                 tgt_dict['held_out'].append(dataset_tgt)
                 mask_dict['held_out'].append(dataset_mask)
             else:
                 raise ValueError(f"Dataset {dataset} submitted but not found in held-in or held-out list of split {datasplit}.")
```

### Comparing `falcon_challenge-0.3.8/falcon_challenge/interface.py` & `falcon_challenge-0.3.9/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.3.9/falcon_challenge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.8
+Version: 0.3.9
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.8/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.3.9/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/assemble_data.py` & `falcon_challenge-0.3.9/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/filtering.py` & `falcon_challenge-0.3.9/preproc/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/h2_preproc.py` & `falcon_challenge-0.3.9/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.3.9/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.3.9/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.3.9/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/m2_preproc.py` & `falcon_challenge-0.3.9/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/merge_answers.py` & `falcon_challenge-0.3.9/preproc/merge_answers.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/nwb_create_utils.py` & `falcon_challenge-0.3.9/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/wrapper_convert_batch.py` & `falcon_challenge-0.3.9/preproc/wrapper_convert_batch.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/preproc/zip_data.py` & `falcon_challenge-0.3.9/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.8/setup.py` & `falcon_challenge-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.3.8',
+    version='0.3.9',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

