# Comparing `tmp/deepchem-2.8.1.dev20240524164912.tar.gz` & `tmp/deepchem-2.8.1.dev20240529195718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.8.1.dev20240524164912.tar", last modified: Fri May 24 16:49:12 2024, max compression
+gzip compressed data, was "deepchem-2.8.1.dev20240529195718.tar", last modified: Wed May 29 19:57:18 2024, max compression
```

## Comparing `deepchem-2.8.1.dev20240524164912.tar` & `deepchem-2.8.1.dev20240529195718.tar`

### file list

```diff
@@ -1,390 +1,390 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.882243 deepchem-2.8.1.dev20240524164912/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-24 16:49:04.000000 deepchem-2.8.1.dev20240524164912/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-24 16:49:12.882243 deepchem-2.8.1.dev20240524164912/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-24 16:49:04.000000 deepchem-2.8.1.dev20240524164912/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.830242 deepchem-2.8.1.dev20240524164912/deepchem/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.830242 deepchem-2.8.1.dev20240524164912/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84152 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)   118030 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.830242 deepchem-2.8.1.dev20240524164912/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.834243 deepchem-2.8.1.dev20240524164912/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/binding_pocket_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/bio_seq_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.834243 deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)    27676 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20248 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    22111 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    38890 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.834243 deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    28058 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    14808 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.838243 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.838243 deepchem-2.8.1.dev20240524164912/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.838243 deepchem-2.8.1.dev20240524164912/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22429 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.838243 deepchem-2.8.1.dev20240524164912/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17151 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.842243 deepchem-2.8.1.dev20240524164912/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/metalearning/maml.py
--rw-r--r--   0 runner    (1001) docker     (127)    16233 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/metalearning/torch_maml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.842243 deepchem-2.8.1.dev20240524164912/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.846243 deepchem-2.8.1.dev20240524164912/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17354 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.846243 deepchem-2.8.1.dev20240524164912/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/dft/dftxc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.846243 deepchem-2.8.1.dev20240524164912/deepchem/models/dft/hamilton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/dft/hamilton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/dft/hamilton/orbparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.846243 deepchem-2.8.1.dev20240524164912/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    57408 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.846243 deepchem-2.8.1.dev20240524164912/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28179 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    57000 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (127)   144759 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.846243 deepchem-2.8.1.dev20240524164912/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    62329 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    27252 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    25969 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.846243 deepchem-2.8.1.dev20240524164912/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.854243 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/acnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31166 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/dtnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    29583 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (127)    22218 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    58182 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gan.py
--rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14944 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    51159 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28998 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    39504 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (127)    38435 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23460 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    35955 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)   245729 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17126 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (127)    17860 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (127)    24055 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    27274 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/seqtoseq.py
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/text_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    54165 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/weavemodel_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.854243 deepchem-2.8.1.dev20240524164912/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.862243 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)   165414 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.862243 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    36564 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.862243 deepchem-2.8.1.dev20240524164912/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.862243 deepchem-2.8.1.dev20240524164912/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.862243 deepchem-2.8.1.dev20240524164912/deepchem/rl/torch_rl/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/torch_rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34135 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/torch_rl/torch_a2c.py
--rw-r--r--   0 runner    (1001) docker     (127)    32978 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/rl/torch_rl/torch_ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.866243 deepchem-2.8.1.dev20240524164912/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64330 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.866243 deepchem-2.8.1.dev20240524164912/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    91191 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.870243 deepchem-2.8.1.dev20240524164912/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/attribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/debug_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.870243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.870243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/api/getxc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/api/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.870243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/data/datastruct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.870243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/df/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/df/base_df.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.870243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/grid/base_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14735 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/grid/radial_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.870243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15817 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/base_hamilton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.870243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/intor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/intor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/intor/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/orbparams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.874243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/qccalc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/qccalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/qccalc/base_qccalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/qccalc/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/qccalc/scf_qccalc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.874243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/system/base_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.874243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.874243 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/xc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/xc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35724 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/xc/base_xc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/xc/libxc.py
--rw-r--r--   0 runner    (1001) docker     (127)    40477 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/xc/libxc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/dftutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.874243 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)    23731 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/editable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/grad.py
--rw-r--r--   0 runner    (1001) docker     (127)    50928 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/linop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.874243 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/minimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/rootfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/rootsolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/pure_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    45298 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    37426 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/symeig.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/equivariance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19262 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/periodic_table_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65661 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/safeops_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.882243 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_attribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31537 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_dft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31918 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_differentiation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_equivariance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_periodic_table_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_safe_ops_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:49:12.830242 deepchem-2.8.1.dev20240524164912/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-24 16:49:12.000000 deepchem-2.8.1.dev20240524164912/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-05-24 16:49:12.000000 deepchem-2.8.1.dev20240524164912/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:49:12.000000 deepchem-2.8.1.dev20240524164912/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 16:49:12.000000 deepchem-2.8.1.dev20240524164912/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 16:49:12.000000 deepchem-2.8.1.dev20240524164912/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-24 16:49:12.882243 deepchem-2.8.1.dev20240524164912/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-24 16:49:05.000000 deepchem-2.8.1.dev20240524164912/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.391995 deepchem-2.8.1.dev20240529195718/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-29 19:57:18.391995 deepchem-2.8.1.dev20240529195718/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.339995 deepchem-2.8.1.dev20240529195718/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.339995 deepchem-2.8.1.dev20240529195718/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84152 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118030 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.339995 deepchem-2.8.1.dev20240529195718/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.343995 deepchem-2.8.1.dev20240529195718/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/binding_pocket_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/bio_seq_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.343995 deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27676 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20248 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22111 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38890 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.343995 deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28058 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14808 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.347995 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.347995 deepchem-2.8.1.dev20240529195718/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.347995 deepchem-2.8.1.dev20240529195718/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22429 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.351995 deepchem-2.8.1.dev20240529195718/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17151 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.351995 deepchem-2.8.1.dev20240529195718/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/metalearning/maml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16233 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/metalearning/torch_maml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.351995 deepchem-2.8.1.dev20240529195718/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.355995 deepchem-2.8.1.dev20240529195718/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17354 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.355995 deepchem-2.8.1.dev20240529195718/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/dft/dftxc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.355995 deepchem-2.8.1.dev20240529195718/deepchem/models/dft/hamilton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/dft/hamilton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/dft/hamilton/orbparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.355995 deepchem-2.8.1.dev20240529195718/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57408 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.355995 deepchem-2.8.1.dev20240529195718/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28179 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57000 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144759 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.355995 deepchem-2.8.1.dev20240529195718/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62329 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27252 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25969 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.355995 deepchem-2.8.1.dev20240529195718/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.363995 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/acnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31166 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/dtnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29583 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22218 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58182 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14944 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51159 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28998 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39504 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38435 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23460 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35955 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250738 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17126 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17860 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24055 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27274 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/seqtoseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/text_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54165 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/weavemodel_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.363995 deepchem-2.8.1.dev20240529195718/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.371995 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165414 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.371995 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36564 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.371995 deepchem-2.8.1.dev20240529195718/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.371995 deepchem-2.8.1.dev20240529195718/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.375995 deepchem-2.8.1.dev20240529195718/deepchem/rl/torch_rl/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/torch_rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34135 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/torch_rl/torch_a2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32978 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/rl/torch_rl/torch_ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.375995 deepchem-2.8.1.dev20240529195718/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64330 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.375995 deepchem-2.8.1.dev20240529195718/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91191 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.379995 deepchem-2.8.1.dev20240529195718/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/attribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/debug_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.379995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.379995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/api/getxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/api/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.379995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/data/datastruct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.379995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/df/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/df/base_df.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.383995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/grid/base_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14735 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/grid/radial_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.383995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15817 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/base_hamilton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.383995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/intor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/intor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/intor/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/orbparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.383995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/qccalc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/qccalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/qccalc/base_qccalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/qccalc/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/qccalc/scf_qccalc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.383995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/system/base_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.383995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.383995 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/xc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/xc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35724 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/xc/base_xc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/xc/libxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40477 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/xc/libxc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/dftutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.387995 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23731 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/editable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/grad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50928 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/linop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.387995 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/rootfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/rootsolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/pure_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45298 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37426 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/symeig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/equivariance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19262 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/periodic_table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65661 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/safeops_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.391995 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_attribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31537 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_dft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31918 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_differentiation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_equivariance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_periodic_table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_safe_ops_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-29 19:57:10.000000 deepchem-2.8.1.dev20240529195718/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:57:18.339995 deepchem-2.8.1.dev20240529195718/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-29 19:57:18.000000 deepchem-2.8.1.dev20240529195718/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-05-29 19:57:18.000000 deepchem-2.8.1.dev20240529195718/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:57:18.000000 deepchem-2.8.1.dev20240529195718/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 19:57:18.000000 deepchem-2.8.1.dev20240529195718/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 19:57:18.000000 deepchem-2.8.1.dev20240529195718/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-29 19:57:18.391995 deepchem-2.8.1.dev20240529195718/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-29 19:57:11.000000 deepchem-2.8.1.dev20240529195718/setup.py
```

### Comparing `deepchem-2.8.1.dev20240524164912/LICENSE` & `deepchem-2.8.1.dev20240529195718/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/PKG-INFO` & `deepchem-2.8.1.dev20240529195718/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.8.1.dev20240524164912
+Version: 2.8.1.dev20240529195718
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.8.1.dev20240524164912/README.md` & `deepchem-2.8.1.dev20240529195718/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/data/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/data/data_loader.py` & `deepchem-2.8.1.dev20240529195718/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/data/datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/data/pytorch_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/data/supports.py` & `deepchem-2.8.1.dev20240529195718/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/dock/binding_pocket.py` & `deepchem-2.8.1.dev20240529195718/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/dock/docking.py` & `deepchem-2.8.1.dev20240529195718/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/dock/pose_generation.py` & `deepchem-2.8.1.dev20240529195718/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/dock/pose_scoring.py` & `deepchem-2.8.1.dev20240529195718/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/atomic_conformation.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/base_classes.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/bert_tokenizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/binding_pocket_features.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/bio_seq_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/bio_seq_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/dft_data.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/graph_data.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/graph_features.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/mol_graphs.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/reaction_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.8.1.dev20240529195718/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/hyper/base_classes.py` & `deepchem-2.8.1.dev20240529195718/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/hyper/gaussian_process.py` & `deepchem-2.8.1.dev20240529195718/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/hyper/grid_search.py` & `deepchem-2.8.1.dev20240529195718/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/hyper/random_search.py` & `deepchem-2.8.1.dev20240529195718/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/metalearning/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/metalearning/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/metalearning/maml.py` & `deepchem-2.8.1.dev20240529195718/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/metalearning/torch_maml.py` & `deepchem-2.8.1.dev20240529195718/deepchem/metalearning/torch_maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/metrics/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/metrics/genomic_metrics.py` & `deepchem-2.8.1.dev20240529195718/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/metrics/metric.py` & `deepchem-2.8.1.dev20240529195718/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/metrics/score_function.py` & `deepchem-2.8.1.dev20240529195718/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/IRV.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/atomic_conv.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/callbacks.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/chemnet_layers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/chemnet_models.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/dft/dftxc.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/dft/hamilton/orbparams.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/dft/hamilton/orbparams.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/dft/nnxc.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/dft/scf.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/fcnet.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/gan.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/graph_models.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/jax_models/jax_model.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/jax_models/layers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/keras_model.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/layers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/losses.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/models.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/molgan.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/multitask.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/normalizing_flows.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/optimizers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/progressive_multitask.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/robust_multitask.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/scscore.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/seqtoseq.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/text_cnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from deepchem.models.torch_models.infograph import InfoGraphStar, InfoGraphStarModel, InfoGraphEncoder, GINEncoder, InfoGraph, InfoGraphModel, InfoGraphEncoder
 from deepchem.models.torch_models.mpnn import MPNN, MPNNModel
 from deepchem.models.torch_models.lcnn import LCNN, LCNNModel
 from deepchem.models.torch_models.pagtn import Pagtn, PagtnModel
 from deepchem.models.torch_models.mat import MAT, MATModel
 from deepchem.models.torch_models.megnet import MEGNetModel
 from deepchem.models.torch_models.normalizing_flows_pytorch import NormalizingFlow
-from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, WeaveGather, MolGANConvolutionLayer, MolGANAggregationLayer, MolGANMultiConvolutionLayer, MolGANEncoderLayer, VariationalRandomizer, EncoderRNN, DecoderRNN, AtomicConv, GraphConv
+from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, WeaveGather, MolGANConvolutionLayer, MolGANAggregationLayer, MolGANMultiConvolutionLayer, MolGANEncoderLayer, VariationalRandomizer, EncoderRNN, DecoderRNN, AtomicConv, GraphConv, GraphPool
 from deepchem.models.torch_models.cnn import CNN
 from deepchem.models.torch_models.scscore import ScScore, ScScoreModel
 from deepchem.models.torch_models.weavemodel_pytorch import Weave, WeaveModel
 from deepchem.models.torch_models.attention import ScaledDotProductAttention, SelfAttention
 from deepchem.models.torch_models.grover import GroverModel, GroverPretrain, GroverFinetune
 from deepchem.models.torch_models.readout import GroverReadout
 from deepchem.models.torch_models.dtnn import DTNN, DTNNModel
```

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/acnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/acnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/attention.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/chemberta.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/cnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/dtnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/dtnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/ferminet.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/flows.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gan.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gat.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gcn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/grover.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/hf_models.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/infograph.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/layers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -13234,2126 +13234,2439 @@
 00033b10: 7220 7061 7373 696e 6720 7468 726f 7567  r passing throug
 00033b20: 6820 7468 6520 6c61 7965 7220 7768 6963  h the layer whic
 00033b30: 6820 6861 7320 7468 6520 7368 6170 6520  h has the shape 
 00033b40: 2862 6174 6368 5f73 697a 652c 206e 756d  (batch_size, num
 00033b50: 6265 7220 6f66 2065 6c65 6374 726f 6e73  ber of electrons
 00033b60: 2c20 6e75 6d62 6572 206f 6620 656c 6563  , number of elec
 00033b70: 7472 6f6e 202c 206e 5f74 776f 2073 6861  tron , n_two sha
-00033b80: 7065 292e 0a20 2020 2020 2020 2022 2222  pe)..        """
-00033b90: 0a20 2020 2020 2020 2066 6f72 206c 2069  .        for l i
-00033ba0: 6e20 7261 6e67 6528 7365 6c66 2e6c 6179  n range(self.lay
-00033bb0: 6572 5f73 697a 6529 3a0a 2020 2020 2020  er_size):.      
-00033bc0: 2020 2020 2020 2320 4361 6c63 756c 6174        # Calculat
-00033bd0: 696e 6720 6f6e 652d 656c 6563 7472 6f6e  ing one-electron
-00033be0: 2066 6561 7475 7265 2773 2061 7665 7261   feature's avera
-00033bf0: 6765 0a20 2020 2020 2020 2020 2020 2067  ge.            g
-00033c00: 5f6f 6e65 5f75 703a 2074 6f72 6368 2e54  _one_up: torch.T
-00033c10: 656e 736f 7220 3d20 746f 7263 682e 6d65  ensor = torch.me
-00033c20: 616e 280a 2020 2020 2020 2020 2020 2020  an(.            
-00033c30: 2020 2020 6f6e 655f 656c 6563 7472 6f6e      one_electron
-00033c40: 5b3a 2c20 3a73 656c 662e 7370 696e 5b30  [:, :self.spin[0
-00033c50: 5d2c 203a 5d2c 2064 696d 3d2d 3229 0a20  ], :], dim=-2). 
-00033c60: 2020 2020 2020 2020 2020 2067 5f6f 6e65             g_one
-00033c70: 5f64 6f77 6e3a 2074 6f72 6368 2e54 656e  _down: torch.Ten
-00033c80: 736f 7220 3d20 746f 7263 682e 6d65 616e  sor = torch.mean
-00033c90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00033ca0: 2020 6f6e 655f 656c 6563 7472 6f6e 5b3a    one_electron[:
-00033cb0: 2c20 7365 6c66 2e73 7069 6e5b 305d 3a2c  , self.spin[0]:,
-00033cc0: 203a 5d2c 2064 696d 3d2d 3229 0a20 2020   :], dim=-2).   
-00033cd0: 2020 2020 2020 2020 2023 2074 656d 706f           # tempo
-00033ce0: 7261 7279 206c 6973 7473 2063 6f6e 7461  rary lists conta
-00033cf0: 696e 696e 6720 6561 6368 2065 6c65 6374  ining each elect
-00033d00: 726f 6e27 7320 656d 6265 6464 696e 6773  ron's embeddings
-00033d10: 2077 6869 6368 2077 696c 6c20 6265 2074   which will be t
-00033d20: 6f72 6368 2e73 7461 636b 206f 6e20 7468  orch.stack on th
-00033d30: 6520 656e 640a 2020 2020 2020 2020 2020  e end.          
-00033d40: 2020 6f6e 655f 656c 6563 7472 6f6e 5f74    one_electron_t
-00033d50: 6d70 203d 205b 5d0a 2020 2020 2020 2020  mp = [].        
-00033d60: 2020 2020 7477 6f5f 656c 6563 7472 6f6e      two_electron
-00033d70: 5f74 6d70 203d 205b 5d0a 2020 2020 2020  _tmp = [].      
-00033d80: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00033d90: 616e 6765 2873 656c 662e 746f 7461 6c5f  ange(self.total_
-00033da0: 656c 6563 7472 6f6e 293a 0a20 2020 2020  electron):.     
-00033db0: 2020 2020 2020 2020 2020 2023 2043 616c             # Cal
-00033dc0: 6375 6c61 7469 6e67 2074 776f 2d65 6c65  culating two-ele
-00033dd0: 6374 726f 6e20 6665 6174 7572 6527 7320  ctron feature's 
-00033de0: 6176 6572 6167 650a 2020 2020 2020 2020  average.        
-00033df0: 2020 2020 2020 2020 675f 7477 6f5f 7570          g_two_up
-00033e00: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00033e10: 2074 6f72 6368 2e6d 6561 6e28 0a20 2020   torch.mean(.   
-00033e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033e30: 2074 776f 5f65 6c65 6374 726f 6e5b 3a2c   two_electron[:,
-00033e40: 2069 2c20 3a73 656c 662e 7370 696e 5b30   i, :self.spin[0
-00033e50: 5d2c 203a 5d2c 2064 696d 3d31 290a 2020  ], :], dim=1).  
-00033e60: 2020 2020 2020 2020 2020 2020 2020 675f                g_
-00033e70: 7477 6f5f 646f 776e 3a20 746f 7263 682e  two_down: torch.
-00033e80: 5465 6e73 6f72 203d 2074 6f72 6368 2e6d  Tensor = torch.m
-00033e90: 6561 6e28 0a20 2020 2020 2020 2020 2020  ean(.           
-00033ea0: 2020 2020 2020 2020 2074 776f 5f65 6c65           two_ele
-00033eb0: 6374 726f 6e5b 3a2c 2069 2c20 7365 6c66  ctron[:, i, self
-00033ec0: 2e73 7069 6e5b 305d 3a2c 203a 5d2c 2064  .spin[0]:, :], d
-00033ed0: 696d 3d31 290a 2020 2020 2020 2020 2020  im=1).          
-00033ee0: 2020 2020 2020 663a 2074 6f72 6368 2e54        f: torch.T
-00033ef0: 656e 736f 7220 3d20 746f 7263 682e 6361  ensor = torch.ca
-00033f00: 7428 286f 6e65 5f65 6c65 6374 726f 6e5b  t((one_electron[
-00033f10: 3a2c 2069 2c20 3a5d 2c20 675f 6f6e 655f  :, i, :], g_one_
-00033f20: 7570 2c0a 2020 2020 2020 2020 2020 2020  up,.            
-00033f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033f50: 2067 5f6f 6e65 5f64 6f77 6e2c 2067 5f74   g_one_down, g_t
-00033f60: 776f 5f75 702c 2067 5f74 776f 5f64 6f77  wo_up, g_two_dow
-00033f70: 6e29 2c0a 2020 2020 2020 2020 2020 2020  n),.            
-00033f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033fa0: 6469 6d3d 3129 0a20 2020 2020 2020 2020  dim=1).         
-00033fb0: 2020 2020 2020 2069 6620 6c20 3d3d 2030         if l == 0
-00033fc0: 206f 7220 2873 656c 662e 6e5f 6f6e 655b   or (self.n_one[
-00033fd0: 6c5d 2021 3d20 7365 6c66 2e6e 5f6f 6e65  l] != self.n_one
-00033fe0: 5b6c 202d 2031 5d29 206f 7220 280a 2020  [l - 1]) or (.  
-00033ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034000: 2020 2020 2020 7365 6c66 2e6e 5f74 776f        self.n_two
-00034010: 5b6c 5d20 213d 2073 656c 662e 6e5f 7477  [l] != self.n_tw
-00034020: 6f5b 6c20 2d20 315d 293a 0a20 2020 2020  o[l - 1]):.     
-00034030: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00034040: 6e65 5f65 6c65 6374 726f 6e5f 746d 702e  ne_electron_tmp.
-00034050: 6170 7065 6e64 2828 746f 7263 682e 7461  append((torch.ta
-00034060: 6e68 2873 656c 662e 765b 6c5d 2866 2929  nh(self.v[l](f))
-00034070: 2920 2b0a 2020 2020 2020 2020 2020 2020  ) +.            
-00034080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033b80: 7065 292e 0a20 2020 2020 2020 2020 2020  pe)..           
+00033b90: 2054 6865 2074 776f 2065 6c65 6374 726f   The two electro
+00033ba0: 6e20 6665 6174 7572 6520 6166 7465 7220  n feature after 
+00033bb0: 7061 7373 696e 6720 7468 726f 7567 6820  passing through 
+00033bc0: 7468 6520 6c61 7965 7220 7768 6963 6820  the layer which 
+00033bd0: 6861 7320 7468 6520 7368 6170 6520 2862  has the shape (b
+00033be0: 6174 6368 5f73 697a 652c 206e 756d 6265  atch_size, numbe
+00033bf0: 7220 6f66 2065 6c65 6374 726f 6e73 2c20  r of electrons, 
+00033c00: 6e75 6d62 6572 206f 6620 656c 6563 7472  number of electr
+00033c10: 6f6e 202c 206e 5f74 776f 2073 6861 7065  on , n_two shape
+00033c20: 292e 0a20 2020 2020 2020 2022 2222 0a20  )..        """. 
+00033c30: 2020 2020 2020 2066 6f72 206c 2069 6e20         for l in 
+00033c40: 7261 6e67 6528 7365 6c66 2e6c 6179 6572  range(self.layer
+00033c50: 5f73 697a 6529 3a0a 2020 2020 2020 2020  _size):.        
+00033c60: 2020 2020 2320 4361 6c63 756c 6174 696e      # Calculatin
+00033c70: 6720 6f6e 652d 656c 6563 7472 6f6e 2066  g one-electron f
+00033c80: 6561 7475 7265 2773 2061 7665 7261 6765  eature's average
+00033c90: 0a20 2020 2020 2020 2020 2020 2067 5f6f  .            g_o
+00033ca0: 6e65 5f75 703a 2074 6f72 6368 2e54 656e  ne_up: torch.Ten
+00033cb0: 736f 7220 3d20 746f 7263 682e 6d65 616e  sor = torch.mean
+00033cc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00033cd0: 2020 6f6e 655f 656c 6563 7472 6f6e 5b3a    one_electron[:
+00033ce0: 2c20 3a73 656c 662e 7370 696e 5b30 5d2c  , :self.spin[0],
+00033cf0: 203a 5d2c 2064 696d 3d2d 3229 0a20 2020   :], dim=-2).   
+00033d00: 2020 2020 2020 2020 2067 5f6f 6e65 5f64           g_one_d
+00033d10: 6f77 6e3a 2074 6f72 6368 2e54 656e 736f  own: torch.Tenso
+00033d20: 7220 3d20 746f 7263 682e 6d65 616e 280a  r = torch.mean(.
+00033d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033d40: 6f6e 655f 656c 6563 7472 6f6e 5b3a 2c20  one_electron[:, 
+00033d50: 7365 6c66 2e73 7069 6e5b 305d 3a2c 203a  self.spin[0]:, :
+00033d60: 5d2c 2064 696d 3d2d 3229 0a20 2020 2020  ], dim=-2).     
+00033d70: 2020 2020 2020 2023 2074 656d 706f 7261         # tempora
+00033d80: 7279 206c 6973 7473 2063 6f6e 7461 696e  ry lists contain
+00033d90: 696e 6720 6561 6368 2065 6c65 6374 726f  ing each electro
+00033da0: 6e27 7320 656d 6265 6464 696e 6773 2077  n's embeddings w
+00033db0: 6869 6368 2077 696c 6c20 6265 2074 6f72  hich will be tor
+00033dc0: 6368 2e73 7461 636b 206f 6e20 7468 6520  ch.stack on the 
+00033dd0: 656e 640a 2020 2020 2020 2020 2020 2020  end.            
+00033de0: 6f6e 655f 656c 6563 7472 6f6e 5f74 6d70  one_electron_tmp
+00033df0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+00033e00: 2020 7477 6f5f 656c 6563 7472 6f6e 5f74    two_electron_t
+00033e10: 6d70 203d 205b 5d0a 2020 2020 2020 2020  mp = [].        
+00033e20: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00033e30: 6765 2873 656c 662e 746f 7461 6c5f 656c  ge(self.total_el
+00033e40: 6563 7472 6f6e 293a 0a20 2020 2020 2020  ectron):.       
+00033e50: 2020 2020 2020 2020 2023 2043 616c 6375           # Calcu
+00033e60: 6c61 7469 6e67 2074 776f 2d65 6c65 6374  lating two-elect
+00033e70: 726f 6e20 6665 6174 7572 6527 7320 6176  ron feature's av
+00033e80: 6572 6167 650a 2020 2020 2020 2020 2020  erage.          
+00033e90: 2020 2020 2020 675f 7477 6f5f 7570 3a20        g_two_up: 
+00033ea0: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+00033eb0: 6f72 6368 2e6d 6561 6e28 0a20 2020 2020  orch.mean(.     
+00033ec0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00033ed0: 776f 5f65 6c65 6374 726f 6e5b 3a2c 2069  wo_electron[:, i
+00033ee0: 2c20 3a73 656c 662e 7370 696e 5b30 5d2c  , :self.spin[0],
+00033ef0: 203a 5d2c 2064 696d 3d31 290a 2020 2020   :], dim=1).    
+00033f00: 2020 2020 2020 2020 2020 2020 675f 7477              g_tw
+00033f10: 6f5f 646f 776e 3a20 746f 7263 682e 5465  o_down: torch.Te
+00033f20: 6e73 6f72 203d 2074 6f72 6368 2e6d 6561  nsor = torch.mea
+00033f30: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00033f40: 2020 2020 2020 2074 776f 5f65 6c65 6374         two_elect
+00033f50: 726f 6e5b 3a2c 2069 2c20 7365 6c66 2e73  ron[:, i, self.s
+00033f60: 7069 6e5b 305d 3a2c 203a 5d2c 2064 696d  pin[0]:, :], dim
+00033f70: 3d31 290a 2020 2020 2020 2020 2020 2020  =1).            
+00033f80: 2020 2020 663a 2074 6f72 6368 2e54 656e      f: torch.Ten
+00033f90: 736f 7220 3d20 746f 7263 682e 6361 7428  sor = torch.cat(
+00033fa0: 286f 6e65 5f65 6c65 6374 726f 6e5b 3a2c  (one_electron[:,
+00033fb0: 2069 2c20 3a5d 2c20 675f 6f6e 655f 7570   i, :], g_one_up
+00033fc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00033fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033fe0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00033ff0: 5f6f 6e65 5f64 6f77 6e2c 2067 5f74 776f  _one_down, g_two
+00034000: 5f75 702c 2067 5f74 776f 5f64 6f77 6e29  _up, g_two_down)
+00034010: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00034020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034030: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00034040: 6d3d 3129 0a20 2020 2020 2020 2020 2020  m=1).           
+00034050: 2020 2020 2069 6620 6c20 3d3d 2030 206f       if l == 0 o
+00034060: 7220 2873 656c 662e 6e5f 6f6e 655b 6c5d  r (self.n_one[l]
+00034070: 2021 3d20 7365 6c66 2e6e 5f6f 6e65 5b6c   != self.n_one[l
+00034080: 202d 2031 5d29 206f 7220 280a 2020 2020   - 1]) or (.    
 00034090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000340a0: 7365 6c66 2e70 726f 6a65 6374 696f 6e5f  self.projection_
-000340b0: 6d6f 6475 6c65 5b30 5d0a 2020 2020 2020  module[0].      
-000340c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000340d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000340e0: 2020 2020 2020 286f 6e65 5f65 6c65 6374        (one_elect
-000340f0: 726f 6e5b 3a2c 2069 2c20 3a5d 2929 0a20  ron[:, i, :])). 
-00034100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034110: 2020 2074 776f 5f65 6c65 6374 726f 6e5f     two_electron_
-00034120: 746d 702e 6170 7065 6e64 280a 2020 2020  tmp.append(.    
-00034130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034140: 2020 2020 2874 6f72 6368 2e74 616e 6828      (torch.tanh(
-00034150: 7365 6c66 2e77 5b6c 5d28 7477 6f5f 656c  self.w[l](two_el
-00034160: 6563 7472 6f6e 5b3a 2c20 692c 203a 2c20  ectron[:, i, :, 
-00034170: 3a5d 2929 2920 2b0a 2020 2020 2020 2020  :]))) +.        
-00034180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034190: 7365 6c66 2e70 726f 6a65 6374 696f 6e5f  self.projection_
-000341a0: 6d6f 6475 6c65 5b31 5d28 7477 6f5f 656c  module[1](two_el
-000341b0: 6563 7472 6f6e 5b3a 2c20 692c 203a 2c20  ectron[:, i, :, 
-000341c0: 3a5d 2929 0a20 2020 2020 2020 2020 2020  :])).           
-000341d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000341e0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000341f0: 6e65 5f65 6c65 6374 726f 6e5f 746d 702e  ne_electron_tmp.
-00034200: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-00034210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034220: 2874 6f72 6368 2e74 616e 6828 7365 6c66  (torch.tanh(self
-00034230: 2e76 5b6c 5d28 6629 2920 2b20 6f6e 655f  .v[l](f)) + one_
-00034240: 656c 6563 7472 6f6e 5b3a 2c20 692c 203a  electron[:, i, :
-00034250: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00034260: 2020 2020 2020 2020 7477 6f5f 656c 6563          two_elec
-00034270: 7472 6f6e 5f74 6d70 2e61 7070 656e 6428  tron_tmp.append(
-00034280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00034290: 2020 2020 2020 2020 2028 746f 7263 682e           (torch.
-000342a0: 7461 6e68 2873 656c 662e 775b 6c5d 2874  tanh(self.w[l](t
-000342b0: 776f 5f65 6c65 6374 726f 6e5b 3a2c 2069  wo_electron[:, i
-000342c0: 2c20 3a2c 203a 5d29 2920 2b0a 2020 2020  , :, :])) +.    
-000342d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000342e0: 2020 2020 2074 776f 5f65 6c65 6374 726f       two_electro
-000342f0: 6e5b 3a2c 2069 2c20 3a2c 203a 5d29 290a  n[:, i, :, :])).
-00034300: 2020 2020 2020 2020 2020 2020 6f6e 655f              one_
-00034310: 656c 6563 7472 6f6e 203d 2074 6f72 6368  electron = torch
-00034320: 2e73 7461 636b 286f 6e65 5f65 6c65 6374  .stack(one_elect
-00034330: 726f 6e5f 746d 702c 2064 696d 3d31 290a  ron_tmp, dim=1).
-00034340: 2020 2020 2020 2020 2020 2020 7477 6f5f              two_
-00034350: 656c 6563 7472 6f6e 203d 2074 6f72 6368  electron = torch
-00034360: 2e73 7461 636b 2874 776f 5f65 6c65 6374  .stack(two_elect
-00034370: 726f 6e5f 746d 702c 2064 696d 3d31 290a  ron_tmp, dim=1).
-00034380: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00034390: 6f6e 655f 656c 6563 7472 6f6e 2c20 7477  one_electron, tw
-000343a0: 6f5f 656c 6563 7472 6f6e 0a0a 0a63 6c61  o_electron...cla
-000343b0: 7373 2046 6572 6d69 6e65 7445 6e76 656c  ss FerminetEnvel
-000343c0: 6f70 6528 746f 7263 682e 6e6e 2e4d 6f64  ope(torch.nn.Mod
-000343d0: 756c 6529 3a0a 2020 2020 2222 220a 2020  ule):.    """.  
-000343e0: 2020 4120 5079 746f 7263 6820 4d6f 6475    A Pytorch Modu
-000343f0: 6c65 2069 6d70 6c65 6d65 6e74 696e 6720  le implementing 
-00034400: 7468 6520 6665 726d 696e 6574 2773 2065  the ferminet's e
-00034410: 6e76 6c6f 7065 206c 6179 6572 205f 5b31  nvlope layer _[1
-00034420: 5d2c 2077 6869 6368 2069 7320 7573 6564  ], which is used
-00034430: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-00034440: 6520 7370 696e 2075 7020 616e 6420 7370  e spin up and sp
-00034450: 696e 2064 6f77 6e20 6f72 6269 7461 6c20  in down orbital 
-00034460: 7661 6c75 6573 2e0a 2020 2020 5468 6973  values..    This
-00034470: 2069 7320 6120 6865 6c70 6572 2063 6c61   is a helper cla
-00034480: 7373 2066 6f72 2074 6865 2046 6572 6d69  ss for the Fermi
-00034490: 6e65 7420 6d6f 6465 6c2e 0a20 2020 2054  net model..    T
-000344a0: 6865 206c 6179 6572 2063 6f6e 7369 7374  he layer consist
-000344b0: 7320 6f66 2034 2074 7970 6573 206f 6620  s of 4 types of 
-000344c0: 7061 7261 6d65 7465 7220 6c69 7374 7320  parameter lists 
-000344d0: 2d20 656e 7665 6c6f 7065 5f77 2c20 656e  - envelope_w, en
-000344e0: 7665 6c6f 7065 5f67 2c20 7369 676d 6120  velope_g, sigma 
-000344f0: 616e 6420 7069 2c20 7768 6963 6820 6865  and pi, which he
-00034500: 6c70 7320 746f 2063 616c 6375 6c61 7465  lps to calculate
-00034510: 2074 6865 206f 7262 6974 616c 2076 6c61   the orbital vla
-00034520: 7565 732e 0a0a 2020 2020 5265 6665 7265  ues...    Refere
-00034530: 6e63 6573 0a20 2020 202d 2d2d 2d2d 2d2d  nces.    -------
-00034540: 2d2d 2d0a 2020 2020 2e2e 205b 315d 2053  ---.    .. [1] S
-00034550: 7065 6e63 6572 2c20 4a61 6d65 7320 532e  pencer, James S.
-00034560: 2c20 6574 2061 6c2e 2042 6574 7465 722c  , et al. Better,
-00034570: 2046 6173 7465 7220 4665 726d 696f 6e69   Faster Fermioni
-00034580: 6320 4e65 7572 616c 204e 6574 776f 726b  c Neural Network
-00034590: 732e 2061 7258 6976 3a32 3031 312e 3037  s. arXiv:2011.07
-000345a0: 3132 352c 2061 7258 6976 2c20 3133 204e  125, arXiv, 13 N
-000345b0: 6f76 2e20 3230 3230 2e20 6172 5869 762e  ov. 2020. arXiv.
-000345c0: 6f72 672c 2068 7474 703a 2f2f 6172 7869  org, http://arxi
-000345d0: 762e 6f72 672f 6162 732f 3230 3131 2e30  v.org/abs/2011.0
-000345e0: 3731 3235 2e0a 0a20 2020 2045 7861 6d70  7125...    Examp
-000345f0: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-00034600: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
-00034610: 6465 6570 6368 656d 2061 7320 6463 0a20  deepchem as dc. 
-00034620: 2020 203e 3e3e 2069 6d70 6f72 7420 746f     >>> import to
-00034630: 7263 680a 2020 2020 3e3e 3e20 656e 7665  rch.    >>> enve
-00034640: 6c6f 7065 5f6c 6179 6572 203d 2064 632e  lope_layer = dc.
-00034650: 6d6f 6465 6c73 2e74 6f72 6368 5f6d 6f64  models.torch_mod
-00034660: 656c 732e 6c61 7965 7273 2e46 6572 6d69  els.layers.Fermi
-00034670: 6e65 7445 6e76 656c 6f70 6528 5b33 322c  netEnvelope([32,
-00034680: 2033 322c 2033 325d 2c20 5b31 362c 2031   32, 32], [16, 1
-00034690: 362c 2031 365d 2c20 3130 2c20 382c 205b  6, 16], 10, 8, [
-000346a0: 352c 2035 5d2c 2035 2c20 3136 290a 2020  5, 5], 5, 16).  
-000346b0: 2020 3e3e 3e20 6f6e 655f 656c 6563 7472    >>> one_electr
-000346c0: 6f6e 203d 2074 6f72 6368 2e72 616e 646e  on = torch.randn
-000346d0: 2838 2c20 3130 2c20 3332 290a 2020 2020  (8, 10, 32).    
-000346e0: 3e3e 3e20 6f6e 655f 656c 6563 7472 6f6e  >>> one_electron
-000346f0: 5f70 6572 6d75 7465 6420 3d20 746f 7263  _permuted = torc
-00034700: 682e 7261 6e64 6e28 382c 2031 302c 2035  h.randn(8, 10, 5
-00034710: 2c20 3329 0a20 2020 203e 3e3e 2070 7369  , 3).    >>> psi
-00034720: 2c20 7073 695f 7570 2c20 7073 695f 646f  , psi_up, psi_do
-00034730: 776e 203d 2065 6e76 656c 6f70 655f 6c61  wn = envelope_la
-00034740: 7965 722e 666f 7277 6172 6428 6f6e 655f  yer.forward(one_
-00034750: 656c 6563 7472 6f6e 2c20 6f6e 655f 656c  electron, one_el
-00034760: 6563 7472 6f6e 5f70 6572 6d75 7465 6429  ectron_permuted)
-00034770: 0a20 2020 203e 3e3e 2070 7369 2e73 697a  .    >>> psi.siz
-00034780: 6528 290a 2020 2020 746f 7263 682e 5369  e().    torch.Si
-00034790: 7a65 285b 385d 290a 2020 2020 3e3e 3e20  ze([8]).    >>> 
-000347a0: 7073 695f 7570 2e73 697a 6528 290a 2020  psi_up.size().  
-000347b0: 2020 746f 7263 682e 5369 7a65 285b 382c    torch.Size([8,
-000347c0: 2031 362c 2035 2c20 355d 290a 2020 2020   16, 5, 5]).    
-000347d0: 3e3e 3e20 7073 695f 646f 776e 2e73 697a  >>> psi_down.siz
-000347e0: 6528 290a 2020 2020 746f 7263 682e 5369  e().    torch.Si
-000347f0: 7a65 285b 382c 2031 362c 2035 2c20 355d  ze([8, 16, 5, 5]
-00034800: 290a 2020 2020 2222 220a 0a20 2020 2064  ).    """..    d
-00034810: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00034820: 2c20 6e5f 6f6e 653a 204c 6973 745b 696e  , n_one: List[in
-00034830: 745d 2c20 6e5f 7477 6f3a 204c 6973 745b  t], n_two: List[
-00034840: 696e 745d 2c20 746f 7461 6c5f 656c 6563  int], total_elec
-00034850: 7472 6f6e 3a20 696e 742c 0a20 2020 2020  tron: int,.     
-00034860: 2020 2020 2020 2020 2020 2020 6261 7463              batc
-00034870: 685f 7369 7a65 3a20 696e 742c 2073 7069  h_size: int, spi
-00034880: 6e3a 204c 6973 745b 696e 745d 2c20 6e6f  n: List[int], no
-00034890: 5f6f 665f 6174 6f6d 733a 2069 6e74 2c0a  _of_atoms: int,.
-000348a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000348b0: 2064 6574 6572 6d69 6e61 6e74 3a20 696e   determinant: in
-000348c0: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
-000348d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000348e0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000348f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e5f  -----.        n_
-00034900: 6f6e 653a 204c 6973 745b 696e 745d 0a20  one: List[int]. 
-00034910: 2020 2020 2020 2020 2020 204c 6973 7420             List 
-00034920: 6f66 2069 6e74 6567 6572 2076 616c 7565  of integer value
-00034930: 7320 636f 6e74 6169 6e69 6e67 2074 6865  s containing the
-00034940: 2064 696d 656e 7369 6f6e 7320 6f66 2065   dimensions of e
-00034950: 6163 6820 6e5f 6f6e 6520 6c61 7965 7227  ach n_one layer'
-00034960: 7320 6f75 7470 7574 0a20 2020 2020 2020  s output.       
-00034970: 206e 5f74 776f 3a20 4c69 7374 5b69 6e74   n_two: List[int
-00034980: 5d0a 2020 2020 2020 2020 2020 2020 4c69  ].            Li
-00034990: 7374 206f 6620 696e 7465 6765 7220 7661  st of integer va
-000349a0: 6c75 6573 2063 6f6e 7461 696e 696e 6720  lues containing 
-000349b0: 7468 6520 6469 6d65 6e73 696f 6e73 206f  the dimensions o
-000349c0: 6620 6561 6368 206e 5f6f 6e65 206c 6179  f each n_one lay
-000349d0: 6572 2773 206f 7574 7075 740a 2020 2020  er's output.    
-000349e0: 2020 2020 746f 7461 6c5f 656c 6563 7472      total_electr
-000349f0: 6f6e 3a20 696e 740a 2020 2020 2020 2020  on: int.        
-00034a00: 2020 2020 5661 6c75 6520 636f 6e74 6169      Value contai
-00034a10: 6e69 6e67 2074 6865 2074 6f74 616c 206e  ning the total n
-00034a20: 756d 6265 7220 6f66 2065 6c65 6374 726f  umber of electro
-00034a30: 6e73 2069 6e20 7468 6520 6d6f 6c65 6375  ns in the molecu
-00034a40: 6c65 2073 7973 7465 6d0a 2020 2020 2020  le system.      
-00034a50: 2020 6261 7463 685f 7369 7a65 3a20 696e    batch_size: in
-00034a60: 740a 2020 2020 2020 2020 2020 2020 5661  t.            Va
-00034a70: 6c75 6520 636f 6e74 6169 6e69 6e67 2074  lue containing t
-00034a80: 6865 206e 756d 6265 7220 6f66 2062 6174  he number of bat
-00034a90: 6368 6573 2066 6f72 2074 6865 2069 6e70  ches for the inp
-00034aa0: 7574 2070 726f 7669 6465 640a 2020 2020  ut provided.    
-00034ab0: 2020 2020 7370 696e 3a20 4c69 7374 5b69      spin: List[i
-00034ac0: 6e74 5d0a 2020 2020 2020 2020 2020 2020  nt].            
-00034ad0: 4c69 7374 2064 6174 6120 7374 7275 6374  List data struct
-00034ae0: 7572 6520 696e 2074 6865 2066 6f72 6d61  ure in the forma
-00034af0: 7420 6f66 205b 6e75 6d62 6572 206f 6620  t of [number of 
-00034b00: 7570 2d73 7069 6e20 656c 6563 7472 6f6e  up-spin electron
-00034b10: 732c 206e 756d 6265 7220 6f66 2064 6f77  s, number of dow
-00034b20: 6e2d 7370 696e 2065 6c65 6374 726f 6e73  n-spin electrons
-00034b30: 5d0a 2020 2020 2020 2020 6e6f 5f6f 665f  ].        no_of_
-00034b40: 6174 6f6d 733a 2069 6e74 0a20 2020 2020  atoms: int.     
-00034b50: 2020 2020 2020 2056 616c 7565 2063 6f6e         Value con
-00034b60: 7461 696e 696e 6720 7468 6520 6e75 6d62  taining the numb
-00034b70: 6572 206f 6620 6174 6f6d 7320 696e 2074  er of atoms in t
-00034b80: 6865 206d 6f6c 6563 756c 6520 7379 7374  he molecule syst
-00034b90: 656d 0a20 2020 2020 2020 2064 6574 6572  em.        deter
-00034ba0: 6d69 6e61 6e74 3a20 696e 740a 2020 2020  minant: int.    
-00034bb0: 2020 2020 2020 2020 5468 6520 6e75 6d62          The numb
-00034bc0: 6572 206f 6620 6465 7465 726d 696e 616e  er of determinan
-00034bd0: 7473 2074 6f20 6265 2069 6e63 6f72 706f  ts to be incorpo
-00034be0: 7261 7465 6420 696e 2074 6865 2070 6f73  rated in the pos
-00034bf0: 742d 4846 2073 6f6c 7574 696f 6e2e 0a20  t-HF solution.. 
-00034c00: 2020 2020 2020 2065 6e76 656c 6f70 655f         envelope_
-00034c10: 773a 2074 6f72 6368 2e6e 6e2e 5061 7261  w: torch.nn.Para
-00034c20: 6d65 7465 724c 6973 740a 2020 2020 2020  meterList.      
-00034c30: 2020 2020 2020 746f 7263 6820 5061 7261        torch Para
-00034c40: 6d65 7465 724c 6973 7420 636f 6e74 6169  meterList contai
-00034c50: 6e69 6e67 2074 6865 2074 6f72 6368 2054  ning the torch T
-00034c60: 656e 736f 7220 7769 7468 206e 5f6f 6e65  ensor with n_one
-00034c70: 206c 6179 6572 2773 2064 696d 656e 7369   layer's dimensi
-00034c80: 6f6e 2073 697a 652e 0a20 2020 2020 2020  on size..       
-00034c90: 2065 6e76 656c 6f70 655f 673a 2074 6f72   envelope_g: tor
-00034ca0: 6368 2e6e 6e2e 5061 7261 6d65 7465 724c  ch.nn.ParameterL
-00034cb0: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
-00034cc0: 746f 7263 6820 5061 7261 6d65 7465 724c  torch ParameterL
-00034cd0: 6973 7420 636f 6e74 6169 6e69 6e67 2074  ist containing t
-00034ce0: 6865 2074 6f72 6368 2054 656e 736f 7220  he torch Tensor 
-00034cf0: 7769 7468 2074 6865 2075 6e69 7420 6469  with the unit di
-00034d00: 6d65 6e73 696f 6e20 7369 7a65 2c20 7768  mension size, wh
-00034d10: 6963 6820 6163 7473 2061 7320 6269 6173  ich acts as bias
-00034d20: 2e0a 2020 2020 2020 2020 7369 676d 613a  ..        sigma:
-00034d30: 2074 6f72 6368 2e6e 6e2e 5061 7261 6d65   torch.nn.Parame
-00034d40: 7465 724c 6973 740a 2020 2020 2020 2020  terList.        
-00034d50: 2020 2020 746f 7263 6820 5061 7261 6d65      torch Parame
-00034d60: 7465 724c 6973 7420 636f 6e74 6169 6e69  terList containi
-00034d70: 6e67 2074 6865 2074 6f72 6368 2054 656e  ng the torch Ten
-00034d80: 736f 7220 7769 7468 2074 6865 2075 6e69  sor with the uni
-00034d90: 7420 6469 6d65 6e73 696f 6e20 7369 7a65  t dimension size
-00034da0: 2e0a 2020 2020 2020 2020 7069 3a20 746f  ..        pi: to
-00034db0: 7263 682e 6e6e 2e50 6172 616d 6574 6572  rch.nn.Parameter
-00034dc0: 4c69 7374 0a20 2020 2020 2020 2020 2020  List.           
-00034dd0: 2074 6f72 6368 2050 6172 616d 6574 6572   torch Parameter
-00034de0: 4c69 7374 2063 6f6e 7461 696e 696e 6720  List containing 
-00034df0: 7468 6520 6c69 6e65 6172 206c 6179 6572  the linear layer
-00034e00: 2077 6974 6820 7468 6520 6e5f 7477 6f20   with the n_two 
-00034e10: 6c61 7965 7227 7320 6469 6d65 6e73 696f  layer's dimensio
-00034e20: 6e20 7369 7a65 2e0a 2020 2020 2020 2020  n size..        
-00034e30: 6c61 7965 725f 7369 7a65 3a20 696e 740a  layer_size: int.
-00034e40: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
-00034e50: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
-00034e60: 206e 756d 6265 7220 6f66 206e 5f6f 6e65   number of n_one
-00034e70: 2061 6e64 206e 5f74 776f 206c 6179 6572   and n_two layer
-00034e80: 730a 2020 2020 2020 2020 2222 220a 0a20  s.        """.. 
-00034e90: 2020 2020 2020 2073 7570 6572 2846 6572         super(Fer
-00034ea0: 6d69 6e65 7445 6e76 656c 6f70 652c 2073  minetEnvelope, s
-00034eb0: 656c 6629 2e5f 5f69 6e69 745f 5f28 290a  elf).__init__().
-00034ec0: 2020 2020 2020 2020 7365 6c66 2e6e 5f6f          self.n_o
-00034ed0: 6e65 203d 206e 5f6f 6e65 0a20 2020 2020  ne = n_one.     
-00034ee0: 2020 2073 656c 662e 6e5f 7477 6f20 3d20     self.n_two = 
-00034ef0: 6e5f 7477 6f0a 2020 2020 2020 2020 7365  n_two.        se
-00034f00: 6c66 2e74 6f74 616c 5f65 6c65 6374 726f  lf.total_electro
-00034f10: 6e20 3d20 746f 7461 6c5f 656c 6563 7472  n = total_electr
-00034f20: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
-00034f30: 6261 7463 685f 7369 7a65 203d 2062 6174  batch_size = bat
-00034f40: 6368 5f73 697a 650a 2020 2020 2020 2020  ch_size.        
-00034f50: 7365 6c66 2e73 7069 6e20 3d20 7370 696e  self.spin = spin
-00034f60: 0a20 2020 2020 2020 2073 656c 662e 6e6f  .        self.no
-00034f70: 5f6f 665f 6174 6f6d 7320 3d20 6e6f 5f6f  _of_atoms = no_o
-00034f80: 665f 6174 6f6d 730a 2020 2020 2020 2020  f_atoms.        
-00034f90: 7365 6c66 2e64 6574 6572 6d69 6e61 6e74  self.determinant
-00034fa0: 203d 2064 6574 6572 6d69 6e61 6e74 0a0a   = determinant..
-00034fb0: 2020 2020 2020 2020 7365 6c66 2e6c 6179          self.lay
-00034fc0: 6572 5f73 697a 653a 2069 6e74 203d 206c  er_size: int = l
-00034fd0: 656e 2873 656c 662e 6e5f 6f6e 6529 0a0a  en(self.n_one)..
-00034fe0: 2020 2020 2020 2020 7365 6c66 2e65 6e76          self.env
-00034ff0: 656c 6f70 655f 7720 3d20 746f 7263 682e  elope_w = torch.
-00035000: 6e6e 2e50 6172 616d 6574 6572 4c69 7374  nn.ParameterList
-00035010: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00035020: 656e 7665 6c6f 7065 5f67 203d 2074 6f72  envelope_g = tor
-00035030: 6368 2e6e 6e2e 5061 7261 6d65 7465 724c  ch.nn.ParameterL
-00035040: 6973 7428 290a 2020 2020 2020 2020 7365  ist().        se
-00035050: 6c66 2e73 6967 6d61 203d 2074 6f72 6368  lf.sigma = torch
-00035060: 2e6e 6e2e 5061 7261 6d65 7465 724c 6973  .nn.ParameterLis
-00035070: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-00035080: 2e70 6920 3d20 746f 7263 682e 6e6e 2e50  .pi = torch.nn.P
-00035090: 6172 616d 6574 6572 4c69 7374 2829 0a20  arameterList(). 
-000350a0: 2020 2020 2020 2073 656c 662e 7764 6574         self.wdet
-000350b0: 203d 2074 6f72 6368 2e6e 6e2e 5061 7261   = torch.nn.Para
-000350c0: 6d65 7465 724c 6973 7428 290a 0a20 2020  meterList()..   
-000350d0: 2020 2020 2023 2069 6e69 7469 616c 697a       # initializ
-000350e0: 6564 2077 6569 6768 7473 2077 6974 6820  ed weights with 
-000350f0: 746f 7263 682e 7a65 726f 732c 2074 6f72  torch.zeros, tor
-00035100: 6368 2e65 7965 2061 6e64 2075 7369 6e67  ch.eye and using
-00035110: 2078 6176 6965 7220 696e 6974 2e0a 2020   xavier init..  
-00035120: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00035130: 616e 6765 2873 656c 662e 6465 7465 726d  ange(self.determ
-00035140: 696e 616e 7429 3a0a 2020 2020 2020 2020  inant):.        
-00035150: 2020 2020 7365 6c66 2e77 6465 742e 6170      self.wdet.ap
-00035160: 7065 6e64 2874 6f72 6368 2e6e 6e2e 696e  pend(torch.nn.in
-00035170: 6974 2e6e 6f72 6d61 6c5f 2874 6f72 6368  it.normal_(torch
-00035180: 2e7a 6572 6f73 2831 2929 2e73 7175 6565  .zeros(1)).squee
-00035190: 7a65 2830 2929 0a20 2020 2020 2020 2020  ze(0)).         
-000351a0: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-000351b0: 6528 7365 6c66 2e74 6f74 616c 5f65 6c65  e(self.total_ele
-000351c0: 6374 726f 6e29 3a0a 2020 2020 2020 2020  ctron):.        
-000351d0: 2020 2020 2020 2020 7365 6c66 2e65 6e76          self.env
-000351e0: 656c 6f70 655f 772e 6170 7065 6e64 280a  elope_w.append(.
-000351f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035200: 2020 2020 2874 6f72 6368 2e6e 6e2e 696e      (torch.nn.in
-00035210: 6974 2e6e 6f72 6d61 6c5f 2874 6f72 6368  it.normal_(torch
-00035220: 2e7a 6572 6f73 286e 5f6f 6e65 5b2d 315d  .zeros(n_one[-1]
-00035230: 2c20 3129 2c29 202f 0a20 2020 2020 2020  , 1),) /.       
-00035240: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00035250: 7468 2e73 7172 7428 6e5f 6f6e 655b 2d31  th.sqrt(n_one[-1
-00035260: 5d29 292e 7371 7565 657a 6528 2d31 2929  ])).squeeze(-1))
-00035270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00035280: 2073 656c 662e 656e 7665 6c6f 7065 5f67   self.envelope_g
-00035290: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-000352a0: 2020 2020 2020 2020 2020 2020 2028 746f               (to
-000352b0: 7263 682e 6e6e 2e69 6e69 742e 6e6f 726d  rch.nn.init.norm
-000352c0: 616c 5f28 746f 7263 682e 7a65 726f 7328  al_(torch.zeros(
-000352d0: 3129 2929 2e73 7175 6565 7a65 2830 2929  1))).squeeze(0))
-000352e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000352f0: 2066 6f72 206b 2069 6e20 7261 6e67 6528   for k in range(
-00035300: 7365 6c66 2e6e 6f5f 6f66 5f61 746f 6d73  self.no_of_atoms
-00035310: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00035320: 2020 2020 2020 2073 656c 662e 7069 2e61         self.pi.a
-00035330: 7070 656e 6428 2874 6f72 6368 2e7a 6572  ppend((torch.zer
-00035340: 6f73 2831 2929 290a 2020 2020 2020 2020  os(1))).        
-00035350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00035360: 2e73 6967 6d61 2e61 7070 656e 6428 746f  .sigma.append(to
-00035370: 7263 682e 6579 6528 3329 290a 0a20 2020  rch.eye(3))..   
-00035380: 2064 6566 2066 6f72 7761 7264 2873 656c   def forward(sel
-00035390: 662c 206f 6e65 5f65 6c65 6374 726f 6e3a  f, one_electron:
-000353a0: 2074 6f72 6368 2e54 656e 736f 722c 0a20   torch.Tensor,. 
-000353b0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000353c0: 6e65 5f65 6c65 6374 726f 6e5f 7665 6374  ne_electron_vect
-000353d0: 6f72 5f70 6572 6d75 7465 643a 2074 6f72  or_permuted: tor
-000353e0: 6368 2e54 656e 736f 7229 3a0a 2020 2020  ch.Tensor):.    
-000353f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00035400: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00035410: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00035420: 2020 2020 2020 6f6e 655f 656c 6563 7472        one_electr
-00035430: 6f6e 3a20 746f 7263 682e 5465 6e73 6f72  on: torch.Tensor
-00035440: 0a20 2020 2020 2020 2020 2020 2054 6f72  .            Tor
-00035450: 6368 2074 656e 736f 7220 7768 6963 6820  ch tensor which 
-00035460: 6973 206f 7574 7075 7420 6672 6f6d 2046  is output from F
-00035470: 6572 6d69 6e45 6c65 6374 726f 6e46 6561  erminElectronFea
-00035480: 7475 7265 206c 6179 6572 2069 6e20 7468  ture layer in th
-00035490: 6520 7368 6170 6520 6f66 2028 6261 7463  e shape of (batc
-000354a0: 685f 7369 7a65 2c20 6e75 6d62 6572 206f  h_size, number o
-000354b0: 6620 656c 6374 726f 6e73 2c20 6e5f 6f6e  f elctrons, n_on
-000354c0: 6520 6c61 7965 7220 7369 7a65 292e 0a20  e layer size).. 
-000354d0: 2020 2020 2020 206f 6e65 5f65 6c65 6374         one_elect
-000354e0: 726f 6e5f 7665 6374 6f72 5f70 6572 6d75  ron_vector_permu
-000354f0: 7465 643a 2074 6f72 6368 2e54 656e 736f  ted: torch.Tenso
-00035500: 720a 2020 2020 2020 2020 2020 2020 546f  r.            To
-00035510: 7263 6820 7465 6e73 6f72 2077 6869 6368  rch tensor which
-00035520: 2069 7320 7368 6170 6520 7065 726d 7574   is shape permut
-00035530: 6564 2076 6563 746f 7220 6f66 2074 6865  ed vector of the
-00035540: 206f 7269 6769 6e61 6c20 6f6e 655f 656c   original one_el
-00035550: 6563 7472 6f6e 2076 6563 746f 7220 7465  ectron vector te
-00035560: 6e73 6f72 2e20 7368 6170 6520 6f66 2074  nsor. shape of t
-00035570: 6865 2074 656e 736f 7220 7368 6f75 6c64  he tensor should
-00035580: 2062 6520 2862 6174 6368 5f73 697a 652c   be (batch_size,
-00035590: 206e 756d 6265 7220 6f66 2061 746f 6d73   number of atoms
-000355a0: 2c20 6e75 6d62 6572 206f 6620 656c 6563  , number of elec
-000355b0: 7472 6f6e 732c 2033 292e 0a0a 2020 2020  trons, 3)...    
-000355c0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000355d0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-000355e0: 2020 2020 7073 695f 7570 3a20 746f 7263      psi_up: torc
-000355f0: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
-00035600: 2020 2020 2054 6f72 6368 2074 656e 736f       Torch tenso
-00035610: 7220 7769 7468 2061 2073 6361 6c61 7220  r with a scalar 
-00035620: 7661 6c75 6520 636f 6e74 6169 6e69 6e67  value containing
-00035630: 2074 6865 2073 616d 706c 6564 2077 6176   the sampled wav
-00035640: 6566 756e 6374 696f 6e20 7661 6c75 6520  efunction value 
-00035650: 666f 7220 6561 6368 2062 6174 6368 2e0a  for each batch..
-00035660: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00035670: 2020 2020 7073 6920 3d20 746f 7263 682e      psi = torch.
-00035680: 7a65 726f 7328 7365 6c66 2e62 6174 6368  zeros(self.batch
-00035690: 5f73 697a 6529 0a20 2020 2020 2020 2070  _size).        p
-000356a0: 7369 5f75 7020 3d20 5b5d 0a20 2020 2020  si_up = [].     
-000356b0: 2020 2070 7369 5f64 6f77 6e20 3d20 5b5d     psi_down = []
-000356c0: 0a20 2020 2020 2020 2066 6f72 206b 2069  .        for k i
-000356d0: 6e20 7261 6e67 6528 7365 6c66 2e64 6574  n range(self.det
-000356e0: 6572 6d69 6e61 6e74 293a 0a20 2020 2020  erminant):.     
-000356f0: 2020 2020 2020 2023 2074 656d 706f 7261         # tempora
-00035700: 7279 206c 6973 7420 746f 2073 7461 636b  ry list to stack
-00035710: 2075 706f 6e20 656c 6563 7472 6f6e 7320   upon electrons 
-00035720: 6178 6973 2061 7420 7468 6520 656e 640a  axis at the end.
-00035730: 2020 2020 2020 2020 2020 2020 6465 7420              det 
-00035740: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-00035750: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00035760: 7365 6c66 2e73 7069 6e5b 305d 293a 0a20  self.spin[0]):. 
-00035770: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00035780: 6e65 5f64 5f69 6e64 6578 203d 2028 6b20  ne_d_index = (k 
-00035790: 2a20 2873 656c 662e 746f 7461 6c5f 656c  * (self.total_el
-000357a0: 6563 7472 6f6e 2929 202b 2069 0a20 2020  ectron)) + i.   
-000357b0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000357c0: 206a 2069 6e20 7261 6e67 6528 7365 6c66   j in range(self
-000357d0: 2e73 7069 6e5b 305d 293a 0a20 2020 2020  .spin[0]):.     
-000357e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000357f0: 6574 2e61 7070 656e 6428 2828 746f 7263  et.append(((torc
-00035800: 682e 7375 6d28 0a20 2020 2020 2020 2020  h.sum(.         
-00035810: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00035820: 7365 6c66 2e65 6e76 656c 6f70 655f 775b  self.envelope_w[
-00035830: 6f6e 655f 645f 696e 6465 785d 202a 206f  one_d_index] * o
-00035840: 6e65 5f65 6c65 6374 726f 6e5b 3a2c 206a  ne_electron[:, j
-00035850: 2c20 3a5d 2920 2b0a 2020 2020 2020 2020  , :]) +.        
-00035860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035870: 7365 6c66 2e65 6e76 656c 6f70 655f 675b  self.envelope_g[
-00035880: 6f6e 655f 645f 696e 6465 785d 2c0a 2020  one_d_index],.  
-00035890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000358a0: 2020 2020 2020 6469 6d3d 3129 2920 2a20        dim=1)) * 
-000358b0: 746f 7263 682e 7375 6d28 746f 7263 682e  torch.sum(torch.
-000358c0: 6578 7028 2d74 6f72 6368 2e61 6273 280a  exp(-torch.abs(.
-000358d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000358e0: 2020 2020 2020 2020 2020 2020 746f 7263              torc
-000358f0: 682e 6e6f 726d 286f 6e65 5f65 6c65 6374  h.norm(one_elect
-00035900: 726f 6e5f 7665 6374 6f72 5f70 6572 6d75  ron_vector_permu
-00035910: 7465 645b 3a2c 206a 2c20 3a2c 203a 5d0a  ted[:, j, :, :].
-00035920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000340a0: 2020 2020 7365 6c66 2e6e 5f74 776f 5b6c      self.n_two[l
+000340b0: 5d20 213d 2073 656c 662e 6e5f 7477 6f5b  ] != self.n_two[
+000340c0: 6c20 2d20 315d 293a 0a20 2020 2020 2020  l - 1]):.       
+000340d0: 2020 2020 2020 2020 2020 2020 206f 6e65               one
+000340e0: 5f65 6c65 6374 726f 6e5f 746d 702e 6170  _electron_tmp.ap
+000340f0: 7065 6e64 2828 746f 7263 682e 7461 6e68  pend((torch.tanh
+00034100: 2873 656c 662e 765b 6c5d 2866 2929 2920  (self.v[l](f))) 
+00034110: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
+00034120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034130: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00034140: 6c66 2e70 726f 6a65 6374 696f 6e5f 6d6f  lf.projection_mo
+00034150: 6475 6c65 5b30 5d0a 2020 2020 2020 2020  dule[0].        
+00034160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034180: 2020 2020 286f 6e65 5f65 6c65 6374 726f      (one_electro
+00034190: 6e5b 3a2c 2069 2c20 3a5d 2929 0a20 2020  n[:, i, :])).   
+000341a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000341b0: 2074 776f 5f65 6c65 6374 726f 6e5f 746d   two_electron_tm
+000341c0: 702e 6170 7065 6e64 280a 2020 2020 2020  p.append(.      
+000341d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000341e0: 2020 2874 6f72 6368 2e74 616e 6828 7365    (torch.tanh(se
+000341f0: 6c66 2e77 5b6c 5d28 7477 6f5f 656c 6563  lf.w[l](two_elec
+00034200: 7472 6f6e 5b3a 2c20 692c 203a 2c20 3a5d  tron[:, i, :, :]
+00034210: 2929 2920 2b0a 2020 2020 2020 2020 2020  ))) +.          
+00034220: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00034230: 6c66 2e70 726f 6a65 6374 696f 6e5f 6d6f  lf.projection_mo
+00034240: 6475 6c65 5b31 5d28 7477 6f5f 656c 6563  dule[1](two_elec
+00034250: 7472 6f6e 5b3a 2c20 692c 203a 2c20 3a5d  tron[:, i, :, :]
+00034260: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00034270: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00034280: 2020 2020 2020 2020 2020 2020 206f 6e65               one
+00034290: 5f65 6c65 6374 726f 6e5f 746d 702e 6170  _electron_tmp.ap
+000342a0: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+000342b0: 2020 2020 2020 2020 2020 2020 2020 2874                (t
+000342c0: 6f72 6368 2e74 616e 6828 7365 6c66 2e76  orch.tanh(self.v
+000342d0: 5b6c 5d28 6629 2920 2b20 6f6e 655f 656c  [l](f)) + one_el
+000342e0: 6563 7472 6f6e 5b3a 2c20 692c 203a 5d29  ectron[:, i, :])
+000342f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00034300: 2020 2020 2020 7477 6f5f 656c 6563 7472        two_electr
+00034310: 6f6e 5f74 6d70 2e61 7070 656e 6428 0a20  on_tmp.append(. 
+00034320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034330: 2020 2020 2020 2028 746f 7263 682e 7461         (torch.ta
+00034340: 6e68 2873 656c 662e 775b 6c5d 2874 776f  nh(self.w[l](two
+00034350: 5f65 6c65 6374 726f 6e5b 3a2c 2069 2c20  _electron[:, i, 
+00034360: 3a2c 203a 5d29 2920 2b0a 2020 2020 2020  :, :])) +.      
+00034370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034380: 2020 2074 776f 5f65 6c65 6374 726f 6e5b     two_electron[
+00034390: 3a2c 2069 2c20 3a2c 203a 5d29 290a 2020  :, i, :, :])).  
+000343a0: 2020 2020 2020 2020 2020 6f6e 655f 656c            one_el
+000343b0: 6563 7472 6f6e 203d 2074 6f72 6368 2e73  ectron = torch.s
+000343c0: 7461 636b 286f 6e65 5f65 6c65 6374 726f  tack(one_electro
+000343d0: 6e5f 746d 702c 2064 696d 3d31 290a 2020  n_tmp, dim=1).  
+000343e0: 2020 2020 2020 2020 2020 7477 6f5f 656c            two_el
+000343f0: 6563 7472 6f6e 203d 2074 6f72 6368 2e73  ectron = torch.s
+00034400: 7461 636b 2874 776f 5f65 6c65 6374 726f  tack(two_electro
+00034410: 6e5f 746d 702c 2064 696d 3d31 290a 0a20  n_tmp, dim=1).. 
+00034420: 2020 2020 2020 2072 6574 7572 6e20 6f6e         return on
+00034430: 655f 656c 6563 7472 6f6e 2c20 7477 6f5f  e_electron, two_
+00034440: 656c 6563 7472 6f6e 0a0a 0a63 6c61 7373  electron...class
+00034450: 2046 6572 6d69 6e65 7445 6e76 656c 6f70   FerminetEnvelop
+00034460: 6528 746f 7263 682e 6e6e 2e4d 6f64 756c  e(torch.nn.Modul
+00034470: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+00034480: 4120 5079 746f 7263 6820 4d6f 6475 6c65  A Pytorch Module
+00034490: 2069 6d70 6c65 6d65 6e74 696e 6720 7468   implementing th
+000344a0: 6520 6665 726d 696e 6574 2773 2065 6e76  e ferminet's env
+000344b0: 6c6f 7065 206c 6179 6572 205f 5b31 5d2c  lope layer _[1],
+000344c0: 2077 6869 6368 2069 7320 7573 6564 2074   which is used t
+000344d0: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
+000344e0: 7370 696e 2075 7020 616e 6420 7370 696e  spin up and spin
+000344f0: 2064 6f77 6e20 6f72 6269 7461 6c20 7661   down orbital va
+00034500: 6c75 6573 2e0a 2020 2020 5468 6973 2069  lues..    This i
+00034510: 7320 6120 6865 6c70 6572 2063 6c61 7373  s a helper class
+00034520: 2066 6f72 2074 6865 2046 6572 6d69 6e65   for the Fermine
+00034530: 7420 6d6f 6465 6c2e 0a20 2020 2054 6865  t model..    The
+00034540: 206c 6179 6572 2063 6f6e 7369 7374 7320   layer consists 
+00034550: 6f66 2034 2074 7970 6573 206f 6620 7061  of 4 types of pa
+00034560: 7261 6d65 7465 7220 6c69 7374 7320 2d20  rameter lists - 
+00034570: 656e 7665 6c6f 7065 5f77 2c20 656e 7665  envelope_w, enve
+00034580: 6c6f 7065 5f67 2c20 7369 676d 6120 616e  lope_g, sigma an
+00034590: 6420 7069 2c20 7768 6963 6820 6865 6c70  d pi, which help
+000345a0: 7320 746f 2063 616c 6375 6c61 7465 2074  s to calculate t
+000345b0: 6865 206f 7262 6974 616c 2076 6c61 7565  he orbital vlaue
+000345c0: 732e 0a0a 2020 2020 5265 6665 7265 6e63  s...    Referenc
+000345d0: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  es.    ---------
+000345e0: 2d0a 2020 2020 2e2e 205b 315d 2053 7065  -.    .. [1] Spe
+000345f0: 6e63 6572 2c20 4a61 6d65 7320 532e 2c20  ncer, James S., 
+00034600: 6574 2061 6c2e 2042 6574 7465 722c 2046  et al. Better, F
+00034610: 6173 7465 7220 4665 726d 696f 6e69 6320  aster Fermionic 
+00034620: 4e65 7572 616c 204e 6574 776f 726b 732e  Neural Networks.
+00034630: 2061 7258 6976 3a32 3031 312e 3037 3132   arXiv:2011.0712
+00034640: 352c 2061 7258 6976 2c20 3133 204e 6f76  5, arXiv, 13 Nov
+00034650: 2e20 3230 3230 2e20 6172 5869 762e 6f72  . 2020. arXiv.or
+00034660: 672c 2068 7474 703a 2f2f 6172 7869 762e  g, http://arxiv.
+00034670: 6f72 672f 6162 732f 3230 3131 2e30 3731  org/abs/2011.071
+00034680: 3235 2e0a 0a20 2020 2045 7861 6d70 6c65  25...    Example
+00034690: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
+000346a0: 2020 203e 3e3e 2069 6d70 6f72 7420 6465     >>> import de
+000346b0: 6570 6368 656d 2061 7320 6463 0a20 2020  epchem as dc.   
+000346c0: 203e 3e3e 2069 6d70 6f72 7420 746f 7263   >>> import torc
+000346d0: 680a 2020 2020 3e3e 3e20 656e 7665 6c6f  h.    >>> envelo
+000346e0: 7065 5f6c 6179 6572 203d 2064 632e 6d6f  pe_layer = dc.mo
+000346f0: 6465 6c73 2e74 6f72 6368 5f6d 6f64 656c  dels.torch_model
+00034700: 732e 6c61 7965 7273 2e46 6572 6d69 6e65  s.layers.Fermine
+00034710: 7445 6e76 656c 6f70 6528 5b33 322c 2033  tEnvelope([32, 3
+00034720: 322c 2033 325d 2c20 5b31 362c 2031 362c  2, 32], [16, 16,
+00034730: 2031 365d 2c20 3130 2c20 382c 205b 352c   16], 10, 8, [5,
+00034740: 2035 5d2c 2035 2c20 3136 290a 2020 2020   5], 5, 16).    
+00034750: 3e3e 3e20 6f6e 655f 656c 6563 7472 6f6e  >>> one_electron
+00034760: 203d 2074 6f72 6368 2e72 616e 646e 2838   = torch.randn(8
+00034770: 2c20 3130 2c20 3332 290a 2020 2020 3e3e  , 10, 32).    >>
+00034780: 3e20 6f6e 655f 656c 6563 7472 6f6e 5f70  > one_electron_p
+00034790: 6572 6d75 7465 6420 3d20 746f 7263 682e  ermuted = torch.
+000347a0: 7261 6e64 6e28 382c 2031 302c 2035 2c20  randn(8, 10, 5, 
+000347b0: 3329 0a20 2020 203e 3e3e 2070 7369 2c20  3).    >>> psi, 
+000347c0: 7073 695f 7570 2c20 7073 695f 646f 776e  psi_up, psi_down
+000347d0: 203d 2065 6e76 656c 6f70 655f 6c61 7965   = envelope_laye
+000347e0: 722e 666f 7277 6172 6428 6f6e 655f 656c  r.forward(one_el
+000347f0: 6563 7472 6f6e 2c20 6f6e 655f 656c 6563  ectron, one_elec
+00034800: 7472 6f6e 5f70 6572 6d75 7465 6429 0a20  tron_permuted). 
+00034810: 2020 203e 3e3e 2070 7369 2e73 697a 6528     >>> psi.size(
+00034820: 290a 2020 2020 746f 7263 682e 5369 7a65  ).    torch.Size
+00034830: 285b 385d 290a 2020 2020 3e3e 3e20 7073  ([8]).    >>> ps
+00034840: 695f 7570 2e73 697a 6528 290a 2020 2020  i_up.size().    
+00034850: 746f 7263 682e 5369 7a65 285b 382c 2031  torch.Size([8, 1
+00034860: 362c 2035 2c20 355d 290a 2020 2020 3e3e  6, 5, 5]).    >>
+00034870: 3e20 7073 695f 646f 776e 2e73 697a 6528  > psi_down.size(
+00034880: 290a 2020 2020 746f 7263 682e 5369 7a65  ).    torch.Size
+00034890: 285b 382c 2031 362c 2035 2c20 355d 290a  ([8, 16, 5, 5]).
+000348a0: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+000348b0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+000348c0: 6e5f 6f6e 653a 204c 6973 745b 696e 745d  n_one: List[int]
+000348d0: 2c20 6e5f 7477 6f3a 204c 6973 745b 696e  , n_two: List[in
+000348e0: 745d 2c20 746f 7461 6c5f 656c 6563 7472  t], total_electr
+000348f0: 6f6e 3a20 696e 742c 0a20 2020 2020 2020  on: int,.       
+00034900: 2020 2020 2020 2020 2020 6261 7463 685f            batch_
+00034910: 7369 7a65 3a20 696e 742c 2073 7069 6e3a  size: int, spin:
+00034920: 204c 6973 745b 696e 745d 2c20 6e6f 5f6f   List[int], no_o
+00034930: 665f 6174 6f6d 733a 2069 6e74 2c0a 2020  f_atoms: int,.  
+00034940: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00034950: 6574 6572 6d69 6e61 6e74 3a20 696e 7429  eterminant: int)
+00034960: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00034970: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00034980: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00034990: 2d2d 2d0a 2020 2020 2020 2020 6e5f 6f6e  ---.        n_on
+000349a0: 653a 204c 6973 745b 696e 745d 0a20 2020  e: List[int].   
+000349b0: 2020 2020 2020 2020 204c 6973 7420 6f66           List of
+000349c0: 2069 6e74 6567 6572 2076 616c 7565 7320   integer values 
+000349d0: 636f 6e74 6169 6e69 6e67 2074 6865 2064  containing the d
+000349e0: 696d 656e 7369 6f6e 7320 6f66 2065 6163  imensions of eac
+000349f0: 6820 6e5f 6f6e 6520 6c61 7965 7227 7320  h n_one layer's 
+00034a00: 6f75 7470 7574 0a20 2020 2020 2020 206e  output.        n
+00034a10: 5f74 776f 3a20 4c69 7374 5b69 6e74 5d0a  _two: List[int].
+00034a20: 2020 2020 2020 2020 2020 2020 4c69 7374              List
+00034a30: 206f 6620 696e 7465 6765 7220 7661 6c75   of integer valu
+00034a40: 6573 2063 6f6e 7461 696e 696e 6720 7468  es containing th
+00034a50: 6520 6469 6d65 6e73 696f 6e73 206f 6620  e dimensions of 
+00034a60: 6561 6368 206e 5f6f 6e65 206c 6179 6572  each n_one layer
+00034a70: 2773 206f 7574 7075 740a 2020 2020 2020  's output.      
+00034a80: 2020 746f 7461 6c5f 656c 6563 7472 6f6e    total_electron
+00034a90: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+00034aa0: 2020 5661 6c75 6520 636f 6e74 6169 6e69    Value containi
+00034ab0: 6e67 2074 6865 2074 6f74 616c 206e 756d  ng the total num
+00034ac0: 6265 7220 6f66 2065 6c65 6374 726f 6e73  ber of electrons
+00034ad0: 2069 6e20 7468 6520 6d6f 6c65 6375 6c65   in the molecule
+00034ae0: 2073 7973 7465 6d0a 2020 2020 2020 2020   system.        
+00034af0: 6261 7463 685f 7369 7a65 3a20 696e 740a  batch_size: int.
+00034b00: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+00034b10: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
+00034b20: 206e 756d 6265 7220 6f66 2062 6174 6368   number of batch
+00034b30: 6573 2066 6f72 2074 6865 2069 6e70 7574  es for the input
+00034b40: 2070 726f 7669 6465 640a 2020 2020 2020   provided.      
+00034b50: 2020 7370 696e 3a20 4c69 7374 5b69 6e74    spin: List[int
+00034b60: 5d0a 2020 2020 2020 2020 2020 2020 4c69  ].            Li
+00034b70: 7374 2064 6174 6120 7374 7275 6374 7572  st data structur
+00034b80: 6520 696e 2074 6865 2066 6f72 6d61 7420  e in the format 
+00034b90: 6f66 205b 6e75 6d62 6572 206f 6620 7570  of [number of up
+00034ba0: 2d73 7069 6e20 656c 6563 7472 6f6e 732c  -spin electrons,
+00034bb0: 206e 756d 6265 7220 6f66 2064 6f77 6e2d   number of down-
+00034bc0: 7370 696e 2065 6c65 6374 726f 6e73 5d0a  spin electrons].
+00034bd0: 2020 2020 2020 2020 6e6f 5f6f 665f 6174          no_of_at
+00034be0: 6f6d 733a 2069 6e74 0a20 2020 2020 2020  oms: int.       
+00034bf0: 2020 2020 2056 616c 7565 2063 6f6e 7461       Value conta
+00034c00: 696e 696e 6720 7468 6520 6e75 6d62 6572  ining the number
+00034c10: 206f 6620 6174 6f6d 7320 696e 2074 6865   of atoms in the
+00034c20: 206d 6f6c 6563 756c 6520 7379 7374 656d   molecule system
+00034c30: 0a20 2020 2020 2020 2064 6574 6572 6d69  .        determi
+00034c40: 6e61 6e74 3a20 696e 740a 2020 2020 2020  nant: int.      
+00034c50: 2020 2020 2020 5468 6520 6e75 6d62 6572        The number
+00034c60: 206f 6620 6465 7465 726d 696e 616e 7473   of determinants
+00034c70: 2074 6f20 6265 2069 6e63 6f72 706f 7261   to be incorpora
+00034c80: 7465 6420 696e 2074 6865 2070 6f73 742d  ted in the post-
+00034c90: 4846 2073 6f6c 7574 696f 6e2e 0a20 2020  HF solution..   
+00034ca0: 2020 2020 2065 6e76 656c 6f70 655f 773a       envelope_w:
+00034cb0: 2074 6f72 6368 2e6e 6e2e 5061 7261 6d65   torch.nn.Parame
+00034cc0: 7465 724c 6973 740a 2020 2020 2020 2020  terList.        
+00034cd0: 2020 2020 746f 7263 6820 5061 7261 6d65      torch Parame
+00034ce0: 7465 724c 6973 7420 636f 6e74 6169 6e69  terList containi
+00034cf0: 6e67 2074 6865 2074 6f72 6368 2054 656e  ng the torch Ten
+00034d00: 736f 7220 7769 7468 206e 5f6f 6e65 206c  sor with n_one l
+00034d10: 6179 6572 2773 2064 696d 656e 7369 6f6e  ayer's dimension
+00034d20: 2073 697a 652e 0a20 2020 2020 2020 2065   size..        e
+00034d30: 6e76 656c 6f70 655f 673a 2074 6f72 6368  nvelope_g: torch
+00034d40: 2e6e 6e2e 5061 7261 6d65 7465 724c 6973  .nn.ParameterLis
+00034d50: 740a 2020 2020 2020 2020 2020 2020 746f  t.            to
+00034d60: 7263 6820 5061 7261 6d65 7465 724c 6973  rch ParameterLis
+00034d70: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
+00034d80: 2074 6f72 6368 2054 656e 736f 7220 7769   torch Tensor wi
+00034d90: 7468 2074 6865 2075 6e69 7420 6469 6d65  th the unit dime
+00034da0: 6e73 696f 6e20 7369 7a65 2c20 7768 6963  nsion size, whic
+00034db0: 6820 6163 7473 2061 7320 6269 6173 2e0a  h acts as bias..
+00034dc0: 2020 2020 2020 2020 7369 676d 613a 2074          sigma: t
+00034dd0: 6f72 6368 2e6e 6e2e 5061 7261 6d65 7465  orch.nn.Paramete
+00034de0: 724c 6973 740a 2020 2020 2020 2020 2020  rList.          
+00034df0: 2020 746f 7263 6820 5061 7261 6d65 7465    torch Paramete
+00034e00: 724c 6973 7420 636f 6e74 6169 6e69 6e67  rList containing
+00034e10: 2074 6865 2074 6f72 6368 2054 656e 736f   the torch Tenso
+00034e20: 7220 7769 7468 2074 6865 2075 6e69 7420  r with the unit 
+00034e30: 6469 6d65 6e73 696f 6e20 7369 7a65 2e0a  dimension size..
+00034e40: 2020 2020 2020 2020 7069 3a20 746f 7263          pi: torc
+00034e50: 682e 6e6e 2e50 6172 616d 6574 6572 4c69  h.nn.ParameterLi
+00034e60: 7374 0a20 2020 2020 2020 2020 2020 2074  st.            t
+00034e70: 6f72 6368 2050 6172 616d 6574 6572 4c69  orch ParameterLi
+00034e80: 7374 2063 6f6e 7461 696e 696e 6720 7468  st containing th
+00034e90: 6520 6c69 6e65 6172 206c 6179 6572 2077  e linear layer w
+00034ea0: 6974 6820 7468 6520 6e5f 7477 6f20 6c61  ith the n_two la
+00034eb0: 7965 7227 7320 6469 6d65 6e73 696f 6e20  yer's dimension 
+00034ec0: 7369 7a65 2e0a 2020 2020 2020 2020 6c61  size..        la
+00034ed0: 7965 725f 7369 7a65 3a20 696e 740a 2020  yer_size: int.  
+00034ee0: 2020 2020 2020 2020 2020 5661 6c75 6520            Value 
+00034ef0: 636f 6e74 6169 6e69 6e67 2074 6865 206e  containing the n
+00034f00: 756d 6265 7220 6f66 206e 5f6f 6e65 2061  umber of n_one a
+00034f10: 6e64 206e 5f74 776f 206c 6179 6572 730a  nd n_two layers.
+00034f20: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00034f30: 2020 2020 2073 7570 6572 2846 6572 6d69       super(Fermi
+00034f40: 6e65 7445 6e76 656c 6f70 652c 2073 656c  netEnvelope, sel
+00034f50: 6629 2e5f 5f69 6e69 745f 5f28 290a 2020  f).__init__().  
+00034f60: 2020 2020 2020 7365 6c66 2e6e 5f6f 6e65        self.n_one
+00034f70: 203d 206e 5f6f 6e65 0a20 2020 2020 2020   = n_one.       
+00034f80: 2073 656c 662e 6e5f 7477 6f20 3d20 6e5f   self.n_two = n_
+00034f90: 7477 6f0a 2020 2020 2020 2020 7365 6c66  two.        self
+00034fa0: 2e74 6f74 616c 5f65 6c65 6374 726f 6e20  .total_electron 
+00034fb0: 3d20 746f 7461 6c5f 656c 6563 7472 6f6e  = total_electron
+00034fc0: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
+00034fd0: 7463 685f 7369 7a65 203d 2062 6174 6368  tch_size = batch
+00034fe0: 5f73 697a 650a 2020 2020 2020 2020 7365  _size.        se
+00034ff0: 6c66 2e73 7069 6e20 3d20 7370 696e 0a20  lf.spin = spin. 
+00035000: 2020 2020 2020 2073 656c 662e 6e6f 5f6f         self.no_o
+00035010: 665f 6174 6f6d 7320 3d20 6e6f 5f6f 665f  f_atoms = no_of_
+00035020: 6174 6f6d 730a 2020 2020 2020 2020 7365  atoms.        se
+00035030: 6c66 2e64 6574 6572 6d69 6e61 6e74 203d  lf.determinant =
+00035040: 2064 6574 6572 6d69 6e61 6e74 0a0a 2020   determinant..  
+00035050: 2020 2020 2020 7365 6c66 2e6c 6179 6572        self.layer
+00035060: 5f73 697a 653a 2069 6e74 203d 206c 656e  _size: int = len
+00035070: 2873 656c 662e 6e5f 6f6e 6529 0a0a 2020  (self.n_one)..  
+00035080: 2020 2020 2020 7365 6c66 2e65 6e76 656c        self.envel
+00035090: 6f70 655f 7720 3d20 746f 7263 682e 6e6e  ope_w = torch.nn
+000350a0: 2e50 6172 616d 6574 6572 4c69 7374 2829  .ParameterList()
+000350b0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
+000350c0: 7665 6c6f 7065 5f67 203d 2074 6f72 6368  velope_g = torch
+000350d0: 2e6e 6e2e 5061 7261 6d65 7465 724c 6973  .nn.ParameterLis
+000350e0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+000350f0: 2e73 6967 6d61 203d 2074 6f72 6368 2e6e  .sigma = torch.n
+00035100: 6e2e 5061 7261 6d65 7465 724c 6973 7428  n.ParameterList(
+00035110: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
+00035120: 6920 3d20 746f 7263 682e 6e6e 2e50 6172  i = torch.nn.Par
+00035130: 616d 6574 6572 4c69 7374 2829 0a20 2020  ameterList().   
+00035140: 2020 2020 2073 656c 662e 7764 6574 203d       self.wdet =
+00035150: 2074 6f72 6368 2e6e 6e2e 5061 7261 6d65   torch.nn.Parame
+00035160: 7465 724c 6973 7428 290a 0a20 2020 2020  terList()..     
+00035170: 2020 2023 2069 6e69 7469 616c 697a 6564     # initialized
+00035180: 2077 6569 6768 7473 2077 6974 6820 746f   weights with to
+00035190: 7263 682e 7a65 726f 732c 2074 6f72 6368  rch.zeros, torch
+000351a0: 2e65 7965 2061 6e64 2075 7369 6e67 2078  .eye and using x
+000351b0: 6176 6965 7220 696e 6974 2e0a 2020 2020  avier init..    
+000351c0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+000351d0: 6765 2873 656c 662e 6465 7465 726d 696e  ge(self.determin
+000351e0: 616e 7429 3a0a 2020 2020 2020 2020 2020  ant):.          
+000351f0: 2020 7365 6c66 2e77 6465 742e 6170 7065    self.wdet.appe
+00035200: 6e64 2874 6f72 6368 2e6e 6e2e 696e 6974  nd(torch.nn.init
+00035210: 2e6e 6f72 6d61 6c5f 2874 6f72 6368 2e7a  .normal_(torch.z
+00035220: 6572 6f73 2831 2929 2e73 7175 6565 7a65  eros(1)).squeeze
+00035230: 2830 2929 0a20 2020 2020 2020 2020 2020  (0)).           
+00035240: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+00035250: 7365 6c66 2e74 6f74 616c 5f65 6c65 6374  self.total_elect
+00035260: 726f 6e29 3a0a 2020 2020 2020 2020 2020  ron):.          
+00035270: 2020 2020 2020 7365 6c66 2e65 6e76 656c        self.envel
+00035280: 6f70 655f 772e 6170 7065 6e64 280a 2020  ope_w.append(.  
+00035290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000352a0: 2020 2874 6f72 6368 2e6e 6e2e 696e 6974    (torch.nn.init
+000352b0: 2e6e 6f72 6d61 6c5f 2874 6f72 6368 2e7a  .normal_(torch.z
+000352c0: 6572 6f73 286e 5f6f 6e65 5b2d 315d 2c20  eros(n_one[-1], 
+000352d0: 3129 2c29 202f 0a20 2020 2020 2020 2020  1),) /.         
+000352e0: 2020 2020 2020 2020 2020 2020 6d61 7468              math
+000352f0: 2e73 7172 7428 6e5f 6f6e 655b 2d31 5d29  .sqrt(n_one[-1])
+00035300: 292e 7371 7565 657a 6528 2d31 2929 0a20  ).squeeze(-1)). 
+00035310: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00035320: 656c 662e 656e 7665 6c6f 7065 5f67 2e61  elf.envelope_g.a
+00035330: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
+00035340: 2020 2020 2020 2020 2020 2028 746f 7263             (torc
+00035350: 682e 6e6e 2e69 6e69 742e 6e6f 726d 616c  h.nn.init.normal
+00035360: 5f28 746f 7263 682e 7a65 726f 7328 3129  _(torch.zeros(1)
+00035370: 2929 2e73 7175 6565 7a65 2830 2929 0a20  )).squeeze(0)). 
+00035380: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00035390: 6f72 206b 2069 6e20 7261 6e67 6528 7365  or k in range(se
+000353a0: 6c66 2e6e 6f5f 6f66 5f61 746f 6d73 293a  lf.no_of_atoms):
+000353b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000353c0: 2020 2020 2073 656c 662e 7069 2e61 7070       self.pi.app
+000353d0: 656e 6428 2874 6f72 6368 2e7a 6572 6f73  end((torch.zeros
+000353e0: 2831 2929 290a 2020 2020 2020 2020 2020  (1))).          
+000353f0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00035400: 6967 6d61 2e61 7070 656e 6428 746f 7263  igma.append(torc
+00035410: 682e 6579 6528 3329 290a 0a20 2020 2064  h.eye(3))..    d
+00035420: 6566 2066 6f72 7761 7264 2873 656c 662c  ef forward(self,
+00035430: 206f 6e65 5f65 6c65 6374 726f 6e3a 2074   one_electron: t
+00035440: 6f72 6368 2e54 656e 736f 722c 0a20 2020  orch.Tensor,.   
+00035450: 2020 2020 2020 2020 2020 2020 206f 6e65               one
+00035460: 5f65 6c65 6374 726f 6e5f 7665 6374 6f72  _electron_vector
+00035470: 5f70 6572 6d75 7465 643a 2074 6f72 6368  _permuted: torch
+00035480: 2e54 656e 736f 7229 3a0a 2020 2020 2020  .Tensor):.      
+00035490: 2020 2222 220a 2020 2020 2020 2020 5061    """.        Pa
+000354a0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+000354b0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000354c0: 2020 2020 6f6e 655f 656c 6563 7472 6f6e      one_electron
+000354d0: 3a20 746f 7263 682e 5465 6e73 6f72 0a20  : torch.Tensor. 
+000354e0: 2020 2020 2020 2020 2020 2054 6f72 6368             Torch
+000354f0: 2074 656e 736f 7220 7768 6963 6820 6973   tensor which is
+00035500: 206f 7574 7075 7420 6672 6f6d 2046 6572   output from Fer
+00035510: 6d69 6e45 6c65 6374 726f 6e46 6561 7475  minElectronFeatu
+00035520: 7265 206c 6179 6572 2069 6e20 7468 6520  re layer in the 
+00035530: 7368 6170 6520 6f66 2028 6261 7463 685f  shape of (batch_
+00035540: 7369 7a65 2c20 6e75 6d62 6572 206f 6620  size, number of 
+00035550: 656c 6374 726f 6e73 2c20 6e5f 6f6e 6520  elctrons, n_one 
+00035560: 6c61 7965 7220 7369 7a65 292e 0a20 2020  layer size)..   
+00035570: 2020 2020 206f 6e65 5f65 6c65 6374 726f       one_electro
+00035580: 6e5f 7665 6374 6f72 5f70 6572 6d75 7465  n_vector_permute
+00035590: 643a 2074 6f72 6368 2e54 656e 736f 720a  d: torch.Tensor.
+000355a0: 2020 2020 2020 2020 2020 2020 546f 7263              Torc
+000355b0: 6820 7465 6e73 6f72 2077 6869 6368 2069  h tensor which i
+000355c0: 7320 7368 6170 6520 7065 726d 7574 6564  s shape permuted
+000355d0: 2076 6563 746f 7220 6f66 2074 6865 206f   vector of the o
+000355e0: 7269 6769 6e61 6c20 6f6e 655f 656c 6563  riginal one_elec
+000355f0: 7472 6f6e 2076 6563 746f 7220 7465 6e73  tron vector tens
+00035600: 6f72 2e20 7368 6170 6520 6f66 2074 6865  or. shape of the
+00035610: 2074 656e 736f 7220 7368 6f75 6c64 2062   tensor should b
+00035620: 6520 2862 6174 6368 5f73 697a 652c 206e  e (batch_size, n
+00035630: 756d 6265 7220 6f66 2061 746f 6d73 2c20  umber of atoms, 
+00035640: 6e75 6d62 6572 206f 6620 656c 6563 7472  number of electr
+00035650: 6f6e 732c 2033 292e 0a0a 2020 2020 2020  ons, 3)...      
+00035660: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00035670: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00035680: 2020 7073 695f 7570 3a20 746f 7263 682e    psi_up: torch.
+00035690: 5465 6e73 6f72 0a20 2020 2020 2020 2020  Tensor.         
+000356a0: 2020 2054 6f72 6368 2074 656e 736f 7220     Torch tensor 
+000356b0: 7769 7468 2061 2073 6361 6c61 7220 7661  with a scalar va
+000356c0: 6c75 6520 636f 6e74 6169 6e69 6e67 2074  lue containing t
+000356d0: 6865 2073 616d 706c 6564 2077 6176 6566  he sampled wavef
+000356e0: 756e 6374 696f 6e20 7661 6c75 6520 666f  unction value fo
+000356f0: 7220 6561 6368 2062 6174 6368 2e0a 2020  r each batch..  
+00035700: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00035710: 2020 7073 6920 3d20 746f 7263 682e 7a65    psi = torch.ze
+00035720: 726f 7328 7365 6c66 2e62 6174 6368 5f73  ros(self.batch_s
+00035730: 697a 6529 0a20 2020 2020 2020 2070 7369  ize).        psi
+00035740: 5f75 7020 3d20 5b5d 0a20 2020 2020 2020  _up = [].       
+00035750: 2070 7369 5f64 6f77 6e20 3d20 5b5d 0a20   psi_down = []. 
+00035760: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00035770: 7261 6e67 6528 7365 6c66 2e64 6574 6572  range(self.deter
+00035780: 6d69 6e61 6e74 293a 0a20 2020 2020 2020  minant):.       
+00035790: 2020 2020 2023 2074 656d 706f 7261 7279       # temporary
+000357a0: 206c 6973 7420 746f 2073 7461 636b 2075   list to stack u
+000357b0: 706f 6e20 656c 6563 7472 6f6e 7320 6178  pon electrons ax
+000357c0: 6973 2061 7420 7468 6520 656e 640a 2020  is at the end.  
+000357d0: 2020 2020 2020 2020 2020 6465 7420 3d20            det = 
+000357e0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+000357f0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00035800: 6c66 2e73 7069 6e5b 305d 293a 0a20 2020  lf.spin[0]):.   
+00035810: 2020 2020 2020 2020 2020 2020 206f 6e65               one
+00035820: 5f64 5f69 6e64 6578 203d 2028 6b20 2a20  _d_index = (k * 
+00035830: 2873 656c 662e 746f 7461 6c5f 656c 6563  (self.total_elec
+00035840: 7472 6f6e 2929 202b 2069 0a20 2020 2020  tron)) + i.     
+00035850: 2020 2020 2020 2020 2020 2066 6f72 206a             for j
+00035860: 2069 6e20 7261 6e67 6528 7365 6c66 2e73   in range(self.s
+00035870: 7069 6e5b 305d 293a 0a20 2020 2020 2020  pin[0]):.       
+00035880: 2020 2020 2020 2020 2020 2020 2064 6574               det
+00035890: 2e61 7070 656e 6428 2828 746f 7263 682e  .append(((torch.
+000358a0: 7375 6d28 0a20 2020 2020 2020 2020 2020  sum(.           
+000358b0: 2020 2020 2020 2020 2020 2020 2028 7365               (se
+000358c0: 6c66 2e65 6e76 656c 6f70 655f 775b 6f6e  lf.envelope_w[on
+000358d0: 655f 645f 696e 6465 785d 202a 206f 6e65  e_d_index] * one
+000358e0: 5f65 6c65 6374 726f 6e5b 3a2c 206a 2c20  _electron[:, j, 
+000358f0: 3a5d 2920 2b0a 2020 2020 2020 2020 2020  :]) +.          
+00035900: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00035910: 6c66 2e65 6e76 656c 6f70 655f 675b 6f6e  lf.envelope_g[on
+00035920: 655f 645f 696e 6465 785d 2c0a 2020 2020  e_d_index],.    
 00035930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035940: 2020 2020 2020 2040 2073 656c 662e 7369         @ self.si
-00035950: 676d 615b 6f6e 655f 645f 696e 6465 785d  gma[one_d_index]
-00035960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00035940: 2020 2020 6469 6d3d 3129 2920 2a20 746f      dim=1)) * to
+00035950: 7263 682e 7375 6d28 746f 7263 682e 6578  rch.sum(torch.ex
+00035960: 7028 2d74 6f72 6368 2e61 6273 280a 2020  p(-torch.abs(.  
 00035970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035980: 2020 2020 2020 2020 2064 696d 3d32 2929           dim=2))
-00035990: 2920 2a20 7365 6c66 2e70 695b 6f6e 655f  ) * self.pi[one_
-000359a0: 645f 696e 6465 785d 2e54 2c0a 2020 2020  d_index].T,.    
-000359b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035980: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
+00035990: 6e6f 726d 286f 6e65 5f65 6c65 6374 726f  norm(one_electro
+000359a0: 6e5f 7665 6374 6f72 5f70 6572 6d75 7465  n_vector_permute
+000359b0: 645b 3a2c 206a 2c20 3a2c 203a 5d0a 2020  d[:, j, :, :].  
 000359c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000359d0: 2020 2020 2020 2020 6469 6d3d 3129 2929          dim=1)))
-000359e0: 0a20 2020 2020 2020 2020 2020 2070 7369  .            psi
-000359f0: 5f75 702e 6170 7065 6e64 280a 2020 2020  _up.append(.    
-00035a00: 2020 2020 2020 2020 2020 2020 746f 7263              torc
-00035a10: 682e 7265 7368 6170 6528 746f 7263 682e  h.reshape(torch.
-00035a20: 7374 6163 6b28 6465 742c 2064 696d 3d31  stack(det, dim=1
-00035a30: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00035a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035a50: 2028 7365 6c66 2e62 6174 6368 5f73 697a   (self.batch_siz
-00035a60: 652c 2073 656c 662e 7370 696e 5b30 5d2c  e, self.spin[0],
-00035a70: 2073 656c 662e 7370 696e 5b30 5d29 2929   self.spin[0])))
-00035a80: 0a0a 2020 2020 2020 2020 2020 2020 6465  ..            de
-00035a90: 7420 3d20 5b5d 0a20 2020 2020 2020 2020  t = [].         
-00035aa0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00035ab0: 6528 7365 6c66 2e73 7069 6e5b 305d 2c20  e(self.spin[0], 
-00035ac0: 7365 6c66 2e73 7069 6e5b 305d 202b 2073  self.spin[0] + s
-00035ad0: 656c 662e 7370 696e 5b31 5d29 3a0a 2020  elf.spin[1]):.  
-00035ae0: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-00035af0: 655f 645f 696e 6465 7820 3d20 286b 202a  e_d_index = (k *
-00035b00: 2028 7365 6c66 2e74 6f74 616c 5f65 6c65   (self.total_ele
-00035b10: 6374 726f 6e29 2920 2b20 690a 2020 2020  ctron)) + i.    
-00035b20: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00035b30: 6a20 696e 2072 616e 6765 2873 656c 662e  j in range(self.
-00035b40: 7370 696e 5b30 5d2c 2073 656c 662e 7370  spin[0], self.sp
-00035b50: 696e 5b30 5d20 2b20 7365 6c66 2e73 7069  in[0] + self.spi
-00035b60: 6e5b 315d 293a 0a20 2020 2020 2020 2020  n[1]):.         
-00035b70: 2020 2020 2020 2020 2020 2064 6574 2e61             det.a
-00035b80: 7070 656e 6428 2828 746f 7263 682e 7375  ppend(((torch.su
-00035b90: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-00035ba0: 2020 2020 2020 2020 2020 2028 7365 6c66             (self
-00035bb0: 2e65 6e76 656c 6f70 655f 775b 6f6e 655f  .envelope_w[one_
-00035bc0: 645f 696e 6465 785d 202a 206f 6e65 5f65  d_index] * one_e
-00035bd0: 6c65 6374 726f 6e5b 3a2c 206a 2c20 3a5d  lectron[:, j, :]
-00035be0: 2920 2b0a 2020 2020 2020 2020 2020 2020  ) +.            
-00035bf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00035c00: 2e65 6e76 656c 6f70 655f 675b 6f6e 655f  .envelope_g[one_
-00035c10: 645f 696e 6465 785d 2c0a 2020 2020 2020  d_index],.      
-00035c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035c30: 2020 6469 6d3d 3129 2920 2a20 746f 7263    dim=1)) * torc
-00035c40: 682e 7375 6d28 746f 7263 682e 6578 7028  h.sum(torch.exp(
-00035c50: 2d74 6f72 6368 2e61 6273 280a 2020 2020  -torch.abs(.    
-00035c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035c70: 2020 2020 2020 2020 746f 7263 682e 6e6f          torch.no
-00035c80: 726d 286f 6e65 5f65 6c65 6374 726f 6e5f  rm(one_electron_
-00035c90: 7665 6374 6f72 5f70 6572 6d75 7465 645b  vector_permuted[
-00035ca0: 3a2c 206a 2c20 3a2c 203a 5d0a 2020 2020  :, j, :, :].    
-00035cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000359d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000359e0: 2020 2020 2040 2073 656c 662e 7369 676d       @ self.sigm
+000359f0: 615b 6f6e 655f 645f 696e 6465 785d 2c0a  a[one_d_index],.
+00035a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035a20: 2020 2020 2020 2064 696d 3d32 2929 2920         dim=2))) 
+00035a30: 2a20 7365 6c66 2e70 695b 6f6e 655f 645f  * self.pi[one_d_
+00035a40: 696e 6465 785d 2e54 2c0a 2020 2020 2020  index].T,.      
+00035a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035a70: 2020 2020 2020 6469 6d3d 3129 2929 0a20        dim=1))). 
+00035a80: 2020 2020 2020 2020 2020 2070 7369 5f75             psi_u
+00035a90: 702e 6170 7065 6e64 280a 2020 2020 2020  p.append(.      
+00035aa0: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
+00035ab0: 7265 7368 6170 6528 746f 7263 682e 7374  reshape(torch.st
+00035ac0: 6163 6b28 6465 742c 2064 696d 3d31 292c  ack(det, dim=1),
+00035ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00035ae0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00035af0: 7365 6c66 2e62 6174 6368 5f73 697a 652c  self.batch_size,
+00035b00: 2073 656c 662e 7370 696e 5b30 5d2c 2073   self.spin[0], s
+00035b10: 656c 662e 7370 696e 5b30 5d29 2929 0a0a  elf.spin[0])))..
+00035b20: 2020 2020 2020 2020 2020 2020 6465 7420              det 
+00035b30: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00035b40: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00035b50: 7365 6c66 2e73 7069 6e5b 305d 2c20 7365  self.spin[0], se
+00035b60: 6c66 2e73 7069 6e5b 305d 202b 2073 656c  lf.spin[0] + sel
+00035b70: 662e 7370 696e 5b31 5d29 3a0a 2020 2020  f.spin[1]):.    
+00035b80: 2020 2020 2020 2020 2020 2020 6f6e 655f              one_
+00035b90: 645f 696e 6465 7820 3d20 286b 202a 2028  d_index = (k * (
+00035ba0: 7365 6c66 2e74 6f74 616c 5f65 6c65 6374  self.total_elect
+00035bb0: 726f 6e29 2920 2b20 690a 2020 2020 2020  ron)) + i.      
+00035bc0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+00035bd0: 696e 2072 616e 6765 2873 656c 662e 7370  in range(self.sp
+00035be0: 696e 5b30 5d2c 2073 656c 662e 7370 696e  in[0], self.spin
+00035bf0: 5b30 5d20 2b20 7365 6c66 2e73 7069 6e5b  [0] + self.spin[
+00035c00: 315d 293a 0a20 2020 2020 2020 2020 2020  1]):.           
+00035c10: 2020 2020 2020 2020 2064 6574 2e61 7070           det.app
+00035c20: 656e 6428 2828 746f 7263 682e 7375 6d28  end(((torch.sum(
+00035c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00035c40: 2020 2020 2020 2020 2028 7365 6c66 2e65           (self.e
+00035c50: 6e76 656c 6f70 655f 775b 6f6e 655f 645f  nvelope_w[one_d_
+00035c60: 696e 6465 785d 202a 206f 6e65 5f65 6c65  index] * one_ele
+00035c70: 6374 726f 6e5b 3a2c 206a 2c20 3a5d 2920  ctron[:, j, :]) 
+00035c80: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
+00035c90: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+00035ca0: 6e76 656c 6f70 655f 675b 6f6e 655f 645f  nvelope_g[one_d_
+00035cb0: 696e 6465 785d 2c0a 2020 2020 2020 2020  index],.        
 00035cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035cd0: 2020 2040 2073 656c 662e 7369 676d 615b     @ self.sigma[
-00035ce0: 6f6e 655f 645f 696e 6465 785d 2c0a 2020  one_d_index],.  
-00035cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035cd0: 6469 6d3d 3129 2920 2a20 746f 7263 682e  dim=1)) * torch.
+00035ce0: 7375 6d28 746f 7263 682e 6578 7028 2d74  sum(torch.exp(-t
+00035cf0: 6f72 6368 2e61 6273 280a 2020 2020 2020  orch.abs(.      
 00035d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035d10: 2020 2020 2064 696d 3d32 2929 2920 2a20       dim=2))) * 
-00035d20: 7365 6c66 2e70 695b 6f6e 655f 645f 696e  self.pi[one_d_in
-00035d30: 6465 785d 2e54 2c0a 2020 2020 2020 2020  dex].T,.        
-00035d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035d10: 2020 2020 2020 746f 7263 682e 6e6f 726d        torch.norm
+00035d20: 286f 6e65 5f65 6c65 6374 726f 6e5f 7665  (one_electron_ve
+00035d30: 6374 6f72 5f70 6572 6d75 7465 645b 3a2c  ctor_permuted[:,
+00035d40: 206a 2c20 3a2c 203a 5d0a 2020 2020 2020   j, :, :].      
 00035d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035d60: 2020 2020 6469 6d3d 3129 2929 0a20 2020      dim=1))).   
-00035d70: 2020 2020 2020 2020 2070 7369 5f64 6f77           psi_dow
-00035d80: 6e2e 6170 7065 6e64 280a 2020 2020 2020  n.append(.      
-00035d90: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
-00035da0: 7265 7368 6170 6528 746f 7263 682e 7374  reshape(torch.st
-00035db0: 6163 6b28 6465 742c 2064 696d 3d31 292c  ack(det, dim=1),
-00035dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00035dd0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00035de0: 7365 6c66 2e62 6174 6368 5f73 697a 652c  self.batch_size,
-00035df0: 2073 656c 662e 7370 696e 5b31 5d2c 2073   self.spin[1], s
-00035e00: 656c 662e 7370 696e 5b31 5d29 2929 0a0a  elf.spin[1])))..
-00035e10: 2020 2020 2020 2020 2020 2020 645f 646f              d_do
-00035e20: 776e 203d 2074 6f72 6368 2e64 6574 2870  wn = torch.det(p
-00035e30: 7369 5f64 6f77 6e5b 2d31 5d29 0a20 2020  si_down[-1]).   
-00035e40: 2020 2020 2020 2020 2064 5f75 7020 3d20           d_up = 
-00035e50: 746f 7263 682e 6465 7428 7073 695f 7570  torch.det(psi_up
-00035e60: 5b2d 315d 290a 2020 2020 2020 2020 2020  [-1]).          
-00035e70: 2020 6465 745f 6675 6c6c 203d 2064 5f75    det_full = d_u
-00035e80: 7020 2a20 645f 646f 776e 0a20 2020 2020  p * d_down.     
-00035e90: 2020 2020 2020 2070 7369 203d 2070 7369         psi = psi
-00035ea0: 202b 2073 656c 662e 7764 6574 5b6b 5d20   + self.wdet[k] 
-00035eb0: 2a20 6465 745f 6675 6c6c 0a20 2020 2020  * det_full.     
-00035ec0: 2020 2070 7369 5f6d 6174 7269 785f 7570     psi_matrix_up
-00035ed0: 203d 2074 6f72 6368 2e73 7461 636b 2870   = torch.stack(p
-00035ee0: 7369 5f75 702c 2064 696d 3d31 290a 2020  si_up, dim=1).  
-00035ef0: 2020 2020 2020 7073 695f 6d61 7472 6978        psi_matrix
-00035f00: 5f64 6f77 6e20 3d20 746f 7263 682e 7374  _down = torch.st
-00035f10: 6163 6b28 7073 695f 646f 776e 2c20 6469  ack(psi_down, di
-00035f20: 6d3d 3129 0a20 2020 2020 2020 2072 6574  m=1).        ret
-00035f30: 7572 6e20 7073 692c 2070 7369 5f6d 6174  urn psi, psi_mat
-00035f40: 7269 785f 7570 2c20 7073 695f 6d61 7472  rix_up, psi_matr
-00035f50: 6978 5f64 6f77 6e0a 0a0a 636c 6173 7320  ix_down...class 
-00035f60: 4d58 4d4e 6574 4c6f 6361 6c4d 6573 7361  MXMNetLocalMessa
-00035f70: 6765 5061 7373 696e 6728 6e6e 2e4d 6f64  gePassing(nn.Mod
-00035f80: 756c 6529 3a0a 2020 2020 2222 220a 2020  ule):.    """.  
-00035f90: 2020 5468 6520 4d58 4d4e 6574 4c6f 6361    The MXMNetLoca
-00035fa0: 6c4d 6573 7361 6765 5061 7373 696e 6720  lMessagePassing 
-00035fb0: 636c 6173 7320 6465 6669 6e65 7320 6120  class defines a 
-00035fc0: 6c6f 6361 6c20 6d65 7373 6167 6520 7061  local message pa
-00035fd0: 7373 696e 6720 6c61 7965 7220 7573 6564  ssing layer used
-00035fe0: 2069 6e20 7468 6520 4d58 4d4e 6574 206d   in the MXMNet m
-00035ff0: 6f64 656c 205b 315d 5f2e 0a20 2020 2054  odel [1]_..    T
-00036000: 6869 7320 6c61 7965 7220 696e 7465 6772  his layer integr
-00036010: 6174 6573 2063 726f 7373 2d6c 6179 6572  ates cross-layer
-00036020: 206d 6170 7069 6e67 7320 696e 7369 6465   mappings inside
-00036030: 2074 6865 206c 6f63 616c 206d 6573 7361   the local messa
-00036040: 6765 2070 6173 7369 6e67 2c20 616c 6c6f  ge passing, allo
-00036050: 7769 6e67 2066 6f72 2074 6865 2074 7261  wing for the tra
-00036060: 6e73 666f 726d 6174 696f 6e0a 2020 2020  nsformation.    
-00036070: 6f66 2069 6e70 7574 2074 656e 736f 7273  of input tensors
-00036080: 2072 6570 7265 7365 6e74 696e 6720 7061   representing pa
-00036090: 6972 7769 7365 2064 6973 7461 6e63 6573  irwise distances
-000360a0: 2061 6e64 2061 6e67 6c65 7320 6265 7477   and angles betw
-000360b0: 6565 6e20 6174 6f6d 7320 696e 2061 206d  een atoms in a m
-000360c0: 6f6c 6563 756c 6172 2073 7973 7465 6d2e  olecular system.
-000360d0: 0a20 2020 2054 6865 206c 6179 6572 2061  .    The layer a
-000360e0: 6767 7265 6761 7465 7320 696e 666f 726d  ggregates inform
-000360f0: 6174 696f 6e20 7573 696e 6720 6d65 7373  ation using mess
-00036100: 6167 6520 7061 7373 696e 6720 616e 6420  age passing and 
-00036110: 7570 6461 7465 7320 6174 6f6d 2072 6570  updates atom rep
-00036120: 7265 7365 6e74 6174 696f 6e73 2061 6363  resentations acc
-00036130: 6f72 6469 6e67 6c79 2e0a 2020 2020 5468  ordingly..    Th
-00036140: 6520 332d 7374 6570 206d 6573 7361 6765  e 3-step message
-00036150: 2070 6173 7369 6e67 2073 6368 656d 6520   passing scheme 
-00036160: 6973 2070 726f 706f 7365 6420 696e 2074  is proposed in t
-00036170: 6865 2070 6170 6572 205b 315d 5f2e 0a0a  he paper [1]_...
-00036180: 2020 2020 312e 2053 7465 7020 3120 636f      1. Step 1 co
-00036190: 6e74 6169 6e73 204d 6573 7361 6765 2050  ntains Message P
-000361a0: 6173 7369 6e67 2031 2074 6861 7420 6361  assing 1 that ca
-000361b0: 7074 7572 6573 2074 6865 2074 776f 2d68  ptures the two-h
-000361c0: 6f70 2061 6e67 6c65 7320 616e 6420 7265  op angles and re
-000361d0: 6c61 7465 6420 7061 6972 7769 7365 2064  lated pairwise d
-000361e0: 6973 7461 6e63 6573 2074 6f20 7570 6461  istances to upda
-000361f0: 7465 2065 6467 652d 6c65 7665 6c20 656d  te edge-level em
-00036200: 6265 6464 696e 6773 207b 6d6a 697d 2e0a  beddings {mji}..
-00036210: 2020 2020 322e 2053 7465 7020 3220 636f      2. Step 2 co
-00036220: 6e74 6169 6e73 204d 6573 7361 6765 2050  ntains Message P
-00036230: 6173 7369 6e67 2032 2074 6861 7420 6361  assing 2 that ca
-00036240: 7074 7572 6573 2074 6865 206f 6e65 2d68  ptures the one-h
-00036250: 6f70 2061 6e67 6c65 7320 616e 6420 7265  op angles and re
-00036260: 6c61 7465 6420 7061 6972 7769 7365 2064  lated pairwise d
-00036270: 6973 7461 6e63 6573 2074 6f20 6675 7274  istances to furt
-00036280: 6865 7220 7570 6461 7465 207b 6d6a 697d  her update {mji}
-00036290: 2e0a 2020 2020 332e 2053 7465 7020 3320  ..    3. Step 3 
-000362a0: 6669 6e61 6c6c 7920 6167 6772 6567 6174  finally aggregat
-000362b0: 6573 207b 6d6a 697d 2074 6f20 7570 6461  es {mji} to upda
-000362c0: 7465 2074 6865 206e 6f64 652d 6c65 7665  te the node-leve
-000362d0: 6c20 656d 6265 6464 696e 6720 6869 2e0a  l embedding hi..
-000362e0: 0a20 2020 2054 6865 7365 2073 7465 7073  .    These steps
-000362f0: 2069 6e20 7468 6520 742d 7468 2069 7465   in the t-th ite
-00036300: 7261 7469 6f6e 2063 616e 2062 6520 666f  ration can be fo
-00036310: 726d 756c 6174 6564 2061 7320 666f 6c6c  rmulated as foll
-00036320: 6f77 733a 0a0a 2020 2020 4c65 743a 0a20  ows:..    Let:. 
-00036330: 2020 2020 2020 202d 202a 2a6d 6c70 2a2a         - **mlp**
-00036340: 203a 2060 604d 756c 7469 6c61 7965 7250   : ``MultilayerP
-00036350: 6572 6365 7074 726f 6e60 600a 2020 2020  erceptron``.    
-00036360: 2020 2020 2d20 2a2a 7265 732a 2a20 3a20      - **res** : 
-00036370: 6060 5265 7369 6475 616c 426c 6f63 6b60  ``ResidualBlock`
-00036380: 600a 2020 2020 2020 2020 2d20 2a2a 682a  `.        - **h*
-00036390: 2a20 3a20 6060 6e6f 6465 5f66 6561 7475  * : ``node_featu
-000363a0: 7265 7360 600a 2020 2020 2020 2020 2d20  res``.        - 
-000363b0: 2a2a 6d2a 2a20 3a20 6060 6d65 7373 6167  **m** : ``messag
-000363c0: 6520 7769 7468 2072 6164 6961 6c20 6261  e with radial ba
-000363d0: 7369 7320 6675 6e63 7469 6f6e 6060 0a20  sis function``. 
-000363e0: 2020 2020 2020 202d 202a 2a69 6478 5f6b         - **idx_k
-000363f0: 6a2a 2a3a 2060 6054 656e 736f 7220 636f  j**: ``Tensor co
-00036400: 6e74 6169 6e69 6e67 2069 6e64 6963 6573  ntaining indices
-00036410: 2066 6f72 2074 6865 206b 2061 6e64 206a   for the k and j
-00036420: 2061 746f 6d73 6060 0a20 2020 2020 2020   atoms``.       
-00036430: 202d 202a 2a78 5f69 2a2a 203a 2060 6054   - **x_i** : ``T
-00036440: 6865 206e 6f64 6520 746f 2062 6520 7570  he node to be up
-00036450: 6461 7465 6460 600a 2020 2020 2020 2020  dated``.        
-00036460: 2d20 2a2a 685f 692a 2a20 3a20 6060 5468  - **h_i** : ``Th
-00036470: 6520 6869 6464 656e 2073 7461 7465 206f  e hidden state o
-00036480: 6620 785f 6960 600a 2020 2020 2020 2020  f x_i``.        
-00036490: 2d20 2a2a 785f 6a2a 2a20 3a20 6060 5468  - **x_j** : ``Th
-000364a0: 6520 6e65 6967 6862 6f75 7220 6e6f 6465  e neighbour node
-000364b0: 2063 6f6e 6e65 6374 6564 2074 6f20 785f   connected to x_
-000364c0: 6920 6279 2065 6467 6520 655f 696a 6060  i by edge e_ij``
-000364d0: 0a20 2020 2020 2020 202d 202a 2a68 5f6a  .        - **h_j
-000364e0: 2a2a 203a 2060 6054 6865 2068 6964 6465  ** : ``The hidde
-000364f0: 6e20 7374 6174 6520 6f66 2078 5f6a 6060  n state of x_j``
-00036500: 0a20 2020 2020 2020 202d 202a 2a72 6266  .        - **rbf
-00036510: 2a2a 203a 2060 6049 6e70 7574 2074 656e  ** : ``Input ten
-00036520: 736f 7220 7265 7072 6573 656e 7469 6e67  sor representing
-00036530: 2072 6164 6961 6c20 6261 7369 7320 6675   radial basis fu
-00036540: 6e63 7469 6f6e 7360 600a 2020 2020 2020  nctions``.      
-00036550: 2020 2d20 2a2a 7362 662a 2a20 3a20 6060    - **sbf** : ``
-00036560: 496e 7075 7420 7465 6e73 6f72 2072 6570  Input tensor rep
-00036570: 7265 7365 6e74 696e 6720 7468 6520 7370  resenting the sp
-00036580: 6865 7269 6361 6c20 6261 7369 7320 6675  herical basis fu
-00036590: 6e63 7469 6f6e 7360 600a 2020 2020 2020  nctions``.      
-000365a0: 2020 2d20 2a2a 6964 785f 6a6a 2a2a 203a    - **idx_jj** :
-000365b0: 2060 6054 656e 736f 7220 636f 6e74 6169   ``Tensor contai
-000365c0: 6e69 6e67 2069 6e64 6963 6573 2066 6f72  ning indices for
-000365d0: 2074 6865 206a 2061 6e64 206a 2720 7768   the j and j' wh
-000365e0: 6572 6520 6a27 2069 7320 6f74 6865 7220  ere j' is other 
-000365f0: 6e65 6967 6862 6f75 7273 206f 6620 6960  neighbours of i`
-00036600: 600a 0a20 2020 2053 7465 7020 313a 204d  `..    Step 1: M
-00036610: 6573 7361 6765 2050 6173 7369 6e67 2031  essage Passing 1
-00036620: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
-00036630: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-00036640: 0a0a 2020 2020 2020 2020 2020 2020 6d20  ..            m 
-00036650: 3d20 5b68 5b69 5d20 7c7c 2068 5b6a 5d20  = [h[i] || h[j] 
-00036660: 7c7c 2072 6266 5d0a 2020 2020 2020 2020  || rbf].        
-00036670: 2020 2020 6d5f 6b6a 203d 206d 6c70 5f6b      m_kj = mlp_k
-00036680: 6a28 6d5b 6964 785f 6b6a 5d29 202a 2028  j(m[idx_kj]) * (
-00036690: 7262 662a 5729 202a 206d 6c70 5f73 6266  rbf*W) * mlp_sbf
-000366a0: 3128 7362 6631 290a 2020 2020 2020 2020  1(sbf1).        
-000366b0: 2020 2020 6d5f 6a69 203d 206d 6c70 5f6a      m_ji = mlp_j
-000366c0: 695f 3128 6d29 202b 2072 6564 7563 655f  i_1(m) + reduce_
-000366d0: 7375 6d28 6d5f 6b6a 290a 0a20 2020 2053  sum(m_kj)..    S
-000366e0: 7465 7020 323a 204d 6573 7361 6765 2050  tep 2: Message P
-000366f0: 6173 7369 6e67 2032 0a0a 2020 2020 2020  assing 2..      
-00036700: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-00036710: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-00036720: 2020 2020 2020 6d5f 6a69 203d 206d 6c70        m_ji = mlp
-00036730: 5f6a 6a28 6d5f 6a69 5b69 6478 5f6a 6a5d  _jj(m_ji[idx_jj]
-00036740: 2920 2a20 2872 6266 2a57 2920 2a20 6d6c  ) * (rbf*W) * ml
-00036750: 705f 7362 6632 2873 6266 3229 0a20 2020  p_sbf2(sbf2).   
-00036760: 2020 2020 2020 2020 206d 5f6a 6920 3d20           m_ji = 
-00036770: 6d6c 705f 6a69 5f32 286d 5f6a 6929 202b  mlp_ji_2(m_ji) +
-00036780: 2072 6564 7563 655f 7375 6d28 6d5f 6a69   reduce_sum(m_ji
-00036790: 290a 0a20 2020 2053 7465 7020 333a 2041  )..    Step 3: A
-000367a0: 6767 7265 6761 7469 6f6e 2061 6e64 2055  ggregation and U
-000367b0: 7064 6174 650a 0a20 2020 2020 2020 202a  pdate..        *
-000367c0: 2a49 6e20 6561 6368 2061 6767 7265 6761  *In each aggrega
-000367d0: 7469 6f6e 2073 7465 702a 2a0a 0a20 2020  tion step**..   
-000367e0: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
-000367f0: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
-00036800: 2020 2020 2020 2020 206d 203d 2072 6564           m = red
-00036810: 7563 655f 7375 6d28 6d5f 6a69 2a28 7262  uce_sum(m_ji*(rb
-00036820: 662a 5729 290a 0a20 2020 2020 2020 202a  f*W))..        *
-00036830: 2a49 6e20 6561 6368 2075 7064 6174 6520  *In each update 
-00036840: 7374 6570 2a2a 0a0a 2020 2020 2020 2020  step**..        
-00036850: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00036860: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-00036870: 2020 2020 686d 5f69 203d 2072 6573 3128      hm_i = res1(
-00036880: 6d29 0a20 2020 2020 2020 2020 2020 2068  m).            h
-00036890: 5f69 5f6e 6577 203d 206d 6c70 3228 686d  _i_new = mlp2(hm
-000368a0: 5f69 2920 2b20 685f 690a 2020 2020 2020  _i) + h_i.      
-000368b0: 2020 2020 2020 685f 695f 6e65 7720 3d20        h_i_new = 
-000368c0: 7265 7332 2868 5f69 5f6e 6577 290a 2020  res2(h_i_new).  
-000368d0: 2020 2020 2020 2020 2020 685f 695f 6e65            h_i_ne
-000368e0: 7720 3d20 7265 7333 2868 5f69 5f6e 6577  w = res3(h_i_new
-000368f0: 290a 0a20 2020 2052 6566 6572 656e 6365  )..    Reference
-00036900: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00036910: 0a20 2020 202e 2e20 5b31 5d20 4d6f 6c65  .    .. [1] Mole
-00036920: 6375 6c61 7220 4d65 6368 616e 6963 732d  cular Mechanics-
-00036930: 4472 6976 656e 2047 7261 7068 204e 6575  Driven Graph Neu
-00036940: 7261 6c20 4e65 7477 6f72 6b20 7769 7468  ral Network with
-00036950: 204d 756c 7469 706c 6578 2047 7261 7068   Multiplex Graph
-00036960: 2066 6f72 204d 6f6c 6563 756c 6172 2053   for Molecular S
-00036970: 7472 7563 7475 7265 732e 2068 7474 7073  tructures. https
-00036980: 3a2f 2f61 7278 6976 2e6f 7267 2f70 6466  ://arxiv.org/pdf
-00036990: 2f32 3031 312e 3037 3435 370a 2020 2020  /2011.07457.    
-000369a0: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
-000369b0: 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20 6469  -----.    >>> di
-000369c0: 6d20 3d20 310a 2020 2020 3e3e 3e20 6820  m = 1.    >>> h 
-000369d0: 3d20 746f 7263 682e 7465 6e73 6f72 285b  = torch.tensor([
-000369e0: 5b30 2e38 3334 335d 2c20 5b31 2e32 3731  [0.8343], [1.271
-000369f0: 335d 2c20 5b31 2e32 3731 335d 2c20 5b31  3], [1.2713], [1
-00036a00: 2e32 3731 335d 2c20 5b31 2e32 3731 335d  .2713], [1.2713]
-00036a10: 5d29 0a20 2020 203e 3e3e 2072 6266 203d  ]).    >>> rbf =
-00036a20: 2074 6f72 6368 2e74 656e 736f 7228 5b5b   torch.tensor([[
-00036a30: 2d30 2e32 3632 385d 2c20 5b2d 302e 3236  -0.2628], [-0.26
-00036a40: 3238 5d2c 205b 2d30 2e32 3632 385d 2c20  28], [-0.2628], 
-00036a50: 5b2d 302e 3236 3238 5d2c 0a20 2020 202e  [-0.2628],.    .
-00036a60: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
-00036a70: 2020 2020 2020 205b 2d30 2e32 3632 395d         [-0.2629]
-00036a80: 2c20 5b2d 302e 3236 3239 5d2c 205b 2d30  , [-0.2629], [-0
-00036a90: 2e32 3632 385d 2c20 5b2d 302e 3236 3238  .2628], [-0.2628
-00036aa0: 5d5d 290a 2020 2020 3e3e 3e20 7362 6631  ]]).    >>> sbf1
-00036ab0: 203d 2074 6f72 6368 2e74 656e 736f 7228   = torch.tensor(
-00036ac0: 5b5b 2d30 2e32 3736 375d 2c20 5b2d 302e  [[-0.2767], [-0.
-00036ad0: 3237 3637 5d2c 205b 2d30 2e32 3736 375d  2767], [-0.2767]
-00036ae0: 2c20 5b2d 302e 3237 3637 5d2c 0a20 2020  , [-0.2767],.   
-00036af0: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
-00036b00: 2020 2020 2020 2020 2020 5b2d 302e 3237            [-0.27
-00036b10: 3637 5d2c 205b 2d30 2e32 3736 375d 2c20  67], [-0.2767], 
-00036b20: 5b2d 302e 3237 3637 5d2c 205b 2d30 2e32  [-0.2767], [-0.2
-00036b30: 3736 375d 2c0a 2020 2020 2e2e 2e20 2020  767],.    ...   
-00036b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036b50: 2020 205b 2d30 2e32 3736 375d 2c20 5b2d     [-0.2767], [-
-00036b60: 302e 3237 3637 5d2c 205b 2d30 2e32 3736  0.2767], [-0.276
-00036b70: 375d 2c20 5b2d 302e 3237 3637 5d5d 290a  7], [-0.2767]]).
-00036b80: 2020 2020 3e3e 3e20 7362 6632 203d 2074      >>> sbf2 = t
-00036b90: 6f72 6368 2e74 656e 736f 7228 5b5b 2d30  orch.tensor([[-0
-00036ba0: 2e30 3330 315d 2c20 5b2d 302e 3033 3031  .0301], [-0.0301
-00036bb0: 5d2c 205b 2d30 2e31 3438 335d 2c20 5b2d  ], [-0.1483], [-
-00036bc0: 302e 3134 3836 5d2c 205b 2d30 2e31 3438  0.1486], [-0.148
-00036bd0: 345d 2c0a 2020 2020 2e2e 2e20 2020 2020  4],.    ...     
+00035d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035d70: 2040 2073 656c 662e 7369 676d 615b 6f6e   @ self.sigma[on
+00035d80: 655f 645f 696e 6465 785d 2c0a 2020 2020  e_d_index],.    
+00035d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035db0: 2020 2064 696d 3d32 2929 2920 2a20 7365     dim=2))) * se
+00035dc0: 6c66 2e70 695b 6f6e 655f 645f 696e 6465  lf.pi[one_d_inde
+00035dd0: 785d 2e54 2c0a 2020 2020 2020 2020 2020  x].T,.          
+00035de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035e00: 2020 6469 6d3d 3129 2929 0a20 2020 2020    dim=1))).     
+00035e10: 2020 2020 2020 2070 7369 5f64 6f77 6e2e         psi_down.
+00035e20: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+00035e30: 2020 2020 2020 2020 746f 7263 682e 7265          torch.re
+00035e40: 7368 6170 6528 746f 7263 682e 7374 6163  shape(torch.stac
+00035e50: 6b28 6465 742c 2064 696d 3d31 292c 0a20  k(det, dim=1),. 
+00035e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035e70: 2020 2020 2020 2020 2020 2020 2028 7365               (se
+00035e80: 6c66 2e62 6174 6368 5f73 697a 652c 2073  lf.batch_size, s
+00035e90: 656c 662e 7370 696e 5b31 5d2c 2073 656c  elf.spin[1], sel
+00035ea0: 662e 7370 696e 5b31 5d29 2929 0a0a 2020  f.spin[1])))..  
+00035eb0: 2020 2020 2020 2020 2020 645f 646f 776e            d_down
+00035ec0: 203d 2074 6f72 6368 2e64 6574 2870 7369   = torch.det(psi
+00035ed0: 5f64 6f77 6e5b 2d31 5d29 0a20 2020 2020  _down[-1]).     
+00035ee0: 2020 2020 2020 2064 5f75 7020 3d20 746f         d_up = to
+00035ef0: 7263 682e 6465 7428 7073 695f 7570 5b2d  rch.det(psi_up[-
+00035f00: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
+00035f10: 6465 745f 6675 6c6c 203d 2064 5f75 7020  det_full = d_up 
+00035f20: 2a20 645f 646f 776e 0a20 2020 2020 2020  * d_down.       
+00035f30: 2020 2020 2070 7369 203d 2070 7369 202b       psi = psi +
+00035f40: 2073 656c 662e 7764 6574 5b6b 5d20 2a20   self.wdet[k] * 
+00035f50: 6465 745f 6675 6c6c 0a20 2020 2020 2020  det_full.       
+00035f60: 2070 7369 5f6d 6174 7269 785f 7570 203d   psi_matrix_up =
+00035f70: 2074 6f72 6368 2e73 7461 636b 2870 7369   torch.stack(psi
+00035f80: 5f75 702c 2064 696d 3d31 290a 2020 2020  _up, dim=1).    
+00035f90: 2020 2020 7073 695f 6d61 7472 6978 5f64      psi_matrix_d
+00035fa0: 6f77 6e20 3d20 746f 7263 682e 7374 6163  own = torch.stac
+00035fb0: 6b28 7073 695f 646f 776e 2c20 6469 6d3d  k(psi_down, dim=
+00035fc0: 3129 0a20 2020 2020 2020 2072 6574 7572  1).        retur
+00035fd0: 6e20 7073 692c 2070 7369 5f6d 6174 7269  n psi, psi_matri
+00035fe0: 785f 7570 2c20 7073 695f 6d61 7472 6978  x_up, psi_matrix
+00035ff0: 5f64 6f77 6e0a 0a0a 636c 6173 7320 4d58  _down...class MX
+00036000: 4d4e 6574 4c6f 6361 6c4d 6573 7361 6765  MNetLocalMessage
+00036010: 5061 7373 696e 6728 6e6e 2e4d 6f64 756c  Passing(nn.Modul
+00036020: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+00036030: 5468 6520 4d58 4d4e 6574 4c6f 6361 6c4d  The MXMNetLocalM
+00036040: 6573 7361 6765 5061 7373 696e 6720 636c  essagePassing cl
+00036050: 6173 7320 6465 6669 6e65 7320 6120 6c6f  ass defines a lo
+00036060: 6361 6c20 6d65 7373 6167 6520 7061 7373  cal message pass
+00036070: 696e 6720 6c61 7965 7220 7573 6564 2069  ing layer used i
+00036080: 6e20 7468 6520 4d58 4d4e 6574 206d 6f64  n the MXMNet mod
+00036090: 656c 205b 315d 5f2e 0a20 2020 2054 6869  el [1]_..    Thi
+000360a0: 7320 6c61 7965 7220 696e 7465 6772 6174  s layer integrat
+000360b0: 6573 2063 726f 7373 2d6c 6179 6572 206d  es cross-layer m
+000360c0: 6170 7069 6e67 7320 696e 7369 6465 2074  appings inside t
+000360d0: 6865 206c 6f63 616c 206d 6573 7361 6765  he local message
+000360e0: 2070 6173 7369 6e67 2c20 616c 6c6f 7769   passing, allowi
+000360f0: 6e67 2066 6f72 2074 6865 2074 7261 6e73  ng for the trans
+00036100: 666f 726d 6174 696f 6e0a 2020 2020 6f66  formation.    of
+00036110: 2069 6e70 7574 2074 656e 736f 7273 2072   input tensors r
+00036120: 6570 7265 7365 6e74 696e 6720 7061 6972  epresenting pair
+00036130: 7769 7365 2064 6973 7461 6e63 6573 2061  wise distances a
+00036140: 6e64 2061 6e67 6c65 7320 6265 7477 6565  nd angles betwee
+00036150: 6e20 6174 6f6d 7320 696e 2061 206d 6f6c  n atoms in a mol
+00036160: 6563 756c 6172 2073 7973 7465 6d2e 0a20  ecular system.. 
+00036170: 2020 2054 6865 206c 6179 6572 2061 6767     The layer agg
+00036180: 7265 6761 7465 7320 696e 666f 726d 6174  regates informat
+00036190: 696f 6e20 7573 696e 6720 6d65 7373 6167  ion using messag
+000361a0: 6520 7061 7373 696e 6720 616e 6420 7570  e passing and up
+000361b0: 6461 7465 7320 6174 6f6d 2072 6570 7265  dates atom repre
+000361c0: 7365 6e74 6174 696f 6e73 2061 6363 6f72  sentations accor
+000361d0: 6469 6e67 6c79 2e0a 2020 2020 5468 6520  dingly..    The 
+000361e0: 332d 7374 6570 206d 6573 7361 6765 2070  3-step message p
+000361f0: 6173 7369 6e67 2073 6368 656d 6520 6973  assing scheme is
+00036200: 2070 726f 706f 7365 6420 696e 2074 6865   proposed in the
+00036210: 2070 6170 6572 205b 315d 5f2e 0a0a 2020   paper [1]_...  
+00036220: 2020 312e 2053 7465 7020 3120 636f 6e74    1. Step 1 cont
+00036230: 6169 6e73 204d 6573 7361 6765 2050 6173  ains Message Pas
+00036240: 7369 6e67 2031 2074 6861 7420 6361 7074  sing 1 that capt
+00036250: 7572 6573 2074 6865 2074 776f 2d68 6f70  ures the two-hop
+00036260: 2061 6e67 6c65 7320 616e 6420 7265 6c61   angles and rela
+00036270: 7465 6420 7061 6972 7769 7365 2064 6973  ted pairwise dis
+00036280: 7461 6e63 6573 2074 6f20 7570 6461 7465  tances to update
+00036290: 2065 6467 652d 6c65 7665 6c20 656d 6265   edge-level embe
+000362a0: 6464 696e 6773 207b 6d6a 697d 2e0a 2020  ddings {mji}..  
+000362b0: 2020 322e 2053 7465 7020 3220 636f 6e74    2. Step 2 cont
+000362c0: 6169 6e73 204d 6573 7361 6765 2050 6173  ains Message Pas
+000362d0: 7369 6e67 2032 2074 6861 7420 6361 7074  sing 2 that capt
+000362e0: 7572 6573 2074 6865 206f 6e65 2d68 6f70  ures the one-hop
+000362f0: 2061 6e67 6c65 7320 616e 6420 7265 6c61   angles and rela
+00036300: 7465 6420 7061 6972 7769 7365 2064 6973  ted pairwise dis
+00036310: 7461 6e63 6573 2074 6f20 6675 7274 6865  tances to furthe
+00036320: 7220 7570 6461 7465 207b 6d6a 697d 2e0a  r update {mji}..
+00036330: 2020 2020 332e 2053 7465 7020 3320 6669      3. Step 3 fi
+00036340: 6e61 6c6c 7920 6167 6772 6567 6174 6573  nally aggregates
+00036350: 207b 6d6a 697d 2074 6f20 7570 6461 7465   {mji} to update
+00036360: 2074 6865 206e 6f64 652d 6c65 7665 6c20   the node-level 
+00036370: 656d 6265 6464 696e 6720 6869 2e0a 0a20  embedding hi... 
+00036380: 2020 2054 6865 7365 2073 7465 7073 2069     These steps i
+00036390: 6e20 7468 6520 742d 7468 2069 7465 7261  n the t-th itera
+000363a0: 7469 6f6e 2063 616e 2062 6520 666f 726d  tion can be form
+000363b0: 756c 6174 6564 2061 7320 666f 6c6c 6f77  ulated as follow
+000363c0: 733a 0a0a 2020 2020 4c65 743a 0a20 2020  s:..    Let:.   
+000363d0: 2020 2020 202d 202a 2a6d 6c70 2a2a 203a       - **mlp** :
+000363e0: 2060 604d 756c 7469 6c61 7965 7250 6572   ``MultilayerPer
+000363f0: 6365 7074 726f 6e60 600a 2020 2020 2020  ceptron``.      
+00036400: 2020 2d20 2a2a 7265 732a 2a20 3a20 6060    - **res** : ``
+00036410: 5265 7369 6475 616c 426c 6f63 6b60 600a  ResidualBlock``.
+00036420: 2020 2020 2020 2020 2d20 2a2a 682a 2a20          - **h** 
+00036430: 3a20 6060 6e6f 6465 5f66 6561 7475 7265  : ``node_feature
+00036440: 7360 600a 2020 2020 2020 2020 2d20 2a2a  s``.        - **
+00036450: 6d2a 2a20 3a20 6060 6d65 7373 6167 6520  m** : ``message 
+00036460: 7769 7468 2072 6164 6961 6c20 6261 7369  with radial basi
+00036470: 7320 6675 6e63 7469 6f6e 6060 0a20 2020  s function``.   
+00036480: 2020 2020 202d 202a 2a69 6478 5f6b 6a2a       - **idx_kj*
+00036490: 2a3a 2060 6054 656e 736f 7220 636f 6e74  *: ``Tensor cont
+000364a0: 6169 6e69 6e67 2069 6e64 6963 6573 2066  aining indices f
+000364b0: 6f72 2074 6865 206b 2061 6e64 206a 2061  or the k and j a
+000364c0: 746f 6d73 6060 0a20 2020 2020 2020 202d  toms``.        -
+000364d0: 202a 2a78 5f69 2a2a 203a 2060 6054 6865   **x_i** : ``The
+000364e0: 206e 6f64 6520 746f 2062 6520 7570 6461   node to be upda
+000364f0: 7465 6460 600a 2020 2020 2020 2020 2d20  ted``.        - 
+00036500: 2a2a 685f 692a 2a20 3a20 6060 5468 6520  **h_i** : ``The 
+00036510: 6869 6464 656e 2073 7461 7465 206f 6620  hidden state of 
+00036520: 785f 6960 600a 2020 2020 2020 2020 2d20  x_i``.        - 
+00036530: 2a2a 785f 6a2a 2a20 3a20 6060 5468 6520  **x_j** : ``The 
+00036540: 6e65 6967 6862 6f75 7220 6e6f 6465 2063  neighbour node c
+00036550: 6f6e 6e65 6374 6564 2074 6f20 785f 6920  onnected to x_i 
+00036560: 6279 2065 6467 6520 655f 696a 6060 0a20  by edge e_ij``. 
+00036570: 2020 2020 2020 202d 202a 2a68 5f6a 2a2a         - **h_j**
+00036580: 203a 2060 6054 6865 2068 6964 6465 6e20   : ``The hidden 
+00036590: 7374 6174 6520 6f66 2078 5f6a 6060 0a20  state of x_j``. 
+000365a0: 2020 2020 2020 202d 202a 2a72 6266 2a2a         - **rbf**
+000365b0: 203a 2060 6049 6e70 7574 2074 656e 736f   : ``Input tenso
+000365c0: 7220 7265 7072 6573 656e 7469 6e67 2072  r representing r
+000365d0: 6164 6961 6c20 6261 7369 7320 6675 6e63  adial basis func
+000365e0: 7469 6f6e 7360 600a 2020 2020 2020 2020  tions``.        
+000365f0: 2d20 2a2a 7362 662a 2a20 3a20 6060 496e  - **sbf** : ``In
+00036600: 7075 7420 7465 6e73 6f72 2072 6570 7265  put tensor repre
+00036610: 7365 6e74 696e 6720 7468 6520 7370 6865  senting the sphe
+00036620: 7269 6361 6c20 6261 7369 7320 6675 6e63  rical basis func
+00036630: 7469 6f6e 7360 600a 2020 2020 2020 2020  tions``.        
+00036640: 2d20 2a2a 6964 785f 6a6a 2a2a 203a 2060  - **idx_jj** : `
+00036650: 6054 656e 736f 7220 636f 6e74 6169 6e69  `Tensor containi
+00036660: 6e67 2069 6e64 6963 6573 2066 6f72 2074  ng indices for t
+00036670: 6865 206a 2061 6e64 206a 2720 7768 6572  he j and j' wher
+00036680: 6520 6a27 2069 7320 6f74 6865 7220 6e65  e j' is other ne
+00036690: 6967 6862 6f75 7273 206f 6620 6960 600a  ighbours of i``.
+000366a0: 0a20 2020 2053 7465 7020 313a 204d 6573  .    Step 1: Mes
+000366b0: 7361 6765 2050 6173 7369 6e67 2031 0a0a  sage Passing 1..
+000366c0: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
+000366d0: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+000366e0: 2020 2020 2020 2020 2020 2020 6d20 3d20              m = 
+000366f0: 5b68 5b69 5d20 7c7c 2068 5b6a 5d20 7c7c  [h[i] || h[j] ||
+00036700: 2072 6266 5d0a 2020 2020 2020 2020 2020   rbf].          
+00036710: 2020 6d5f 6b6a 203d 206d 6c70 5f6b 6a28    m_kj = mlp_kj(
+00036720: 6d5b 6964 785f 6b6a 5d29 202a 2028 7262  m[idx_kj]) * (rb
+00036730: 662a 5729 202a 206d 6c70 5f73 6266 3128  f*W) * mlp_sbf1(
+00036740: 7362 6631 290a 2020 2020 2020 2020 2020  sbf1).          
+00036750: 2020 6d5f 6a69 203d 206d 6c70 5f6a 695f    m_ji = mlp_ji_
+00036760: 3128 6d29 202b 2072 6564 7563 655f 7375  1(m) + reduce_su
+00036770: 6d28 6d5f 6b6a 290a 0a20 2020 2053 7465  m(m_kj)..    Ste
+00036780: 7020 323a 204d 6573 7361 6765 2050 6173  p 2: Message Pas
+00036790: 7369 6e67 2032 0a0a 2020 2020 2020 2020  sing 2..        
+000367a0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000367b0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+000367c0: 2020 2020 6d5f 6a69 203d 206d 6c70 5f6a      m_ji = mlp_j
+000367d0: 6a28 6d5f 6a69 5b69 6478 5f6a 6a5d 2920  j(m_ji[idx_jj]) 
+000367e0: 2a20 2872 6266 2a57 2920 2a20 6d6c 705f  * (rbf*W) * mlp_
+000367f0: 7362 6632 2873 6266 3229 0a20 2020 2020  sbf2(sbf2).     
+00036800: 2020 2020 2020 206d 5f6a 6920 3d20 6d6c         m_ji = ml
+00036810: 705f 6a69 5f32 286d 5f6a 6929 202b 2072  p_ji_2(m_ji) + r
+00036820: 6564 7563 655f 7375 6d28 6d5f 6a69 290a  educe_sum(m_ji).
+00036830: 0a20 2020 2053 7465 7020 333a 2041 6767  .    Step 3: Agg
+00036840: 7265 6761 7469 6f6e 2061 6e64 2055 7064  regation and Upd
+00036850: 6174 650a 0a20 2020 2020 2020 202a 2a49  ate..        **I
+00036860: 6e20 6561 6368 2061 6767 7265 6761 7469  n each aggregati
+00036870: 6f6e 2073 7465 702a 2a0a 0a20 2020 2020  on step**..     
+00036880: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+00036890: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+000368a0: 2020 2020 2020 206d 203d 2072 6564 7563         m = reduc
+000368b0: 655f 7375 6d28 6d5f 6a69 2a28 7262 662a  e_sum(m_ji*(rbf*
+000368c0: 5729 290a 0a20 2020 2020 2020 202a 2a49  W))..        **I
+000368d0: 6e20 6561 6368 2075 7064 6174 6520 7374  n each update st
+000368e0: 6570 2a2a 0a0a 2020 2020 2020 2020 2e2e  ep**..        ..
+000368f0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00036900: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
+00036910: 2020 686d 5f69 203d 2072 6573 3128 6d29    hm_i = res1(m)
+00036920: 0a20 2020 2020 2020 2020 2020 2068 5f69  .            h_i
+00036930: 5f6e 6577 203d 206d 6c70 3228 686d 5f69  _new = mlp2(hm_i
+00036940: 2920 2b20 685f 690a 2020 2020 2020 2020  ) + h_i.        
+00036950: 2020 2020 685f 695f 6e65 7720 3d20 7265      h_i_new = re
+00036960: 7332 2868 5f69 5f6e 6577 290a 2020 2020  s2(h_i_new).    
+00036970: 2020 2020 2020 2020 685f 695f 6e65 7720          h_i_new 
+00036980: 3d20 7265 7333 2868 5f69 5f6e 6577 290a  = res3(h_i_new).
+00036990: 0a20 2020 2052 6566 6572 656e 6365 730a  .    References.
+000369a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000369b0: 2020 202e 2e20 5b31 5d20 4d6f 6c65 6375     .. [1] Molecu
+000369c0: 6c61 7220 4d65 6368 616e 6963 732d 4472  lar Mechanics-Dr
+000369d0: 6976 656e 2047 7261 7068 204e 6575 7261  iven Graph Neura
+000369e0: 6c20 4e65 7477 6f72 6b20 7769 7468 204d  l Network with M
+000369f0: 756c 7469 706c 6578 2047 7261 7068 2066  ultiplex Graph f
+00036a00: 6f72 204d 6f6c 6563 756c 6172 2053 7472  or Molecular Str
+00036a10: 7563 7475 7265 732e 2068 7474 7073 3a2f  uctures. https:/
+00036a20: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+00036a30: 3031 312e 3037 3435 370a 2020 2020 4578  011.07457.    Ex
+00036a40: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+00036a50: 2d2d 2d0a 2020 2020 3e3e 3e20 6469 6d20  ---.    >>> dim 
+00036a60: 3d20 310a 2020 2020 3e3e 3e20 6820 3d20  = 1.    >>> h = 
+00036a70: 746f 7263 682e 7465 6e73 6f72 285b 5b30  torch.tensor([[0
+00036a80: 2e38 3334 335d 2c20 5b31 2e32 3731 335d  .8343], [1.2713]
+00036a90: 2c20 5b31 2e32 3731 335d 2c20 5b31 2e32  , [1.2713], [1.2
+00036aa0: 3731 335d 2c20 5b31 2e32 3731 335d 5d29  713], [1.2713]])
+00036ab0: 0a20 2020 203e 3e3e 2072 6266 203d 2074  .    >>> rbf = t
+00036ac0: 6f72 6368 2e74 656e 736f 7228 5b5b 2d30  orch.tensor([[-0
+00036ad0: 2e32 3632 385d 2c20 5b2d 302e 3236 3238  .2628], [-0.2628
+00036ae0: 5d2c 205b 2d30 2e32 3632 385d 2c20 5b2d  ], [-0.2628], [-
+00036af0: 302e 3236 3238 5d2c 0a20 2020 202e 2e2e  0.2628],.    ...
+00036b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036b10: 2020 2020 205b 2d30 2e32 3632 395d 2c20       [-0.2629], 
+00036b20: 5b2d 302e 3236 3239 5d2c 205b 2d30 2e32  [-0.2629], [-0.2
+00036b30: 3632 385d 2c20 5b2d 302e 3236 3238 5d5d  628], [-0.2628]]
+00036b40: 290a 2020 2020 3e3e 3e20 7362 6631 203d  ).    >>> sbf1 =
+00036b50: 2074 6f72 6368 2e74 656e 736f 7228 5b5b   torch.tensor([[
+00036b60: 2d30 2e32 3736 375d 2c20 5b2d 302e 3237  -0.2767], [-0.27
+00036b70: 3637 5d2c 205b 2d30 2e32 3736 375d 2c20  67], [-0.2767], 
+00036b80: 5b2d 302e 3237 3637 5d2c 0a20 2020 202e  [-0.2767],.    .
+00036b90: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
+00036ba0: 2020 2020 2020 2020 5b2d 302e 3237 3637          [-0.2767
+00036bb0: 5d2c 205b 2d30 2e32 3736 375d 2c20 5b2d  ], [-0.2767], [-
+00036bc0: 302e 3237 3637 5d2c 205b 2d30 2e32 3736  0.2767], [-0.276
+00036bd0: 375d 2c0a 2020 2020 2e2e 2e20 2020 2020  7],.    ...     
 00036be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036bf0: 205b 2d30 2e30 3330 315d 2c20 5b2d 302e   [-0.0301], [-0.
-00036c00: 3134 3833 5d2c 205b 2d30 2e30 3330 315d  1483], [-0.0301]
-00036c10: 2c20 5b2d 302e 3134 3835 5d2c 205b 2d30  , [-0.1485], [-0
-00036c20: 2e31 3438 335d 2c0a 2020 2020 2e2e 2e20  .1483],.    ... 
-00036c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036c40: 2020 2020 205b 2d30 2e30 3330 315d 2c20       [-0.0301], 
-00036c50: 5b2d 302e 3134 3836 5d2c 205b 2d30 2e31  [-0.1486], [-0.1
-00036c60: 3438 355d 2c20 5b2d 302e 3033 3031 5d2c  485], [-0.0301],
-00036c70: 205b 2d30 2e31 3438 365d 2c0a 2020 2020   [-0.1486],.    
-00036c80: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
-00036c90: 2020 2020 2020 2020 205b 2d30 2e30 3330           [-0.030
-00036ca0: 315d 2c20 5b2d 302e 3134 3834 5d2c 205b  1], [-0.1484], [
-00036cb0: 2d30 2e31 3438 335d 2c20 5b2d 302e 3134  -0.1483], [-0.14
-00036cc0: 3836 5d2c 205b 2d30 2e30 3330 315d 5d29  86], [-0.0301]])
-00036cd0: 0a20 2020 203e 3e3e 2069 6478 5f6b 6a20  .    >>> idx_kj 
-00036ce0: 3d20 746f 7263 682e 7465 6e73 6f72 285b  = torch.tensor([
-00036cf0: 332c 2035 2c20 372c 2031 2c20 352c 2037  3, 5, 7, 1, 5, 7
-00036d00: 2c20 312c 2033 2c20 372c 2031 2c20 332c  , 1, 3, 7, 1, 3,
-00036d10: 2035 5d29 0a20 2020 203e 3e3e 2069 6478   5]).    >>> idx
-00036d20: 5f6a 695f 3120 3d20 746f 7263 682e 7465  _ji_1 = torch.te
-00036d30: 6e73 6f72 285b 302c 2030 2c20 302c 2032  nsor([0, 0, 0, 2
-00036d40: 2c20 322c 2032 2c20 342c 2034 2c20 342c  , 2, 2, 4, 4, 4,
-00036d50: 2036 2c20 362c 2036 5d29 0a20 2020 203e   6, 6, 6]).    >
-00036d60: 3e3e 2069 6478 5f6a 6a20 3d20 746f 7263  >> idx_jj = torc
-00036d70: 682e 7465 6e73 6f72 285b 302c 2031 2c20  h.tensor([0, 1, 
-00036d80: 332c 2035 2c20 372c 2032 2c20 312c 2033  3, 5, 7, 2, 1, 3
-00036d90: 2c20 352c 2037 2c20 342c 2031 2c20 332c  , 5, 7, 4, 1, 3,
-00036da0: 2035 2c20 372c 2036 2c20 312c 2033 2c20   5, 7, 6, 1, 3, 
-00036db0: 352c 2037 5d29 0a20 2020 203e 3e3e 2069  5, 7]).    >>> i
-00036dc0: 6478 5f6a 695f 3220 3d20 746f 7263 682e  dx_ji_2 = torch.
-00036dd0: 7465 6e73 6f72 285b 302c 2031 2c20 312c  tensor([0, 1, 1,
-00036de0: 2031 2c20 312c 2032 2c20 332c 2033 2c20   1, 1, 2, 3, 3, 
-00036df0: 332c 2033 2c20 342c 2035 2c20 352c 2035  3, 3, 4, 5, 5, 5
-00036e00: 2c20 352c 2036 2c20 372c 2037 2c20 372c  , 5, 6, 7, 7, 7,
-00036e10: 2037 5d29 0a20 2020 203e 3e3e 2065 6467   7]).    >>> edg
-00036e20: 655f 696e 6465 7820 3d20 746f 7263 682e  e_index = torch.
-00036e30: 7465 6e73 6f72 285b 5b30 2c20 312c 2030  tensor([[0, 1, 0
-00036e40: 2c20 322c 2030 2c20 332c 2030 2c20 345d  , 2, 0, 3, 0, 4]
-00036e50: 2c0a 2020 2020 2e2e 2e20 2020 2020 2020  ,.    ...       
-00036e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036e70: 2020 2020 5b31 2c20 302c 2032 2c20 302c      [1, 0, 2, 0,
-00036e80: 2033 2c20 302c 2034 2c20 305d 5d29 0a20   3, 0, 4, 0]]). 
-00036e90: 2020 203e 3e3e 206f 7574 203d 204d 584d     >>> out = MXM
-00036ea0: 4e65 744c 6f63 616c 4d65 7373 6167 6550  NetLocalMessageP
-00036eb0: 6173 7369 6e67 2864 696d 2c20 6163 7469  assing(dim, acti
-00036ec0: 7661 7469 6f6e 5f66 6e3d 2773 696c 7527  vation_fn='silu'
-00036ed0: 290a 2020 2020 3e3e 3e20 6f75 7470 7574  ).    >>> output
-00036ee0: 203d 206f 7574 2868 2c0a 2020 2020 2e2e   = out(h,.    ..
-00036ef0: 2e20 2020 2020 2020 2020 2020 2020 7262  .             rb
-00036f00: 662c 0a20 2020 202e 2e2e 2020 2020 2020  f,.    ...      
-00036f10: 2020 2020 2020 2073 6266 312c 0a20 2020         sbf1,.   
-00036f20: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
-00036f30: 2073 6266 322c 0a20 2020 202e 2e2e 2020   sbf2,.    ...  
-00036f40: 2020 2020 2020 2020 2020 2069 6478 5f6b             idx_k
-00036f50: 6a2c 0a20 2020 202e 2e2e 2020 2020 2020  j,.    ...      
-00036f60: 2020 2020 2020 2069 6478 5f6a 695f 312c         idx_ji_1,
-00036f70: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
-00036f80: 2020 2020 2069 6478 5f6a 6a2c 0a20 2020       idx_jj,.   
-00036f90: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
-00036fa0: 2069 6478 5f6a 695f 322c 0a20 2020 202e   idx_ji_2,.    .
-00036fb0: 2e2e 2020 2020 2020 2020 2020 2020 2065  ..             e
-00036fc0: 6467 655f 696e 6465 7829 0a20 2020 203e  dge_index).    >
-00036fd0: 3e3e 206f 7574 7075 745b 305d 2e73 6861  >> output[0].sha
-00036fe0: 7065 0a20 2020 2074 6f72 6368 2e53 697a  pe.    torch.Siz
-00036ff0: 6528 5b35 2c20 315d 290a 2020 2020 3e3e  e([5, 1]).    >>
-00037000: 3e20 6f75 7470 7574 5b31 5d2e 7368 6170  > output[1].shap
-00037010: 650a 2020 2020 746f 7263 682e 5369 7a65  e.    torch.Size
-00037020: 285b 352c 2031 5d29 0a20 2020 2022 2222  ([5, 1]).    """
-00037030: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00037040: 5f5f 2873 656c 662c 2064 696d 3a20 696e  __(self, dim: in
-00037050: 742c 2061 6374 6976 6174 696f 6e5f 666e  t, activation_fn
-00037060: 3a20 556e 696f 6e5b 4361 6c6c 6162 6c65  : Union[Callable
-00037070: 2c20 7374 725d 203d 2027 7369 6c75 2729  , str] = 'silu')
-00037080: 3a0a 2020 2020 2020 2020 2222 2249 6e69  :.        """Ini
-00037090: 7469 616c 697a 6573 2074 6865 204d 584d  tializes the MXM
-000370a0: 4e65 744c 6f63 616c 4d65 7373 6167 6550  NetLocalMessageP
-000370b0: 6173 7369 6e67 206c 6179 6572 2e0a 0a20  assing layer... 
-000370c0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-000370d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-000370e0: 2d2d 2d2d 0a20 2020 2020 2020 2064 696d  ----.        dim
-000370f0: 203a 2069 6e74 0a20 2020 2020 2020 2020   : int.         
-00037100: 2020 2054 6865 2064 696d 656e 7369 6f6e     The dimension
-00037110: 206f 6620 7468 6520 696e 7075 7420 616e   of the input an
-00037120: 6420 6f75 7470 7574 2074 656e 736f 7273  d output tensors
-00037130: 2066 6f72 2074 6865 206c 6f63 616c 206d   for the local m
-00037140: 6573 7361 6765 2070 6173 7369 6e67 206c  essage passing l
-00037150: 6179 6572 2e0a 2020 2020 2020 2020 6163  ayer..        ac
-00037160: 7469 7661 7469 6f6e 5f66 6e20 3a20 556e  tivation_fn : Un
-00037170: 696f 6e5b 4361 6c6c 6162 6c65 2c20 7374  ion[Callable, st
-00037180: 725d 2c20 6f70 7469 6f6e 616c 2028 6465  r], optional (de
-00037190: 6661 756c 743a 2027 7369 6c75 2729 0a20  fault: 'silu'). 
-000371a0: 2020 2020 2020 2020 2020 2054 6865 2061             The a
-000371b0: 6374 6976 6174 696f 6e20 6675 6e63 7469  ctivation functi
-000371c0: 6f6e 2074 6f20 6265 2075 7365 6420 696e  on to be used in
-000371d0: 2074 6865 206d 756c 7469 6c61 7965 7220   the multilayer 
-000371e0: 7065 7263 6570 7472 6f6e 7320 284d 4c50  perceptrons (MLP
-000371f0: 7329 2077 6974 6869 6e20 7468 6520 6c61  s) within the la
-00037200: 7965 722e 0a20 2020 2020 2020 2022 2222  yer..        """
-00037210: 0a20 2020 2020 2020 2073 7570 6572 284d  .        super(M
-00037220: 584d 4e65 744c 6f63 616c 4d65 7373 6167  XMNetLocalMessag
-00037230: 6550 6173 7369 6e67 2c20 7365 6c66 292e  ePassing, self).
-00037240: 5f5f 696e 6974 5f5f 2829 0a0a 2020 2020  __init__()..    
-00037250: 2020 2020 6163 7469 7661 7469 6f6e 5f66      activation_f
-00037260: 6e20 3d20 6765 745f 6163 7469 7661 7469  n = get_activati
-00037270: 6f6e 2861 6374 6976 6174 696f 6e5f 666e  on(activation_fn
-00037280: 290a 2020 2020 2020 2020 7365 6c66 2e68  ).        self.h
-00037290: 5f6d 6c70 3a20 4d75 6c74 696c 6179 6572  _mlp: Multilayer
-000372a0: 5065 7263 6570 7472 6f6e 203d 204d 756c  Perceptron = Mul
-000372b0: 7469 6c61 7965 7250 6572 6365 7074 726f  tilayerPerceptro
-000372c0: 6e28 0a20 2020 2020 2020 2020 2020 2064  n(.            d
-000372d0: 5f69 6e70 7574 3d64 696d 2c20 645f 6f75  _input=dim, d_ou
-000372e0: 7470 7574 3d64 696d 2c20 6163 7469 7661  tput=dim, activa
-000372f0: 7469 6f6e 5f66 6e3d 6163 7469 7661 7469  tion_fn=activati
-00037300: 6f6e 5f66 6e29 0a20 2020 2020 2020 2073  on_fn).        s
-00037310: 656c 662e 6d6c 705f 6b6a 3a20 4d75 6c74  elf.mlp_kj: Mult
-00037320: 696c 6179 6572 5065 7263 6570 7472 6f6e  ilayerPerceptron
-00037330: 203d 204d 756c 7469 6c61 7965 7250 6572   = MultilayerPer
-00037340: 6365 7074 726f 6e28 0a20 2020 2020 2020  ceptron(.       
-00037350: 2020 2020 2064 5f69 6e70 7574 3d33 202a       d_input=3 *
-00037360: 2064 696d 2c20 645f 6f75 7470 7574 3d64   dim, d_output=d
-00037370: 696d 2c20 6163 7469 7661 7469 6f6e 5f66  im, activation_f
-00037380: 6e3d 6163 7469 7661 7469 6f6e 5f66 6e29  n=activation_fn)
-00037390: 0a20 2020 2020 2020 2073 656c 662e 6d6c  .        self.ml
-000373a0: 705f 6a69 5f31 3a20 4d75 6c74 696c 6179  p_ji_1: Multilay
-000373b0: 6572 5065 7263 6570 7472 6f6e 203d 204d  erPerceptron = M
-000373c0: 756c 7469 6c61 7965 7250 6572 6365 7074  ultilayerPercept
-000373d0: 726f 6e28 0a20 2020 2020 2020 2020 2020  ron(.           
-000373e0: 2064 5f69 6e70 7574 3d33 202a 2064 696d   d_input=3 * dim
-000373f0: 2c20 645f 6f75 7470 7574 3d64 696d 2c20  , d_output=dim, 
-00037400: 6163 7469 7661 7469 6f6e 5f66 6e3d 6163  activation_fn=ac
-00037410: 7469 7661 7469 6f6e 5f66 6e29 0a20 2020  tivation_fn).   
-00037420: 2020 2020 2073 656c 662e 6d6c 705f 6a69       self.mlp_ji
-00037430: 5f32 3a20 4d75 6c74 696c 6179 6572 5065  _2: MultilayerPe
-00037440: 7263 6570 7472 6f6e 203d 204d 756c 7469  rceptron = Multi
-00037450: 6c61 7965 7250 6572 6365 7074 726f 6e28  layerPerceptron(
-00037460: 0a20 2020 2020 2020 2020 2020 2064 5f69  .            d_i
-00037470: 6e70 7574 3d64 696d 2c20 645f 6f75 7470  nput=dim, d_outp
-00037480: 7574 3d64 696d 2c20 6163 7469 7661 7469  ut=dim, activati
-00037490: 6f6e 5f66 6e3d 6163 7469 7661 7469 6f6e  on_fn=activation
-000374a0: 5f66 6e29 0a20 2020 2020 2020 2073 656c  _fn).        sel
-000374b0: 662e 6d6c 705f 6a6a 3a20 4d75 6c74 696c  f.mlp_jj: Multil
-000374c0: 6179 6572 5065 7263 6570 7472 6f6e 203d  ayerPerceptron =
-000374d0: 204d 756c 7469 6c61 7965 7250 6572 6365   MultilayerPerce
-000374e0: 7074 726f 6e28 0a20 2020 2020 2020 2020  ptron(.         
-000374f0: 2020 2064 5f69 6e70 7574 3d64 696d 2c20     d_input=dim, 
-00037500: 645f 6f75 7470 7574 3d64 696d 2c20 6163  d_output=dim, ac
-00037510: 7469 7661 7469 6f6e 5f66 6e3d 6163 7469  tivation_fn=acti
-00037520: 7661 7469 6f6e 5f66 6e29 0a0a 2020 2020  vation_fn)..    
-00037530: 2020 2020 7365 6c66 2e6d 6c70 5f73 6266      self.mlp_sbf
-00037540: 313a 204d 756c 7469 6c61 7965 7250 6572  1: MultilayerPer
-00037550: 6365 7074 726f 6e20 3d20 4d75 6c74 696c  ceptron = Multil
-00037560: 6179 6572 5065 7263 6570 7472 6f6e 280a  ayerPerceptron(.
-00037570: 2020 2020 2020 2020 2020 2020 645f 696e              d_in
-00037580: 7075 743d 6469 6d2c 0a20 2020 2020 2020  put=dim,.       
-00037590: 2020 2020 2064 5f68 6964 6465 6e3d 2864       d_hidden=(d
-000375a0: 696d 2c29 2c0a 2020 2020 2020 2020 2020  im,),.          
-000375b0: 2020 645f 6f75 7470 7574 3d64 696d 2c0a    d_output=dim,.
-000375c0: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-000375d0: 7661 7469 6f6e 5f66 6e3d 6163 7469 7661  vation_fn=activa
-000375e0: 7469 6f6e 5f66 6e29 0a20 2020 2020 2020  tion_fn).       
-000375f0: 2073 656c 662e 6d6c 705f 7362 6632 3a20   self.mlp_sbf2: 
-00037600: 4d75 6c74 696c 6179 6572 5065 7263 6570  MultilayerPercep
-00037610: 7472 6f6e 203d 204d 756c 7469 6c61 7965  tron = Multilaye
-00037620: 7250 6572 6365 7074 726f 6e28 0a20 2020  rPerceptron(.   
-00037630: 2020 2020 2020 2020 2064 5f69 6e70 7574           d_input
-00037640: 3d64 696d 2c0a 2020 2020 2020 2020 2020  =dim,.          
-00037650: 2020 645f 6869 6464 656e 3d28 6469 6d2c    d_hidden=(dim,
-00037660: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
-00037670: 5f6f 7574 7075 743d 6469 6d2c 0a20 2020  _output=dim,.   
-00037680: 2020 2020 2020 2020 2061 6374 6976 6174           activat
-00037690: 696f 6e5f 666e 3d61 6374 6976 6174 696f  ion_fn=activatio
-000376a0: 6e5f 666e 290a 0a20 2020 2020 2020 2073  n_fn)..        s
-000376b0: 656c 662e 7265 7331 3a20 4d75 6c74 696c  elf.res1: Multil
-000376c0: 6179 6572 5065 7263 6570 7472 6f6e 203d  ayerPerceptron =
-000376d0: 204d 756c 7469 6c61 7965 7250 6572 6365   MultilayerPerce
-000376e0: 7074 726f 6e28 0a20 2020 2020 2020 2020  ptron(.         
-000376f0: 2020 2064 5f69 6e70 7574 3d64 696d 2c0a     d_input=dim,.
-00037700: 2020 2020 2020 2020 2020 2020 645f 6869              d_hi
-00037710: 6464 656e 3d28 6469 6d2c 292c 0a20 2020  dden=(dim,),.   
-00037720: 2020 2020 2020 2020 2064 5f6f 7574 7075           d_outpu
-00037730: 743d 6469 6d2c 0a20 2020 2020 2020 2020  t=dim,.         
-00037740: 2020 2061 6374 6976 6174 696f 6e5f 666e     activation_fn
-00037750: 3d61 6374 6976 6174 696f 6e5f 666e 2c0a  =activation_fn,.
-00037760: 2020 2020 2020 2020 2020 2020 736b 6970              skip
-00037770: 5f63 6f6e 6e65 6374 696f 6e3d 5472 7565  _connection=True
-00037780: 2c0a 2020 2020 2020 2020 2020 2020 7765  ,.            we
-00037790: 6967 6874 6564 5f73 6b69 703d 4661 6c73  ighted_skip=Fals
-000377a0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-000377b0: 7265 7332 3a20 4d75 6c74 696c 6179 6572  res2: Multilayer
-000377c0: 5065 7263 6570 7472 6f6e 203d 204d 756c  Perceptron = Mul
-000377d0: 7469 6c61 7965 7250 6572 6365 7074 726f  tilayerPerceptro
-000377e0: 6e28 0a20 2020 2020 2020 2020 2020 2064  n(.            d
-000377f0: 5f69 6e70 7574 3d64 696d 2c0a 2020 2020  _input=dim,.    
-00037800: 2020 2020 2020 2020 645f 6869 6464 656e          d_hidden
-00037810: 3d28 6469 6d2c 292c 0a20 2020 2020 2020  =(dim,),.       
-00037820: 2020 2020 2064 5f6f 7574 7075 743d 6469       d_output=di
-00037830: 6d2c 0a20 2020 2020 2020 2020 2020 2061  m,.            a
-00037840: 6374 6976 6174 696f 6e5f 666e 3d61 6374  ctivation_fn=act
-00037850: 6976 6174 696f 6e5f 666e 2c0a 2020 2020  ivation_fn,.    
-00037860: 2020 2020 2020 2020 736b 6970 5f63 6f6e          skip_con
-00037870: 6e65 6374 696f 6e3d 5472 7565 2c0a 2020  nection=True,.  
-00037880: 2020 2020 2020 2020 2020 7765 6967 6874            weight
-00037890: 6564 5f73 6b69 703d 4661 6c73 6529 0a20  ed_skip=False). 
-000378a0: 2020 2020 2020 2073 656c 662e 7265 7333         self.res3
-000378b0: 3a20 4d75 6c74 696c 6179 6572 5065 7263  : MultilayerPerc
-000378c0: 6570 7472 6f6e 203d 204d 756c 7469 6c61  eptron = Multila
-000378d0: 7965 7250 6572 6365 7074 726f 6e28 0a20  yerPerceptron(. 
-000378e0: 2020 2020 2020 2020 2020 2064 5f69 6e70             d_inp
-000378f0: 7574 3d64 696d 2c0a 2020 2020 2020 2020  ut=dim,.        
-00037900: 2020 2020 645f 6869 6464 656e 3d28 6469      d_hidden=(di
-00037910: 6d2c 292c 0a20 2020 2020 2020 2020 2020  m,),.           
-00037920: 2064 5f6f 7574 7075 743d 6469 6d2c 0a20   d_output=dim,. 
-00037930: 2020 2020 2020 2020 2020 2061 6374 6976             activ
-00037940: 6174 696f 6e5f 666e 3d61 6374 6976 6174  ation_fn=activat
-00037950: 696f 6e5f 666e 2c0a 2020 2020 2020 2020  ion_fn,.        
-00037960: 2020 2020 736b 6970 5f63 6f6e 6e65 6374      skip_connect
-00037970: 696f 6e3d 5472 7565 2c0a 2020 2020 2020  ion=True,.      
-00037980: 2020 2020 2020 7765 6967 6874 6564 5f73        weighted_s
-00037990: 6b69 703d 4661 6c73 6529 0a0a 2020 2020  kip=False)..    
-000379a0: 2020 2020 7365 6c66 2e6c 696e 5f72 6266      self.lin_rbf
-000379b0: 313a 206e 6e2e 4c69 6e65 6172 203d 206e  1: nn.Linear = n
-000379c0: 6e2e 4c69 6e65 6172 2864 696d 2c20 6469  n.Linear(dim, di
-000379d0: 6d2c 2062 6961 733d 4661 6c73 6529 0a20  m, bias=False). 
-000379e0: 2020 2020 2020 2073 656c 662e 6c69 6e5f         self.lin_
-000379f0: 7262 6632 3a20 6e6e 2e4c 696e 6561 7220  rbf2: nn.Linear 
-00037a00: 3d20 6e6e 2e4c 696e 6561 7228 6469 6d2c  = nn.Linear(dim,
-00037a10: 2064 696d 2c20 6269 6173 3d46 616c 7365   dim, bias=False
-00037a20: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00037a30: 696e 5f72 6266 5f6f 7574 3a20 6e6e 2e4c  in_rbf_out: nn.L
-00037a40: 696e 6561 7220 3d20 6e6e 2e4c 696e 6561  inear = nn.Linea
-00037a50: 7228 6469 6d2c 2064 696d 2c20 6269 6173  r(dim, dim, bias
-00037a60: 3d46 616c 7365 290a 0a20 2020 2020 2020  =False)..       
-00037a70: 2073 656c 662e 6d6c 703a 204d 756c 7469   self.mlp: Multi
-00037a80: 6c61 7965 7250 6572 6365 7074 726f 6e20  layerPerceptron 
-00037a90: 3d20 4d75 6c74 696c 6179 6572 5065 7263  = MultilayerPerc
-00037aa0: 6570 7472 6f6e 280a 2020 2020 2020 2020  eptron(.        
-00037ab0: 2020 2020 645f 696e 7075 743d 6469 6d2c      d_input=dim,
-00037ac0: 2064 5f6f 7574 7075 743d 6469 6d2c 2061   d_output=dim, a
-00037ad0: 6374 6976 6174 696f 6e5f 666e 3d61 6374  ctivation_fn=act
-00037ae0: 6976 6174 696f 6e5f 666e 290a 2020 2020  ivation_fn).    
-00037af0: 2020 2020 7365 6c66 2e6f 7574 5f6d 6c70      self.out_mlp
-00037b00: 3a20 4d75 6c74 696c 6179 6572 5065 7263  : MultilayerPerc
-00037b10: 6570 7472 6f6e 203d 204d 756c 7469 6c61  eptron = Multila
-00037b20: 7965 7250 6572 6365 7074 726f 6e28 0a20  yerPerceptron(. 
-00037b30: 2020 2020 2020 2020 2020 2064 5f69 6e70             d_inp
-00037b40: 7574 3d64 696d 2c0a 2020 2020 2020 2020  ut=dim,.        
-00037b50: 2020 2020 645f 6869 6464 656e 3d28 6469      d_hidden=(di
-00037b60: 6d2c 2064 696d 292c 0a20 2020 2020 2020  m, dim),.       
-00037b70: 2020 2020 2064 5f6f 7574 7075 743d 6469       d_output=di
-00037b80: 6d2c 0a20 2020 2020 2020 2020 2020 2061  m,.            a
-00037b90: 6374 6976 6174 696f 6e5f 666e 3d61 6374  ctivation_fn=act
-00037ba0: 6976 6174 696f 6e5f 666e 290a 2020 2020  ivation_fn).    
-00037bb0: 2020 2020 7365 6c66 2e6f 7574 5f57 3a20      self.out_W: 
-00037bc0: 6e6e 2e4c 696e 6561 7220 3d20 6e6e 2e4c  nn.Linear = nn.L
-00037bd0: 696e 6561 7228 6469 6d2c 2031 290a 0a20  inear(dim, 1).. 
-00037be0: 2020 2064 6566 2066 6f72 7761 7264 2873     def forward(s
-00037bf0: 656c 662c 206e 6f64 655f 6665 6174 7572  elf, node_featur
-00037c00: 6573 3a20 746f 7263 682e 5465 6e73 6f72  es: torch.Tensor
-00037c10: 2c20 7262 663a 2074 6f72 6368 2e54 656e  , rbf: torch.Ten
-00037c20: 736f 722c 0a20 2020 2020 2020 2020 2020  sor,.           
-00037c30: 2020 2020 2073 6266 313a 2074 6f72 6368       sbf1: torch
-00037c40: 2e54 656e 736f 722c 2073 6266 323a 2074  .Tensor, sbf2: t
-00037c50: 6f72 6368 2e54 656e 736f 722c 2069 6478  orch.Tensor, idx
-00037c60: 5f6b 6a3a 2074 6f72 6368 2e54 656e 736f  _kj: torch.Tenso
-00037c70: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00037c80: 2020 2069 6478 5f6a 695f 313a 2074 6f72     idx_ji_1: tor
-00037c90: 6368 2e54 656e 736f 722c 2069 6478 5f6a  ch.Tensor, idx_j
-00037ca0: 6a3a 2074 6f72 6368 2e54 656e 736f 722c  j: torch.Tensor,
-00037cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00037cc0: 2069 6478 5f6a 695f 323a 2074 6f72 6368   idx_ji_2: torch
-00037cd0: 2e54 656e 736f 722c 0a20 2020 2020 2020  .Tensor,.       
-00037ce0: 2020 2020 2020 2020 2065 6467 655f 696e           edge_in
-00037cf0: 6465 783a 2074 6f72 6368 2e54 656e 736f  dex: torch.Tenso
-00037d00: 7229 202d 3e20 5475 706c 655b 746f 7263  r) -> Tuple[torc
-00037d10: 682e 5465 6e73 6f72 2c20 746f 7263 682e  h.Tensor, torch.
-00037d20: 5465 6e73 6f72 5d3a 0a20 2020 2020 2020  Tensor]:.       
-00037d30: 2022 2222 5468 6520 666f 7277 6172 6420   """The forward 
-00037d40: 6d65 7468 6f64 2070 6572 666f 726d 7320  method performs 
-00037d50: 7468 6520 636f 6d70 7574 6174 696f 6e20  the computation 
-00037d60: 666f 7220 7468 6520 4d58 4d4e 6574 4c6f  for the MXMNetLo
-00037d70: 6361 6c4d 6573 7361 6765 5061 7373 696e  calMessagePassin
-00037d80: 6720 4c61 7965 722e 0a20 2020 2020 2020  g Layer..       
-00037d90: 2054 6869 7320 6d65 7468 6f64 2070 726f   This method pro
-00037da0: 6365 7373 6573 2074 6865 2069 6e70 7574  cesses the input
-00037db0: 2074 656e 736f 7273 2072 6570 7265 7365   tensors represe
-00037dc0: 6e74 696e 6720 6174 6f6d 2066 6561 7475  nting atom featu
-00037dd0: 7265 732c 2072 6164 6961 6c20 6261 7369  res, radial basi
-00037de0: 7320 6675 6e63 7469 6f6e 7320 2852 4246  s functions (RBF
-00037df0: 292c 2061 6e64 2073 7068 6572 6963 616c  ), and spherical
-00037e00: 2062 6173 6973 2066 756e 6374 696f 6e73   basis functions
-00037e10: 2028 5342 4629 2075 7369 6e67 206d 6573   (SBF) using mes
-00037e20: 7361 6765 2070 6173 7369 6e67 206f 7665  sage passing ove
-00037e30: 7220 7468 6520 6d6f 6c65 6375 6c61 7220  r the molecular 
-00037e40: 6772 6170 682e 2054 6865 206d 6573 7361  graph. The messa
-00037e50: 6765 2070 6173 7369 6e67 2075 7064 6174  ge passing updat
-00037e60: 6573 2074 6865 2061 746f 6d20 7265 7072  es the atom repr
-00037e70: 6573 656e 7461 7469 6f6e 732c 2061 6e64  esentations, and
-00037e80: 2074 6865 2072 6573 756c 7469 6e67 2074   the resulting t
-00037e90: 656e 736f 7220 7265 7072 6573 656e 7473  ensor represents
-00037ea0: 2074 6865 2075 7064 6174 6564 2061 746f   the updated ato
-00037eb0: 6d20 6665 6174 7572 6520 6166 7465 7220  m feature after 
-00037ec0: 6c6f 6361 6c20 6d65 7373 6167 6520 7061  local message pa
-00037ed0: 7373 696e 672e 0a0a 2020 2020 2020 2020  ssing...        
-00037ee0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00037ef0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00037f00: 2020 2020 2020 6e6f 6465 5f66 6561 7475        node_featu
-00037f10: 7265 7320 3a20 746f 7263 682e 5465 6e73  res : torch.Tens
-00037f20: 6f72 0a20 2020 2020 2020 2020 2020 2049  or.            I
-00037f30: 6e70 7574 2074 656e 736f 7220 7265 7072  nput tensor repr
-00037f40: 6573 656e 7469 6e67 2061 746f 6d20 6665  esenting atom fe
-00037f50: 6174 7572 6573 2e0a 2020 2020 2020 2020  atures..        
-00037f60: 7262 6620 3a20 746f 7263 682e 5465 6e73  rbf : torch.Tens
-00037f70: 6f72 0a20 2020 2020 2020 2020 2020 2049  or.            I
-00037f80: 6e70 7574 2074 656e 736f 7220 7265 7072  nput tensor repr
-00037f90: 6573 656e 7469 6e67 2072 6164 6961 6c20  esenting radial 
-00037fa0: 6261 7369 7320 6675 6e63 7469 6f6e 732e  basis functions.
-00037fb0: 0a20 2020 2020 2020 2073 6266 3120 3a20  .        sbf1 : 
-00037fc0: 746f 7263 682e 5465 6e73 6f72 0a20 2020  torch.Tensor.   
-00037fd0: 2020 2020 2020 2020 2049 6e70 7574 2074           Input t
-00037fe0: 656e 736f 7220 7265 7072 6573 656e 7469  ensor representi
-00037ff0: 6e67 2074 6865 2066 6972 7374 2073 6574  ng the first set
-00038000: 206f 6620 7370 6865 7269 6361 6c20 6261   of spherical ba
-00038010: 7369 7320 6675 6e63 7469 6f6e 732e 0a20  sis functions.. 
-00038020: 2020 2020 2020 2073 6266 3220 3a20 746f         sbf2 : to
-00038030: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
-00038040: 2020 2020 2020 2049 6e70 7574 2074 656e         Input ten
-00038050: 736f 7220 7265 7072 6573 656e 7469 6e67  sor representing
-00038060: 2074 6865 2073 6563 6f6e 6420 7365 7420   the second set 
-00038070: 6f66 2073 7068 6572 6963 616c 2062 6173  of spherical bas
-00038080: 6973 2066 756e 6374 696f 6e73 2e0a 2020  is functions..  
-00038090: 2020 2020 2020 6964 785f 6b6a 203a 2074        idx_kj : t
-000380a0: 6f72 6368 2e54 656e 736f 720a 2020 2020  orch.Tensor.    
-000380b0: 2020 2020 2020 2020 5465 6e73 6f72 2063          Tensor c
-000380c0: 6f6e 7461 696e 696e 6720 696e 6469 6365  ontaining indice
-000380d0: 7320 666f 7220 7468 6520 6b20 616e 6420  s for the k and 
-000380e0: 6a20 6174 6f6d 7320 696e 766f 6c76 6564  j atoms involved
-000380f0: 2069 6e20 6561 6368 2069 6e74 6572 6163   in each interac
-00038100: 7469 6f6e 2e0a 2020 2020 2020 2020 6964  tion..        id
-00038110: 785f 6a69 5f31 203a 2074 6f72 6368 2e54  x_ji_1 : torch.T
-00038120: 656e 736f 720a 2020 2020 2020 2020 2020  ensor.          
-00038130: 2020 5465 6e73 6f72 2063 6f6e 7461 696e    Tensor contain
-00038140: 696e 6720 696e 6469 6365 7320 666f 7220  ing indices for 
-00038150: 7468 6520 6a20 616e 6420 6920 6174 6f6d  the j and i atom
-00038160: 7320 696e 766f 6c76 6564 2069 6e20 7468  s involved in th
-00038170: 6520 6669 7273 7420 6d65 7373 6167 6520  e first message 
-00038180: 7061 7373 696e 6720 7374 6570 2e0a 2020  passing step..  
-00038190: 2020 2020 2020 6964 785f 6a6a 203a 2074        idx_jj : t
-000381a0: 6f72 6368 2e54 656e 736f 720a 2020 2020  orch.Tensor.    
-000381b0: 2020 2020 2020 2020 5465 6e73 6f72 2063          Tensor c
-000381c0: 6f6e 7461 696e 696e 6720 696e 6469 6365  ontaining indice
-000381d0: 7320 666f 7220 7468 6520 6a20 616e 6420  s for the j and 
-000381e0: 6a27 2061 746f 6d73 2069 6e76 6f6c 7665  j' atoms involve
-000381f0: 6420 696e 2074 6865 2073 6563 6f6e 6420  d in the second 
-00038200: 6d65 7373 6167 6520 7061 7373 696e 6720  message passing 
-00038210: 7374 6570 2e0a 2020 2020 2020 2020 6964  step..        id
-00038220: 785f 6a69 5f32 203a 2074 6f72 6368 2e54  x_ji_2 : torch.T
-00038230: 656e 736f 720a 2020 2020 2020 2020 2020  ensor.          
-00038240: 2020 5465 6e73 6f72 2063 6f6e 7461 696e    Tensor contain
-00038250: 696e 6720 696e 6469 6365 7320 666f 7220  ing indices for 
-00038260: 7468 6520 6a20 616e 6420 6920 6174 6f6d  the j and i atom
-00038270: 7320 696e 766f 6c76 6564 2069 6e20 7468  s involved in th
-00038280: 6520 7365 636f 6e64 206d 6573 7361 6765  e second message
-00038290: 2070 6173 7369 6e67 2073 7465 702e 0a20   passing step.. 
-000382a0: 2020 2020 2020 2065 6467 655f 696e 6465         edge_inde
-000382b0: 7820 3a20 746f 7263 682e 5465 6e73 6f72  x : torch.Tensor
-000382c0: 0a20 2020 2020 2020 2020 2020 2054 656e  .            Ten
-000382d0: 736f 7220 636f 6e74 6169 6e69 6e67 2074  sor containing t
-000382e0: 6865 2065 6467 6520 696e 6469 6365 7320  he edge indices 
-000382f0: 6f66 2074 6865 206d 6f6c 6563 756c 6172  of the molecular
-00038300: 2067 7261 7068 2c20 7769 7468 2073 6861   graph, with sha
-00038310: 7065 2028 322c 204d 292c 2077 6865 7265  pe (2, M), where
-00038320: 204d 2069 7320 7468 6520 6e75 6d62 6572   M is the number
-00038330: 206f 6620 6564 6765 732e 0a0a 2020 2020   of edges...    
-00038340: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00038350: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00038360: 2020 2020 6e6f 6465 5f66 6561 7475 7265      node_feature
-00038370: 733a 2074 6f72 6368 2e54 656e 736f 720a  s: torch.Tensor.
-00038380: 2020 2020 2020 2020 2020 2020 5570 6461              Upda
-00038390: 7465 6420 6174 6f6d 2072 6570 7265 7365  ted atom represe
-000383a0: 6e74 6174 696f 6e73 2061 6674 6572 206c  ntations after l
-000383b0: 6f63 616c 206d 6573 7361 6765 2070 6173  ocal message pas
-000383c0: 7369 6e67 2e0a 2020 2020 2020 2020 6f75  sing..        ou
-000383d0: 7470 7574 3a20 746f 7263 682e 5465 6e73  tput: torch.Tens
-000383e0: 6f72 0a20 2020 2020 2020 2020 2020 204f  or.            O
-000383f0: 7574 7075 7420 7465 6e73 6f72 2072 6570  utput tensor rep
-00038400: 7265 7365 6e74 696e 6720 6120 6669 7865  resenting a fixe
-00038410: 642d 7369 7a65 2072 6570 7265 7365 6e74  d-size represent
-00038420: 6174 696f 6e2c 2077 6974 6820 7368 6170  ation, with shap
-00038430: 6520 284e 2c20 3129 2e0a 2020 2020 2020  e (N, 1)..      
-00038440: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-00038450: 6573 6964 7561 6c5f 6e6f 6465 5f66 6561  esidual_node_fea
-00038460: 7475 7265 733a 2074 6f72 6368 2e54 656e  tures: torch.Ten
-00038470: 736f 7220 3d20 6e6f 6465 5f66 6561 7475  sor = node_featu
-00038480: 7265 730a 0a20 2020 2020 2020 2023 2049  res..        # I
-00038490: 6e74 6567 7261 7465 2074 6865 2043 726f  ntegrate the Cro
-000384a0: 7373 204c 6179 6572 204d 6170 7069 6e67  ss Layer Mapping
-000384b0: 2069 6e73 6964 6520 7468 6520 4c6f 6361   inside the Loca
-000384c0: 6c20 4d65 7373 6167 6520 5061 7373 696e  l Message Passin
-000384d0: 670a 2020 2020 2020 2020 6e6f 6465 5f66  g.        node_f
-000384e0: 6561 7475 7265 7320 3d20 7365 6c66 2e68  eatures = self.h
-000384f0: 5f6d 6c70 286e 6f64 655f 6665 6174 7572  _mlp(node_featur
-00038500: 6573 290a 0a20 2020 2020 2020 2023 204d  es)..        # M
-00038510: 6573 7361 6765 2050 6173 7369 6e67 2031  essage Passing 1
-00038520: 0a20 2020 2020 2020 206a 2c20 6920 3d20  .        j, i = 
-00038530: 6564 6765 5f69 6e64 6578 0a20 2020 2020  edge_index.     
-00038540: 2020 206d 3a20 746f 7263 682e 5465 6e73     m: torch.Tens
-00038550: 6f72 203d 2074 6f72 6368 2e63 6174 285b  or = torch.cat([
-00038560: 6e6f 6465 5f66 6561 7475 7265 735b 695d  node_features[i]
-00038570: 2c20 6e6f 6465 5f66 6561 7475 7265 735b  , node_features[
-00038580: 6a5d 2c20 7262 665d 2c0a 2020 2020 2020  j], rbf],.      
-00038590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000385a0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-000385b0: 6d3d 2d31 290a 0a20 2020 2020 2020 206d  m=-1)..        m
-000385c0: 5f6b 6a3a 2074 6f72 6368 2e54 656e 736f  _kj: torch.Tenso
-000385d0: 7220 3d20 7365 6c66 2e6d 6c70 5f6b 6a28  r = self.mlp_kj(
-000385e0: 6d29 0a20 2020 2020 2020 206d 5f6b 6a20  m).        m_kj 
-000385f0: 3d20 6d5f 6b6a 202a 2073 656c 662e 6c69  = m_kj * self.li
-00038600: 6e5f 7262 6631 2872 6266 290a 2020 2020  n_rbf1(rbf).    
-00038610: 2020 2020 6d5f 6b6a 203d 206d 5f6b 6a5b      m_kj = m_kj[
-00038620: 6964 785f 6b6a 5d20 2a20 7365 6c66 2e6d  idx_kj] * self.m
-00038630: 6c70 5f73 6266 3128 7362 6631 290a 2020  lp_sbf1(sbf1).  
-00038640: 2020 2020 2020 6d5f 6b6a 203d 2073 6361        m_kj = sca
-00038650: 7474 6572 286d 5f6b 6a2c 2069 6478 5f6a  tter(m_kj, idx_j
-00038660: 695f 312c 2064 696d 3d30 2c20 6469 6d5f  i_1, dim=0, dim_
-00038670: 7369 7a65 3d6d 2e73 697a 6528 3029 2c20  size=m.size(0), 
-00038680: 7265 6475 6365 3d27 6164 6427 290a 0a20  reduce='add').. 
-00038690: 2020 2020 2020 206d 5f6a 695f 313a 2074         m_ji_1: t
-000386a0: 6f72 6368 2e54 656e 736f 7220 3d20 7365  orch.Tensor = se
-000386b0: 6c66 2e6d 6c70 5f6a 695f 3128 6d29 0a0a  lf.mlp_ji_1(m)..
-000386c0: 2020 2020 2020 2020 6d20 3d20 6d5f 6a69          m = m_ji
-000386d0: 5f31 202b 206d 5f6b 6a0a 0a20 2020 2020  _1 + m_kj..     
-000386e0: 2020 2023 204d 6573 7361 6765 2050 6173     # Message Pas
-000386f0: 7369 6e67 2032 0a20 2020 2020 2020 206d  sing 2.        m
-00038700: 5f6a 6a3a 2074 6f72 6368 2e54 656e 736f  _jj: torch.Tenso
-00038710: 7220 3d20 7365 6c66 2e6d 6c70 5f6a 6a28  r = self.mlp_jj(
-00038720: 6d29 0a20 2020 2020 2020 206d 5f6a 6a20  m).        m_jj 
-00038730: 3d20 6d5f 6a6a 202a 2073 656c 662e 6c69  = m_jj * self.li
-00038740: 6e5f 7262 6632 2872 6266 290a 2020 2020  n_rbf2(rbf).    
-00038750: 2020 2020 6d5f 6a6a 203d 206d 5f6a 6a5b      m_jj = m_jj[
-00038760: 6964 785f 6a6a 5d20 2a20 7365 6c66 2e6d  idx_jj] * self.m
-00038770: 6c70 5f73 6266 3228 7362 6632 290a 2020  lp_sbf2(sbf2).  
-00038780: 2020 2020 2020 6d5f 6a6a 203d 2073 6361        m_jj = sca
-00038790: 7474 6572 286d 5f6a 6a2c 2069 6478 5f6a  tter(m_jj, idx_j
-000387a0: 695f 322c 2064 696d 3d30 2c20 6469 6d5f  i_2, dim=0, dim_
-000387b0: 7369 7a65 3d6d 2e73 697a 6528 3029 2c20  size=m.size(0), 
-000387c0: 7265 6475 6365 3d27 6164 6427 290a 0a20  reduce='add').. 
-000387d0: 2020 2020 2020 206d 5f6a 695f 323a 2074         m_ji_2: t
-000387e0: 6f72 6368 2e54 656e 736f 7220 3d20 7365  orch.Tensor = se
-000387f0: 6c66 2e6d 6c70 5f6a 695f 3228 6d29 0a0a  lf.mlp_ji_2(m)..
-00038800: 2020 2020 2020 2020 6d20 3d20 6d5f 6a69          m = m_ji
-00038810: 5f32 202b 206d 5f6a 6a0a 0a20 2020 2020  _2 + m_jj..     
-00038820: 2020 2023 2041 6767 7265 6761 7469 6f6e     # Aggregation
-00038830: 0a20 2020 2020 2020 206d 203d 2073 656c  .        m = sel
-00038840: 662e 6c69 6e5f 7262 665f 6f75 7428 7262  f.lin_rbf_out(rb
-00038850: 6629 202a 206d 0a20 2020 2020 2020 206e  f) * m.        n
-00038860: 6f64 655f 6665 6174 7572 6573 203d 2073  ode_features = s
-00038870: 6361 7474 6572 286d 2c0a 2020 2020 2020  catter(m,.      
-00038880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00038890: 2020 2020 2020 2020 2020 692c 0a20 2020            i,.   
-000388a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000388b0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-000388c0: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
-000388d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000388e0: 2020 2020 6469 6d5f 7369 7a65 3d6e 6f64      dim_size=nod
-000388f0: 655f 6665 6174 7572 6573 2e73 697a 6528  e_features.size(
-00038900: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
-00038910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00038920: 2020 2020 7265 6475 6365 3d27 6164 6427      reduce='add'
-00038930: 290a 0a20 2020 2020 2020 2023 2055 7064  )..        # Upd
-00038940: 6174 6520 6675 6e63 7469 6f6e 2066 5f75  ate function f_u
-00038950: 0a20 2020 2020 2020 206e 6f64 655f 6665  .        node_fe
-00038960: 6174 7572 6573 203d 2073 656c 662e 7265  atures = self.re
-00038970: 7331 286e 6f64 655f 6665 6174 7572 6573  s1(node_features
-00038980: 290a 2020 2020 2020 2020 6e6f 6465 5f66  ).        node_f
-00038990: 6561 7475 7265 7320 3d20 7365 6c66 2e6d  eatures = self.m
-000389a0: 6c70 286e 6f64 655f 6665 6174 7572 6573  lp(node_features
-000389b0: 2920 2b20 7265 7369 6475 616c 5f6e 6f64  ) + residual_nod
-000389c0: 655f 6665 6174 7572 6573 0a20 2020 2020  e_features.     
-000389d0: 2020 206e 6f64 655f 6665 6174 7572 6573     node_features
-000389e0: 203d 2073 656c 662e 7265 7332 286e 6f64   = self.res2(nod
-000389f0: 655f 6665 6174 7572 6573 290a 2020 2020  e_features).    
-00038a00: 2020 2020 6e6f 6465 5f66 6561 7475 7265      node_feature
-00038a10: 7320 3d20 7365 6c66 2e72 6573 3328 6e6f  s = self.res3(no
-00038a20: 6465 5f66 6561 7475 7265 7329 0a0a 2020  de_features)..  
-00038a30: 2020 2020 2020 2320 4f75 7470 7574 204d        # Output M
-00038a40: 6f64 756c 650a 2020 2020 2020 2020 6f75  odule.        ou
-00038a50: 743a 2074 6f72 6368 2e54 656e 736f 7220  t: torch.Tensor 
-00038a60: 3d20 7365 6c66 2e6f 7574 5f6d 6c70 286e  = self.out_mlp(n
-00038a70: 6f64 655f 6665 6174 7572 6573 290a 2020  ode_features).  
-00038a80: 2020 2020 2020 6f75 7470 7574 3a20 746f        output: to
-00038a90: 7263 682e 5465 6e73 6f72 203d 2073 656c  rch.Tensor = sel
-00038aa0: 662e 6f75 745f 5728 6f75 7429 0a0a 2020  f.out_W(out)..  
-00038ab0: 2020 2020 2020 7265 7475 726e 206e 6f64        return nod
-00038ac0: 655f 6665 6174 7572 6573 2c20 6f75 7470  e_features, outp
-00038ad0: 7574 0a0a 0a63 6c61 7373 204d 584d 4e65  ut...class MXMNe
-00038ae0: 7453 7068 6572 6963 616c 4261 7369 734c  tSphericalBasisL
-00038af0: 6179 6572 2874 6f72 6368 2e6e 6e2e 4d6f  ayer(torch.nn.Mo
-00038b00: 6475 6c65 293a 0a20 2020 2022 2222 4974  dule):.    """It
-00038b10: 2074 616b 6573 2070 6169 7277 6973 6520   takes pairwise 
-00038b20: 6469 7374 616e 6365 7320 616e 6420 616e  distances and an
-00038b30: 676c 6573 2062 6574 7765 656e 2061 746f  gles between ato
-00038b40: 6d73 2061 7320 696e 7075 7420 616e 6420  ms as input and 
-00038b50: 636f 6d62 696e 6573 2072 6164 6961 6c20  combines radial 
-00038b60: 6261 7369 7320 6675 6e63 7469 6f6e 7320  basis functions 
-00038b70: 7769 7468 2073 7068 6572 6963 616c 2068  with spherical h
-00038b80: 6172 6d6f 6e69 630a 2020 2020 6675 6e63  armonic.    func
-00038b90: 7469 6f6e 7320 746f 2067 656e 6572 6174  tions to generat
-00038ba0: 6520 6120 6669 7865 642d 7369 7a65 2072  e a fixed-size r
-00038bb0: 6570 7265 7365 6e74 6174 696f 6e20 7468  epresentation th
-00038bc0: 6174 2063 6170 7475 7265 7320 626f 7468  at captures both
-00038bd0: 2072 6164 6961 6c20 616e 6420 6f72 6965   radial and orie
-00038be0: 6e74 6174 696f 6e20 696e 666f 726d 6174  ntation informat
-00038bf0: 696f 6e2e 2054 6869 7320 7479 7065 206f  ion. This type o
-00038c00: 660a 2020 2020 7265 7072 6573 656e 7461  f.    representa
-00038c10: 7469 6f6e 2069 7320 636f 6d6d 6f6e 6c79  tion is commonly
-00038c20: 2075 7365 6420 696e 206d 6f6c 6563 756c   used in molecul
-00038c30: 6172 206d 6f64 656c 696e 6720 616e 6420  ar modeling and 
-00038c40: 7369 6d75 6c61 7469 6f6e 7320 746f 2063  simulations to c
-00038c50: 6170 7475 7265 2074 6865 2062 6568 6176  apture the behav
-00038c60: 696f 7220 6f66 2061 746f 6d73 2061 6e64  ior of atoms and
-00038c70: 206d 6f6c 6563 756c 6573 2069 6e0a 2020   molecules in.  
-00038c80: 2020 6368 656d 6963 616c 2073 7973 7465    chemical syste
-00038c90: 6d73 2e0a 0a20 2020 2049 6e73 6964 6520  ms...    Inside 
-00038ca0: 7468 6520 696e 6974 6961 6c69 7a61 7469  the initializati
-00038cb0: 6f6e 2c20 4265 7373 656c 2062 6173 6973  on, Bessel basis
-00038cc0: 2066 756e 6374 696f 6e73 2061 6e64 2072   functions and r
-00038cd0: 6561 6c20 7370 6865 7269 6361 6c20 6861  eal spherical ha
-00038ce0: 726d 6f6e 6963 2066 756e 6374 696f 6e73  rmonic functions
-00038cf0: 2061 7265 2067 656e 6572 6174 6564 2e0a   are generated..
-00038d00: 2020 2020 5468 6520 4265 7373 656c 2062      The Bessel b
-00038d10: 6173 6973 2066 756e 6374 696f 6e73 2063  asis functions c
-00038d20: 6170 7475 7265 2074 6865 2072 6164 6961  apture the radia
-00038d30: 6c20 696e 666f 726d 6174 696f 6e2c 2061  l information, a
-00038d40: 6e64 2074 6865 2073 7068 6572 6963 616c  nd the spherical
-00038d50: 2068 6172 6d6f 6e69 6320 6675 6e63 7469   harmonic functi
-00038d60: 6f6e 7320 6361 7074 7572 6520 7468 6520  ons capture the 
-00038d70: 6f72 6965 6e74 6174 696f 6e20 696e 666f  orientation info
-00038d80: 726d 6174 696f 6e2e 0a20 2020 2054 6865  rmation..    The
-00038d90: 7365 2066 756e 6374 696f 6e73 2061 7265  se functions are
-00038da0: 2067 656e 6572 6174 6564 2062 6173 6564   generated based
-00038db0: 206f 6e20 7468 6520 7072 6f76 6964 6564   on the provided
-00038dc0: 206e 756d 5f73 7068 6572 6963 616c 2061   num_spherical a
-00038dd0: 6e64 206e 756d 5f72 6164 6961 6c20 7061  nd num_radial pa
-00038de0: 7261 6d65 7465 7273 2e0a 0a20 2020 2045  rameters...    E
-00038df0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-00038e00: 2d2d 2d2d 0a20 2020 203e 3e3e 2064 6973  ----.    >>> dis
-00038e10: 7420 3d20 746f 7263 682e 7465 6e73 6f72  t = torch.tensor
-00038e20: 285b 302e 352c 2031 2e30 2c20 322e 302c  ([0.5, 1.0, 2.0,
-00038e30: 2033 2e30 5d29 0a20 2020 203e 3e3e 2061   3.0]).    >>> a
-00038e40: 6e67 6c65 203d 2074 6f72 6368 2e74 656e  ngle = torch.ten
-00038e50: 736f 7228 5b30 2e31 2c20 302e 322c 2030  sor([0.1, 0.2, 0
-00038e60: 2e33 2c20 302e 345d 290a 2020 2020 3e3e  .3, 0.4]).    >>
-00038e70: 3e20 6964 785f 6b6a 203d 2074 6f72 6368  > idx_kj = torch
-00038e80: 2e74 656e 736f 7228 5b30 2c20 312c 2032  .tensor([0, 1, 2
-00038e90: 2c20 335d 290a 2020 2020 3e3e 3e20 7370  , 3]).    >>> sp
-00038ea0: 6865 7269 6361 6c5f 6c61 7965 7220 3d20  herical_layer = 
-00038eb0: 4d58 4d4e 6574 5370 6865 7269 6361 6c42  MXMNetSphericalB
-00038ec0: 6173 6973 4c61 7965 7228 656e 7665 6c6f  asisLayer(envelo
-00038ed0: 7065 5f65 7870 6f6e 656e 743d 322c 206e  pe_exponent=2, n
-00038ee0: 756d 5f73 7068 6572 6963 616c 3d32 2c20  um_spherical=2, 
-00038ef0: 6e75 6d5f 7261 6469 616c 3d32 2c20 6375  num_radial=2, cu
-00038f00: 746f 6666 3d32 2e30 290a 2020 2020 3e3e  toff=2.0).    >>
-00038f10: 3e20 6f75 7470 7574 203d 2073 7068 6572  > output = spher
-00038f20: 6963 616c 5f6c 6179 6572 2864 6973 742c  ical_layer(dist,
-00038f30: 2061 6e67 6c65 2c20 6964 785f 6b6a 290a   angle, idx_kj).
-00038f40: 2020 2020 3e3e 3e20 6f75 7470 7574 2e73      >>> output.s
-00038f50: 6861 7065 0a20 2020 2074 6f72 6368 2e53  hape.    torch.S
-00038f60: 697a 6528 5b34 2c20 345d 290a 2020 2020  ize([4, 4]).    
-00038f70: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
-00038f80: 6e69 745f 5f28 7365 6c66 2c0a 2020 2020  nit__(self,.    
-00038f90: 2020 2020 2020 2020 2020 2020 206e 756d               num
-00038fa0: 5f73 7068 6572 6963 616c 3a20 696e 742c  _spherical: int,
-00038fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00038fc0: 2020 6e75 6d5f 7261 6469 616c 3a20 696e    num_radial: in
-00038fd0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00038fe0: 2020 2020 6375 746f 6666 3a20 666c 6f61      cutoff: floa
-00038ff0: 7420 3d20 352e 302c 0a20 2020 2020 2020  t = 5.0,.       
-00039000: 2020 2020 2020 2020 2020 656e 7665 6c6f            envelo
-00039010: 7065 5f65 7870 6f6e 656e 743a 2069 6e74  pe_exponent: int
-00039020: 203d 2035 293a 0a20 2020 2020 2020 2022   = 5):.        "
-00039030: 2222 496e 6974 6961 6c69 7a65 2074 6865  ""Initialize the
-00039040: 204d 584d 4e65 7453 7068 6572 6963 616c   MXMNetSpherical
-00039050: 4261 7369 734c 6179 6572 2e0a 0a20 2020  BasisLayer...   
-00039060: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00039070: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00039080: 2d2d 0a20 2020 2020 2020 206e 756d 5f73  --.        num_s
-00039090: 7068 6572 6963 616c 3a20 696e 740a 2020  pherical: int.  
-000390a0: 2020 2020 2020 2020 2020 5468 6520 6e75            The nu
-000390b0: 6d62 6572 206f 6620 7370 6865 7269 6361  mber of spherica
-000390c0: 6c20 6861 726d 6f6e 6963 2066 756e 6374  l harmonic funct
-000390d0: 696f 6e73 2074 6f20 7573 652e 2054 6865  ions to use. The
-000390e0: 7365 2066 756e 6374 696f 6e73 2063 6170  se functions cap
-000390f0: 7475 7265 206f 7269 656e 7461 7469 6f6e  ture orientation
-00039100: 2069 6e66 6f72 6d61 7469 6f6e 2072 656c   information rel
-00039110: 6174 6564 2074 6f20 6174 6f6d 2070 6f73  ated to atom pos
-00039120: 6974 696f 6e73 2e0a 2020 2020 2020 2020  itions..        
-00039130: 6e75 6d5f 7261 6469 616c 3a20 696e 740a  num_radial: int.
-00039140: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00039150: 6e75 6d62 6572 206f 6620 7261 6469 616c  number of radial
-00039160: 2062 6173 6973 2066 756e 6374 696f 6e73   basis functions
-00039170: 2074 6f20 7573 652e 2054 6865 7365 2066   to use. These f
-00039180: 756e 6374 696f 6e73 2063 6170 7475 7265  unctions capture
-00039190: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-000391a0: 7574 2070 6169 7277 6973 6520 6469 7374  ut pairwise dist
-000391b0: 616e 6365 7320 6265 7477 6565 6e20 6174  ances between at
-000391c0: 6f6d 732e 0a20 2020 2020 2020 2063 7574  oms..        cut
-000391d0: 6f66 663a 2066 6c6f 6174 2c20 6f70 7469  off: float, opti
-000391e0: 6f6e 616c 2028 6465 6661 756c 7420 352e  onal (default 5.
-000391f0: 3029 0a20 2020 2020 2020 2020 2020 2054  0).            T
-00039200: 6865 2063 7574 6f66 6620 6469 7374 616e  he cutoff distan
-00039210: 6365 2066 6f72 2074 6865 2072 6164 6961  ce for the radia
-00039220: 6c20 6261 7369 7320 6675 6e63 7469 6f6e  l basis function
-00039230: 732e 2049 7420 7370 6563 6966 6965 7320  s. It specifies 
-00039240: 7468 6520 6469 7374 616e 6365 2062 6579  the distance bey
-00039250: 6f6e 6420 7768 6963 6820 7468 6520 696e  ond which the in
-00039260: 7465 7261 6374 696f 6e73 2061 7265 2069  teractions are i
-00039270: 676e 6f72 6564 2e0a 2020 2020 2020 2020  gnored..        
-00039280: 656e 7665 6c6f 7065 5f65 7870 6f6e 656e  envelope_exponen
-00039290: 743a 2069 6e74 2c20 6f70 7469 6f6e 616c  t: int, optional
-000392a0: 2028 6465 6661 756c 7420 3529 0a20 2020   (default 5).   
-000392b0: 2020 2020 2020 2020 2054 6865 2065 7870           The exp
-000392c0: 6f6e 656e 7420 666f 7220 7468 6520 656e  onent for the en
-000392d0: 7665 6c6f 7065 2066 756e 6374 696f 6e2e  velope function.
-000392e0: 2049 7420 636f 6e74 726f 6c73 2074 6865   It controls the
-000392f0: 2064 6567 7265 6520 6f66 2064 616d 7069   degree of dampi
-00039300: 6e67 2066 6f72 2074 6865 2072 6164 6961  ng for the radia
-00039310: 6c20 6261 7369 7320 6675 6e63 7469 6f6e  l basis function
-00039320: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00039330: 2020 2020 2020 2073 7570 6572 284d 584d         super(MXM
-00039340: 4e65 7453 7068 6572 6963 616c 4261 7369  NetSphericalBasi
-00039350: 734c 6179 6572 2c20 7365 6c66 292e 5f5f  sLayer, self).__
-00039360: 696e 6974 5f5f 2829 0a0a 2020 2020 2020  init__()..      
-00039370: 2020 6173 7365 7274 206e 756d 5f72 6164    assert num_rad
-00039380: 6961 6c20 3c3d 2036 340a 2020 2020 2020  ial <= 64.      
-00039390: 2020 7365 6c66 2e6e 756d 5f73 7068 6572    self.num_spher
-000393a0: 6963 616c 3a20 696e 7420 3d20 6e75 6d5f  ical: int = num_
-000393b0: 7370 6865 7269 6361 6c0a 2020 2020 2020  spherical.      
-000393c0: 2020 7365 6c66 2e6e 756d 5f72 6164 6961    self.num_radia
-000393d0: 6c3a 2069 6e74 203d 206e 756d 5f72 6164  l: int = num_rad
-000393e0: 6961 6c0a 2020 2020 2020 2020 7365 6c66  ial.        self
-000393f0: 2e63 7574 6f66 663a 2066 6c6f 6174 203d  .cutoff: float =
-00039400: 2063 7574 6f66 660a 2020 2020 2020 2020   cutoff.        
-00039410: 7365 6c66 2e65 6e76 656c 6f70 653a 205f  self.envelope: _
-00039420: 4d58 4d4e 6574 456e 7665 6c6f 7065 203d  MXMNetEnvelope =
-00039430: 205f 4d58 4d4e 6574 456e 7665 6c6f 7065   _MXMNetEnvelope
-00039440: 2865 6e76 656c 6f70 655f 6578 706f 6e65  (envelope_expone
-00039450: 6e74 290a 0a20 2020 2020 2020 2062 6573  nt)..        bes
-00039460: 7365 6c5f 666f 726d 733a 204c 6973 7420  sel_forms: List 
-00039470: 3d20 6265 7373 656c 5f62 6173 6973 286e  = bessel_basis(n
-00039480: 756d 5f73 7068 6572 6963 616c 2c20 6e75  um_spherical, nu
-00039490: 6d5f 7261 6469 616c 290a 2020 2020 2020  m_radial).      
-000394a0: 2020 7370 685f 6861 726d 5f66 6f72 6d73    sph_harm_forms
-000394b0: 3a20 4c69 7374 5b4c 6973 745b 7374 725d  : List[List[str]
-000394c0: 5d20 3d20 7265 616c 5f73 7068 5f68 6172  ] = real_sph_har
-000394d0: 6d28 6e75 6d5f 7370 6865 7269 6361 6c29  m(num_spherical)
-000394e0: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
-000394f0: 685f 6675 6e63 733a 204c 6973 7420 3d20  h_funcs: List = 
-00039500: 5b5d 0a20 2020 2020 2020 2073 656c 662e  [].        self.
-00039510: 6265 7373 656c 5f66 756e 6373 3a20 4c69  bessel_funcs: Li
-00039520: 7374 203d 205b 5d0a 2020 2020 2020 2020  st = [].        
-00039530: 783a 2041 6e79 0a20 2020 2020 2020 2074  x: Any.        t
-00039540: 6865 7461 3a20 416e 790a 2020 2020 2020  heta: Any.      
-00039550: 2020 782c 2074 6865 7461 203d 2073 796d    x, theta = sym
-00039560: 2e73 796d 626f 6c73 2827 7820 7468 6574  .symbols('x thet
-00039570: 6127 290a 2020 2020 2020 2020 6d6f 6475  a').        modu
-00039580: 6c65 733a 2044 6963 7420 3d20 7b27 7369  les: Dict = {'si
-00039590: 6e27 3a20 746f 7263 682e 7369 6e2c 2027  n': torch.sin, '
-000395a0: 636f 7327 3a20 746f 7263 682e 636f 737d  cos': torch.cos}
-000395b0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-000395c0: 6e20 7261 6e67 6528 6e75 6d5f 7370 6865  n range(num_sphe
-000395d0: 7269 6361 6c29 3a0a 2020 2020 2020 2020  rical):.        
-000395e0: 2020 2020 6966 2069 203d 3d20 303a 0a20      if i == 0:. 
-000395f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00039600: 7068 313a 2041 6e79 203d 2073 796d 2e6c  ph1: Any = sym.l
-00039610: 616d 6264 6966 7928 5b74 6865 7461 5d2c  ambdify([theta],
-00039620: 2073 7068 5f68 6172 6d5f 666f 726d 735b   sph_harm_forms[
-00039630: 695d 5b30 5d2c 0a20 2020 2020 2020 2020  i][0],.         
-00039640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039660: 6d6f 6475 6c65 7329 2830 290a 2020 2020  modules)(0).    
-00039670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00039680: 2e73 7068 5f66 756e 6373 2e61 7070 656e  .sph_funcs.appen
-00039690: 6428 6c61 6d62 6461 2078 3a20 746f 7263  d(lambda x: torc
-000396a0: 682e 7a65 726f 735f 6c69 6b65 2878 2920  h.zeros_like(x) 
-000396b0: 2b20 7370 6831 290a 2020 2020 2020 2020  + sph1).        
-000396c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000396d0: 2020 2020 2020 2020 2020 7370 683a 2041            sph: A
-000396e0: 6e79 203d 2073 796d 2e6c 616d 6264 6966  ny = sym.lambdif
-000396f0: 7928 5b74 6865 7461 5d2c 2073 7068 5f68  y([theta], sph_h
-00039700: 6172 6d5f 666f 726d 735b 695d 5b30 5d2c  arm_forms[i][0],
-00039710: 206d 6f64 756c 6573 290a 2020 2020 2020   modules).      
-00039720: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00039730: 7068 5f66 756e 6373 2e61 7070 656e 6428  ph_funcs.append(
-00039740: 7370 6829 0a20 2020 2020 2020 2020 2020  sph).           
-00039750: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-00039760: 6e75 6d5f 7261 6469 616c 293a 0a20 2020  num_radial):.   
-00039770: 2020 2020 2020 2020 2020 2020 2062 6573               bes
-00039780: 7365 6c3a 2041 6e79 203d 2073 796d 2e6c  sel: Any = sym.l
-00039790: 616d 6264 6966 7928 5b78 5d2c 2062 6573  ambdify([x], bes
-000397a0: 7365 6c5f 666f 726d 735b 695d 5b6a 5d2c  sel_forms[i][j],
-000397b0: 206d 6f64 756c 6573 290a 2020 2020 2020   modules).      
-000397c0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000397d0: 6573 7365 6c5f 6675 6e63 732e 6170 7065  essel_funcs.appe
-000397e0: 6e64 2862 6573 7365 6c29 0a0a 2020 2020  nd(bessel)..    
-000397f0: 6465 6620 666f 7277 6172 6428 7365 6c66  def forward(self
-00039800: 2c20 6469 7374 3a20 746f 7263 682e 5465  , dist: torch.Te
-00039810: 6e73 6f72 2c20 616e 676c 653a 2074 6f72  nsor, angle: tor
-00039820: 6368 2e54 656e 736f 722c 0a20 2020 2020  ch.Tensor,.     
-00039830: 2020 2020 2020 2020 2020 2069 6478 5f6b             idx_k
-00039840: 6a3a 2074 6f72 6368 2e54 656e 736f 7229  j: torch.Tensor)
-00039850: 202d 3e20 746f 7263 682e 5465 6e73 6f72   -> torch.Tensor
-00039860: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00039870: 2020 2020 2020 466f 7277 6172 6420 7061        Forward pa
-00039880: 7373 206f 6620 7468 6520 4d58 4d4e 6574  ss of the MXMNet
-00039890: 5370 6865 7269 6361 6c42 6173 6973 4c61  SphericalBasisLa
-000398a0: 7965 722e 0a0a 2020 2020 2020 2020 5061  yer...        Pa
-000398b0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-000398c0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000398d0: 2020 2020 6469 7374 3a20 746f 7263 682e      dist: torch.
-000398e0: 5465 6e73 6f72 0a20 2020 2020 2020 2020  Tensor.         
-000398f0: 2020 2049 6e70 7574 2074 656e 736f 7220     Input tensor 
-00039900: 7265 7072 6573 656e 7469 6e67 2070 6169  representing pai
-00039910: 7277 6973 6520 6469 7374 616e 6365 7320  rwise distances 
-00039920: 6265 7477 6565 6e20 6174 6f6d 732e 0a20  between atoms.. 
-00039930: 2020 2020 2020 2061 6e67 6c65 3a20 746f         angle: to
-00039940: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
-00039950: 2020 2020 2020 2049 6e70 7574 2074 656e         Input ten
-00039960: 736f 7220 7265 7072 6573 656e 7469 6e67  sor representing
-00039970: 2070 6169 7277 6973 6520 616e 676c 6573   pairwise angles
-00039980: 2062 6574 7765 656e 2061 746f 6d73 2e0a   between atoms..
-00039990: 2020 2020 2020 2020 6964 785f 6b6a 3a20          idx_kj: 
-000399a0: 746f 7263 682e 5465 6e73 6f72 0a20 2020  torch.Tensor.   
-000399b0: 2020 2020 2020 2020 2054 656e 736f 7220           Tensor 
-000399c0: 636f 6e74 6169 6e69 6e67 2069 6e64 6963  containing indic
-000399d0: 6573 2066 6f72 2074 6865 206b 2061 6e64  es for the k and
-000399e0: 206a 2061 746f 6d73 2e0a 0a20 2020 2020   j atoms...     
-000399f0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00039a00: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00039a10: 2020 206f 7574 7075 743a 2074 6f72 6368     output: torch
-00039a20: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
-00039a30: 2020 2020 5468 6520 6f75 7470 7574 2074      The output t
-00039a40: 656e 736f 7220 636f 6e74 6169 6e69 6e67  ensor containing
-00039a50: 2074 6865 2066 6978 6564 2d73 697a 6520   the fixed-size 
-00039a60: 7265 7072 6573 656e 7461 7469 6f6e 2e0a  representation..
-00039a70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00039a80: 2020 2020 6469 7374 203d 2064 6973 7420      dist = dist 
-00039a90: 2f20 7365 6c66 2e63 7574 6f66 660a 2020  / self.cutoff.  
-00039aa0: 2020 2020 2020 7262 663a 2074 6f72 6368        rbf: torch
-00039ab0: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
-00039ac0: 7374 6163 6b28 5b66 2864 6973 7429 2066  stack([f(dist) f
-00039ad0: 6f72 2066 2069 6e20 7365 6c66 2e62 6573  or f in self.bes
-00039ae0: 7365 6c5f 6675 6e63 735d 2c0a 2020 2020  sel_funcs],.    
-00039af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039b10: 2020 2020 6469 6d3d 3129 0a20 2020 2020      dim=1).     
-00039b20: 2020 2072 6266 203d 2073 656c 662e 656e     rbf = self.en
-00039b30: 7665 6c6f 7065 2864 6973 7429 2e75 6e73  velope(dist).uns
-00039b40: 7175 6565 7a65 282d 3129 202a 2072 6266  queeze(-1) * rbf
-00039b50: 0a0a 2020 2020 2020 2020 6362 663a 2074  ..        cbf: t
-00039b60: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
-00039b70: 7263 682e 7374 6163 6b28 5b66 2861 6e67  rch.stack([f(ang
-00039b80: 6c65 2920 666f 7220 6620 696e 2073 656c  le) for f in sel
-00039b90: 662e 7370 685f 6675 6e63 735d 2c0a 2020  f.sph_funcs],.  
+00036bf0: 205b 2d30 2e32 3736 375d 2c20 5b2d 302e   [-0.2767], [-0.
+00036c00: 3237 3637 5d2c 205b 2d30 2e32 3736 375d  2767], [-0.2767]
+00036c10: 2c20 5b2d 302e 3237 3637 5d5d 290a 2020  , [-0.2767]]).  
+00036c20: 2020 3e3e 3e20 7362 6632 203d 2074 6f72    >>> sbf2 = tor
+00036c30: 6368 2e74 656e 736f 7228 5b5b 2d30 2e30  ch.tensor([[-0.0
+00036c40: 3330 315d 2c20 5b2d 302e 3033 3031 5d2c  301], [-0.0301],
+00036c50: 205b 2d30 2e31 3438 335d 2c20 5b2d 302e   [-0.1483], [-0.
+00036c60: 3134 3836 5d2c 205b 2d30 2e31 3438 345d  1486], [-0.1484]
+00036c70: 2c0a 2020 2020 2e2e 2e20 2020 2020 2020  ,.    ...       
+00036c80: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00036c90: 2d30 2e30 3330 315d 2c20 5b2d 302e 3134  -0.0301], [-0.14
+00036ca0: 3833 5d2c 205b 2d30 2e30 3330 315d 2c20  83], [-0.0301], 
+00036cb0: 5b2d 302e 3134 3835 5d2c 205b 2d30 2e31  [-0.1485], [-0.1
+00036cc0: 3438 335d 2c0a 2020 2020 2e2e 2e20 2020  483],.    ...   
+00036cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036ce0: 2020 205b 2d30 2e30 3330 315d 2c20 5b2d     [-0.0301], [-
+00036cf0: 302e 3134 3836 5d2c 205b 2d30 2e31 3438  0.1486], [-0.148
+00036d00: 355d 2c20 5b2d 302e 3033 3031 5d2c 205b  5], [-0.0301], [
+00036d10: 2d30 2e31 3438 365d 2c0a 2020 2020 2e2e  -0.1486],.    ..
+00036d20: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00036d30: 2020 2020 2020 205b 2d30 2e30 3330 315d         [-0.0301]
+00036d40: 2c20 5b2d 302e 3134 3834 5d2c 205b 2d30  , [-0.1484], [-0
+00036d50: 2e31 3438 335d 2c20 5b2d 302e 3134 3836  .1483], [-0.1486
+00036d60: 5d2c 205b 2d30 2e30 3330 315d 5d29 0a20  ], [-0.0301]]). 
+00036d70: 2020 203e 3e3e 2069 6478 5f6b 6a20 3d20     >>> idx_kj = 
+00036d80: 746f 7263 682e 7465 6e73 6f72 285b 332c  torch.tensor([3,
+00036d90: 2035 2c20 372c 2031 2c20 352c 2037 2c20   5, 7, 1, 5, 7, 
+00036da0: 312c 2033 2c20 372c 2031 2c20 332c 2035  1, 3, 7, 1, 3, 5
+00036db0: 5d29 0a20 2020 203e 3e3e 2069 6478 5f6a  ]).    >>> idx_j
+00036dc0: 695f 3120 3d20 746f 7263 682e 7465 6e73  i_1 = torch.tens
+00036dd0: 6f72 285b 302c 2030 2c20 302c 2032 2c20  or([0, 0, 0, 2, 
+00036de0: 322c 2032 2c20 342c 2034 2c20 342c 2036  2, 2, 4, 4, 4, 6
+00036df0: 2c20 362c 2036 5d29 0a20 2020 203e 3e3e  , 6, 6]).    >>>
+00036e00: 2069 6478 5f6a 6a20 3d20 746f 7263 682e   idx_jj = torch.
+00036e10: 7465 6e73 6f72 285b 302c 2031 2c20 332c  tensor([0, 1, 3,
+00036e20: 2035 2c20 372c 2032 2c20 312c 2033 2c20   5, 7, 2, 1, 3, 
+00036e30: 352c 2037 2c20 342c 2031 2c20 332c 2035  5, 7, 4, 1, 3, 5
+00036e40: 2c20 372c 2036 2c20 312c 2033 2c20 352c  , 7, 6, 1, 3, 5,
+00036e50: 2037 5d29 0a20 2020 203e 3e3e 2069 6478   7]).    >>> idx
+00036e60: 5f6a 695f 3220 3d20 746f 7263 682e 7465  _ji_2 = torch.te
+00036e70: 6e73 6f72 285b 302c 2031 2c20 312c 2031  nsor([0, 1, 1, 1
+00036e80: 2c20 312c 2032 2c20 332c 2033 2c20 332c  , 1, 2, 3, 3, 3,
+00036e90: 2033 2c20 342c 2035 2c20 352c 2035 2c20   3, 4, 5, 5, 5, 
+00036ea0: 352c 2036 2c20 372c 2037 2c20 372c 2037  5, 6, 7, 7, 7, 7
+00036eb0: 5d29 0a20 2020 203e 3e3e 2065 6467 655f  ]).    >>> edge_
+00036ec0: 696e 6465 7820 3d20 746f 7263 682e 7465  index = torch.te
+00036ed0: 6e73 6f72 285b 5b30 2c20 312c 2030 2c20  nsor([[0, 1, 0, 
+00036ee0: 322c 2030 2c20 332c 2030 2c20 345d 2c0a  2, 0, 3, 0, 4],.
+00036ef0: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+00036f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036f10: 2020 5b31 2c20 302c 2032 2c20 302c 2033    [1, 0, 2, 0, 3
+00036f20: 2c20 302c 2034 2c20 305d 5d29 0a20 2020  , 0, 4, 0]]).   
+00036f30: 203e 3e3e 206f 7574 203d 204d 584d 4e65   >>> out = MXMNe
+00036f40: 744c 6f63 616c 4d65 7373 6167 6550 6173  tLocalMessagePas
+00036f50: 7369 6e67 2864 696d 2c20 6163 7469 7661  sing(dim, activa
+00036f60: 7469 6f6e 5f66 6e3d 2773 696c 7527 290a  tion_fn='silu').
+00036f70: 2020 2020 3e3e 3e20 6f75 7470 7574 203d      >>> output =
+00036f80: 206f 7574 2868 2c0a 2020 2020 2e2e 2e20   out(h,.    ... 
+00036f90: 2020 2020 2020 2020 2020 2020 7262 662c              rbf,
+00036fa0: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
+00036fb0: 2020 2020 2073 6266 312c 0a20 2020 202e       sbf1,.    .
+00036fc0: 2e2e 2020 2020 2020 2020 2020 2020 2073  ..             s
+00036fd0: 6266 322c 0a20 2020 202e 2e2e 2020 2020  bf2,.    ...    
+00036fe0: 2020 2020 2020 2020 2069 6478 5f6b 6a2c           idx_kj,
+00036ff0: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
+00037000: 2020 2020 2069 6478 5f6a 695f 312c 0a20       idx_ji_1,. 
+00037010: 2020 202e 2e2e 2020 2020 2020 2020 2020     ...          
+00037020: 2020 2069 6478 5f6a 6a2c 0a20 2020 202e     idx_jj,.    .
+00037030: 2e2e 2020 2020 2020 2020 2020 2020 2069  ..             i
+00037040: 6478 5f6a 695f 322c 0a20 2020 202e 2e2e  dx_ji_2,.    ...
+00037050: 2020 2020 2020 2020 2020 2020 2065 6467               edg
+00037060: 655f 696e 6465 7829 0a20 2020 203e 3e3e  e_index).    >>>
+00037070: 206f 7574 7075 745b 305d 2e73 6861 7065   output[0].shape
+00037080: 0a20 2020 2074 6f72 6368 2e53 697a 6528  .    torch.Size(
+00037090: 5b35 2c20 315d 290a 2020 2020 3e3e 3e20  [5, 1]).    >>> 
+000370a0: 6f75 7470 7574 5b31 5d2e 7368 6170 650a  output[1].shape.
+000370b0: 2020 2020 746f 7263 682e 5369 7a65 285b      torch.Size([
+000370c0: 352c 2031 5d29 0a20 2020 2022 2222 0a0a  5, 1]).    """..
+000370d0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000370e0: 2873 656c 662c 2064 696d 3a20 696e 742c  (self, dim: int,
+000370f0: 2061 6374 6976 6174 696f 6e5f 666e 3a20   activation_fn: 
+00037100: 556e 696f 6e5b 4361 6c6c 6162 6c65 2c20  Union[Callable, 
+00037110: 7374 725d 203d 2027 7369 6c75 2729 3a0a  str] = 'silu'):.
+00037120: 2020 2020 2020 2020 2222 2249 6e69 7469          """Initi
+00037130: 616c 697a 6573 2074 6865 204d 584d 4e65  alizes the MXMNe
+00037140: 744c 6f63 616c 4d65 7373 6167 6550 6173  tLocalMessagePas
+00037150: 7369 6e67 206c 6179 6572 2e0a 0a20 2020  sing layer...   
+00037160: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00037170: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00037180: 2d2d 0a20 2020 2020 2020 2064 696d 203a  --.        dim :
+00037190: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+000371a0: 2054 6865 2064 696d 656e 7369 6f6e 206f   The dimension o
+000371b0: 6620 7468 6520 696e 7075 7420 616e 6420  f the input and 
+000371c0: 6f75 7470 7574 2074 656e 736f 7273 2066  output tensors f
+000371d0: 6f72 2074 6865 206c 6f63 616c 206d 6573  or the local mes
+000371e0: 7361 6765 2070 6173 7369 6e67 206c 6179  sage passing lay
+000371f0: 6572 2e0a 2020 2020 2020 2020 6163 7469  er..        acti
+00037200: 7661 7469 6f6e 5f66 6e20 3a20 556e 696f  vation_fn : Unio
+00037210: 6e5b 4361 6c6c 6162 6c65 2c20 7374 725d  n[Callable, str]
+00037220: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
+00037230: 756c 743a 2027 7369 6c75 2729 0a20 2020  ult: 'silu').   
+00037240: 2020 2020 2020 2020 2054 6865 2061 6374           The act
+00037250: 6976 6174 696f 6e20 6675 6e63 7469 6f6e  ivation function
+00037260: 2074 6f20 6265 2075 7365 6420 696e 2074   to be used in t
+00037270: 6865 206d 756c 7469 6c61 7965 7220 7065  he multilayer pe
+00037280: 7263 6570 7472 6f6e 7320 284d 4c50 7329  rceptrons (MLPs)
+00037290: 2077 6974 6869 6e20 7468 6520 6c61 7965   within the laye
+000372a0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+000372b0: 2020 2020 2020 2073 7570 6572 284d 584d         super(MXM
+000372c0: 4e65 744c 6f63 616c 4d65 7373 6167 6550  NetLocalMessageP
+000372d0: 6173 7369 6e67 2c20 7365 6c66 292e 5f5f  assing, self).__
+000372e0: 696e 6974 5f5f 2829 0a0a 2020 2020 2020  init__()..      
+000372f0: 2020 6163 7469 7661 7469 6f6e 5f66 6e20    activation_fn 
+00037300: 3d20 6765 745f 6163 7469 7661 7469 6f6e  = get_activation
+00037310: 2861 6374 6976 6174 696f 6e5f 666e 290a  (activation_fn).
+00037320: 2020 2020 2020 2020 7365 6c66 2e68 5f6d          self.h_m
+00037330: 6c70 3a20 4d75 6c74 696c 6179 6572 5065  lp: MultilayerPe
+00037340: 7263 6570 7472 6f6e 203d 204d 756c 7469  rceptron = Multi
+00037350: 6c61 7965 7250 6572 6365 7074 726f 6e28  layerPerceptron(
+00037360: 0a20 2020 2020 2020 2020 2020 2064 5f69  .            d_i
+00037370: 6e70 7574 3d64 696d 2c20 645f 6f75 7470  nput=dim, d_outp
+00037380: 7574 3d64 696d 2c20 6163 7469 7661 7469  ut=dim, activati
+00037390: 6f6e 5f66 6e3d 6163 7469 7661 7469 6f6e  on_fn=activation
+000373a0: 5f66 6e29 0a20 2020 2020 2020 2073 656c  _fn).        sel
+000373b0: 662e 6d6c 705f 6b6a 3a20 4d75 6c74 696c  f.mlp_kj: Multil
+000373c0: 6179 6572 5065 7263 6570 7472 6f6e 203d  ayerPerceptron =
+000373d0: 204d 756c 7469 6c61 7965 7250 6572 6365   MultilayerPerce
+000373e0: 7074 726f 6e28 0a20 2020 2020 2020 2020  ptron(.         
+000373f0: 2020 2064 5f69 6e70 7574 3d33 202a 2064     d_input=3 * d
+00037400: 696d 2c20 645f 6f75 7470 7574 3d64 696d  im, d_output=dim
+00037410: 2c20 6163 7469 7661 7469 6f6e 5f66 6e3d  , activation_fn=
+00037420: 6163 7469 7661 7469 6f6e 5f66 6e29 0a20  activation_fn). 
+00037430: 2020 2020 2020 2073 656c 662e 6d6c 705f         self.mlp_
+00037440: 6a69 5f31 3a20 4d75 6c74 696c 6179 6572  ji_1: Multilayer
+00037450: 5065 7263 6570 7472 6f6e 203d 204d 756c  Perceptron = Mul
+00037460: 7469 6c61 7965 7250 6572 6365 7074 726f  tilayerPerceptro
+00037470: 6e28 0a20 2020 2020 2020 2020 2020 2064  n(.            d
+00037480: 5f69 6e70 7574 3d33 202a 2064 696d 2c20  _input=3 * dim, 
+00037490: 645f 6f75 7470 7574 3d64 696d 2c20 6163  d_output=dim, ac
+000374a0: 7469 7661 7469 6f6e 5f66 6e3d 6163 7469  tivation_fn=acti
+000374b0: 7661 7469 6f6e 5f66 6e29 0a20 2020 2020  vation_fn).     
+000374c0: 2020 2073 656c 662e 6d6c 705f 6a69 5f32     self.mlp_ji_2
+000374d0: 3a20 4d75 6c74 696c 6179 6572 5065 7263  : MultilayerPerc
+000374e0: 6570 7472 6f6e 203d 204d 756c 7469 6c61  eptron = Multila
+000374f0: 7965 7250 6572 6365 7074 726f 6e28 0a20  yerPerceptron(. 
+00037500: 2020 2020 2020 2020 2020 2064 5f69 6e70             d_inp
+00037510: 7574 3d64 696d 2c20 645f 6f75 7470 7574  ut=dim, d_output
+00037520: 3d64 696d 2c20 6163 7469 7661 7469 6f6e  =dim, activation
+00037530: 5f66 6e3d 6163 7469 7661 7469 6f6e 5f66  _fn=activation_f
+00037540: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
+00037550: 6d6c 705f 6a6a 3a20 4d75 6c74 696c 6179  mlp_jj: Multilay
+00037560: 6572 5065 7263 6570 7472 6f6e 203d 204d  erPerceptron = M
+00037570: 756c 7469 6c61 7965 7250 6572 6365 7074  ultilayerPercept
+00037580: 726f 6e28 0a20 2020 2020 2020 2020 2020  ron(.           
+00037590: 2064 5f69 6e70 7574 3d64 696d 2c20 645f   d_input=dim, d_
+000375a0: 6f75 7470 7574 3d64 696d 2c20 6163 7469  output=dim, acti
+000375b0: 7661 7469 6f6e 5f66 6e3d 6163 7469 7661  vation_fn=activa
+000375c0: 7469 6f6e 5f66 6e29 0a0a 2020 2020 2020  tion_fn)..      
+000375d0: 2020 7365 6c66 2e6d 6c70 5f73 6266 313a    self.mlp_sbf1:
+000375e0: 204d 756c 7469 6c61 7965 7250 6572 6365   MultilayerPerce
+000375f0: 7074 726f 6e20 3d20 4d75 6c74 696c 6179  ptron = Multilay
+00037600: 6572 5065 7263 6570 7472 6f6e 280a 2020  erPerceptron(.  
+00037610: 2020 2020 2020 2020 2020 645f 696e 7075            d_inpu
+00037620: 743d 6469 6d2c 0a20 2020 2020 2020 2020  t=dim,.         
+00037630: 2020 2064 5f68 6964 6465 6e3d 2864 696d     d_hidden=(dim
+00037640: 2c29 2c0a 2020 2020 2020 2020 2020 2020  ,),.            
+00037650: 645f 6f75 7470 7574 3d64 696d 2c0a 2020  d_output=dim,.  
+00037660: 2020 2020 2020 2020 2020 6163 7469 7661            activa
+00037670: 7469 6f6e 5f66 6e3d 6163 7469 7661 7469  tion_fn=activati
+00037680: 6f6e 5f66 6e29 0a20 2020 2020 2020 2073  on_fn).        s
+00037690: 656c 662e 6d6c 705f 7362 6632 3a20 4d75  elf.mlp_sbf2: Mu
+000376a0: 6c74 696c 6179 6572 5065 7263 6570 7472  ltilayerPerceptr
+000376b0: 6f6e 203d 204d 756c 7469 6c61 7965 7250  on = MultilayerP
+000376c0: 6572 6365 7074 726f 6e28 0a20 2020 2020  erceptron(.     
+000376d0: 2020 2020 2020 2064 5f69 6e70 7574 3d64         d_input=d
+000376e0: 696d 2c0a 2020 2020 2020 2020 2020 2020  im,.            
+000376f0: 645f 6869 6464 656e 3d28 6469 6d2c 292c  d_hidden=(dim,),
+00037700: 0a20 2020 2020 2020 2020 2020 2064 5f6f  .            d_o
+00037710: 7574 7075 743d 6469 6d2c 0a20 2020 2020  utput=dim,.     
+00037720: 2020 2020 2020 2061 6374 6976 6174 696f         activatio
+00037730: 6e5f 666e 3d61 6374 6976 6174 696f 6e5f  n_fn=activation_
+00037740: 666e 290a 0a20 2020 2020 2020 2073 656c  fn)..        sel
+00037750: 662e 7265 7331 3a20 4d75 6c74 696c 6179  f.res1: Multilay
+00037760: 6572 5065 7263 6570 7472 6f6e 203d 204d  erPerceptron = M
+00037770: 756c 7469 6c61 7965 7250 6572 6365 7074  ultilayerPercept
+00037780: 726f 6e28 0a20 2020 2020 2020 2020 2020  ron(.           
+00037790: 2064 5f69 6e70 7574 3d64 696d 2c0a 2020   d_input=dim,.  
+000377a0: 2020 2020 2020 2020 2020 645f 6869 6464            d_hidd
+000377b0: 656e 3d28 6469 6d2c 292c 0a20 2020 2020  en=(dim,),.     
+000377c0: 2020 2020 2020 2064 5f6f 7574 7075 743d         d_output=
+000377d0: 6469 6d2c 0a20 2020 2020 2020 2020 2020  dim,.           
+000377e0: 2061 6374 6976 6174 696f 6e5f 666e 3d61   activation_fn=a
+000377f0: 6374 6976 6174 696f 6e5f 666e 2c0a 2020  ctivation_fn,.  
+00037800: 2020 2020 2020 2020 2020 736b 6970 5f63            skip_c
+00037810: 6f6e 6e65 6374 696f 6e3d 5472 7565 2c0a  onnection=True,.
+00037820: 2020 2020 2020 2020 2020 2020 7765 6967              weig
+00037830: 6874 6564 5f73 6b69 703d 4661 6c73 6529  hted_skip=False)
+00037840: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00037850: 7332 3a20 4d75 6c74 696c 6179 6572 5065  s2: MultilayerPe
+00037860: 7263 6570 7472 6f6e 203d 204d 756c 7469  rceptron = Multi
+00037870: 6c61 7965 7250 6572 6365 7074 726f 6e28  layerPerceptron(
+00037880: 0a20 2020 2020 2020 2020 2020 2064 5f69  .            d_i
+00037890: 6e70 7574 3d64 696d 2c0a 2020 2020 2020  nput=dim,.      
+000378a0: 2020 2020 2020 645f 6869 6464 656e 3d28        d_hidden=(
+000378b0: 6469 6d2c 292c 0a20 2020 2020 2020 2020  dim,),.         
+000378c0: 2020 2064 5f6f 7574 7075 743d 6469 6d2c     d_output=dim,
+000378d0: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
+000378e0: 6976 6174 696f 6e5f 666e 3d61 6374 6976  ivation_fn=activ
+000378f0: 6174 696f 6e5f 666e 2c0a 2020 2020 2020  ation_fn,.      
+00037900: 2020 2020 2020 736b 6970 5f63 6f6e 6e65        skip_conne
+00037910: 6374 696f 6e3d 5472 7565 2c0a 2020 2020  ction=True,.    
+00037920: 2020 2020 2020 2020 7765 6967 6874 6564          weighted
+00037930: 5f73 6b69 703d 4661 6c73 6529 0a20 2020  _skip=False).   
+00037940: 2020 2020 2073 656c 662e 7265 7333 3a20       self.res3: 
+00037950: 4d75 6c74 696c 6179 6572 5065 7263 6570  MultilayerPercep
+00037960: 7472 6f6e 203d 204d 756c 7469 6c61 7965  tron = Multilaye
+00037970: 7250 6572 6365 7074 726f 6e28 0a20 2020  rPerceptron(.   
+00037980: 2020 2020 2020 2020 2064 5f69 6e70 7574           d_input
+00037990: 3d64 696d 2c0a 2020 2020 2020 2020 2020  =dim,.          
+000379a0: 2020 645f 6869 6464 656e 3d28 6469 6d2c    d_hidden=(dim,
+000379b0: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
+000379c0: 5f6f 7574 7075 743d 6469 6d2c 0a20 2020  _output=dim,.   
+000379d0: 2020 2020 2020 2020 2061 6374 6976 6174           activat
+000379e0: 696f 6e5f 666e 3d61 6374 6976 6174 696f  ion_fn=activatio
+000379f0: 6e5f 666e 2c0a 2020 2020 2020 2020 2020  n_fn,.          
+00037a00: 2020 736b 6970 5f63 6f6e 6e65 6374 696f    skip_connectio
+00037a10: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
+00037a20: 2020 2020 7765 6967 6874 6564 5f73 6b69      weighted_ski
+00037a30: 703d 4661 6c73 6529 0a0a 2020 2020 2020  p=False)..      
+00037a40: 2020 7365 6c66 2e6c 696e 5f72 6266 313a    self.lin_rbf1:
+00037a50: 206e 6e2e 4c69 6e65 6172 203d 206e 6e2e   nn.Linear = nn.
+00037a60: 4c69 6e65 6172 2864 696d 2c20 6469 6d2c  Linear(dim, dim,
+00037a70: 2062 6961 733d 4661 6c73 6529 0a20 2020   bias=False).   
+00037a80: 2020 2020 2073 656c 662e 6c69 6e5f 7262       self.lin_rb
+00037a90: 6632 3a20 6e6e 2e4c 696e 6561 7220 3d20  f2: nn.Linear = 
+00037aa0: 6e6e 2e4c 696e 6561 7228 6469 6d2c 2064  nn.Linear(dim, d
+00037ab0: 696d 2c20 6269 6173 3d46 616c 7365 290a  im, bias=False).
+00037ac0: 2020 2020 2020 2020 7365 6c66 2e6c 696e          self.lin
+00037ad0: 5f72 6266 5f6f 7574 3a20 6e6e 2e4c 696e  _rbf_out: nn.Lin
+00037ae0: 6561 7220 3d20 6e6e 2e4c 696e 6561 7228  ear = nn.Linear(
+00037af0: 6469 6d2c 2064 696d 2c20 6269 6173 3d46  dim, dim, bias=F
+00037b00: 616c 7365 290a 0a20 2020 2020 2020 2073  alse)..        s
+00037b10: 656c 662e 6d6c 703a 204d 756c 7469 6c61  elf.mlp: Multila
+00037b20: 7965 7250 6572 6365 7074 726f 6e20 3d20  yerPerceptron = 
+00037b30: 4d75 6c74 696c 6179 6572 5065 7263 6570  MultilayerPercep
+00037b40: 7472 6f6e 280a 2020 2020 2020 2020 2020  tron(.          
+00037b50: 2020 645f 696e 7075 743d 6469 6d2c 2064    d_input=dim, d
+00037b60: 5f6f 7574 7075 743d 6469 6d2c 2061 6374  _output=dim, act
+00037b70: 6976 6174 696f 6e5f 666e 3d61 6374 6976  ivation_fn=activ
+00037b80: 6174 696f 6e5f 666e 290a 2020 2020 2020  ation_fn).      
+00037b90: 2020 7365 6c66 2e6f 7574 5f6d 6c70 3a20    self.out_mlp: 
+00037ba0: 4d75 6c74 696c 6179 6572 5065 7263 6570  MultilayerPercep
+00037bb0: 7472 6f6e 203d 204d 756c 7469 6c61 7965  tron = Multilaye
+00037bc0: 7250 6572 6365 7074 726f 6e28 0a20 2020  rPerceptron(.   
+00037bd0: 2020 2020 2020 2020 2064 5f69 6e70 7574           d_input
+00037be0: 3d64 696d 2c0a 2020 2020 2020 2020 2020  =dim,.          
+00037bf0: 2020 645f 6869 6464 656e 3d28 6469 6d2c    d_hidden=(dim,
+00037c00: 2064 696d 292c 0a20 2020 2020 2020 2020   dim),.         
+00037c10: 2020 2064 5f6f 7574 7075 743d 6469 6d2c     d_output=dim,
+00037c20: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
+00037c30: 6976 6174 696f 6e5f 666e 3d61 6374 6976  ivation_fn=activ
+00037c40: 6174 696f 6e5f 666e 290a 2020 2020 2020  ation_fn).      
+00037c50: 2020 7365 6c66 2e6f 7574 5f57 3a20 6e6e    self.out_W: nn
+00037c60: 2e4c 696e 6561 7220 3d20 6e6e 2e4c 696e  .Linear = nn.Lin
+00037c70: 6561 7228 6469 6d2c 2031 290a 0a20 2020  ear(dim, 1)..   
+00037c80: 2064 6566 2066 6f72 7761 7264 2873 656c   def forward(sel
+00037c90: 662c 206e 6f64 655f 6665 6174 7572 6573  f, node_features
+00037ca0: 3a20 746f 7263 682e 5465 6e73 6f72 2c20  : torch.Tensor, 
+00037cb0: 7262 663a 2074 6f72 6368 2e54 656e 736f  rbf: torch.Tenso
+00037cc0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00037cd0: 2020 2073 6266 313a 2074 6f72 6368 2e54     sbf1: torch.T
+00037ce0: 656e 736f 722c 2073 6266 323a 2074 6f72  ensor, sbf2: tor
+00037cf0: 6368 2e54 656e 736f 722c 2069 6478 5f6b  ch.Tensor, idx_k
+00037d00: 6a3a 2074 6f72 6368 2e54 656e 736f 722c  j: torch.Tensor,
+00037d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00037d20: 2069 6478 5f6a 695f 313a 2074 6f72 6368   idx_ji_1: torch
+00037d30: 2e54 656e 736f 722c 2069 6478 5f6a 6a3a  .Tensor, idx_jj:
+00037d40: 2074 6f72 6368 2e54 656e 736f 722c 0a20   torch.Tensor,. 
+00037d50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00037d60: 6478 5f6a 695f 323a 2074 6f72 6368 2e54  dx_ji_2: torch.T
+00037d70: 656e 736f 722c 0a20 2020 2020 2020 2020  ensor,.         
+00037d80: 2020 2020 2020 2065 6467 655f 696e 6465         edge_inde
+00037d90: 783a 2074 6f72 6368 2e54 656e 736f 7229  x: torch.Tensor)
+00037da0: 202d 3e20 5475 706c 655b 746f 7263 682e   -> Tuple[torch.
+00037db0: 5465 6e73 6f72 2c20 746f 7263 682e 5465  Tensor, torch.Te
+00037dc0: 6e73 6f72 5d3a 0a20 2020 2020 2020 2022  nsor]:.        "
+00037dd0: 2222 5468 6520 666f 7277 6172 6420 6d65  ""The forward me
+00037de0: 7468 6f64 2070 6572 666f 726d 7320 7468  thod performs th
+00037df0: 6520 636f 6d70 7574 6174 696f 6e20 666f  e computation fo
+00037e00: 7220 7468 6520 4d58 4d4e 6574 4c6f 6361  r the MXMNetLoca
+00037e10: 6c4d 6573 7361 6765 5061 7373 696e 6720  lMessagePassing 
+00037e20: 4c61 7965 722e 0a20 2020 2020 2020 2054  Layer..        T
+00037e30: 6869 7320 6d65 7468 6f64 2070 726f 6365  his method proce
+00037e40: 7373 6573 2074 6865 2069 6e70 7574 2074  sses the input t
+00037e50: 656e 736f 7273 2072 6570 7265 7365 6e74  ensors represent
+00037e60: 696e 6720 6174 6f6d 2066 6561 7475 7265  ing atom feature
+00037e70: 732c 2072 6164 6961 6c20 6261 7369 7320  s, radial basis 
+00037e80: 6675 6e63 7469 6f6e 7320 2852 4246 292c  functions (RBF),
+00037e90: 2061 6e64 2073 7068 6572 6963 616c 2062   and spherical b
+00037ea0: 6173 6973 2066 756e 6374 696f 6e73 2028  asis functions (
+00037eb0: 5342 4629 2075 7369 6e67 206d 6573 7361  SBF) using messa
+00037ec0: 6765 2070 6173 7369 6e67 206f 7665 7220  ge passing over 
+00037ed0: 7468 6520 6d6f 6c65 6375 6c61 7220 6772  the molecular gr
+00037ee0: 6170 682e 2054 6865 206d 6573 7361 6765  aph. The message
+00037ef0: 2070 6173 7369 6e67 2075 7064 6174 6573   passing updates
+00037f00: 2074 6865 2061 746f 6d20 7265 7072 6573   the atom repres
+00037f10: 656e 7461 7469 6f6e 732c 2061 6e64 2074  entations, and t
+00037f20: 6865 2072 6573 756c 7469 6e67 2074 656e  he resulting ten
+00037f30: 736f 7220 7265 7072 6573 656e 7473 2074  sor represents t
+00037f40: 6865 2075 7064 6174 6564 2061 746f 6d20  he updated atom 
+00037f50: 6665 6174 7572 6520 6166 7465 7220 6c6f  feature after lo
+00037f60: 6361 6c20 6d65 7373 6167 6520 7061 7373  cal message pass
+00037f70: 696e 672e 0a0a 2020 2020 2020 2020 5061  ing...        Pa
+00037f80: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00037f90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00037fa0: 2020 2020 6e6f 6465 5f66 6561 7475 7265      node_feature
+00037fb0: 7320 3a20 746f 7263 682e 5465 6e73 6f72  s : torch.Tensor
+00037fc0: 0a20 2020 2020 2020 2020 2020 2049 6e70  .            Inp
+00037fd0: 7574 2074 656e 736f 7220 7265 7072 6573  ut tensor repres
+00037fe0: 656e 7469 6e67 2061 746f 6d20 6665 6174  enting atom feat
+00037ff0: 7572 6573 2e0a 2020 2020 2020 2020 7262  ures..        rb
+00038000: 6620 3a20 746f 7263 682e 5465 6e73 6f72  f : torch.Tensor
+00038010: 0a20 2020 2020 2020 2020 2020 2049 6e70  .            Inp
+00038020: 7574 2074 656e 736f 7220 7265 7072 6573  ut tensor repres
+00038030: 656e 7469 6e67 2072 6164 6961 6c20 6261  enting radial ba
+00038040: 7369 7320 6675 6e63 7469 6f6e 732e 0a20  sis functions.. 
+00038050: 2020 2020 2020 2073 6266 3120 3a20 746f         sbf1 : to
+00038060: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
+00038070: 2020 2020 2020 2049 6e70 7574 2074 656e         Input ten
+00038080: 736f 7220 7265 7072 6573 656e 7469 6e67  sor representing
+00038090: 2074 6865 2066 6972 7374 2073 6574 206f   the first set o
+000380a0: 6620 7370 6865 7269 6361 6c20 6261 7369  f spherical basi
+000380b0: 7320 6675 6e63 7469 6f6e 732e 0a20 2020  s functions..   
+000380c0: 2020 2020 2073 6266 3220 3a20 746f 7263       sbf2 : torc
+000380d0: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
+000380e0: 2020 2020 2049 6e70 7574 2074 656e 736f       Input tenso
+000380f0: 7220 7265 7072 6573 656e 7469 6e67 2074  r representing t
+00038100: 6865 2073 6563 6f6e 6420 7365 7420 6f66  he second set of
+00038110: 2073 7068 6572 6963 616c 2062 6173 6973   spherical basis
+00038120: 2066 756e 6374 696f 6e73 2e0a 2020 2020   functions..    
+00038130: 2020 2020 6964 785f 6b6a 203a 2074 6f72      idx_kj : tor
+00038140: 6368 2e54 656e 736f 720a 2020 2020 2020  ch.Tensor.      
+00038150: 2020 2020 2020 5465 6e73 6f72 2063 6f6e        Tensor con
+00038160: 7461 696e 696e 6720 696e 6469 6365 7320  taining indices 
+00038170: 666f 7220 7468 6520 6b20 616e 6420 6a20  for the k and j 
+00038180: 6174 6f6d 7320 696e 766f 6c76 6564 2069  atoms involved i
+00038190: 6e20 6561 6368 2069 6e74 6572 6163 7469  n each interacti
+000381a0: 6f6e 2e0a 2020 2020 2020 2020 6964 785f  on..        idx_
+000381b0: 6a69 5f31 203a 2074 6f72 6368 2e54 656e  ji_1 : torch.Ten
+000381c0: 736f 720a 2020 2020 2020 2020 2020 2020  sor.            
+000381d0: 5465 6e73 6f72 2063 6f6e 7461 696e 696e  Tensor containin
+000381e0: 6720 696e 6469 6365 7320 666f 7220 7468  g indices for th
+000381f0: 6520 6a20 616e 6420 6920 6174 6f6d 7320  e j and i atoms 
+00038200: 696e 766f 6c76 6564 2069 6e20 7468 6520  involved in the 
+00038210: 6669 7273 7420 6d65 7373 6167 6520 7061  first message pa
+00038220: 7373 696e 6720 7374 6570 2e0a 2020 2020  ssing step..    
+00038230: 2020 2020 6964 785f 6a6a 203a 2074 6f72      idx_jj : tor
+00038240: 6368 2e54 656e 736f 720a 2020 2020 2020  ch.Tensor.      
+00038250: 2020 2020 2020 5465 6e73 6f72 2063 6f6e        Tensor con
+00038260: 7461 696e 696e 6720 696e 6469 6365 7320  taining indices 
+00038270: 666f 7220 7468 6520 6a20 616e 6420 6a27  for the j and j'
+00038280: 2061 746f 6d73 2069 6e76 6f6c 7665 6420   atoms involved 
+00038290: 696e 2074 6865 2073 6563 6f6e 6420 6d65  in the second me
+000382a0: 7373 6167 6520 7061 7373 696e 6720 7374  ssage passing st
+000382b0: 6570 2e0a 2020 2020 2020 2020 6964 785f  ep..        idx_
+000382c0: 6a69 5f32 203a 2074 6f72 6368 2e54 656e  ji_2 : torch.Ten
+000382d0: 736f 720a 2020 2020 2020 2020 2020 2020  sor.            
+000382e0: 5465 6e73 6f72 2063 6f6e 7461 696e 696e  Tensor containin
+000382f0: 6720 696e 6469 6365 7320 666f 7220 7468  g indices for th
+00038300: 6520 6a20 616e 6420 6920 6174 6f6d 7320  e j and i atoms 
+00038310: 696e 766f 6c76 6564 2069 6e20 7468 6520  involved in the 
+00038320: 7365 636f 6e64 206d 6573 7361 6765 2070  second message p
+00038330: 6173 7369 6e67 2073 7465 702e 0a20 2020  assing step..   
+00038340: 2020 2020 2065 6467 655f 696e 6465 7820       edge_index 
+00038350: 3a20 746f 7263 682e 5465 6e73 6f72 0a20  : torch.Tensor. 
+00038360: 2020 2020 2020 2020 2020 2054 656e 736f             Tenso
+00038370: 7220 636f 6e74 6169 6e69 6e67 2074 6865  r containing the
+00038380: 2065 6467 6520 696e 6469 6365 7320 6f66   edge indices of
+00038390: 2074 6865 206d 6f6c 6563 756c 6172 2067   the molecular g
+000383a0: 7261 7068 2c20 7769 7468 2073 6861 7065  raph, with shape
+000383b0: 2028 322c 204d 292c 2077 6865 7265 204d   (2, M), where M
+000383c0: 2069 7320 7468 6520 6e75 6d62 6572 206f   is the number o
+000383d0: 6620 6564 6765 732e 0a0a 2020 2020 2020  f edges...      
+000383e0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+000383f0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00038400: 2020 6e6f 6465 5f66 6561 7475 7265 733a    node_features:
+00038410: 2074 6f72 6368 2e54 656e 736f 720a 2020   torch.Tensor.  
+00038420: 2020 2020 2020 2020 2020 5570 6461 7465            Update
+00038430: 6420 6174 6f6d 2072 6570 7265 7365 6e74  d atom represent
+00038440: 6174 696f 6e73 2061 6674 6572 206c 6f63  ations after loc
+00038450: 616c 206d 6573 7361 6765 2070 6173 7369  al message passi
+00038460: 6e67 2e0a 2020 2020 2020 2020 6f75 7470  ng..        outp
+00038470: 7574 3a20 746f 7263 682e 5465 6e73 6f72  ut: torch.Tensor
+00038480: 0a20 2020 2020 2020 2020 2020 204f 7574  .            Out
+00038490: 7075 7420 7465 6e73 6f72 2072 6570 7265  put tensor repre
+000384a0: 7365 6e74 696e 6720 6120 6669 7865 642d  senting a fixed-
+000384b0: 7369 7a65 2072 6570 7265 7365 6e74 6174  size representat
+000384c0: 696f 6e2c 2077 6974 6820 7368 6170 6520  ion, with shape 
+000384d0: 284e 2c20 3129 2e0a 2020 2020 2020 2020  (N, 1)..        
+000384e0: 2222 220a 0a20 2020 2020 2020 2072 6573  """..        res
+000384f0: 6964 7561 6c5f 6e6f 6465 5f66 6561 7475  idual_node_featu
+00038500: 7265 733a 2074 6f72 6368 2e54 656e 736f  res: torch.Tenso
+00038510: 7220 3d20 6e6f 6465 5f66 6561 7475 7265  r = node_feature
+00038520: 730a 0a20 2020 2020 2020 2023 2049 6e74  s..        # Int
+00038530: 6567 7261 7465 2074 6865 2043 726f 7373  egrate the Cross
+00038540: 204c 6179 6572 204d 6170 7069 6e67 2069   Layer Mapping i
+00038550: 6e73 6964 6520 7468 6520 4c6f 6361 6c20  nside the Local 
+00038560: 4d65 7373 6167 6520 5061 7373 696e 670a  Message Passing.
+00038570: 2020 2020 2020 2020 6e6f 6465 5f66 6561          node_fea
+00038580: 7475 7265 7320 3d20 7365 6c66 2e68 5f6d  tures = self.h_m
+00038590: 6c70 286e 6f64 655f 6665 6174 7572 6573  lp(node_features
+000385a0: 290a 0a20 2020 2020 2020 2023 204d 6573  )..        # Mes
+000385b0: 7361 6765 2050 6173 7369 6e67 2031 0a20  sage Passing 1. 
+000385c0: 2020 2020 2020 206a 2c20 6920 3d20 6564         j, i = ed
+000385d0: 6765 5f69 6e64 6578 0a20 2020 2020 2020  ge_index.       
+000385e0: 206d 3a20 746f 7263 682e 5465 6e73 6f72   m: torch.Tensor
+000385f0: 203d 2074 6f72 6368 2e63 6174 285b 6e6f   = torch.cat([no
+00038600: 6465 5f66 6561 7475 7265 735b 695d 2c20  de_features[i], 
+00038610: 6e6f 6465 5f66 6561 7475 7265 735b 6a5d  node_features[j]
+00038620: 2c20 7262 665d 2c0a 2020 2020 2020 2020  , rbf],.        
+00038630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00038640: 2020 2020 2020 2020 2020 2020 6469 6d3d              dim=
+00038650: 2d31 290a 0a20 2020 2020 2020 206d 5f6b  -1)..        m_k
+00038660: 6a3a 2074 6f72 6368 2e54 656e 736f 7220  j: torch.Tensor 
+00038670: 3d20 7365 6c66 2e6d 6c70 5f6b 6a28 6d29  = self.mlp_kj(m)
+00038680: 0a20 2020 2020 2020 206d 5f6b 6a20 3d20  .        m_kj = 
+00038690: 6d5f 6b6a 202a 2073 656c 662e 6c69 6e5f  m_kj * self.lin_
+000386a0: 7262 6631 2872 6266 290a 2020 2020 2020  rbf1(rbf).      
+000386b0: 2020 6d5f 6b6a 203d 206d 5f6b 6a5b 6964    m_kj = m_kj[id
+000386c0: 785f 6b6a 5d20 2a20 7365 6c66 2e6d 6c70  x_kj] * self.mlp
+000386d0: 5f73 6266 3128 7362 6631 290a 2020 2020  _sbf1(sbf1).    
+000386e0: 2020 2020 6d5f 6b6a 203d 2073 6361 7474      m_kj = scatt
+000386f0: 6572 286d 5f6b 6a2c 2069 6478 5f6a 695f  er(m_kj, idx_ji_
+00038700: 312c 2064 696d 3d30 2c20 6469 6d5f 7369  1, dim=0, dim_si
+00038710: 7a65 3d6d 2e73 697a 6528 3029 2c20 7265  ze=m.size(0), re
+00038720: 6475 6365 3d27 6164 6427 290a 0a20 2020  duce='add')..   
+00038730: 2020 2020 206d 5f6a 695f 313a 2074 6f72       m_ji_1: tor
+00038740: 6368 2e54 656e 736f 7220 3d20 7365 6c66  ch.Tensor = self
+00038750: 2e6d 6c70 5f6a 695f 3128 6d29 0a0a 2020  .mlp_ji_1(m)..  
+00038760: 2020 2020 2020 6d20 3d20 6d5f 6a69 5f31        m = m_ji_1
+00038770: 202b 206d 5f6b 6a0a 0a20 2020 2020 2020   + m_kj..       
+00038780: 2023 204d 6573 7361 6765 2050 6173 7369   # Message Passi
+00038790: 6e67 2032 0a20 2020 2020 2020 206d 5f6a  ng 2.        m_j
+000387a0: 6a3a 2074 6f72 6368 2e54 656e 736f 7220  j: torch.Tensor 
+000387b0: 3d20 7365 6c66 2e6d 6c70 5f6a 6a28 6d29  = self.mlp_jj(m)
+000387c0: 0a20 2020 2020 2020 206d 5f6a 6a20 3d20  .        m_jj = 
+000387d0: 6d5f 6a6a 202a 2073 656c 662e 6c69 6e5f  m_jj * self.lin_
+000387e0: 7262 6632 2872 6266 290a 2020 2020 2020  rbf2(rbf).      
+000387f0: 2020 6d5f 6a6a 203d 206d 5f6a 6a5b 6964    m_jj = m_jj[id
+00038800: 785f 6a6a 5d20 2a20 7365 6c66 2e6d 6c70  x_jj] * self.mlp
+00038810: 5f73 6266 3228 7362 6632 290a 2020 2020  _sbf2(sbf2).    
+00038820: 2020 2020 6d5f 6a6a 203d 2073 6361 7474      m_jj = scatt
+00038830: 6572 286d 5f6a 6a2c 2069 6478 5f6a 695f  er(m_jj, idx_ji_
+00038840: 322c 2064 696d 3d30 2c20 6469 6d5f 7369  2, dim=0, dim_si
+00038850: 7a65 3d6d 2e73 697a 6528 3029 2c20 7265  ze=m.size(0), re
+00038860: 6475 6365 3d27 6164 6427 290a 0a20 2020  duce='add')..   
+00038870: 2020 2020 206d 5f6a 695f 323a 2074 6f72       m_ji_2: tor
+00038880: 6368 2e54 656e 736f 7220 3d20 7365 6c66  ch.Tensor = self
+00038890: 2e6d 6c70 5f6a 695f 3228 6d29 0a0a 2020  .mlp_ji_2(m)..  
+000388a0: 2020 2020 2020 6d20 3d20 6d5f 6a69 5f32        m = m_ji_2
+000388b0: 202b 206d 5f6a 6a0a 0a20 2020 2020 2020   + m_jj..       
+000388c0: 2023 2041 6767 7265 6761 7469 6f6e 0a20   # Aggregation. 
+000388d0: 2020 2020 2020 206d 203d 2073 656c 662e         m = self.
+000388e0: 6c69 6e5f 7262 665f 6f75 7428 7262 6629  lin_rbf_out(rbf)
+000388f0: 202a 206d 0a20 2020 2020 2020 206e 6f64   * m.        nod
+00038900: 655f 6665 6174 7572 6573 203d 2073 6361  e_features = sca
+00038910: 7474 6572 286d 2c0a 2020 2020 2020 2020  tter(m,.        
+00038920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00038930: 2020 2020 2020 2020 692c 0a20 2020 2020          i,.     
+00038940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00038950: 2020 2020 2020 2020 2020 2064 696d 3d30             dim=0
+00038960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00038970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00038980: 2020 6469 6d5f 7369 7a65 3d6e 6f64 655f    dim_size=node_
+00038990: 6665 6174 7572 6573 2e73 697a 6528 3029  features.size(0)
+000389a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000389b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000389c0: 2020 7265 6475 6365 3d27 6164 6427 290a    reduce='add').
+000389d0: 0a20 2020 2020 2020 2023 2055 7064 6174  .        # Updat
+000389e0: 6520 6675 6e63 7469 6f6e 2066 5f75 0a20  e function f_u. 
+000389f0: 2020 2020 2020 206e 6f64 655f 6665 6174         node_feat
+00038a00: 7572 6573 203d 2073 656c 662e 7265 7331  ures = self.res1
+00038a10: 286e 6f64 655f 6665 6174 7572 6573 290a  (node_features).
+00038a20: 2020 2020 2020 2020 6e6f 6465 5f66 6561          node_fea
+00038a30: 7475 7265 7320 3d20 7365 6c66 2e6d 6c70  tures = self.mlp
+00038a40: 286e 6f64 655f 6665 6174 7572 6573 2920  (node_features) 
+00038a50: 2b20 7265 7369 6475 616c 5f6e 6f64 655f  + residual_node_
+00038a60: 6665 6174 7572 6573 0a20 2020 2020 2020  features.       
+00038a70: 206e 6f64 655f 6665 6174 7572 6573 203d   node_features =
+00038a80: 2073 656c 662e 7265 7332 286e 6f64 655f   self.res2(node_
+00038a90: 6665 6174 7572 6573 290a 2020 2020 2020  features).      
+00038aa0: 2020 6e6f 6465 5f66 6561 7475 7265 7320    node_features 
+00038ab0: 3d20 7365 6c66 2e72 6573 3328 6e6f 6465  = self.res3(node
+00038ac0: 5f66 6561 7475 7265 7329 0a0a 2020 2020  _features)..    
+00038ad0: 2020 2020 2320 4f75 7470 7574 204d 6f64      # Output Mod
+00038ae0: 756c 650a 2020 2020 2020 2020 6f75 743a  ule.        out:
+00038af0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+00038b00: 7365 6c66 2e6f 7574 5f6d 6c70 286e 6f64  self.out_mlp(nod
+00038b10: 655f 6665 6174 7572 6573 290a 2020 2020  e_features).    
+00038b20: 2020 2020 6f75 7470 7574 3a20 746f 7263      output: torc
+00038b30: 682e 5465 6e73 6f72 203d 2073 656c 662e  h.Tensor = self.
+00038b40: 6f75 745f 5728 6f75 7429 0a0a 2020 2020  out_W(out)..    
+00038b50: 2020 2020 7265 7475 726e 206e 6f64 655f      return node_
+00038b60: 6665 6174 7572 6573 2c20 6f75 7470 7574  features, output
+00038b70: 0a0a 0a63 6c61 7373 204d 584d 4e65 7453  ...class MXMNetS
+00038b80: 7068 6572 6963 616c 4261 7369 734c 6179  phericalBasisLay
+00038b90: 6572 2874 6f72 6368 2e6e 6e2e 4d6f 6475  er(torch.nn.Modu
+00038ba0: 6c65 293a 0a20 2020 2022 2222 4974 2074  le):.    """It t
+00038bb0: 616b 6573 2070 6169 7277 6973 6520 6469  akes pairwise di
+00038bc0: 7374 616e 6365 7320 616e 6420 616e 676c  stances and angl
+00038bd0: 6573 2062 6574 7765 656e 2061 746f 6d73  es between atoms
+00038be0: 2061 7320 696e 7075 7420 616e 6420 636f   as input and co
+00038bf0: 6d62 696e 6573 2072 6164 6961 6c20 6261  mbines radial ba
+00038c00: 7369 7320 6675 6e63 7469 6f6e 7320 7769  sis functions wi
+00038c10: 7468 2073 7068 6572 6963 616c 2068 6172  th spherical har
+00038c20: 6d6f 6e69 630a 2020 2020 6675 6e63 7469  monic.    functi
+00038c30: 6f6e 7320 746f 2067 656e 6572 6174 6520  ons to generate 
+00038c40: 6120 6669 7865 642d 7369 7a65 2072 6570  a fixed-size rep
+00038c50: 7265 7365 6e74 6174 696f 6e20 7468 6174  resentation that
+00038c60: 2063 6170 7475 7265 7320 626f 7468 2072   captures both r
+00038c70: 6164 6961 6c20 616e 6420 6f72 6965 6e74  adial and orient
+00038c80: 6174 696f 6e20 696e 666f 726d 6174 696f  ation informatio
+00038c90: 6e2e 2054 6869 7320 7479 7065 206f 660a  n. This type of.
+00038ca0: 2020 2020 7265 7072 6573 656e 7461 7469      representati
+00038cb0: 6f6e 2069 7320 636f 6d6d 6f6e 6c79 2075  on is commonly u
+00038cc0: 7365 6420 696e 206d 6f6c 6563 756c 6172  sed in molecular
+00038cd0: 206d 6f64 656c 696e 6720 616e 6420 7369   modeling and si
+00038ce0: 6d75 6c61 7469 6f6e 7320 746f 2063 6170  mulations to cap
+00038cf0: 7475 7265 2074 6865 2062 6568 6176 696f  ture the behavio
+00038d00: 7220 6f66 2061 746f 6d73 2061 6e64 206d  r of atoms and m
+00038d10: 6f6c 6563 756c 6573 2069 6e0a 2020 2020  olecules in.    
+00038d20: 6368 656d 6963 616c 2073 7973 7465 6d73  chemical systems
+00038d30: 2e0a 0a20 2020 2049 6e73 6964 6520 7468  ...    Inside th
+00038d40: 6520 696e 6974 6961 6c69 7a61 7469 6f6e  e initialization
+00038d50: 2c20 4265 7373 656c 2062 6173 6973 2066  , Bessel basis f
+00038d60: 756e 6374 696f 6e73 2061 6e64 2072 6561  unctions and rea
+00038d70: 6c20 7370 6865 7269 6361 6c20 6861 726d  l spherical harm
+00038d80: 6f6e 6963 2066 756e 6374 696f 6e73 2061  onic functions a
+00038d90: 7265 2067 656e 6572 6174 6564 2e0a 2020  re generated..  
+00038da0: 2020 5468 6520 4265 7373 656c 2062 6173    The Bessel bas
+00038db0: 6973 2066 756e 6374 696f 6e73 2063 6170  is functions cap
+00038dc0: 7475 7265 2074 6865 2072 6164 6961 6c20  ture the radial 
+00038dd0: 696e 666f 726d 6174 696f 6e2c 2061 6e64  information, and
+00038de0: 2074 6865 2073 7068 6572 6963 616c 2068   the spherical h
+00038df0: 6172 6d6f 6e69 6320 6675 6e63 7469 6f6e  armonic function
+00038e00: 7320 6361 7074 7572 6520 7468 6520 6f72  s capture the or
+00038e10: 6965 6e74 6174 696f 6e20 696e 666f 726d  ientation inform
+00038e20: 6174 696f 6e2e 0a20 2020 2054 6865 7365  ation..    These
+00038e30: 2066 756e 6374 696f 6e73 2061 7265 2067   functions are g
+00038e40: 656e 6572 6174 6564 2062 6173 6564 206f  enerated based o
+00038e50: 6e20 7468 6520 7072 6f76 6964 6564 206e  n the provided n
+00038e60: 756d 5f73 7068 6572 6963 616c 2061 6e64  um_spherical and
+00038e70: 206e 756d 5f72 6164 6961 6c20 7061 7261   num_radial para
+00038e80: 6d65 7465 7273 2e0a 0a20 2020 2045 7861  meters...    Exa
+00038e90: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+00038ea0: 2d2d 0a20 2020 203e 3e3e 2064 6973 7420  --.    >>> dist 
+00038eb0: 3d20 746f 7263 682e 7465 6e73 6f72 285b  = torch.tensor([
+00038ec0: 302e 352c 2031 2e30 2c20 322e 302c 2033  0.5, 1.0, 2.0, 3
+00038ed0: 2e30 5d29 0a20 2020 203e 3e3e 2061 6e67  .0]).    >>> ang
+00038ee0: 6c65 203d 2074 6f72 6368 2e74 656e 736f  le = torch.tenso
+00038ef0: 7228 5b30 2e31 2c20 302e 322c 2030 2e33  r([0.1, 0.2, 0.3
+00038f00: 2c20 302e 345d 290a 2020 2020 3e3e 3e20  , 0.4]).    >>> 
+00038f10: 6964 785f 6b6a 203d 2074 6f72 6368 2e74  idx_kj = torch.t
+00038f20: 656e 736f 7228 5b30 2c20 312c 2032 2c20  ensor([0, 1, 2, 
+00038f30: 335d 290a 2020 2020 3e3e 3e20 7370 6865  3]).    >>> sphe
+00038f40: 7269 6361 6c5f 6c61 7965 7220 3d20 4d58  rical_layer = MX
+00038f50: 4d4e 6574 5370 6865 7269 6361 6c42 6173  MNetSphericalBas
+00038f60: 6973 4c61 7965 7228 656e 7665 6c6f 7065  isLayer(envelope
+00038f70: 5f65 7870 6f6e 656e 743d 322c 206e 756d  _exponent=2, num
+00038f80: 5f73 7068 6572 6963 616c 3d32 2c20 6e75  _spherical=2, nu
+00038f90: 6d5f 7261 6469 616c 3d32 2c20 6375 746f  m_radial=2, cuto
+00038fa0: 6666 3d32 2e30 290a 2020 2020 3e3e 3e20  ff=2.0).    >>> 
+00038fb0: 6f75 7470 7574 203d 2073 7068 6572 6963  output = spheric
+00038fc0: 616c 5f6c 6179 6572 2864 6973 742c 2061  al_layer(dist, a
+00038fd0: 6e67 6c65 2c20 6964 785f 6b6a 290a 2020  ngle, idx_kj).  
+00038fe0: 2020 3e3e 3e20 6f75 7470 7574 2e73 6861    >>> output.sha
+00038ff0: 7065 0a20 2020 2074 6f72 6368 2e53 697a  pe.    torch.Siz
+00039000: 6528 5b34 2c20 345d 290a 2020 2020 2222  e([4, 4]).    ""
+00039010: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00039020: 745f 5f28 7365 6c66 2c0a 2020 2020 2020  t__(self,.      
+00039030: 2020 2020 2020 2020 2020 206e 756d 5f73             num_s
+00039040: 7068 6572 6963 616c 3a20 696e 742c 0a20  pherical: int,. 
+00039050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039060: 6e75 6d5f 7261 6469 616c 3a20 696e 742c  num_radial: int,
+00039070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00039080: 2020 6375 746f 6666 3a20 666c 6f61 7420    cutoff: float 
+00039090: 3d20 352e 302c 0a20 2020 2020 2020 2020  = 5.0,.         
+000390a0: 2020 2020 2020 2020 656e 7665 6c6f 7065          envelope
+000390b0: 5f65 7870 6f6e 656e 743a 2069 6e74 203d  _exponent: int =
+000390c0: 2035 293a 0a20 2020 2020 2020 2022 2222   5):.        """
+000390d0: 496e 6974 6961 6c69 7a65 2074 6865 204d  Initialize the M
+000390e0: 584d 4e65 7453 7068 6572 6963 616c 4261  XMNetSphericalBa
+000390f0: 7369 734c 6179 6572 2e0a 0a20 2020 2020  sisLayer...     
+00039100: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00039110: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00039120: 0a20 2020 2020 2020 206e 756d 5f73 7068  .        num_sph
+00039130: 6572 6963 616c 3a20 696e 740a 2020 2020  erical: int.    
+00039140: 2020 2020 2020 2020 5468 6520 6e75 6d62          The numb
+00039150: 6572 206f 6620 7370 6865 7269 6361 6c20  er of spherical 
+00039160: 6861 726d 6f6e 6963 2066 756e 6374 696f  harmonic functio
+00039170: 6e73 2074 6f20 7573 652e 2054 6865 7365  ns to use. These
+00039180: 2066 756e 6374 696f 6e73 2063 6170 7475   functions captu
+00039190: 7265 206f 7269 656e 7461 7469 6f6e 2069  re orientation i
+000391a0: 6e66 6f72 6d61 7469 6f6e 2072 656c 6174  nformation relat
+000391b0: 6564 2074 6f20 6174 6f6d 2070 6f73 6974  ed to atom posit
+000391c0: 696f 6e73 2e0a 2020 2020 2020 2020 6e75  ions..        nu
+000391d0: 6d5f 7261 6469 616c 3a20 696e 740a 2020  m_radial: int.  
+000391e0: 2020 2020 2020 2020 2020 5468 6520 6e75            The nu
+000391f0: 6d62 6572 206f 6620 7261 6469 616c 2062  mber of radial b
+00039200: 6173 6973 2066 756e 6374 696f 6e73 2074  asis functions t
+00039210: 6f20 7573 652e 2054 6865 7365 2066 756e  o use. These fun
+00039220: 6374 696f 6e73 2063 6170 7475 7265 2069  ctions capture i
+00039230: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+00039240: 2070 6169 7277 6973 6520 6469 7374 616e   pairwise distan
+00039250: 6365 7320 6265 7477 6565 6e20 6174 6f6d  ces between atom
+00039260: 732e 0a20 2020 2020 2020 2063 7574 6f66  s..        cutof
+00039270: 663a 2066 6c6f 6174 2c20 6f70 7469 6f6e  f: float, option
+00039280: 616c 2028 6465 6661 756c 7420 352e 3029  al (default 5.0)
+00039290: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+000392a0: 2063 7574 6f66 6620 6469 7374 616e 6365   cutoff distance
+000392b0: 2066 6f72 2074 6865 2072 6164 6961 6c20   for the radial 
+000392c0: 6261 7369 7320 6675 6e63 7469 6f6e 732e  basis functions.
+000392d0: 2049 7420 7370 6563 6966 6965 7320 7468   It specifies th
+000392e0: 6520 6469 7374 616e 6365 2062 6579 6f6e  e distance beyon
+000392f0: 6420 7768 6963 6820 7468 6520 696e 7465  d which the inte
+00039300: 7261 6374 696f 6e73 2061 7265 2069 676e  ractions are ign
+00039310: 6f72 6564 2e0a 2020 2020 2020 2020 656e  ored..        en
+00039320: 7665 6c6f 7065 5f65 7870 6f6e 656e 743a  velope_exponent:
+00039330: 2069 6e74 2c20 6f70 7469 6f6e 616c 2028   int, optional (
+00039340: 6465 6661 756c 7420 3529 0a20 2020 2020  default 5).     
+00039350: 2020 2020 2020 2054 6865 2065 7870 6f6e         The expon
+00039360: 656e 7420 666f 7220 7468 6520 656e 7665  ent for the enve
+00039370: 6c6f 7065 2066 756e 6374 696f 6e2e 2049  lope function. I
+00039380: 7420 636f 6e74 726f 6c73 2074 6865 2064  t controls the d
+00039390: 6567 7265 6520 6f66 2064 616d 7069 6e67  egree of damping
+000393a0: 2066 6f72 2074 6865 2072 6164 6961 6c20   for the radial 
+000393b0: 6261 7369 7320 6675 6e63 7469 6f6e 732e  basis functions.
+000393c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000393d0: 2020 2020 2073 7570 6572 284d 584d 4e65       super(MXMNe
+000393e0: 7453 7068 6572 6963 616c 4261 7369 734c  tSphericalBasisL
+000393f0: 6179 6572 2c20 7365 6c66 292e 5f5f 696e  ayer, self).__in
+00039400: 6974 5f5f 2829 0a0a 2020 2020 2020 2020  it__()..        
+00039410: 6173 7365 7274 206e 756d 5f72 6164 6961  assert num_radia
+00039420: 6c20 3c3d 2036 340a 2020 2020 2020 2020  l <= 64.        
+00039430: 7365 6c66 2e6e 756d 5f73 7068 6572 6963  self.num_spheric
+00039440: 616c 3a20 696e 7420 3d20 6e75 6d5f 7370  al: int = num_sp
+00039450: 6865 7269 6361 6c0a 2020 2020 2020 2020  herical.        
+00039460: 7365 6c66 2e6e 756d 5f72 6164 6961 6c3a  self.num_radial:
+00039470: 2069 6e74 203d 206e 756d 5f72 6164 6961   int = num_radia
+00039480: 6c0a 2020 2020 2020 2020 7365 6c66 2e63  l.        self.c
+00039490: 7574 6f66 663a 2066 6c6f 6174 203d 2063  utoff: float = c
+000394a0: 7574 6f66 660a 2020 2020 2020 2020 7365  utoff.        se
+000394b0: 6c66 2e65 6e76 656c 6f70 653a 205f 4d58  lf.envelope: _MX
+000394c0: 4d4e 6574 456e 7665 6c6f 7065 203d 205f  MNetEnvelope = _
+000394d0: 4d58 4d4e 6574 456e 7665 6c6f 7065 2865  MXMNetEnvelope(e
+000394e0: 6e76 656c 6f70 655f 6578 706f 6e65 6e74  nvelope_exponent
+000394f0: 290a 0a20 2020 2020 2020 2062 6573 7365  )..        besse
+00039500: 6c5f 666f 726d 733a 204c 6973 7420 3d20  l_forms: List = 
+00039510: 6265 7373 656c 5f62 6173 6973 286e 756d  bessel_basis(num
+00039520: 5f73 7068 6572 6963 616c 2c20 6e75 6d5f  _spherical, num_
+00039530: 7261 6469 616c 290a 2020 2020 2020 2020  radial).        
+00039540: 7370 685f 6861 726d 5f66 6f72 6d73 3a20  sph_harm_forms: 
+00039550: 4c69 7374 5b4c 6973 745b 7374 725d 5d20  List[List[str]] 
+00039560: 3d20 7265 616c 5f73 7068 5f68 6172 6d28  = real_sph_harm(
+00039570: 6e75 6d5f 7370 6865 7269 6361 6c29 0a20  num_spherical). 
+00039580: 2020 2020 2020 2073 656c 662e 7370 685f         self.sph_
+00039590: 6675 6e63 733a 204c 6973 7420 3d20 5b5d  funcs: List = []
+000395a0: 0a20 2020 2020 2020 2073 656c 662e 6265  .        self.be
+000395b0: 7373 656c 5f66 756e 6373 3a20 4c69 7374  ssel_funcs: List
+000395c0: 203d 205b 5d0a 2020 2020 2020 2020 783a   = [].        x:
+000395d0: 2041 6e79 0a20 2020 2020 2020 2074 6865   Any.        the
+000395e0: 7461 3a20 416e 790a 2020 2020 2020 2020  ta: Any.        
+000395f0: 782c 2074 6865 7461 203d 2073 796d 2e73  x, theta = sym.s
+00039600: 796d 626f 6c73 2827 7820 7468 6574 6127  ymbols('x theta'
+00039610: 290a 2020 2020 2020 2020 6d6f 6475 6c65  ).        module
+00039620: 733a 2044 6963 7420 3d20 7b27 7369 6e27  s: Dict = {'sin'
+00039630: 3a20 746f 7263 682e 7369 6e2c 2027 636f  : torch.sin, 'co
+00039640: 7327 3a20 746f 7263 682e 636f 737d 0a20  s': torch.cos}. 
+00039650: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00039660: 7261 6e67 6528 6e75 6d5f 7370 6865 7269  range(num_spheri
+00039670: 6361 6c29 3a0a 2020 2020 2020 2020 2020  cal):.          
+00039680: 2020 6966 2069 203d 3d20 303a 0a20 2020    if i == 0:.   
+00039690: 2020 2020 2020 2020 2020 2020 2073 7068               sph
+000396a0: 313a 2041 6e79 203d 2073 796d 2e6c 616d  1: Any = sym.lam
+000396b0: 6264 6966 7928 5b74 6865 7461 5d2c 2073  bdify([theta], s
+000396c0: 7068 5f68 6172 6d5f 666f 726d 735b 695d  ph_harm_forms[i]
+000396d0: 5b30 5d2c 0a20 2020 2020 2020 2020 2020  [0],.           
+000396e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000396f0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00039700: 6475 6c65 7329 2830 290a 2020 2020 2020  dules)(0).      
+00039710: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00039720: 7068 5f66 756e 6373 2e61 7070 656e 6428  ph_funcs.append(
+00039730: 6c61 6d62 6461 2078 3a20 746f 7263 682e  lambda x: torch.
+00039740: 7a65 726f 735f 6c69 6b65 2878 2920 2b20  zeros_like(x) + 
+00039750: 7370 6831 290a 2020 2020 2020 2020 2020  sph1).          
+00039760: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00039770: 2020 2020 2020 2020 7370 683a 2041 6e79          sph: Any
+00039780: 203d 2073 796d 2e6c 616d 6264 6966 7928   = sym.lambdify(
+00039790: 5b74 6865 7461 5d2c 2073 7068 5f68 6172  [theta], sph_har
+000397a0: 6d5f 666f 726d 735b 695d 5b30 5d2c 206d  m_forms[i][0], m
+000397b0: 6f64 756c 6573 290a 2020 2020 2020 2020  odules).        
+000397c0: 2020 2020 2020 2020 7365 6c66 2e73 7068          self.sph
+000397d0: 5f66 756e 6373 2e61 7070 656e 6428 7370  _funcs.append(sp
+000397e0: 6829 0a20 2020 2020 2020 2020 2020 2066  h).            f
+000397f0: 6f72 206a 2069 6e20 7261 6e67 6528 6e75  or j in range(nu
+00039800: 6d5f 7261 6469 616c 293a 0a20 2020 2020  m_radial):.     
+00039810: 2020 2020 2020 2020 2020 2062 6573 7365             besse
+00039820: 6c3a 2041 6e79 203d 2073 796d 2e6c 616d  l: Any = sym.lam
+00039830: 6264 6966 7928 5b78 5d2c 2062 6573 7365  bdify([x], besse
+00039840: 6c5f 666f 726d 735b 695d 5b6a 5d2c 206d  l_forms[i][j], m
+00039850: 6f64 756c 6573 290a 2020 2020 2020 2020  odules).        
+00039860: 2020 2020 2020 2020 7365 6c66 2e62 6573          self.bes
+00039870: 7365 6c5f 6675 6e63 732e 6170 7065 6e64  sel_funcs.append
+00039880: 2862 6573 7365 6c29 0a0a 2020 2020 6465  (bessel)..    de
+00039890: 6620 666f 7277 6172 6428 7365 6c66 2c20  f forward(self, 
+000398a0: 6469 7374 3a20 746f 7263 682e 5465 6e73  dist: torch.Tens
+000398b0: 6f72 2c20 616e 676c 653a 2074 6f72 6368  or, angle: torch
+000398c0: 2e54 656e 736f 722c 0a20 2020 2020 2020  .Tensor,.       
+000398d0: 2020 2020 2020 2020 2069 6478 5f6b 6a3a           idx_kj:
+000398e0: 2074 6f72 6368 2e54 656e 736f 7229 202d   torch.Tensor) -
+000398f0: 3e20 746f 7263 682e 5465 6e73 6f72 3a0a  > torch.Tensor:.
+00039900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00039910: 2020 2020 466f 7277 6172 6420 7061 7373      Forward pass
+00039920: 206f 6620 7468 6520 4d58 4d4e 6574 5370   of the MXMNetSp
+00039930: 6865 7269 6361 6c42 6173 6973 4c61 7965  hericalBasisLaye
+00039940: 722e 0a0a 2020 2020 2020 2020 5061 7261  r...        Para
+00039950: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00039960: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00039970: 2020 6469 7374 3a20 746f 7263 682e 5465    dist: torch.Te
+00039980: 6e73 6f72 0a20 2020 2020 2020 2020 2020  nsor.           
+00039990: 2049 6e70 7574 2074 656e 736f 7220 7265   Input tensor re
+000399a0: 7072 6573 656e 7469 6e67 2070 6169 7277  presenting pairw
+000399b0: 6973 6520 6469 7374 616e 6365 7320 6265  ise distances be
+000399c0: 7477 6565 6e20 6174 6f6d 732e 0a20 2020  tween atoms..   
+000399d0: 2020 2020 2061 6e67 6c65 3a20 746f 7263       angle: torc
+000399e0: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
+000399f0: 2020 2020 2049 6e70 7574 2074 656e 736f       Input tenso
+00039a00: 7220 7265 7072 6573 656e 7469 6e67 2070  r representing p
+00039a10: 6169 7277 6973 6520 616e 676c 6573 2062  airwise angles b
+00039a20: 6574 7765 656e 2061 746f 6d73 2e0a 2020  etween atoms..  
+00039a30: 2020 2020 2020 6964 785f 6b6a 3a20 746f        idx_kj: to
+00039a40: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
+00039a50: 2020 2020 2020 2054 656e 736f 7220 636f         Tensor co
+00039a60: 6e74 6169 6e69 6e67 2069 6e64 6963 6573  ntaining indices
+00039a70: 2066 6f72 2074 6865 206b 2061 6e64 206a   for the k and j
+00039a80: 2061 746f 6d73 2e0a 0a20 2020 2020 2020   atoms...       
+00039a90: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00039aa0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00039ab0: 206f 7574 7075 743a 2074 6f72 6368 2e54   output: torch.T
+00039ac0: 656e 736f 720a 2020 2020 2020 2020 2020  ensor.          
+00039ad0: 2020 5468 6520 6f75 7470 7574 2074 656e    The output ten
+00039ae0: 736f 7220 636f 6e74 6169 6e69 6e67 2074  sor containing t
+00039af0: 6865 2066 6978 6564 2d73 697a 6520 7265  he fixed-size re
+00039b00: 7072 6573 656e 7461 7469 6f6e 2e0a 2020  presentation..  
+00039b10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00039b20: 2020 6469 7374 203d 2064 6973 7420 2f20    dist = dist / 
+00039b30: 7365 6c66 2e63 7574 6f66 660a 2020 2020  self.cutoff.    
+00039b40: 2020 2020 7262 663a 2074 6f72 6368 2e54      rbf: torch.T
+00039b50: 656e 736f 7220 3d20 746f 7263 682e 7374  ensor = torch.st
+00039b60: 6163 6b28 5b66 2864 6973 7429 2066 6f72  ack([f(dist) for
+00039b70: 2066 2069 6e20 7365 6c66 2e62 6573 7365   f in self.besse
+00039b80: 6c5f 6675 6e63 735d 2c0a 2020 2020 2020  l_funcs],.      
+00039b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00039ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039bc0: 2020 2020 2020 6469 6d3d 3129 0a20 2020        dim=1).   
-00039bd0: 2020 2020 206e 3a20 696e 7420 3d20 7365       n: int = se
-00039be0: 6c66 2e6e 756d 5f73 7068 6572 6963 616c  lf.num_spherical
-00039bf0: 0a20 2020 2020 2020 206b 3a20 696e 7420  .        k: int 
-00039c00: 3d20 7365 6c66 2e6e 756d 5f72 6164 6961  = self.num_radia
-00039c10: 6c0a 0a20 2020 2020 2020 206f 7574 7075  l..        outpu
-00039c20: 743a 2074 6f72 6368 2e54 656e 736f 7220  t: torch.Tensor 
-00039c30: 3d20 2872 6266 5b69 6478 5f6b 6a5d 2e76  = (rbf[idx_kj].v
-00039c40: 6965 7728 2d31 2c20 6e2c 206b 2920 2a0a  iew(-1, n, k) *.
+00039bb0: 2020 6469 6d3d 3129 0a20 2020 2020 2020    dim=1).       
+00039bc0: 2072 6266 203d 2073 656c 662e 656e 7665   rbf = self.enve
+00039bd0: 6c6f 7065 2864 6973 7429 2e75 6e73 7175  lope(dist).unsqu
+00039be0: 6565 7a65 282d 3129 202a 2072 6266 0a0a  eeze(-1) * rbf..
+00039bf0: 2020 2020 2020 2020 6362 663a 2074 6f72          cbf: tor
+00039c00: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
+00039c10: 682e 7374 6163 6b28 5b66 2861 6e67 6c65  h.stack([f(angle
+00039c20: 2920 666f 7220 6620 696e 2073 656c 662e  ) for f in self.
+00039c30: 7370 685f 6675 6e63 735d 2c0a 2020 2020  sph_funcs],.    
+00039c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00039c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039c70: 6362 662e 7669 6577 282d 312c 206e 2c20  cbf.view(-1, n, 
-00039c80: 3129 292e 7669 6577 282d 312c 206e 202a  1)).view(-1, n *
-00039c90: 206b 290a 2020 2020 2020 2020 7265 7475   k).        retu
-00039ca0: 726e 206f 7574 7075 740a 0a0a 636c 6173  rn output...clas
-00039cb0: 7320 4869 6768 7761 794c 6179 6572 2874  s HighwayLayer(t
-00039cc0: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 293a  orch.nn.Module):
-00039cd0: 0a20 2020 2022 2222 0a20 2020 2048 6967  .    """.    Hig
-00039ce0: 6877 6179 206c 6179 6572 2066 726f 6d20  hway layer from 
-00039cf0: 2254 7261 696e 696e 6720 5665 7279 2044  "Training Very D
-00039d00: 6565 7020 4e65 7477 6f72 6b73 2220 5b31  eep Networks" [1
-00039d10: 5d0a 0a20 2020 2079 203d 2048 2878 2920  ]..    y = H(x) 
-00039d20: 2a20 5428 7829 202b 2078 202a 2043 2878  * T(x) + x * C(x
-00039d30: 292c 2077 6865 7265 0a0a 2020 2020 4828  ), where..    H(
-00039d40: 7829 3a20 312d 6c61 7965 7220 6e65 7572  x): 1-layer neur
-00039d50: 616c 206e 6574 776f 726b 2077 6974 6820  al network with 
-00039d60: 6e6f 6e2d 6c69 6e65 6172 2061 6374 6976  non-linear activ
-00039d70: 6174 696f 6e0a 2020 2020 5428 7829 3a20  ation.    T(x): 
-00039d80: 312d 6c61 7965 7220 6e65 7572 616c 206e  1-layer neural n
-00039d90: 6574 776f 726b 2077 6974 6820 7369 676d  etwork with sigm
-00039da0: 6f69 6420 6163 7469 7661 7469 6f6e 0a20  oid activation. 
-00039db0: 2020 2043 2858 293a 2031 202d 2054 2858     C(X): 1 - T(X
-00039dc0: 293b 2041 7320 7065 7220 7468 6520 6f72  ); As per the or
-00039dd0: 6967 696e 616c 2070 6170 6572 0a0a 2020  iginal paper..  
-00039de0: 2020 5468 6520 6f75 7470 7574 2077 696c    The output wil
-00039df0: 6c20 6265 206f 6620 7468 6520 7361 6d65  l be of the same
-00039e00: 2064 696d 656e 7369 6f6e 2061 7320 7468   dimension as th
-00039e10: 6520 696e 7075 740a 0a20 2020 2052 6566  e input..    Ref
-00039e20: 6572 656e 6365 730a 2020 2020 2d2d 2d2d  erences.    ----
-00039e30: 2d2d 2d2d 2d2d 0a20 2020 202e 2e20 5b31  ------.    .. [1
-00039e40: 5d20 5372 6976 6173 7461 7661 2065 7420  ] Srivastava et 
-00039e50: 616c 2e2c 2022 5472 6169 6e69 6e67 2056  al., "Training V
-00039e60: 6572 7920 4465 6570 204e 6574 776f 726b  ery Deep Network
-00039e70: 7322 2e68 7474 7073 3a2f 2f61 7278 6976  s".https://arxiv
-00039e80: 2e6f 7267 2f61 6273 2f31 3530 372e 3036  .org/abs/1507.06
-00039e90: 3232 380a 0a20 2020 2045 7861 6d70 6c65  228..    Example
-00039ea0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
-00039eb0: 2020 203e 3e3e 2078 203d 2074 6f72 6368     >>> x = torch
-00039ec0: 2e72 616e 646e 2831 362c 2032 3029 0a20  .randn(16, 20). 
-00039ed0: 2020 203e 3e3e 2068 6967 6877 6179 5f6c     >>> highway_l
-00039ee0: 6179 6572 203d 2048 6967 6877 6179 4c61  ayer = HighwayLa
-00039ef0: 7965 7228 645f 696e 7075 743d 782e 7368  yer(d_input=x.sh
-00039f00: 6170 655b 315d 290a 2020 2020 3e3e 3e20  ape[1]).    >>> 
-00039f10: 7920 3d20 6869 6768 7761 795f 6c61 7965  y = highway_laye
-00039f20: 7228 7829 0a20 2020 203e 3e3e 2078 2e73  r(x).    >>> x.s
-00039f30: 6861 7065 0a20 2020 2074 6f72 6368 2e53  hape.    torch.S
-00039f40: 697a 6528 5b31 362c 2032 305d 290a 2020  ize([16, 20]).  
-00039f50: 2020 3e3e 3e20 792e 7368 6170 650a 2020    >>> y.shape.  
-00039f60: 2020 746f 7263 682e 5369 7a65 285b 3136    torch.Size([16
-00039f70: 2c20 3230 5d29 0a20 2020 2022 2222 0a0a  , 20]).    """..
-00039f80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00039f90: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00039fa0: 2020 2020 2020 2020 645f 696e 7075 743a          d_input:
-00039fb0: 2069 6e74 2c0a 2020 2020 2020 2020 2020   int,.          
-00039fc0: 2020 2020 2020 2061 6374 6976 6174 696f         activatio
-00039fd0: 6e5f 666e 3a20 556e 696f 6e5b 4361 6c6c  n_fn: Union[Call
-00039fe0: 6162 6c65 2c20 7374 725d 203d 2027 7265  able, str] = 're
-00039ff0: 6c75 2729 3a0a 2020 2020 2020 2020 2222  lu'):.        ""
-0003a000: 220a 2020 2020 2020 2020 496e 6974 6961  ".        Initia
-0003a010: 6c69 7a65 7320 7468 6520 4869 6768 7761  lizes the Highwa
-0003a020: 794c 6179 6572 2e0a 0a20 2020 2020 2020  yLayer...       
-0003a030: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0003a040: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0003a050: 2020 2020 2020 2020 2020 2064 5f69 6e70             d_inp
-0003a060: 7574 3a20 696e 740a 2020 2020 2020 2020  ut: int.        
-0003a070: 2020 2020 2020 2020 7468 6520 6469 6d65          the dime
-0003a080: 6e73 696f 6e20 6f66 2074 6865 2069 6e70  nsion of the inp
-0003a090: 7574 206c 6179 6572 0a20 2020 2020 2020  ut layer.       
-0003a0a0: 2020 2020 2061 6374 6976 6174 696f 6e5f       activation_
-0003a0b0: 666e 3a20 7374 720a 2020 2020 2020 2020  fn: str.        
-0003a0c0: 2020 2020 2020 2020 7468 6520 6163 7469          the acti
-0003a0d0: 7661 7469 6f6e 2066 756e 6374 696f 6e20  vation function 
-0003a0e0: 746f 2075 7365 2066 6f72 2048 2878 290a  to use for H(x).
-0003a0f0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0003a100: 2020 2020 2073 7570 6572 2848 6967 6877       super(Highw
-0003a110: 6179 4c61 7965 722c 2073 656c 6629 2e5f  ayLayer, self)._
-0003a120: 5f69 6e69 745f 5f28 290a 2020 2020 2020  _init__().      
-0003a130: 2020 7365 6c66 2e64 5f69 6e70 7574 203d    self.d_input =
-0003a140: 2064 5f69 6e70 7574 0a20 2020 2020 2020   d_input.       
-0003a150: 2073 656c 662e 6163 7469 7661 7469 6f6e   self.activation
-0003a160: 5f66 6e20 3d20 6765 745f 6163 7469 7661  _fn = get_activa
-0003a170: 7469 6f6e 2861 6374 6976 6174 696f 6e5f  tion(activation_
-0003a180: 666e 290a 2020 2020 2020 2020 7365 6c66  fn).        self
-0003a190: 2e73 6967 6d6f 6964 5f66 6e20 3d20 6765  .sigmoid_fn = ge
-0003a1a0: 745f 6163 7469 7661 7469 6f6e 2827 7369  t_activation('si
-0003a1b0: 676d 6f69 6427 290a 0a20 2020 2020 2020  gmoid')..       
-0003a1c0: 2073 656c 662e 4820 3d20 6e6e 2e4c 696e   self.H = nn.Lin
-0003a1d0: 6561 7228 645f 696e 7075 742c 2064 5f69  ear(d_input, d_i
-0003a1e0: 6e70 7574 290a 2020 2020 2020 2020 7365  nput).        se
-0003a1f0: 6c66 2e54 203d 206e 6e2e 4c69 6e65 6172  lf.T = nn.Linear
-0003a200: 2864 5f69 6e70 7574 2c20 645f 696e 7075  (d_input, d_inpu
-0003a210: 7429 0a0a 2020 2020 6465 6620 666f 7277  t)..    def forw
-0003a220: 6172 6428 7365 6c66 2c20 783a 2074 6f72  ard(self, x: tor
-0003a230: 6368 2e54 656e 736f 7229 202d 3e20 746f  ch.Tensor) -> to
-0003a240: 7263 682e 5465 6e73 6f72 3a0a 2020 2020  rch.Tensor:.    
-0003a250: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0003a260: 466f 7277 6172 6420 7061 7373 206f 6620  Forward pass of 
-0003a270: 7468 6520 4869 6768 7761 794c 6179 6572  the HighwayLayer
-0003a280: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0003a290: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-0003a2a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0003a2b0: 2078 3a20 746f 7263 682e 5465 6e73 6f72   x: torch.Tensor
-0003a2c0: 0a20 2020 2020 2020 2020 2020 2049 6e70  .            Inp
-0003a2d0: 7574 2074 656e 736f 7220 6f66 2064 696d  ut tensor of dim
-0003a2e0: 656e 7369 6f6e 2028 2c69 6e70 7574 5f64  ension (,input_d
-0003a2f0: 696d 292e 0a0a 2020 2020 2020 2020 5265  im)...        Re
-0003a300: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-0003a310: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6f75  -----.        ou
-0003a320: 7470 7574 3a20 746f 7263 682e 5465 6e73  tput: torch.Tens
-0003a330: 6f72 0a20 2020 2020 2020 2020 2020 204f  or.            O
-0003a340: 7574 7075 7420 7465 6e73 6f72 206f 6620  utput tensor of 
-0003a350: 6469 6d65 6e73 696f 6e20 282c 696e 7075  dimension (,inpu
-0003a360: 745f 6469 6d29 0a20 2020 2020 2020 2022  t_dim).        "
-0003a370: 2222 0a0a 2020 2020 2020 2020 485f 6f75  ""..        H_ou
-0003a380: 7420 3d20 7365 6c66 2e61 6374 6976 6174  t = self.activat
-0003a390: 696f 6e5f 666e 2873 656c 662e 4828 7829  ion_fn(self.H(x)
-0003a3a0: 290a 2020 2020 2020 2020 545f 6f75 7420  ).        T_out 
-0003a3b0: 3d20 7365 6c66 2e73 6967 6d6f 6964 5f66  = self.sigmoid_f
-0003a3c0: 6e28 7365 6c66 2e54 2878 2929 0a20 2020  n(self.T(x)).   
-0003a3d0: 2020 2020 206f 7574 7075 7420 3d20 485f       output = H_
-0003a3e0: 6f75 7420 2a20 545f 6f75 7420 2b20 7820  out * T_out + x 
-0003a3f0: 2a20 2831 202d 2054 5f6f 7574 290a 0a20  * (1 - T_out).. 
-0003a400: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-0003a410: 7470 7574 0a0a 0a63 6c61 7373 2047 7261  tput...class Gra
-0003a420: 7068 436f 6e76 286e 6e2e 4d6f 6475 6c65  phConv(nn.Module
-0003a430: 293a 0a20 2020 2022 2222 4772 6170 6820  ):.    """Graph 
-0003a440: 436f 6e76 6f6c 7574 696f 6e61 6c20 4c61  Convolutional La
-0003a450: 7965 7273 0a0a 2020 2020 5468 6973 206c  yers..    This l
-0003a460: 6179 6572 2069 6d70 6c65 6d65 6e74 7320  ayer implements 
-0003a470: 7468 6520 6772 6170 6820 636f 6e76 6f6c  the graph convol
-0003a480: 7574 696f 6e20 696e 7472 6f64 7563 6564  ution introduced
-0003a490: 2069 6e20 5b31 5d5f 2e20 2054 6865 2067   in [1]_.  The g
-0003a4a0: 7261 7068 0a20 2020 2063 6f6e 766f 6c75  raph.    convolu
-0003a4b0: 7469 6f6e 2063 6f6d 6269 6e65 7320 7065  tion combines pe
-0003a4c0: 722d 6e6f 6465 2066 6561 7475 7265 2076  r-node feature v
-0003a4d0: 6563 7475 7265 7320 696e 2061 206e 6f6e  ectures in a non
-0003a4e0: 6c69 6e65 6172 2066 6173 6869 6f6e 2077  linear fashion w
-0003a4f0: 6974 680a 2020 2020 7468 6520 6665 6174  ith.    the feat
-0003a500: 7572 6520 7665 6374 6f72 7320 666f 7220  ure vectors for 
-0003a510: 6e65 6967 6862 6f72 696e 6720 6e6f 6465  neighboring node
-0003a520: 732e 2020 5468 6973 2022 626c 656e 6473  s.  This "blends
-0003a530: 2220 696e 666f 726d 6174 696f 6e20 696e  " information in
-0003a540: 0a20 2020 206c 6f63 616c 206e 6569 6768  .    local neigh
-0003a550: 626f 7268 6f6f 6473 206f 6620 6120 6772  borhoods of a gr
-0003a560: 6170 682e 0a0a 2020 2020 4578 616d 706c  aph...    Exampl
-0003a570: 650a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  e.    --------. 
-0003a580: 2020 203e 3e3e 2069 6d70 6f72 7420 6465     >>> import de
-0003a590: 6570 6368 656d 2061 7320 6463 0a20 2020  epchem as dc.   
-0003a5a0: 203e 3e3e 2069 6d70 6f72 7420 6e75 6d70   >>> import nump
-0003a5b0: 7920 6173 206e 700a 2020 2020 3e3e 3e20  y as np.    >>> 
-0003a5c0: 696d 706f 7274 2064 6565 7063 6865 6d2e  import deepchem.
-0003a5d0: 6d6f 6465 6c73 2e74 6f72 6368 5f6d 6f64  models.torch_mod
-0003a5e0: 656c 732e 6c61 7965 7273 2061 7320 746f  els.layers as to
-0003a5f0: 7263 685f 6c61 7965 7273 0a20 2020 203e  rch_layers.    >
-0003a600: 3e3e 206f 7574 5f63 6861 6e6e 656c 7320  >> out_channels 
-0003a610: 3d20 320a 2020 2020 3e3e 3e20 6e5f 6174  = 2.    >>> n_at
-0003a620: 6f6d 7320 3d20 3420 2023 2049 6e20 4343  oms = 4  # In CC
-0003a630: 4320 616e 6420 432c 2074 6865 7265 2061  C and C, there a
-0003a640: 7265 2034 2061 746f 6d73 0a20 2020 203e  re 4 atoms.    >
-0003a650: 3e3e 2072 6177 5f73 6d69 6c65 7320 3d20  >> raw_smiles = 
-0003a660: 5b27 4343 4327 2c20 2743 275d 0a20 2020  ['CCC', 'C'].   
-0003a670: 203e 3e3e 2066 726f 6d20 7264 6b69 7420   >>> from rdkit 
-0003a680: 696d 706f 7274 2043 6865 6d0a 2020 2020  import Chem.    
-0003a690: 3e3e 3e20 6d6f 6c73 203d 205b 4368 656d  >>> mols = [Chem
-0003a6a0: 2e4d 6f6c 4672 6f6d 536d 696c 6573 2873  .MolFromSmiles(s
-0003a6b0: 2920 666f 7220 7320 696e 2072 6177 5f73  ) for s in raw_s
-0003a6c0: 6d69 6c65 735d 0a20 2020 203e 3e3e 2066  miles].    >>> f
-0003a6d0: 6561 7475 7269 7a65 7220 3d20 6463 2e66  eaturizer = dc.f
-0003a6e0: 6561 742e 6772 6170 685f 6665 6174 7572  eat.graph_featur
-0003a6f0: 6573 2e43 6f6e 764d 6f6c 4665 6174 7572  es.ConvMolFeatur
-0003a700: 697a 6572 2829 0a20 2020 203e 3e3e 206d  izer().    >>> m
-0003a710: 6f6c 7320 3d20 6665 6174 7572 697a 6572  ols = featurizer
-0003a720: 2e66 6561 7475 7269 7a65 286d 6f6c 7329  .featurize(mols)
-0003a730: 0a20 2020 203e 3e3e 206d 756c 7469 5f6d  .    >>> multi_m
-0003a740: 6f6c 203d 2064 632e 6665 6174 2e6d 6f6c  ol = dc.feat.mol
-0003a750: 5f67 7261 7068 732e 436f 6e76 4d6f 6c2e  _graphs.ConvMol.
-0003a760: 6167 676c 6f6d 6572 6174 655f 6d6f 6c73  agglomerate_mols
-0003a770: 286d 6f6c 7329 0a20 2020 203e 3e3e 2061  (mols).    >>> a
-0003a780: 746f 6d5f 6665 6174 7572 6573 203d 206d  tom_features = m
-0003a790: 756c 7469 5f6d 6f6c 2e67 6574 5f61 746f  ulti_mol.get_ato
-0003a7a0: 6d5f 6665 6174 7572 6573 2829 2e61 7374  m_features().ast
-0003a7b0: 7970 6528 6e70 2e66 6c6f 6174 3332 290a  ype(np.float32).
-0003a7c0: 2020 2020 3e3e 3e20 6465 6772 6565 5f73      >>> degree_s
-0003a7d0: 6c69 6365 203d 206d 756c 7469 5f6d 6f6c  lice = multi_mol
-0003a7e0: 2e64 6567 5f73 6c69 6365 0a20 2020 203e  .deg_slice.    >
-0003a7f0: 3e3e 206d 656d 6265 7273 6869 7020 3d20  >> membership = 
-0003a800: 6d75 6c74 695f 6d6f 6c2e 6d65 6d62 6572  multi_mol.member
-0003a810: 7368 6970 0a20 2020 203e 3e3e 2064 6567  ship.    >>> deg
-0003a820: 5f61 646a 7320 3d20 6d75 6c74 695f 6d6f  _adjs = multi_mo
-0003a830: 6c2e 6765 745f 6465 675f 6164 6a61 6365  l.get_deg_adjace
-0003a840: 6e63 795f 6c69 7374 7328 295b 313a 5d0a  ncy_lists()[1:].
-0003a850: 2020 2020 3e3e 3e20 6172 6773 203d 205b      >>> args = [
-0003a860: 6174 6f6d 5f66 6561 7475 7265 732c 2064  atom_features, d
-0003a870: 6567 7265 655f 736c 6963 652c 206d 656d  egree_slice, mem
-0003a880: 6265 7273 6869 705d 202b 2064 6567 5f61  bership] + deg_a
-0003a890: 646a 730a 2020 2020 3e3e 3e20 6c61 7965  djs.    >>> laye
-0003a8a0: 7220 3d20 746f 7263 685f 6c61 7965 7273  r = torch_layers
-0003a8b0: 2e47 7261 7068 436f 6e76 286f 7574 5f63  .GraphConv(out_c
-0003a8c0: 6861 6e6e 656c 7329 0a20 2020 203e 3e3e  hannels).    >>>
-0003a8d0: 2072 6573 756c 7420 3d20 6c61 7965 7228   result = layer(
-0003a8e0: 6172 6773 290a 2020 2020 3e3e 3e20 7479  args).    >>> ty
-0003a8f0: 7065 2872 6573 756c 7429 0a20 2020 203c  pe(result).    <
-0003a900: 636c 6173 7320 2774 6f72 6368 2e54 656e  class 'torch.Ten
-0003a910: 736f 7227 3e0a 2020 2020 3e3e 3e20 7265  sor'>.    >>> re
-0003a920: 7375 6c74 2e73 6861 7065 0a20 2020 2074  sult.shape.    t
-0003a930: 6f72 6368 2e53 697a 6528 5b34 2c20 325d  orch.Size([4, 2]
-0003a940: 290a 2020 2020 3e3e 3e20 6e75 6d5f 6465  ).    >>> num_de
-0003a950: 6720 3d20 3220 2a20 6c61 7965 722e 6d61  g = 2 * layer.ma
-0003a960: 785f 6465 6772 6565 202b 2028 3120 2d20  x_degree + (1 - 
-0003a970: 6c61 7965 722e 6d69 6e5f 6465 6772 6565  layer.min_degree
-0003a980: 290a 2020 2020 3e3e 3e20 6e75 6d5f 6465  ).    >>> num_de
-0003a990: 670a 2020 2020 3231 0a0a 2020 2020 5265  g.    21..    Re
-0003a9a0: 6665 7265 6e63 6573 0a20 2020 202d 2d2d  ferences.    ---
-0003a9b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e 205b  -------.    .. [
-0003a9c0: 315d 2044 7576 656e 6175 642c 2044 6176  1] Duvenaud, Dav
-0003a9d0: 6964 204b 2e2c 2065 7420 616c 2e20 2243  id K., et al. "C
-0003a9e0: 6f6e 766f 6c75 7469 6f6e 616c 206e 6574  onvolutional net
-0003a9f0: 776f 726b 7320 6f6e 2067 7261 7068 7320  works on graphs 
-0003aa00: 666f 7220 6c65 6172 6e69 6e67 206d 6f6c  for learning mol
-0003aa10: 6563 756c 6172 2066 696e 6765 7270 7269  ecular fingerpri
-0003aa20: 6e74 732e 220a 2020 2020 2020 2020 4164  nts.".        Ad
-0003aa30: 7661 6e63 6573 2069 6e20 6e65 7572 616c  vances in neural
-0003aa40: 2069 6e66 6f72 6d61 7469 6f6e 2070 726f   information pro
-0003aa50: 6365 7373 696e 6720 7379 7374 656d 732e  cessing systems.
-0003aa60: 2032 3031 352e 2068 7474 7073 3a2f 2f61   2015. https://a
-0003aa70: 7278 6976 2e6f 7267 2f61 6273 2f31 3530  rxiv.org/abs/150
-0003aa80: 392e 3039 3239 320a 0a20 2022 2222 0a0a  9.09292..  """..
-0003aa90: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0003aaa0: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-0003aab0: 2020 2020 2020 2020 6f75 745f 6368 616e          out_chan
-0003aac0: 6e65 6c3a 2069 6e74 2c0a 2020 2020 2020  nel: int,.      
-0003aad0: 2020 2020 2020 2020 2020 206d 696e 5f64             min_d
-0003aae0: 6567 3a20 696e 7420 3d20 302c 0a20 2020  eg: int = 0,.   
-0003aaf0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0003ab00: 785f 6465 673a 2069 6e74 203d 2031 302c  x_deg: int = 10,
-0003ab10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003ab20: 2020 6163 7469 7661 7469 6f6e 5f66 6e3a    activation_fn:
-0003ab30: 204f 7074 696f 6e61 6c5b 4361 6c6c 6162   Optional[Callab
-0003ab40: 6c65 5d20 3d20 4e6f 6e65 2c0a 2020 2020  le] = None,.    
-0003ab50: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
-0003ab60: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-0003ab70: 2222 2249 6e69 7469 616c 697a 6520 6120  """Initialize a 
-0003ab80: 6772 6170 6820 636f 6e76 6f6c 7574 696f  graph convolutio
-0003ab90: 6e61 6c20 6c61 7965 722e 0a0a 2020 2020  nal layer...    
-0003aba0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0003abb0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0003abc0: 2d0a 2020 2020 2020 2020 6f75 745f 6368  -.        out_ch
-0003abd0: 616e 6e65 6c3a 2069 6e74 0a20 2020 2020  annel: int.     
-0003abe0: 2020 2020 2020 2054 6865 206e 756d 6265         The numbe
-0003abf0: 7220 6f66 206f 7574 7075 7420 6368 616e  r of output chan
-0003ac00: 6e65 6c73 2070 6572 2067 7261 7068 206e  nels per graph n
-0003ac10: 6f64 652e 0a20 2020 2020 2020 206d 696e  ode..        min
-0003ac20: 5f64 6567 3a20 696e 742c 206f 7074 696f  _deg: int, optio
-0003ac30: 6e61 6c20 2864 6566 6175 6c74 2030 290a  nal (default 0).
-0003ac40: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0003ac50: 6d69 6e69 6d75 6d20 616c 6c6f 7765 6420  minimum allowed 
-0003ac60: 6465 6772 6565 2066 6f72 2065 6163 6820  degree for each 
-0003ac70: 6772 6170 6820 6e6f 6465 2e0a 2020 2020  graph node..    
-0003ac80: 2020 2020 6d61 785f 6465 673a 2069 6e74      max_deg: int
-0003ac90: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
-0003aca0: 756c 7420 3130 290a 2020 2020 2020 2020  ult 10).        
-0003acb0: 2020 2020 5468 6520 6d61 7869 6d75 6d20      The maximum 
-0003acc0: 616c 6c6f 7765 6420 6465 6772 6565 2066  allowed degree f
-0003acd0: 6f72 2065 6163 6820 6772 6170 6820 6e6f  or each graph no
-0003ace0: 6465 2e20 4e6f 7465 2074 6861 7420 7468  de. Note that th
-0003acf0: 6973 0a20 2020 2020 2020 2020 2020 2069  is.            i
-0003ad00: 7320 7365 7420 746f 2031 3020 746f 2068  s set to 10 to h
-0003ad10: 616e 646c 6520 636f 6d70 6c65 7820 6d6f  andle complex mo
-0003ad20: 6c65 6375 6c65 7320 2873 6f6d 6520 6f72  lecules (some or
-0003ad30: 6761 6e6f 6d65 7461 6c6c 6963 0a20 2020  ganometallic.   
-0003ad40: 2020 2020 2020 2020 2063 6f6d 706f 756e           compoun
-0003ad50: 6473 2068 6176 6520 7374 7261 6e67 6520  ds have strange 
-0003ad60: 7374 7275 6374 7572 6573 292e 2049 6620  structures). If 
-0003ad70: 796f 7527 7265 2075 7369 6e67 2074 6869  you're using thi
-0003ad80: 7320 666f 720a 2020 2020 2020 2020 2020  s for.          
-0003ad90: 2020 6e6f 6e2d 6d6f 6c65 6375 6c61 7220    non-molecular 
-0003ada0: 6170 706c 6963 6174 696f 6e73 2c20 796f  applications, yo
-0003adb0: 7520 6d61 7920 6e65 6564 2074 6f20 7365  u may need to se
-0003adc0: 7420 7468 6973 206d 7563 6820 6869 6768  t this much high
-0003add0: 6572 0a20 2020 2020 2020 2020 2020 2064  er.            d
-0003ade0: 6570 656e 6469 6e67 206f 6e20 796f 7572  epending on your
-0003adf0: 2064 6174 6173 6574 2e0a 2020 2020 2020   dataset..      
-0003ae00: 2020 6163 7469 7661 7469 6f6e 5f66 6e3a    activation_fn:
-0003ae10: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
-0003ae20: 2020 2020 2020 4120 6e6f 6e6c 696e 6561        A nonlinea
-0003ae30: 7220 6163 7469 7661 7469 6f6e 2066 756e  r activation fun
-0003ae40: 6374 696f 6e20 746f 2061 7070 6c79 2e20  ction to apply. 
-0003ae50: 4966 2079 6f75 2772 6520 6e6f 7420 7375  If you're not su
-0003ae60: 7265 2c0a 2020 2020 2020 2020 2020 2020  re,.            
-0003ae70: 6074 6f72 6368 2e6e 6e2e 5265 4c55 6020  `torch.nn.ReLU` 
-0003ae80: 6973 2070 726f 6261 626c 7920 6120 676f  is probably a go
-0003ae90: 6f64 2064 6566 6175 6c74 2066 6f72 2079  od default for y
-0003aea0: 6f75 7220 6170 706c 6963 6174 696f 6e2e  our application.
-0003aeb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0003aec0: 2020 2020 2073 7570 6572 2847 7261 7068       super(Graph
-0003aed0: 436f 6e76 2c20 7365 6c66 292e 5f5f 696e  Conv, self).__in
-0003aee0: 6974 5f5f 282a 2a6b 7761 7267 7329 0a20  it__(**kwargs). 
-0003aef0: 2020 2020 2020 2073 656c 662e 6f75 745f         self.out_
-0003af00: 6368 616e 6e65 6c3a 2069 6e74 203d 206f  channel: int = o
-0003af10: 7574 5f63 6861 6e6e 656c 0a20 2020 2020  ut_channel.     
-0003af20: 2020 2073 656c 662e 6d69 6e5f 6465 6772     self.min_degr
-0003af30: 6565 3a20 696e 7420 3d20 6d69 6e5f 6465  ee: int = min_de
-0003af40: 670a 2020 2020 2020 2020 7365 6c66 2e6d  g.        self.m
-0003af50: 6178 5f64 6567 7265 653a 2069 6e74 203d  ax_degree: int =
-0003af60: 206d 6178 5f64 6567 0a20 2020 2020 2020   max_deg.       
-0003af70: 2073 656c 662e 6163 7469 7661 7469 6f6e   self.activation
-0003af80: 5f66 6e3a 204f 7074 696f 6e61 6c5b 4361  _fn: Optional[Ca
-0003af90: 6c6c 6162 6c65 5d20 3d20 6163 7469 7661  llable] = activa
-0003afa0: 7469 6f6e 5f66 6e0a 0a20 2020 2020 2020  tion_fn..       
-0003afb0: 2023 2047 656e 6572 6174 6520 7468 6520   # Generate the 
-0003afc0: 6e62 5f61 6666 696e 6520 7765 6967 6874  nb_affine weight
-0003afd0: 7320 616e 6420 6269 6173 6573 0a20 2020  s and biases.   
-0003afe0: 2020 2020 206e 756d 5f64 6567 3a20 696e       num_deg: in
-0003aff0: 7420 3d20 3220 2a20 7365 6c66 2e6d 6178  t = 2 * self.max
-0003b000: 5f64 6567 7265 6520 2b20 2831 202d 2073  _degree + (1 - s
-0003b010: 656c 662e 6d69 6e5f 6465 6772 6565 290a  elf.min_degree).
-0003b020: 2020 2020 2020 2020 7365 6c66 2e57 5f6c          self.W_l
-0003b030: 6973 743a 206e 6e2e 5061 7261 6d65 7465  ist: nn.Paramete
-0003b040: 724c 6973 7420 3d20 6e6e 2e50 6172 616d  rList = nn.Param
-0003b050: 6574 6572 4c69 7374 285b 0a20 2020 2020  eterList([.     
-0003b060: 2020 2020 2020 206e 6e2e 5061 7261 6d65         nn.Parame
-0003b070: 7465 7228 0a20 2020 2020 2020 2020 2020  ter(.           
-0003b080: 2020 2020 2067 6574 6174 7472 2869 6e69       getattr(ini
-0003b090: 7469 616c 697a 6572 732c 0a20 2020 2020  tializers,.     
-0003b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003b0b0: 2020 2027 7861 7669 6572 5f75 6e69 666f     'xavier_unifo
-0003b0c0: 726d 5f27 2928 746f 7263 682e 656d 7074  rm_')(torch.empt
-0003b0d0: 7928 3735 2c20 7365 6c66 2e6f 7574 5f63  y(75, self.out_c
-0003b0e0: 6861 6e6e 656c 2929 290a 2020 2020 2020  hannel))).      
-0003b0f0: 2020 2020 2020 666f 7220 6b20 696e 2072        for k in r
-0003b100: 616e 6765 286e 756d 5f64 6567 290a 2020  ange(num_deg).  
-0003b110: 2020 2020 2020 5d29 0a20 2020 2020 2020        ]).       
-0003b120: 2073 656c 662e 625f 6c69 7374 3a20 6e6e   self.b_list: nn
-0003b130: 2e50 6172 616d 6574 6572 4c69 7374 203d  .ParameterList =
-0003b140: 206e 6e2e 5061 7261 6d65 7465 724c 6973   nn.ParameterLis
-0003b150: 7428 5b0a 2020 2020 2020 2020 2020 2020  t([.            
-0003b160: 6e6e 2e50 6172 616d 6574 6572 280a 2020  nn.Parameter(.  
-0003b170: 2020 2020 2020 2020 2020 2020 2020 6765                ge
-0003b180: 7461 7474 7228 696e 6974 6961 6c69 7a65  tattr(initialize
-0003b190: 7273 2c20 277a 6572 6f73 5f27 2928 746f  rs, 'zeros_')(to
-0003b1a0: 7263 682e 656d 7074 7928 7365 6c66 2e6f  rch.empty(self.o
-0003b1b0: 7574 5f63 6861 6e6e 656c 2c29 2929 0a20  ut_channel,))). 
-0003b1c0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0003b1d0: 2069 6e20 7261 6e67 6528 6e75 6d5f 6465   in range(num_de
-0003b1e0: 6729 0a20 2020 2020 2020 205d 290a 2020  g).        ]).  
-0003b1f0: 2020 2020 2020 7365 6c66 2e62 7569 6c74        self.built
-0003b200: 203d 2054 7275 650a 0a20 2020 2064 6566   = True..    def
-0003b210: 205f 5f72 6570 725f 5f28 7365 6c66 2920   __repr__(self) 
-0003b220: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-0003b230: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
-0003b240: 726e 7320 6120 7374 7269 6e67 2072 6570  rns a string rep
-0003b250: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
-0003b260: 6865 206f 626a 6563 742e 0a0a 2020 2020  he object...    
-0003b270: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0003b280: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0003b290: 2020 2020 2073 7472 3a20 4120 7374 7269       str: A stri
-0003b2a0: 6e67 2074 6861 7420 636f 6e74 6169 6e73  ng that contains
-0003b2b0: 2074 6865 2063 6c61 7373 206e 616d 6520   the class name 
-0003b2c0: 666f 6c6c 6f77 6564 2062 7920 7468 6520  followed by the 
-0003b2d0: 7661 6c75 6573 206f 6620 6974 7320 696e  values of its in
-0003b2e0: 7374 616e 6365 2076 6172 6961 626c 652e  stance variable.
-0003b2f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0003b300: 2020 2020 2023 2066 6c61 6b65 383a 206e       # flake8: n
-0003b310: 6f71 610a 2020 2020 2020 2020 7265 7475  oqa.        retu
-0003b320: 726e 2028 0a20 2020 2020 2020 2020 2020  rn (.           
-0003b330: 2066 277b 7365 6c66 2e5f 5f63 6c61 7373   f'{self.__class
-0003b340: 5f5f 2e5f 5f6e 616d 655f 5f7d 286f 7574  __.__name__}(out
-0003b350: 5f63 6861 6e6e 656c 3a7b 7365 6c66 2e6f  _channel:{self.o
-0003b360: 7574 5f63 6861 6e6e 656c 7d2c 6d69 6e5f  ut_channel},min_
-0003b370: 6465 673a 7b73 656c 662e 6d69 6e5f 6465  deg:{self.min_de
-0003b380: 677d 2c6d 6178 5f64 6567 3a7b 7365 6c66  g},max_deg:{self
-0003b390: 2e6d 6178 5f64 6567 7d2c 6163 7469 7661  .max_deg},activa
-0003b3a0: 7469 6f6e 5f66 6e3a 7b73 656c 662e 6163  tion_fn:{self.ac
-0003b3b0: 7469 7661 7469 6f6e 5f66 6e7d 2927 0a20  tivation_fn})'. 
-0003b3c0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0003b3d0: 6620 666f 7277 6172 6428 7365 6c66 2c20  f forward(self, 
-0003b3e0: 696e 7075 7473 3a20 4c69 7374 5b6e 702e  inputs: List[np.
-0003b3f0: 6e64 6172 7261 795d 2920 2d3e 2074 6f72  ndarray]) -> tor
-0003b400: 6368 2e54 656e 736f 723a 0a20 2020 2020  ch.Tensor:.     
-0003b410: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
-0003b420: 6865 2066 6f72 7761 7264 2070 6173 7320  he forward pass 
-0003b430: 636f 6d62 696e 6573 2070 6572 2d6e 6f64  combines per-nod
-0003b440: 6520 6665 6174 7572 6520 7665 6374 6f72  e feature vector
-0003b450: 7320 696e 2061 206e 6f6e 6c69 6e65 6172  s in a nonlinear
-0003b460: 2066 6173 6869 6f6e 2077 6974 680a 2020   fashion with.  
-0003b470: 2020 2020 2020 7468 6520 6665 6174 7572        the featur
-0003b480: 6520 7665 6374 6f72 7320 666f 7220 6e65  e vectors for ne
-0003b490: 6967 6862 6f72 696e 6720 6e6f 6465 732e  ighboring nodes.
-0003b4a0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0003b4b0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0003b4c0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2069  ------.        i
-0003b4d0: 6e70 7574 733a 204c 6973 745b 6e70 2e6e  nputs: List[np.n
-0003b4e0: 6461 7272 6179 5d0a 2020 2020 2020 2020  darray].        
-0003b4f0: 5368 6f75 6c64 2063 6f6e 7461 696e 2061  Should contain a
-0003b500: 746f 6d20 6665 6174 7572 6573 2061 6e64  tom features and
-0003b510: 2061 7272 6179 7320 6465 7363 7269 6269   arrays describi
-0003b520: 6e67 2067 7261 7068 2074 6f70 6f6c 6f67  ng graph topolog
-0003b530: 790a 2020 2020 2020 2020 5265 7475 726e  y.        Return
-0003b540: 733a 0a20 2020 2020 2020 202d 2d2d 2d2d  s:.        -----
-0003b550: 2d2d 0a20 2020 2020 2020 2074 6f72 6368  --.        torch
-0003b560: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
-0003b570: 2020 436f 6d62 696e 6564 2061 746f 6d20    Combined atom 
-0003b580: 6665 6174 7572 6573 0a20 2020 2020 2020  features.       
-0003b590: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
-0003b5a0: 4578 7472 6163 7420 6174 6f6d 5f66 6561  Extract atom_fea
-0003b5b0: 7475 7265 730a 2020 2020 2020 2020 6174  tures.        at
-0003b5c0: 6f6d 5f66 6561 7475 7265 733a 2074 6f72  om_features: tor
-0003b5d0: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
-0003b5e0: 682e 7465 6e73 6f72 2869 6e70 7574 735b  h.tensor(inputs[
-0003b5f0: 305d 290a 0a20 2020 2020 2020 2023 2045  0])..        # E
-0003b600: 7874 7261 6374 2067 7261 7068 2074 6f70  xtract graph top
-0003b610: 6f6c 6f67 790a 2020 2020 2020 2020 6465  ology.        de
-0003b620: 675f 736c 6963 653a 206e 702e 6e64 6172  g_slice: np.ndar
-0003b630: 7261 7920 3d20 696e 7075 7473 5b31 5d0a  ray = inputs[1].
-0003b640: 2020 2020 2020 2020 6465 675f 6164 6a5f          deg_adj_
-0003b650: 6c69 7374 733a 204c 6973 745b 6e70 2e6e  lists: List[np.n
-0003b660: 6461 7272 6179 5d20 3d20 696e 7075 7473  darray] = inputs
-0003b670: 5b33 3a5d 0a0a 2020 2020 2020 2020 5720  [3:]..        W 
-0003b680: 3d20 6974 6572 2873 656c 662e 575f 6c69  = iter(self.W_li
-0003b690: 7374 290a 2020 2020 2020 2020 6220 3d20  st).        b = 
-0003b6a0: 6974 6572 2873 656c 662e 625f 6c69 7374  iter(self.b_list
-0003b6b0: 290a 0a20 2020 2020 2020 2023 2053 756d  )..        # Sum
-0003b6c0: 2061 6c6c 206e 6569 6768 626f 7273 2075   all neighbors u
-0003b6d0: 7369 6e67 2061 646a 6163 656e 6379 206d  sing adjacency m
-0003b6e0: 6174 7269 780a 2020 2020 2020 2020 6465  atrix.        de
-0003b6f0: 675f 7375 6d6d 6564 3a20 4c69 7374 5b6e  g_summed: List[n
-0003b700: 702e 6e64 6172 7261 795d 203d 2073 656c  p.ndarray] = sel
-0003b710: 662e 7375 6d5f 6e65 6967 6828 6174 6f6d  f.sum_neigh(atom
-0003b720: 5f66 6561 7475 7265 732c 0a20 2020 2020  _features,.     
-0003b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003b760: 2064 6567 5f61 646a 5f6c 6973 7473 290a   deg_adj_lists).
-0003b770: 0a20 2020 2020 2020 2023 2047 6574 2063  .        # Get c
-0003b780: 6f6c 6c65 6374 696f 6e20 6f66 206d 6f64  ollection of mod
-0003b790: 6966 6965 6420 6174 6f6d 2066 6561 7475  ified atom featu
-0003b7a0: 7265 730a 2020 2020 2020 2020 6e65 775f  res.        new_
-0003b7b0: 7265 6c5f 6174 6f6d 735f 636f 6c6c 6563  rel_atoms_collec
-0003b7c0: 7469 6f6e 203d 205b 5d0a 0a20 2020 2020  tion = []..     
-0003b7d0: 2020 2073 706c 6974 5f66 6561 7475 7265     split_feature
-0003b7e0: 733a 2054 7570 6c65 5b74 6f72 6368 2e54  s: Tuple[torch.T
-0003b7f0: 656e 736f 722c 0a20 2020 2020 2020 2020  ensor,.         
-0003b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003b810: 2020 2020 202e 2e2e 5d20 3d20 746f 7263       ...] = torc
-0003b820: 682e 7370 6c69 7428 6174 6f6d 5f66 6561  h.split(atom_fea
-0003b830: 7475 7265 732c 0a20 2020 2020 2020 2020  tures,.         
-0003b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003b860: 2020 2020 2020 2020 2864 6567 5f73 6c69          (deg_sli
-0003b870: 6365 5b3a 2c20 315d 292e 746f 6c69 7374  ce[:, 1]).tolist
-0003b880: 2829 290a 2020 2020 2020 2020 666f 7220  ()).        for 
-0003b890: 6465 6720 696e 2072 616e 6765 2831 2c20  deg in range(1, 
-0003b8a0: 7365 6c66 2e6d 6178 5f64 6567 7265 6520  self.max_degree 
-0003b8b0: 2b20 3129 3a0a 2020 2020 2020 2020 2020  + 1):.          
-0003b8c0: 2020 2320 4f62 7461 696e 2072 656c 6576    # Obtain relev
-0003b8d0: 616e 7420 6174 6f6d 7320 666f 7220 7468  ant atoms for th
-0003b8e0: 6973 2064 6567 7265 650a 2020 2020 2020  is degree.      
-0003b8f0: 2020 2020 2020 7265 6c5f 6174 6f6d 733a        rel_atoms:
-0003b900: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
-0003b910: 746f 7263 682e 6672 6f6d 5f6e 756d 7079  torch.from_numpy
-0003b920: 2864 6567 5f73 756d 6d65 645b 6465 6720  (deg_summed[deg 
-0003b930: 2d20 315d 290a 0a20 2020 2020 2020 2020  - 1])..         
-0003b940: 2020 2023 2047 6574 2073 656c 6620 6174     # Get self at
-0003b950: 6f6d 730a 2020 2020 2020 2020 2020 2020  oms.            
-0003b960: 7365 6c66 5f61 746f 6d73 3a20 746f 7263  self_atoms: torc
-0003b970: 682e 5465 6e73 6f72 203d 2073 706c 6974  h.Tensor = split
-0003b980: 5f66 6561 7475 7265 735b 6465 6720 2d20  _features[deg - 
-0003b990: 7365 6c66 2e6d 696e 5f64 6567 7265 655d  self.min_degree]
-0003b9a0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0003b9b0: 4170 706c 7920 6869 6464 656e 2061 6666  Apply hidden aff
-0003b9c0: 696e 6520 746f 2072 656c 6576 616e 7420  ine to relevant 
-0003b9d0: 6174 6f6d 7320 616e 6420 6170 7065 6e64  atoms and append
-0003b9e0: 0a20 2020 2020 2020 2020 2020 2072 656c  .            rel
-0003b9f0: 5f6f 7574 3a20 746f 7263 682e 5465 6e73  _out: torch.Tens
-0003ba00: 6f72 203d 2074 6f72 6368 2e6d 6174 6d75  or = torch.matmu
-0003ba10: 6c28 7265 6c5f 6174 6f6d 732e 7479 7065  l(rel_atoms.type
-0003ba20: 2874 6f72 6368 2e66 6c6f 6174 3332 292c  (torch.float32),
-0003ba30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003ba60: 2020 6e65 7874 2857 2929 202b 206e 6578    next(W)) + nex
-0003ba70: 7428 6229 0a20 2020 2020 2020 2020 2020  t(b).           
-0003ba80: 2073 656c 665f 6f75 743a 2074 6f72 6368   self_out: torch
-0003ba90: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
-0003baa0: 6d61 746d 756c 280a 2020 2020 2020 2020  matmul(.        
-0003bab0: 2020 2020 2020 2020 7365 6c66 5f61 746f          self_ato
-0003bac0: 6d73 2e74 7970 6528 746f 7263 682e 666c  ms.type(torch.fl
-0003bad0: 6f61 7433 3229 2c20 6e65 7874 2857 2929  oat32), next(W))
-0003bae0: 202b 206e 6578 7428 6229 0a20 2020 2020   + next(b).     
-0003baf0: 2020 2020 2020 206f 7574 3a20 746f 7263         out: torc
-0003bb00: 682e 5465 6e73 6f72 203d 2072 656c 5f6f  h.Tensor = rel_o
-0003bb10: 7574 202b 2073 656c 665f 6f75 740a 2020  ut + self_out.  
-0003bb20: 2020 2020 2020 2020 2020 6e65 775f 7265            new_re
-0003bb30: 6c5f 6174 6f6d 735f 636f 6c6c 6563 7469  l_atoms_collecti
-0003bb40: 6f6e 2e61 7070 656e 6428 0a20 2020 2020  on.append(.     
-0003bb50: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
-0003bb60: 2e66 726f 6d5f 6e75 6d70 7928 6f75 742e  .from_numpy(out.
-0003bb70: 6465 7461 6368 2829 2e6e 756d 7079 2829  detach().numpy()
-0003bb80: 2929 0a0a 2020 2020 2020 2020 2320 4465  ))..        # De
-0003bb90: 7465 726d 696e 6520 7468 6520 6d69 6e5f  termine the min_
-0003bba0: 6465 673d 3020 6361 7365 0a20 2020 2020  deg=0 case.     
-0003bbb0: 2020 2069 6620 7365 6c66 2e6d 696e 5f64     if self.min_d
-0003bbc0: 6567 7265 6520 3d3d 2030 3a0a 2020 2020  egree == 0:.    
-0003bbd0: 2020 2020 2020 2020 7365 6c66 5f61 746f          self_ato
-0003bbe0: 6d73 203d 2073 706c 6974 5f66 6561 7475  ms = split_featu
-0003bbf0: 7265 735b 305d 0a0a 2020 2020 2020 2020  res[0]..        
-0003bc00: 2020 2020 2320 4f6e 6c79 2075 7365 2074      # Only use t
-0003bc10: 6865 2073 656c 6620 6c61 7965 720a 2020  he self layer.  
-0003bc20: 2020 2020 2020 2020 2020 6f75 7420 3d20            out = 
-0003bc30: 746f 7263 682e 6d61 746d 756c 2873 656c  torch.matmul(sel
-0003bc40: 665f 6174 6f6d 732e 7479 7065 2874 6f72  f_atoms.type(tor
-0003bc50: 6368 2e66 6c6f 6174 3332 292c 0a20 2020  ch.float32),.   
-0003bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003bc70: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-0003bc80: 2857 2929 202b 206e 6578 7428 6229 0a20  (W)) + next(b). 
-0003bc90: 2020 2020 2020 2020 2020 206e 6577 5f72             new_r
-0003bca0: 656c 5f61 746f 6d73 5f63 6f6c 6c65 6374  el_atoms_collect
-0003bcb0: 696f 6e2e 696e 7365 7274 280a 2020 2020  ion.insert(.    
-0003bcc0: 2020 2020 2020 2020 2020 2020 302c 2074              0, t
-0003bcd0: 6f72 6368 2e66 726f 6d5f 6e75 6d70 7928  orch.from_numpy(
-0003bce0: 6f75 742e 6465 7461 6368 2829 2e6e 756d  out.detach().num
-0003bcf0: 7079 2829 2929 0a0a 2020 2020 2020 2020  py()))..        
-0003bd00: 2320 436f 6d62 696e 6520 616c 6c20 6174  # Combine all at
-0003bd10: 6f6d 7320 6261 636b 2069 6e74 6f20 7468  oms back into th
-0003bd20: 6520 6c69 7374 0a20 2020 2020 2020 2061  e list.        a
-0003bd30: 746f 6d5f 6665 6174 7572 6573 203d 2074  tom_features = t
-0003bd40: 6f72 6368 2e63 6f6e 6361 7428 6e65 775f  orch.concat(new_
-0003bd50: 7265 6c5f 6174 6f6d 735f 636f 6c6c 6563  rel_atoms_collec
-0003bd60: 7469 6f6e 2c20 3029 0a0a 2020 2020 2020  tion, 0)..      
-0003bd70: 2020 6966 2073 656c 662e 6163 7469 7661    if self.activa
-0003bd80: 7469 6f6e 5f66 6e20 6973 206e 6f74 204e  tion_fn is not N
-0003bd90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003bda0: 2061 746f 6d5f 6665 6174 7572 6573 203d   atom_features =
-0003bdb0: 2073 656c 662e 6163 7469 7661 7469 6f6e   self.activation
-0003bdc0: 5f66 6e28 6174 6f6d 5f66 6561 7475 7265  _fn(atom_feature
-0003bdd0: 7329 0a0a 2020 2020 2020 2020 7265 7475  s)..        retu
-0003bde0: 726e 2061 746f 6d5f 6665 6174 7572 6573  rn atom_features
-0003bdf0: 0a0a 2020 2020 6465 6620 7375 6d5f 6e65  ..    def sum_ne
-0003be00: 6967 6828 7365 6c66 2c20 6174 6f6d 733a  igh(self, atoms:
-0003be10: 2074 6f72 6368 2e54 656e 736f 722c 2064   torch.Tensor, d
-0003be20: 6567 5f61 646a 5f6c 6973 7473 2920 2d3e  eg_adj_lists) ->
-0003be30: 204c 6973 745b 6e70 2e6e 6461 7272 6179   List[np.ndarray
-0003be40: 5d3a 0a20 2020 2020 2020 2022 2222 5374  ]:.        """St
-0003be50: 6f72 6520 7468 6520 7375 6d6d 6564 2061  ore the summed a
-0003be60: 746f 6d73 2062 7920 6465 6772 6565 2222  toms by degree""
-0003be70: 220a 2020 2020 2020 2020 6465 675f 7375  ".        deg_su
-0003be80: 6d6d 6564 203d 205b 5d0a 0a20 2020 2020  mmed = []..     
-0003be90: 2020 2066 6f72 2064 6567 2069 6e20 7261     for deg in ra
-0003bea0: 6e67 6528 312c 2073 656c 662e 6d61 785f  nge(1, self.max_
-0003beb0: 6465 6772 6565 202b 2031 293a 0a20 2020  degree + 1):.   
-0003bec0: 2020 2020 2020 2020 2067 6174 6865 7265           gathere
-0003bed0: 645f 6174 6f6d 733a 2074 6f72 6368 2e54  d_atoms: torch.T
-0003bee0: 656e 736f 7220 3d20 6174 6f6d 735b 6465  ensor = atoms[de
-0003bef0: 675f 6164 6a5f 6c69 7374 735b 6465 6720  g_adj_lists[deg 
-0003bf00: 2d20 315d 5d0a 2020 2020 2020 2020 2020  - 1]].          
-0003bf10: 2020 2320 5375 6d20 616c 6f6e 6720 6e65    # Sum along ne
-0003bf20: 6967 6862 6f72 7320 6173 2077 656c 6c20  ighbors as well 
-0003bf30: 6173 2073 656c 662c 2061 6e64 2073 746f  as self, and sto
-0003bf40: 7265 0a20 2020 2020 2020 2020 2020 2073  re.            s
-0003bf50: 756d 6d65 645f 6174 6f6d 733a 2074 6f72  ummed_atoms: tor
-0003bf60: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
-0003bf70: 682e 7375 6d28 6761 7468 6572 6564 5f61  h.sum(gathered_a
-0003bf80: 746f 6d73 2c20 3129 0a20 2020 2020 2020  toms, 1).       
-0003bf90: 2020 2020 2064 6567 5f73 756d 6d65 642e       deg_summed.
-0003bfa0: 6170 7065 6e64 2873 756d 6d65 645f 6174  append(summed_at
-0003bfb0: 6f6d 732e 6465 7461 6368 2829 2e6e 756d  oms.detach().num
-0003bfc0: 7079 2829 290a 0a20 2020 2020 2020 2072  py())..        r
-0003bfd0: 6574 7572 6e20 6465 675f 7375 6d6d 6564  eturn deg_summed
-0003bfe0: 0a                                       .
+00039c60: 2020 2020 6469 6d3d 3129 0a20 2020 2020      dim=1).     
+00039c70: 2020 206e 3a20 696e 7420 3d20 7365 6c66     n: int = self
+00039c80: 2e6e 756d 5f73 7068 6572 6963 616c 0a20  .num_spherical. 
+00039c90: 2020 2020 2020 206b 3a20 696e 7420 3d20         k: int = 
+00039ca0: 7365 6c66 2e6e 756d 5f72 6164 6961 6c0a  self.num_radial.
+00039cb0: 0a20 2020 2020 2020 206f 7574 7075 743a  .        output:
+00039cc0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+00039cd0: 2872 6266 5b69 6478 5f6b 6a5d 2e76 6965  (rbf[idx_kj].vie
+00039ce0: 7728 2d31 2c20 6e2c 206b 2920 2a0a 2020  w(-1, n, k) *.  
+00039cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039d00: 2020 2020 2020 2020 2020 2020 2020 6362                cb
+00039d10: 662e 7669 6577 282d 312c 206e 2c20 3129  f.view(-1, n, 1)
+00039d20: 292e 7669 6577 282d 312c 206e 202a 206b  ).view(-1, n * k
+00039d30: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00039d40: 206f 7574 7075 740a 0a0a 636c 6173 7320   output...class 
+00039d50: 4869 6768 7761 794c 6179 6572 2874 6f72  HighwayLayer(tor
+00039d60: 6368 2e6e 6e2e 4d6f 6475 6c65 293a 0a20  ch.nn.Module):. 
+00039d70: 2020 2022 2222 0a20 2020 2048 6967 6877     """.    Highw
+00039d80: 6179 206c 6179 6572 2066 726f 6d20 2254  ay layer from "T
+00039d90: 7261 696e 696e 6720 5665 7279 2044 6565  raining Very Dee
+00039da0: 7020 4e65 7477 6f72 6b73 2220 5b31 5d0a  p Networks" [1].
+00039db0: 0a20 2020 2079 203d 2048 2878 2920 2a20  .    y = H(x) * 
+00039dc0: 5428 7829 202b 2078 202a 2043 2878 292c  T(x) + x * C(x),
+00039dd0: 2077 6865 7265 0a0a 2020 2020 4828 7829   where..    H(x)
+00039de0: 3a20 312d 6c61 7965 7220 6e65 7572 616c  : 1-layer neural
+00039df0: 206e 6574 776f 726b 2077 6974 6820 6e6f   network with no
+00039e00: 6e2d 6c69 6e65 6172 2061 6374 6976 6174  n-linear activat
+00039e10: 696f 6e0a 2020 2020 5428 7829 3a20 312d  ion.    T(x): 1-
+00039e20: 6c61 7965 7220 6e65 7572 616c 206e 6574  layer neural net
+00039e30: 776f 726b 2077 6974 6820 7369 676d 6f69  work with sigmoi
+00039e40: 6420 6163 7469 7661 7469 6f6e 0a20 2020  d activation.   
+00039e50: 2043 2858 293a 2031 202d 2054 2858 293b   C(X): 1 - T(X);
+00039e60: 2041 7320 7065 7220 7468 6520 6f72 6967   As per the orig
+00039e70: 696e 616c 2070 6170 6572 0a0a 2020 2020  inal paper..    
+00039e80: 5468 6520 6f75 7470 7574 2077 696c 6c20  The output will 
+00039e90: 6265 206f 6620 7468 6520 7361 6d65 2064  be of the same d
+00039ea0: 696d 656e 7369 6f6e 2061 7320 7468 6520  imension as the 
+00039eb0: 696e 7075 740a 0a20 2020 2052 6566 6572  input..    Refer
+00039ec0: 656e 6365 730a 2020 2020 2d2d 2d2d 2d2d  ences.    ------
+00039ed0: 2d2d 2d2d 0a20 2020 202e 2e20 5b31 5d20  ----.    .. [1] 
+00039ee0: 5372 6976 6173 7461 7661 2065 7420 616c  Srivastava et al
+00039ef0: 2e2c 2022 5472 6169 6e69 6e67 2056 6572  ., "Training Ver
+00039f00: 7920 4465 6570 204e 6574 776f 726b 7322  y Deep Networks"
+00039f10: 2e68 7474 7073 3a2f 2f61 7278 6976 2e6f  .https://arxiv.o
+00039f20: 7267 2f61 6273 2f31 3530 372e 3036 3232  rg/abs/1507.0622
+00039f30: 380a 0a20 2020 2045 7861 6d70 6c65 730a  8..    Examples.
+00039f40: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+00039f50: 203e 3e3e 2078 203d 2074 6f72 6368 2e72   >>> x = torch.r
+00039f60: 616e 646e 2831 362c 2032 3029 0a20 2020  andn(16, 20).   
+00039f70: 203e 3e3e 2068 6967 6877 6179 5f6c 6179   >>> highway_lay
+00039f80: 6572 203d 2048 6967 6877 6179 4c61 7965  er = HighwayLaye
+00039f90: 7228 645f 696e 7075 743d 782e 7368 6170  r(d_input=x.shap
+00039fa0: 655b 315d 290a 2020 2020 3e3e 3e20 7920  e[1]).    >>> y 
+00039fb0: 3d20 6869 6768 7761 795f 6c61 7965 7228  = highway_layer(
+00039fc0: 7829 0a20 2020 203e 3e3e 2078 2e73 6861  x).    >>> x.sha
+00039fd0: 7065 0a20 2020 2074 6f72 6368 2e53 697a  pe.    torch.Siz
+00039fe0: 6528 5b31 362c 2032 305d 290a 2020 2020  e([16, 20]).    
+00039ff0: 3e3e 3e20 792e 7368 6170 650a 2020 2020  >>> y.shape.    
+0003a000: 746f 7263 682e 5369 7a65 285b 3136 2c20  torch.Size([16, 
+0003a010: 3230 5d29 0a20 2020 2022 2222 0a0a 2020  20]).    """..  
+0003a020: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0003a030: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0003a040: 2020 2020 2020 645f 696e 7075 743a 2069        d_input: i
+0003a050: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+0003a060: 2020 2020 2061 6374 6976 6174 696f 6e5f       activation_
+0003a070: 666e 3a20 556e 696f 6e5b 4361 6c6c 6162  fn: Union[Callab
+0003a080: 6c65 2c20 7374 725d 203d 2027 7265 6c75  le, str] = 'relu
+0003a090: 2729 3a0a 2020 2020 2020 2020 2222 220a  '):.        """.
+0003a0a0: 2020 2020 2020 2020 496e 6974 6961 6c69          Initiali
+0003a0b0: 7a65 7320 7468 6520 4869 6768 7761 794c  zes the HighwayL
+0003a0c0: 6179 6572 2e0a 0a20 2020 2020 2020 2050  ayer...        P
+0003a0d0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0003a0e0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0003a0f0: 2020 2020 2020 2020 2064 5f69 6e70 7574           d_input
+0003a100: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+0003a110: 2020 2020 2020 7468 6520 6469 6d65 6e73        the dimens
+0003a120: 696f 6e20 6f66 2074 6865 2069 6e70 7574  ion of the input
+0003a130: 206c 6179 6572 0a20 2020 2020 2020 2020   layer.         
+0003a140: 2020 2061 6374 6976 6174 696f 6e5f 666e     activation_fn
+0003a150: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+0003a160: 2020 2020 2020 7468 6520 6163 7469 7661        the activa
+0003a170: 7469 6f6e 2066 756e 6374 696f 6e20 746f  tion function to
+0003a180: 2075 7365 2066 6f72 2048 2878 290a 2020   use for H(x).  
+0003a190: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0003a1a0: 2020 2073 7570 6572 2848 6967 6877 6179     super(Highway
+0003a1b0: 4c61 7965 722c 2073 656c 6629 2e5f 5f69  Layer, self).__i
+0003a1c0: 6e69 745f 5f28 290a 2020 2020 2020 2020  nit__().        
+0003a1d0: 7365 6c66 2e64 5f69 6e70 7574 203d 2064  self.d_input = d
+0003a1e0: 5f69 6e70 7574 0a20 2020 2020 2020 2073  _input.        s
+0003a1f0: 656c 662e 6163 7469 7661 7469 6f6e 5f66  elf.activation_f
+0003a200: 6e20 3d20 6765 745f 6163 7469 7661 7469  n = get_activati
+0003a210: 6f6e 2861 6374 6976 6174 696f 6e5f 666e  on(activation_fn
+0003a220: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0003a230: 6967 6d6f 6964 5f66 6e20 3d20 6765 745f  igmoid_fn = get_
+0003a240: 6163 7469 7661 7469 6f6e 2827 7369 676d  activation('sigm
+0003a250: 6f69 6427 290a 0a20 2020 2020 2020 2073  oid')..        s
+0003a260: 656c 662e 4820 3d20 6e6e 2e4c 696e 6561  elf.H = nn.Linea
+0003a270: 7228 645f 696e 7075 742c 2064 5f69 6e70  r(d_input, d_inp
+0003a280: 7574 290a 2020 2020 2020 2020 7365 6c66  ut).        self
+0003a290: 2e54 203d 206e 6e2e 4c69 6e65 6172 2864  .T = nn.Linear(d
+0003a2a0: 5f69 6e70 7574 2c20 645f 696e 7075 7429  _input, d_input)
+0003a2b0: 0a0a 2020 2020 6465 6620 666f 7277 6172  ..    def forwar
+0003a2c0: 6428 7365 6c66 2c20 783a 2074 6f72 6368  d(self, x: torch
+0003a2d0: 2e54 656e 736f 7229 202d 3e20 746f 7263  .Tensor) -> torc
+0003a2e0: 682e 5465 6e73 6f72 3a0a 2020 2020 2020  h.Tensor:.      
+0003a2f0: 2020 2222 220a 2020 2020 2020 2020 466f    """.        Fo
+0003a300: 7277 6172 6420 7061 7373 206f 6620 7468  rward pass of th
+0003a310: 6520 4869 6768 7761 794c 6179 6572 2e0a  e HighwayLayer..
+0003a320: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0003a330: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0003a340: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+0003a350: 3a20 746f 7263 682e 5465 6e73 6f72 0a20  : torch.Tensor. 
+0003a360: 2020 2020 2020 2020 2020 2049 6e70 7574             Input
+0003a370: 2074 656e 736f 7220 6f66 2064 696d 656e   tensor of dimen
+0003a380: 7369 6f6e 2028 2c69 6e70 7574 5f64 696d  sion (,input_dim
+0003a390: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
+0003a3a0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0003a3b0: 2d2d 2d0a 2020 2020 2020 2020 6f75 7470  ---.        outp
+0003a3c0: 7574 3a20 746f 7263 682e 5465 6e73 6f72  ut: torch.Tensor
+0003a3d0: 0a20 2020 2020 2020 2020 2020 204f 7574  .            Out
+0003a3e0: 7075 7420 7465 6e73 6f72 206f 6620 6469  put tensor of di
+0003a3f0: 6d65 6e73 696f 6e20 282c 696e 7075 745f  mension (,input_
+0003a400: 6469 6d29 0a20 2020 2020 2020 2022 2222  dim).        """
+0003a410: 0a0a 2020 2020 2020 2020 485f 6f75 7420  ..        H_out 
+0003a420: 3d20 7365 6c66 2e61 6374 6976 6174 696f  = self.activatio
+0003a430: 6e5f 666e 2873 656c 662e 4828 7829 290a  n_fn(self.H(x)).
+0003a440: 2020 2020 2020 2020 545f 6f75 7420 3d20          T_out = 
+0003a450: 7365 6c66 2e73 6967 6d6f 6964 5f66 6e28  self.sigmoid_fn(
+0003a460: 7365 6c66 2e54 2878 2929 0a20 2020 2020  self.T(x)).     
+0003a470: 2020 206f 7574 7075 7420 3d20 485f 6f75     output = H_ou
+0003a480: 7420 2a20 545f 6f75 7420 2b20 7820 2a20  t * T_out + x * 
+0003a490: 2831 202d 2054 5f6f 7574 290a 0a20 2020  (1 - T_out)..   
+0003a4a0: 2020 2020 2072 6574 7572 6e20 6f75 7470       return outp
+0003a4b0: 7574 0a0a 0a63 6c61 7373 2047 7261 7068  ut...class Graph
+0003a4c0: 436f 6e76 286e 6e2e 4d6f 6475 6c65 293a  Conv(nn.Module):
+0003a4d0: 0a20 2020 2022 2222 4772 6170 6820 436f  .    """Graph Co
+0003a4e0: 6e76 6f6c 7574 696f 6e61 6c20 4c61 7965  nvolutional Laye
+0003a4f0: 7273 0a0a 2020 2020 5468 6973 206c 6179  rs..    This lay
+0003a500: 6572 2069 6d70 6c65 6d65 6e74 7320 7468  er implements th
+0003a510: 6520 6772 6170 6820 636f 6e76 6f6c 7574  e graph convolut
+0003a520: 696f 6e20 696e 7472 6f64 7563 6564 2069  ion introduced i
+0003a530: 6e20 5b31 5d5f 2e20 2054 6865 2067 7261  n [1]_.  The gra
+0003a540: 7068 0a20 2020 2063 6f6e 766f 6c75 7469  ph.    convoluti
+0003a550: 6f6e 2063 6f6d 6269 6e65 7320 7065 722d  on combines per-
+0003a560: 6e6f 6465 2066 6561 7475 7265 2076 6563  node feature vec
+0003a570: 7475 7265 7320 696e 2061 206e 6f6e 6c69  tures in a nonli
+0003a580: 6e65 6172 2066 6173 6869 6f6e 2077 6974  near fashion wit
+0003a590: 680a 2020 2020 7468 6520 6665 6174 7572  h.    the featur
+0003a5a0: 6520 7665 6374 6f72 7320 666f 7220 6e65  e vectors for ne
+0003a5b0: 6967 6862 6f72 696e 6720 6e6f 6465 732e  ighboring nodes.
+0003a5c0: 2020 5468 6973 2022 626c 656e 6473 2220    This "blends" 
+0003a5d0: 696e 666f 726d 6174 696f 6e20 696e 0a20  information in. 
+0003a5e0: 2020 206c 6f63 616c 206e 6569 6768 626f     local neighbo
+0003a5f0: 7268 6f6f 6473 206f 6620 6120 6772 6170  rhoods of a grap
+0003a600: 682e 0a0a 2020 2020 4578 616d 706c 650a  h...    Example.
+0003a610: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0003a620: 203e 3e3e 2069 6d70 6f72 7420 6465 6570   >>> import deep
+0003a630: 6368 656d 2061 7320 6463 0a20 2020 203e  chem as dc.    >
+0003a640: 3e3e 2069 6d70 6f72 7420 6e75 6d70 7920  >> import numpy 
+0003a650: 6173 206e 700a 2020 2020 3e3e 3e20 696d  as np.    >>> im
+0003a660: 706f 7274 2064 6565 7063 6865 6d2e 6d6f  port deepchem.mo
+0003a670: 6465 6c73 2e74 6f72 6368 5f6d 6f64 656c  dels.torch_model
+0003a680: 732e 6c61 7965 7273 2061 7320 746f 7263  s.layers as torc
+0003a690: 685f 6c61 7965 7273 0a20 2020 203e 3e3e  h_layers.    >>>
+0003a6a0: 206f 7574 5f63 6861 6e6e 656c 7320 3d20   out_channels = 
+0003a6b0: 320a 2020 2020 3e3e 3e20 6e5f 6174 6f6d  2.    >>> n_atom
+0003a6c0: 7320 3d20 3420 2023 2049 6e20 4343 4320  s = 4  # In CCC 
+0003a6d0: 616e 6420 432c 2074 6865 7265 2061 7265  and C, there are
+0003a6e0: 2034 2061 746f 6d73 0a20 2020 203e 3e3e   4 atoms.    >>>
+0003a6f0: 2072 6177 5f73 6d69 6c65 7320 3d20 5b27   raw_smiles = ['
+0003a700: 4343 4327 2c20 2743 275d 0a20 2020 203e  CCC', 'C'].    >
+0003a710: 3e3e 2066 726f 6d20 7264 6b69 7420 696d  >> from rdkit im
+0003a720: 706f 7274 2043 6865 6d0a 2020 2020 3e3e  port Chem.    >>
+0003a730: 3e20 6d6f 6c73 203d 205b 4368 656d 2e4d  > mols = [Chem.M
+0003a740: 6f6c 4672 6f6d 536d 696c 6573 2873 2920  olFromSmiles(s) 
+0003a750: 666f 7220 7320 696e 2072 6177 5f73 6d69  for s in raw_smi
+0003a760: 6c65 735d 0a20 2020 203e 3e3e 2066 6561  les].    >>> fea
+0003a770: 7475 7269 7a65 7220 3d20 6463 2e66 6561  turizer = dc.fea
+0003a780: 742e 6772 6170 685f 6665 6174 7572 6573  t.graph_features
+0003a790: 2e43 6f6e 764d 6f6c 4665 6174 7572 697a  .ConvMolFeaturiz
+0003a7a0: 6572 2829 0a20 2020 203e 3e3e 206d 6f6c  er().    >>> mol
+0003a7b0: 7320 3d20 6665 6174 7572 697a 6572 2e66  s = featurizer.f
+0003a7c0: 6561 7475 7269 7a65 286d 6f6c 7329 0a20  eaturize(mols). 
+0003a7d0: 2020 203e 3e3e 206d 756c 7469 5f6d 6f6c     >>> multi_mol
+0003a7e0: 203d 2064 632e 6665 6174 2e6d 6f6c 5f67   = dc.feat.mol_g
+0003a7f0: 7261 7068 732e 436f 6e76 4d6f 6c2e 6167  raphs.ConvMol.ag
+0003a800: 676c 6f6d 6572 6174 655f 6d6f 6c73 286d  glomerate_mols(m
+0003a810: 6f6c 7329 0a20 2020 203e 3e3e 2061 746f  ols).    >>> ato
+0003a820: 6d5f 6665 6174 7572 6573 203d 206d 756c  m_features = mul
+0003a830: 7469 5f6d 6f6c 2e67 6574 5f61 746f 6d5f  ti_mol.get_atom_
+0003a840: 6665 6174 7572 6573 2829 2e61 7374 7970  features().astyp
+0003a850: 6528 6e70 2e66 6c6f 6174 3332 290a 2020  e(np.float32).  
+0003a860: 2020 3e3e 3e20 6465 6772 6565 5f73 6c69    >>> degree_sli
+0003a870: 6365 203d 206d 756c 7469 5f6d 6f6c 2e64  ce = multi_mol.d
+0003a880: 6567 5f73 6c69 6365 0a20 2020 203e 3e3e  eg_slice.    >>>
+0003a890: 206d 656d 6265 7273 6869 7020 3d20 6d75   membership = mu
+0003a8a0: 6c74 695f 6d6f 6c2e 6d65 6d62 6572 7368  lti_mol.membersh
+0003a8b0: 6970 0a20 2020 203e 3e3e 2064 6567 5f61  ip.    >>> deg_a
+0003a8c0: 646a 7320 3d20 6d75 6c74 695f 6d6f 6c2e  djs = multi_mol.
+0003a8d0: 6765 745f 6465 675f 6164 6a61 6365 6e63  get_deg_adjacenc
+0003a8e0: 795f 6c69 7374 7328 295b 313a 5d0a 2020  y_lists()[1:].  
+0003a8f0: 2020 3e3e 3e20 6172 6773 203d 205b 6174    >>> args = [at
+0003a900: 6f6d 5f66 6561 7475 7265 732c 2064 6567  om_features, deg
+0003a910: 7265 655f 736c 6963 652c 206d 656d 6265  ree_slice, membe
+0003a920: 7273 6869 705d 202b 2064 6567 5f61 646a  rship] + deg_adj
+0003a930: 730a 2020 2020 3e3e 3e20 6c61 7965 7220  s.    >>> layer 
+0003a940: 3d20 746f 7263 685f 6c61 7965 7273 2e47  = torch_layers.G
+0003a950: 7261 7068 436f 6e76 286f 7574 5f63 6861  raphConv(out_cha
+0003a960: 6e6e 656c 7329 0a20 2020 203e 3e3e 2072  nnels).    >>> r
+0003a970: 6573 756c 7420 3d20 6c61 7965 7228 6172  esult = layer(ar
+0003a980: 6773 290a 2020 2020 3e3e 3e20 7479 7065  gs).    >>> type
+0003a990: 2872 6573 756c 7429 0a20 2020 203c 636c  (result).    <cl
+0003a9a0: 6173 7320 2774 6f72 6368 2e54 656e 736f  ass 'torch.Tenso
+0003a9b0: 7227 3e0a 2020 2020 3e3e 3e20 7265 7375  r'>.    >>> resu
+0003a9c0: 6c74 2e73 6861 7065 0a20 2020 2074 6f72  lt.shape.    tor
+0003a9d0: 6368 2e53 697a 6528 5b34 2c20 325d 290a  ch.Size([4, 2]).
+0003a9e0: 2020 2020 3e3e 3e20 6e75 6d5f 6465 6720      >>> num_deg 
+0003a9f0: 3d20 3220 2a20 6c61 7965 722e 6d61 785f  = 2 * layer.max_
+0003aa00: 6465 6772 6565 202b 2028 3120 2d20 6c61  degree + (1 - la
+0003aa10: 7965 722e 6d69 6e5f 6465 6772 6565 290a  yer.min_degree).
+0003aa20: 2020 2020 3e3e 3e20 6e75 6d5f 6465 670a      >>> num_deg.
+0003aa30: 2020 2020 3231 0a0a 2020 2020 5265 6665      21..    Refe
+0003aa40: 7265 6e63 6573 0a20 2020 202d 2d2d 2d2d  rences.    -----
+0003aa50: 2d2d 2d2d 2d0a 2020 2020 2e2e 205b 315d  -----.    .. [1]
+0003aa60: 2044 7576 656e 6175 642c 2044 6176 6964   Duvenaud, David
+0003aa70: 204b 2e2c 2065 7420 616c 2e20 2243 6f6e   K., et al. "Con
+0003aa80: 766f 6c75 7469 6f6e 616c 206e 6574 776f  volutional netwo
+0003aa90: 726b 7320 6f6e 2067 7261 7068 7320 666f  rks on graphs fo
+0003aaa0: 7220 6c65 6172 6e69 6e67 206d 6f6c 6563  r learning molec
+0003aab0: 756c 6172 2066 696e 6765 7270 7269 6e74  ular fingerprint
+0003aac0: 732e 220a 2020 2020 2020 2020 4164 7661  s.".        Adva
+0003aad0: 6e63 6573 2069 6e20 6e65 7572 616c 2069  nces in neural i
+0003aae0: 6e66 6f72 6d61 7469 6f6e 2070 726f 6365  nformation proce
+0003aaf0: 7373 696e 6720 7379 7374 656d 732e 2032  ssing systems. 2
+0003ab00: 3031 352e 2068 7474 7073 3a2f 2f61 7278  015. https://arx
+0003ab10: 6976 2e6f 7267 2f61 6273 2f31 3530 392e  iv.org/abs/1509.
+0003ab20: 3039 3239 320a 0a20 2022 2222 0a0a 2020  09292..  """..  
+0003ab30: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0003ab40: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0003ab50: 2020 2020 2020 6f75 745f 6368 616e 6e65        out_channe
+0003ab60: 6c3a 2069 6e74 2c0a 2020 2020 2020 2020  l: int,.        
+0003ab70: 2020 2020 2020 2020 206d 696e 5f64 6567           min_deg
+0003ab80: 3a20 696e 7420 3d20 302c 0a20 2020 2020  : int = 0,.     
+0003ab90: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0003aba0: 6465 673a 2069 6e74 203d 2031 302c 0a20  deg: int = 10,. 
+0003abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003abc0: 6163 7469 7661 7469 6f6e 5f66 6e3a 204f  activation_fn: O
+0003abd0: 7074 696f 6e61 6c5b 4361 6c6c 6162 6c65  ptional[Callable
+0003abe0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0003abf0: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+0003ac00: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
+0003ac10: 2249 6e69 7469 616c 697a 6520 6120 6772  "Initialize a gr
+0003ac20: 6170 6820 636f 6e76 6f6c 7574 696f 6e61  aph convolutiona
+0003ac30: 6c20 6c61 7965 722e 0a0a 2020 2020 2020  l layer...      
+0003ac40: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0003ac50: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0003ac60: 2020 2020 2020 2020 6f75 745f 6368 616e          out_chan
+0003ac70: 6e65 6c3a 2069 6e74 0a20 2020 2020 2020  nel: int.       
+0003ac80: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
+0003ac90: 6f66 206f 7574 7075 7420 6368 616e 6e65  of output channe
+0003aca0: 6c73 2070 6572 2067 7261 7068 206e 6f64  ls per graph nod
+0003acb0: 652e 0a20 2020 2020 2020 206d 696e 5f64  e..        min_d
+0003acc0: 6567 3a20 696e 742c 206f 7074 696f 6e61  eg: int, optiona
+0003acd0: 6c20 2864 6566 6175 6c74 2030 290a 2020  l (default 0).  
+0003ace0: 2020 2020 2020 2020 2020 5468 6520 6d69            The mi
+0003acf0: 6e69 6d75 6d20 616c 6c6f 7765 6420 6465  nimum allowed de
+0003ad00: 6772 6565 2066 6f72 2065 6163 6820 6772  gree for each gr
+0003ad10: 6170 6820 6e6f 6465 2e0a 2020 2020 2020  aph node..      
+0003ad20: 2020 6d61 785f 6465 673a 2069 6e74 2c20    max_deg: int, 
+0003ad30: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
+0003ad40: 7420 3130 290a 2020 2020 2020 2020 2020  t 10).          
+0003ad50: 2020 5468 6520 6d61 7869 6d75 6d20 616c    The maximum al
+0003ad60: 6c6f 7765 6420 6465 6772 6565 2066 6f72  lowed degree for
+0003ad70: 2065 6163 6820 6772 6170 6820 6e6f 6465   each graph node
+0003ad80: 2e20 4e6f 7465 2074 6861 7420 7468 6973  . Note that this
+0003ad90: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
+0003ada0: 7365 7420 746f 2031 3020 746f 2068 616e  set to 10 to han
+0003adb0: 646c 6520 636f 6d70 6c65 7820 6d6f 6c65  dle complex mole
+0003adc0: 6375 6c65 7320 2873 6f6d 6520 6f72 6761  cules (some orga
+0003add0: 6e6f 6d65 7461 6c6c 6963 0a20 2020 2020  nometallic.     
+0003ade0: 2020 2020 2020 2063 6f6d 706f 756e 6473         compounds
+0003adf0: 2068 6176 6520 7374 7261 6e67 6520 7374   have strange st
+0003ae00: 7275 6374 7572 6573 292e 2049 6620 796f  ructures). If yo
+0003ae10: 7527 7265 2075 7369 6e67 2074 6869 7320  u're using this 
+0003ae20: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+0003ae30: 6e6f 6e2d 6d6f 6c65 6375 6c61 7220 6170  non-molecular ap
+0003ae40: 706c 6963 6174 696f 6e73 2c20 796f 7520  plications, you 
+0003ae50: 6d61 7920 6e65 6564 2074 6f20 7365 7420  may need to set 
+0003ae60: 7468 6973 206d 7563 6820 6869 6768 6572  this much higher
+0003ae70: 0a20 2020 2020 2020 2020 2020 2064 6570  .            dep
+0003ae80: 656e 6469 6e67 206f 6e20 796f 7572 2064  ending on your d
+0003ae90: 6174 6173 6574 2e0a 2020 2020 2020 2020  ataset..        
+0003aea0: 6163 7469 7661 7469 6f6e 5f66 6e3a 2066  activation_fn: f
+0003aeb0: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
+0003aec0: 2020 2020 4120 6e6f 6e6c 696e 6561 7220      A nonlinear 
+0003aed0: 6163 7469 7661 7469 6f6e 2066 756e 6374  activation funct
+0003aee0: 696f 6e20 746f 2061 7070 6c79 2e20 4966  ion to apply. If
+0003aef0: 2079 6f75 2772 6520 6e6f 7420 7375 7265   you're not sure
+0003af00: 2c0a 2020 2020 2020 2020 2020 2020 6074  ,.            `t
+0003af10: 6f72 6368 2e6e 6e2e 5265 4c55 6020 6973  orch.nn.ReLU` is
+0003af20: 2070 726f 6261 626c 7920 6120 676f 6f64   probably a good
+0003af30: 2064 6566 6175 6c74 2066 6f72 2079 6f75   default for you
+0003af40: 7220 6170 706c 6963 6174 696f 6e2e 0a20  r application.. 
+0003af50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0003af60: 2020 2073 7570 6572 2847 7261 7068 436f     super(GraphCo
+0003af70: 6e76 2c20 7365 6c66 292e 5f5f 696e 6974  nv, self).__init
+0003af80: 5f5f 282a 2a6b 7761 7267 7329 0a20 2020  __(**kwargs).   
+0003af90: 2020 2020 2073 656c 662e 6f75 745f 6368       self.out_ch
+0003afa0: 616e 6e65 6c3a 2069 6e74 203d 206f 7574  annel: int = out
+0003afb0: 5f63 6861 6e6e 656c 0a20 2020 2020 2020  _channel.       
+0003afc0: 2073 656c 662e 6d69 6e5f 6465 6772 6565   self.min_degree
+0003afd0: 3a20 696e 7420 3d20 6d69 6e5f 6465 670a  : int = min_deg.
+0003afe0: 2020 2020 2020 2020 7365 6c66 2e6d 6178          self.max
+0003aff0: 5f64 6567 7265 653a 2069 6e74 203d 206d  _degree: int = m
+0003b000: 6178 5f64 6567 0a20 2020 2020 2020 2073  ax_deg.        s
+0003b010: 656c 662e 6163 7469 7661 7469 6f6e 5f66  elf.activation_f
+0003b020: 6e3a 204f 7074 696f 6e61 6c5b 4361 6c6c  n: Optional[Call
+0003b030: 6162 6c65 5d20 3d20 6163 7469 7661 7469  able] = activati
+0003b040: 6f6e 5f66 6e0a 0a20 2020 2020 2020 2023  on_fn..        #
+0003b050: 2047 656e 6572 6174 6520 7468 6520 6e62   Generate the nb
+0003b060: 5f61 6666 696e 6520 7765 6967 6874 7320  _affine weights 
+0003b070: 616e 6420 6269 6173 6573 0a20 2020 2020  and biases.     
+0003b080: 2020 206e 756d 5f64 6567 3a20 696e 7420     num_deg: int 
+0003b090: 3d20 3220 2a20 7365 6c66 2e6d 6178 5f64  = 2 * self.max_d
+0003b0a0: 6567 7265 6520 2b20 2831 202d 2073 656c  egree + (1 - sel
+0003b0b0: 662e 6d69 6e5f 6465 6772 6565 290a 2020  f.min_degree).  
+0003b0c0: 2020 2020 2020 7365 6c66 2e57 5f6c 6973        self.W_lis
+0003b0d0: 743a 206e 6e2e 5061 7261 6d65 7465 724c  t: nn.ParameterL
+0003b0e0: 6973 7420 3d20 6e6e 2e50 6172 616d 6574  ist = nn.Paramet
+0003b0f0: 6572 4c69 7374 285b 0a20 2020 2020 2020  erList([.       
+0003b100: 2020 2020 206e 6e2e 5061 7261 6d65 7465       nn.Paramete
+0003b110: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0003b120: 2020 2067 6574 6174 7472 2869 6e69 7469     getattr(initi
+0003b130: 616c 697a 6572 732c 0a20 2020 2020 2020  alizers,.       
+0003b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003b150: 2027 7861 7669 6572 5f75 6e69 666f 726d   'xavier_uniform
+0003b160: 5f27 2928 746f 7263 682e 656d 7074 7928  _')(torch.empty(
+0003b170: 3735 2c20 7365 6c66 2e6f 7574 5f63 6861  75, self.out_cha
+0003b180: 6e6e 656c 2929 290a 2020 2020 2020 2020  nnel))).        
+0003b190: 2020 2020 666f 7220 6b20 696e 2072 616e      for k in ran
+0003b1a0: 6765 286e 756d 5f64 6567 290a 2020 2020  ge(num_deg).    
+0003b1b0: 2020 2020 5d29 0a20 2020 2020 2020 2073      ]).        s
+0003b1c0: 656c 662e 625f 6c69 7374 3a20 6e6e 2e50  elf.b_list: nn.P
+0003b1d0: 6172 616d 6574 6572 4c69 7374 203d 206e  arameterList = n
+0003b1e0: 6e2e 5061 7261 6d65 7465 724c 6973 7428  n.ParameterList(
+0003b1f0: 5b0a 2020 2020 2020 2020 2020 2020 6e6e  [.            nn
+0003b200: 2e50 6172 616d 6574 6572 280a 2020 2020  .Parameter(.    
+0003b210: 2020 2020 2020 2020 2020 2020 6765 7461              geta
+0003b220: 7474 7228 696e 6974 6961 6c69 7a65 7273  ttr(initializers
+0003b230: 2c20 277a 6572 6f73 5f27 2928 746f 7263  , 'zeros_')(torc
+0003b240: 682e 656d 7074 7928 7365 6c66 2e6f 7574  h.empty(self.out
+0003b250: 5f63 6861 6e6e 656c 2c29 2929 0a20 2020  _channel,))).   
+0003b260: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+0003b270: 6e20 7261 6e67 6528 6e75 6d5f 6465 6729  n range(num_deg)
+0003b280: 0a20 2020 2020 2020 205d 290a 2020 2020  .        ]).    
+0003b290: 2020 2020 7365 6c66 2e62 7569 6c74 203d      self.built =
+0003b2a0: 2054 7275 650a 0a20 2020 2064 6566 205f   True..    def _
+0003b2b0: 5f72 6570 725f 5f28 7365 6c66 2920 2d3e  _repr__(self) ->
+0003b2c0: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
+0003b2d0: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+0003b2e0: 7320 6120 7374 7269 6e67 2072 6570 7265  s a string repre
+0003b2f0: 7365 6e74 6174 696f 6e20 6f66 2074 6865  sentation of the
+0003b300: 206f 626a 6563 742e 0a0a 2020 2020 2020   object...      
+0003b310: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0003b320: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0003b330: 2020 2073 7472 3a20 4120 7374 7269 6e67     str: A string
+0003b340: 2074 6861 7420 636f 6e74 6169 6e73 2074   that contains t
+0003b350: 6865 2063 6c61 7373 206e 616d 6520 666f  he class name fo
+0003b360: 6c6c 6f77 6564 2062 7920 7468 6520 7661  llowed by the va
+0003b370: 6c75 6573 206f 6620 6974 7320 696e 7374  lues of its inst
+0003b380: 616e 6365 2076 6172 6961 626c 652e 0a20  ance variable.. 
+0003b390: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0003b3a0: 2020 2023 2066 6c61 6b65 383a 206e 6f71     # flake8: noq
+0003b3b0: 610a 2020 2020 2020 2020 7265 7475 726e  a.        return
+0003b3c0: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
+0003b3d0: 277b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  '{self.__class__
+0003b3e0: 2e5f 5f6e 616d 655f 5f7d 286f 7574 5f63  .__name__}(out_c
+0003b3f0: 6861 6e6e 656c 3a7b 7365 6c66 2e6f 7574  hannel:{self.out
+0003b400: 5f63 6861 6e6e 656c 7d2c 6d69 6e5f 6465  _channel},min_de
+0003b410: 673a 7b73 656c 662e 6d69 6e5f 6465 677d  g:{self.min_deg}
+0003b420: 2c6d 6178 5f64 6567 3a7b 7365 6c66 2e6d  ,max_deg:{self.m
+0003b430: 6178 5f64 6567 7d2c 6163 7469 7661 7469  ax_deg},activati
+0003b440: 6f6e 5f66 6e3a 7b73 656c 662e 6163 7469  on_fn:{self.acti
+0003b450: 7661 7469 6f6e 5f66 6e7d 2927 0a20 2020  vation_fn})'.   
+0003b460: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0003b470: 666f 7277 6172 6428 7365 6c66 2c20 696e  forward(self, in
+0003b480: 7075 7473 3a20 4c69 7374 5b6e 702e 6e64  puts: List[np.nd
+0003b490: 6172 7261 795d 2920 2d3e 2074 6f72 6368  array]) -> torch
+0003b4a0: 2e54 656e 736f 723a 0a20 2020 2020 2020  .Tensor:.       
+0003b4b0: 2022 2222 0a20 2020 2020 2020 2054 6865   """.        The
+0003b4c0: 2066 6f72 7761 7264 2070 6173 7320 636f   forward pass co
+0003b4d0: 6d62 696e 6573 2070 6572 2d6e 6f64 6520  mbines per-node 
+0003b4e0: 6665 6174 7572 6520 7665 6374 6f72 7320  feature vectors 
+0003b4f0: 696e 2061 206e 6f6e 6c69 6e65 6172 2066  in a nonlinear f
+0003b500: 6173 6869 6f6e 2077 6974 680a 2020 2020  ashion with.    
+0003b510: 2020 2020 7468 6520 6665 6174 7572 6520      the feature 
+0003b520: 7665 6374 6f72 7320 666f 7220 6e65 6967  vectors for neig
+0003b530: 6862 6f72 696e 6720 6e6f 6465 732e 0a20  hboring nodes.. 
+0003b540: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0003b550: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0003b560: 2d2d 2d2d 0a20 2020 2020 2020 2069 6e70  ----.        inp
+0003b570: 7574 733a 204c 6973 745b 6e70 2e6e 6461  uts: List[np.nda
+0003b580: 7272 6179 5d0a 2020 2020 2020 2020 5368  rray].        Sh
+0003b590: 6f75 6c64 2063 6f6e 7461 696e 2061 746f  ould contain ato
+0003b5a0: 6d20 6665 6174 7572 6573 2061 6e64 2061  m features and a
+0003b5b0: 7272 6179 7320 6465 7363 7269 6269 6e67  rrays describing
+0003b5c0: 2067 7261 7068 2074 6f70 6f6c 6f67 790a   graph topology.
+0003b5d0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0003b5e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0003b5f0: 0a20 2020 2020 2020 2074 6f72 6368 2e54  .        torch.T
+0003b600: 656e 736f 720a 2020 2020 2020 2020 2020  ensor.          
+0003b610: 436f 6d62 696e 6564 2061 746f 6d20 6665  Combined atom fe
+0003b620: 6174 7572 6573 0a20 2020 2020 2020 2022  atures.        "
+0003b630: 2222 0a0a 2020 2020 2020 2020 2320 4578  ""..        # Ex
+0003b640: 7472 6163 7420 6174 6f6d 5f66 6561 7475  tract atom_featu
+0003b650: 7265 730a 2020 2020 2020 2020 6174 6f6d  res.        atom
+0003b660: 5f66 6561 7475 7265 733a 2074 6f72 6368  _features: torch
+0003b670: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
+0003b680: 7465 6e73 6f72 2869 6e70 7574 735b 305d  tensor(inputs[0]
+0003b690: 290a 0a20 2020 2020 2020 2023 2045 7874  )..        # Ext
+0003b6a0: 7261 6374 2067 7261 7068 2074 6f70 6f6c  ract graph topol
+0003b6b0: 6f67 790a 2020 2020 2020 2020 6465 675f  ogy.        deg_
+0003b6c0: 736c 6963 653a 206e 702e 6e64 6172 7261  slice: np.ndarra
+0003b6d0: 7920 3d20 696e 7075 7473 5b31 5d0a 2020  y = inputs[1].  
+0003b6e0: 2020 2020 2020 6465 675f 6164 6a5f 6c69        deg_adj_li
+0003b6f0: 7374 733a 204c 6973 745b 6e70 2e6e 6461  sts: List[np.nda
+0003b700: 7272 6179 5d20 3d20 696e 7075 7473 5b33  rray] = inputs[3
+0003b710: 3a5d 0a0a 2020 2020 2020 2020 5720 3d20  :]..        W = 
+0003b720: 6974 6572 2873 656c 662e 575f 6c69 7374  iter(self.W_list
+0003b730: 290a 2020 2020 2020 2020 6220 3d20 6974  ).        b = it
+0003b740: 6572 2873 656c 662e 625f 6c69 7374 290a  er(self.b_list).
+0003b750: 0a20 2020 2020 2020 2023 2053 756d 2061  .        # Sum a
+0003b760: 6c6c 206e 6569 6768 626f 7273 2075 7369  ll neighbors usi
+0003b770: 6e67 2061 646a 6163 656e 6379 206d 6174  ng adjacency mat
+0003b780: 7269 780a 2020 2020 2020 2020 6465 675f  rix.        deg_
+0003b790: 7375 6d6d 6564 3a20 4c69 7374 5b6e 702e  summed: List[np.
+0003b7a0: 6e64 6172 7261 795d 203d 2073 656c 662e  ndarray] = self.
+0003b7b0: 7375 6d5f 6e65 6967 6828 6174 6f6d 5f66  sum_neigh(atom_f
+0003b7c0: 6561 7475 7265 732c 0a20 2020 2020 2020  eatures,.       
+0003b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003b7f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0003b800: 6567 5f61 646a 5f6c 6973 7473 290a 0a20  eg_adj_lists).. 
+0003b810: 2020 2020 2020 2023 2047 6574 2063 6f6c         # Get col
+0003b820: 6c65 6374 696f 6e20 6f66 206d 6f64 6966  lection of modif
+0003b830: 6965 6420 6174 6f6d 2066 6561 7475 7265  ied atom feature
+0003b840: 730a 2020 2020 2020 2020 6e65 775f 7265  s.        new_re
+0003b850: 6c5f 6174 6f6d 735f 636f 6c6c 6563 7469  l_atoms_collecti
+0003b860: 6f6e 203d 205b 5d0a 0a20 2020 2020 2020  on = []..       
+0003b870: 2073 706c 6974 5f66 6561 7475 7265 733a   split_features:
+0003b880: 2054 7570 6c65 5b74 6f72 6368 2e54 656e   Tuple[torch.Ten
+0003b890: 736f 722c 0a20 2020 2020 2020 2020 2020  sor,.           
+0003b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003b8b0: 2020 202e 2e2e 5d20 3d20 746f 7263 682e     ...] = torch.
+0003b8c0: 7370 6c69 7428 6174 6f6d 5f66 6561 7475  split(atom_featu
+0003b8d0: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
+0003b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003b900: 2020 2020 2020 2864 6567 5f73 6c69 6365        (deg_slice
+0003b910: 5b3a 2c20 315d 292e 746f 6c69 7374 2829  [:, 1]).tolist()
+0003b920: 290a 2020 2020 2020 2020 666f 7220 6465  ).        for de
+0003b930: 6720 696e 2072 616e 6765 2831 2c20 7365  g in range(1, se
+0003b940: 6c66 2e6d 6178 5f64 6567 7265 6520 2b20  lf.max_degree + 
+0003b950: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
+0003b960: 2320 4f62 7461 696e 2072 656c 6576 616e  # Obtain relevan
+0003b970: 7420 6174 6f6d 7320 666f 7220 7468 6973  t atoms for this
+0003b980: 2064 6567 7265 650a 2020 2020 2020 2020   degree.        
+0003b990: 2020 2020 7265 6c5f 6174 6f6d 733a 2074      rel_atoms: t
+0003b9a0: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
+0003b9b0: 7263 682e 6672 6f6d 5f6e 756d 7079 2864  rch.from_numpy(d
+0003b9c0: 6567 5f73 756d 6d65 645b 6465 6720 2d20  eg_summed[deg - 
+0003b9d0: 315d 290a 0a20 2020 2020 2020 2020 2020  1])..           
+0003b9e0: 2023 2047 6574 2073 656c 6620 6174 6f6d   # Get self atom
+0003b9f0: 730a 2020 2020 2020 2020 2020 2020 7365  s.            se
+0003ba00: 6c66 5f61 746f 6d73 3a20 746f 7263 682e  lf_atoms: torch.
+0003ba10: 5465 6e73 6f72 203d 2073 706c 6974 5f66  Tensor = split_f
+0003ba20: 6561 7475 7265 735b 6465 6720 2d20 7365  eatures[deg - se
+0003ba30: 6c66 2e6d 696e 5f64 6567 7265 655d 0a0a  lf.min_degree]..
+0003ba40: 2020 2020 2020 2020 2020 2020 2320 4170              # Ap
+0003ba50: 706c 7920 6869 6464 656e 2061 6666 696e  ply hidden affin
+0003ba60: 6520 746f 2072 656c 6576 616e 7420 6174  e to relevant at
+0003ba70: 6f6d 7320 616e 6420 6170 7065 6e64 0a20  oms and append. 
+0003ba80: 2020 2020 2020 2020 2020 2072 656c 5f6f             rel_o
+0003ba90: 7574 3a20 746f 7263 682e 5465 6e73 6f72  ut: torch.Tensor
+0003baa0: 203d 2074 6f72 6368 2e6d 6174 6d75 6c28   = torch.matmul(
+0003bab0: 7265 6c5f 6174 6f6d 732e 7479 7065 2874  rel_atoms.type(t
+0003bac0: 6f72 6368 2e66 6c6f 6174 3332 292c 0a20  orch.float32),. 
+0003bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003bb00: 6e65 7874 2857 2929 202b 206e 6578 7428  next(W)) + next(
+0003bb10: 6229 0a20 2020 2020 2020 2020 2020 2073  b).            s
+0003bb20: 656c 665f 6f75 743a 2074 6f72 6368 2e54  elf_out: torch.T
+0003bb30: 656e 736f 7220 3d20 746f 7263 682e 6d61  ensor = torch.ma
+0003bb40: 746d 756c 280a 2020 2020 2020 2020 2020  tmul(.          
+0003bb50: 2020 2020 2020 7365 6c66 5f61 746f 6d73        self_atoms
+0003bb60: 2e74 7970 6528 746f 7263 682e 666c 6f61  .type(torch.floa
+0003bb70: 7433 3229 2c20 6e65 7874 2857 2929 202b  t32), next(W)) +
+0003bb80: 206e 6578 7428 6229 0a20 2020 2020 2020   next(b).       
+0003bb90: 2020 2020 206f 7574 3a20 746f 7263 682e       out: torch.
+0003bba0: 5465 6e73 6f72 203d 2072 656c 5f6f 7574  Tensor = rel_out
+0003bbb0: 202b 2073 656c 665f 6f75 740a 2020 2020   + self_out.    
+0003bbc0: 2020 2020 2020 2020 6e65 775f 7265 6c5f          new_rel_
+0003bbd0: 6174 6f6d 735f 636f 6c6c 6563 7469 6f6e  atoms_collection
+0003bbe0: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
+0003bbf0: 2020 2020 2020 2020 2074 6f72 6368 2e66           torch.f
+0003bc00: 726f 6d5f 6e75 6d70 7928 6f75 742e 6465  rom_numpy(out.de
+0003bc10: 7461 6368 2829 2e6e 756d 7079 2829 2929  tach().numpy()))
+0003bc20: 0a0a 2020 2020 2020 2020 2320 4465 7465  ..        # Dete
+0003bc30: 726d 696e 6520 7468 6520 6d69 6e5f 6465  rmine the min_de
+0003bc40: 673d 3020 6361 7365 0a20 2020 2020 2020  g=0 case.       
+0003bc50: 2069 6620 7365 6c66 2e6d 696e 5f64 6567   if self.min_deg
+0003bc60: 7265 6520 3d3d 2030 3a0a 2020 2020 2020  ree == 0:.      
+0003bc70: 2020 2020 2020 7365 6c66 5f61 746f 6d73        self_atoms
+0003bc80: 203d 2073 706c 6974 5f66 6561 7475 7265   = split_feature
+0003bc90: 735b 305d 0a0a 2020 2020 2020 2020 2020  s[0]..          
+0003bca0: 2020 2320 4f6e 6c79 2075 7365 2074 6865    # Only use the
+0003bcb0: 2073 656c 6620 6c61 7965 720a 2020 2020   self layer.    
+0003bcc0: 2020 2020 2020 2020 6f75 7420 3d20 746f          out = to
+0003bcd0: 7263 682e 6d61 746d 756c 2873 656c 665f  rch.matmul(self_
+0003bce0: 6174 6f6d 732e 7479 7065 2874 6f72 6368  atoms.type(torch
+0003bcf0: 2e66 6c6f 6174 3332 292c 0a20 2020 2020  .float32),.     
+0003bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003bd10: 2020 2020 2020 2020 2020 6e65 7874 2857            next(W
+0003bd20: 2929 202b 206e 6578 7428 6229 0a20 2020  )) + next(b).   
+0003bd30: 2020 2020 2020 2020 206e 6577 5f72 656c           new_rel
+0003bd40: 5f61 746f 6d73 5f63 6f6c 6c65 6374 696f  _atoms_collectio
+0003bd50: 6e2e 696e 7365 7274 280a 2020 2020 2020  n.insert(.      
+0003bd60: 2020 2020 2020 2020 2020 302c 2074 6f72            0, tor
+0003bd70: 6368 2e66 726f 6d5f 6e75 6d70 7928 6f75  ch.from_numpy(ou
+0003bd80: 742e 6465 7461 6368 2829 2e6e 756d 7079  t.detach().numpy
+0003bd90: 2829 2929 0a0a 2020 2020 2020 2020 2320  ()))..        # 
+0003bda0: 436f 6d62 696e 6520 616c 6c20 6174 6f6d  Combine all atom
+0003bdb0: 7320 6261 636b 2069 6e74 6f20 7468 6520  s back into the 
+0003bdc0: 6c69 7374 0a20 2020 2020 2020 2061 746f  list.        ato
+0003bdd0: 6d5f 6665 6174 7572 6573 203d 2074 6f72  m_features = tor
+0003bde0: 6368 2e63 6f6e 6361 7428 6e65 775f 7265  ch.concat(new_re
+0003bdf0: 6c5f 6174 6f6d 735f 636f 6c6c 6563 7469  l_atoms_collecti
+0003be00: 6f6e 2c20 3029 0a0a 2020 2020 2020 2020  on, 0)..        
+0003be10: 6966 2073 656c 662e 6163 7469 7661 7469  if self.activati
+0003be20: 6f6e 5f66 6e20 6973 206e 6f74 204e 6f6e  on_fn is not Non
+0003be30: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+0003be40: 746f 6d5f 6665 6174 7572 6573 203d 2073  tom_features = s
+0003be50: 656c 662e 6163 7469 7661 7469 6f6e 5f66  elf.activation_f
+0003be60: 6e28 6174 6f6d 5f66 6561 7475 7265 7329  n(atom_features)
+0003be70: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0003be80: 2061 746f 6d5f 6665 6174 7572 6573 0a0a   atom_features..
+0003be90: 2020 2020 6465 6620 7375 6d5f 6e65 6967      def sum_neig
+0003bea0: 6828 7365 6c66 2c20 6174 6f6d 733a 2074  h(self, atoms: t
+0003beb0: 6f72 6368 2e54 656e 736f 722c 2064 6567  orch.Tensor, deg
+0003bec0: 5f61 646a 5f6c 6973 7473 2920 2d3e 204c  _adj_lists) -> L
+0003bed0: 6973 745b 6e70 2e6e 6461 7272 6179 5d3a  ist[np.ndarray]:
+0003bee0: 0a20 2020 2020 2020 2022 2222 5374 6f72  .        """Stor
+0003bef0: 6520 7468 6520 7375 6d6d 6564 2061 746f  e the summed ato
+0003bf00: 6d73 2062 7920 6465 6772 6565 2222 220a  ms by degree""".
+0003bf10: 2020 2020 2020 2020 6465 675f 7375 6d6d          deg_summ
+0003bf20: 6564 203d 205b 5d0a 0a20 2020 2020 2020  ed = []..       
+0003bf30: 2066 6f72 2064 6567 2069 6e20 7261 6e67   for deg in rang
+0003bf40: 6528 312c 2073 656c 662e 6d61 785f 6465  e(1, self.max_de
+0003bf50: 6772 6565 202b 2031 293a 0a20 2020 2020  gree + 1):.     
+0003bf60: 2020 2020 2020 2067 6174 6865 7265 645f         gathered_
+0003bf70: 6174 6f6d 733a 2074 6f72 6368 2e54 656e  atoms: torch.Ten
+0003bf80: 736f 7220 3d20 6174 6f6d 735b 6465 675f  sor = atoms[deg_
+0003bf90: 6164 6a5f 6c69 7374 735b 6465 6720 2d20  adj_lists[deg - 
+0003bfa0: 315d 5d0a 2020 2020 2020 2020 2020 2020  1]].            
+0003bfb0: 2320 5375 6d20 616c 6f6e 6720 6e65 6967  # Sum along neig
+0003bfc0: 6862 6f72 7320 6173 2077 656c 6c20 6173  hbors as well as
+0003bfd0: 2073 656c 662c 2061 6e64 2073 746f 7265   self, and store
+0003bfe0: 0a20 2020 2020 2020 2020 2020 2073 756d  .            sum
+0003bff0: 6d65 645f 6174 6f6d 733a 2074 6f72 6368  med_atoms: torch
+0003c000: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
+0003c010: 7375 6d28 6761 7468 6572 6564 5f61 746f  sum(gathered_ato
+0003c020: 6d73 2c20 3129 0a20 2020 2020 2020 2020  ms, 1).         
+0003c030: 2020 2064 6567 5f73 756d 6d65 642e 6170     deg_summed.ap
+0003c040: 7065 6e64 2873 756d 6d65 645f 6174 6f6d  pend(summed_atom
+0003c050: 732e 6465 7461 6368 2829 2e6e 756d 7079  s.detach().numpy
+0003c060: 2829 290a 0a20 2020 2020 2020 2072 6574  ())..        ret
+0003c070: 7572 6e20 6465 675f 7375 6d6d 6564 0a0a  urn deg_summed..
+0003c080: 0a63 6c61 7373 2047 7261 7068 506f 6f6c  .class GraphPool
+0003c090: 286e 6e2e 4d6f 6475 6c65 293a 0a20 2020  (nn.Module):.   
+0003c0a0: 2022 2222 4120 4772 6170 6850 6f6f 6c20   """A GraphPool 
+0003c0b0: 6761 7468 6572 7320 6461 7461 2066 726f  gathers data fro
+0003c0c0: 6d20 6c6f 6361 6c20 6e65 6967 6862 6f72  m local neighbor
+0003c0d0: 686f 6f64 7320 6f66 2061 2067 7261 7068  hoods of a graph
+0003c0e0: 2e0a 0a20 2020 2054 6869 7320 6c61 7965  ...    This laye
+0003c0f0: 7220 646f 6573 2061 206d 6178 2d70 6f6f  r does a max-poo
+0003c100: 6c69 6e67 206f 7665 7220 7468 6520 6665  ling over the fe
+0003c110: 6174 7572 6520 7665 6374 6f72 7320 6f66  ature vectors of
+0003c120: 2061 746f 6d73 2069 6e20 610a 2020 2020   atoms in a.    
+0003c130: 6e65 6967 6862 6f72 686f 6f64 2e20 596f  neighborhood. Yo
+0003c140: 7520 6361 6e20 7468 696e 6b20 6f66 2074  u can think of t
+0003c150: 6869 7320 6c61 7965 7220 6173 2061 6e61  his layer as ana
+0003c160: 6c6f 676f 7573 2074 6f20 6120 6d61 782d  logous to a max-
+0003c170: 706f 6f6c 696e 670a 2020 2020 6c61 7965  pooling.    laye
+0003c180: 7220 666f 7220 3244 2063 6f6e 766f 6c75  r for 2D convolu
+0003c190: 7469 6f6e 7320 6275 7420 7768 6963 6820  tions but which 
+0003c1a0: 6f70 6572 6174 6573 206f 6e20 6772 6170  operates on grap
+0003c1b0: 6873 2069 6e73 7465 6164 2e20 5468 6973  hs instead. This
+0003c1c0: 0a20 2020 2074 6563 686e 6971 7565 2069  .    technique i
+0003c1d0: 7320 6465 7363 7269 6265 6420 696e 205b  s described in [
+0003c1e0: 315d 5f2e 0a0a 2020 2020 4578 616d 706c  1]_...    Exampl
+0003c1f0: 650a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  e.    --------. 
+0003c200: 2020 203e 3e3e 2069 6d70 6f72 7420 6465     >>> import de
+0003c210: 6570 6368 656d 2061 7320 6463 0a20 2020  epchem as dc.   
+0003c220: 203e 3e3e 2069 6d70 6f72 7420 6e75 6d70   >>> import nump
+0003c230: 7920 6173 206e 700a 2020 2020 3e3e 3e20  y as np.    >>> 
+0003c240: 696d 706f 7274 2064 6565 7063 6865 6d2e  import deepchem.
+0003c250: 6d6f 6465 6c73 2e74 6f72 6368 5f6d 6f64  models.torch_mod
+0003c260: 656c 732e 6c61 7965 7273 2061 7320 746f  els.layers as to
+0003c270: 7263 685f 6c61 7965 7273 0a20 2020 203e  rch_layers.    >
+0003c280: 3e3e 206e 5f61 746f 6d73 203d 2034 2020  >> n_atoms = 4  
+0003c290: 2320 496e 2043 4343 2061 6e64 2043 2c20  # In CCC and C, 
+0003c2a0: 7468 6572 6520 6172 6520 3420 6174 6f6d  there are 4 atom
+0003c2b0: 730a 2020 2020 3e3e 3e20 7261 775f 736d  s.    >>> raw_sm
+0003c2c0: 696c 6573 203d 205b 2743 4343 272c 2027  iles = ['CCC', '
+0003c2d0: 4327 5d0a 2020 2020 3e3e 3e20 6672 6f6d  C'].    >>> from
+0003c2e0: 2072 646b 6974 2069 6d70 6f72 7420 4368   rdkit import Ch
+0003c2f0: 656d 0a20 2020 203e 3e3e 206d 6f6c 7320  em.    >>> mols 
+0003c300: 3d20 5b43 6865 6d2e 4d6f 6c46 726f 6d53  = [Chem.MolFromS
+0003c310: 6d69 6c65 7328 7329 2066 6f72 2073 2069  miles(s) for s i
+0003c320: 6e20 7261 775f 736d 696c 6573 5d0a 2020  n raw_smiles].  
+0003c330: 2020 3e3e 3e20 6665 6174 7572 697a 6572    >>> featurizer
+0003c340: 203d 2064 632e 6665 6174 2e67 7261 7068   = dc.feat.graph
+0003c350: 5f66 6561 7475 7265 732e 436f 6e76 4d6f  _features.ConvMo
+0003c360: 6c46 6561 7475 7269 7a65 7228 290a 2020  lFeaturizer().  
+0003c370: 2020 3e3e 3e20 6d6f 6c73 203d 2066 6561    >>> mols = fea
+0003c380: 7475 7269 7a65 722e 6665 6174 7572 697a  turizer.featuriz
+0003c390: 6528 6d6f 6c73 290a 2020 2020 3e3e 3e20  e(mols).    >>> 
+0003c3a0: 6d75 6c74 695f 6d6f 6c20 3d20 6463 2e66  multi_mol = dc.f
+0003c3b0: 6561 742e 6d6f 6c5f 6772 6170 6873 2e43  eat.mol_graphs.C
+0003c3c0: 6f6e 764d 6f6c 2e61 6767 6c6f 6d65 7261  onvMol.agglomera
+0003c3d0: 7465 5f6d 6f6c 7328 6d6f 6c73 290a 2020  te_mols(mols).  
+0003c3e0: 2020 3e3e 3e20 6174 6f6d 5f66 6561 7475    >>> atom_featu
+0003c3f0: 7265 7320 3d20 6d75 6c74 695f 6d6f 6c2e  res = multi_mol.
+0003c400: 6765 745f 6174 6f6d 5f66 6561 7475 7265  get_atom_feature
+0003c410: 7328 292e 6173 7479 7065 286e 702e 666c  s().astype(np.fl
+0003c420: 6f61 7433 3229 0a20 2020 203e 3e3e 2064  oat32).    >>> d
+0003c430: 6567 7265 655f 736c 6963 6520 3d20 6d75  egree_slice = mu
+0003c440: 6c74 695f 6d6f 6c2e 6465 675f 736c 6963  lti_mol.deg_slic
+0003c450: 650a 2020 2020 3e3e 3e20 6d65 6d62 6572  e.    >>> member
+0003c460: 7368 6970 203d 206d 756c 7469 5f6d 6f6c  ship = multi_mol
+0003c470: 2e6d 656d 6265 7273 6869 700a 2020 2020  .membership.    
+0003c480: 3e3e 3e20 6465 675f 6164 6a73 203d 206d  >>> deg_adjs = m
+0003c490: 756c 7469 5f6d 6f6c 2e67 6574 5f64 6567  ulti_mol.get_deg
+0003c4a0: 5f61 646a 6163 656e 6379 5f6c 6973 7473  _adjacency_lists
+0003c4b0: 2829 5b31 3a5d 0a20 2020 203e 3e3e 2061  ()[1:].    >>> a
+0003c4c0: 7267 7320 3d20 5b61 746f 6d5f 6665 6174  rgs = [atom_feat
+0003c4d0: 7572 6573 2c20 6465 6772 6565 5f73 6c69  ures, degree_sli
+0003c4e0: 6365 2c20 6d65 6d62 6572 7368 6970 5d20  ce, membership] 
+0003c4f0: 2b20 6465 675f 6164 6a73 0a20 2020 203e  + deg_adjs.    >
+0003c500: 3e3e 2072 6573 756c 7420 3d20 746f 7263  >> result = torc
+0003c510: 685f 6c61 7965 7273 2e47 7261 7068 506f  h_layers.GraphPo
+0003c520: 6f6c 2829 2861 7267 7329 0a20 2020 203e  ol()(args).    >
+0003c530: 3e3e 2074 7970 6528 7265 7375 6c74 290a  >> type(result).
+0003c540: 2020 2020 3c63 6c61 7373 2027 746f 7263      <class 'torc
+0003c550: 682e 5465 6e73 6f72 273e 0a20 2020 203e  h.Tensor'>.    >
+0003c560: 3e3e 2072 6573 756c 742e 7368 6170 650a  >> result.shape.
+0003c570: 2020 2020 746f 7263 682e 5369 7a65 285b      torch.Size([
+0003c580: 342c 2037 355d 290a 0a20 2020 2052 6566  4, 75])..    Ref
+0003c590: 6572 656e 6365 730a 2020 2020 2d2d 2d2d  erences.    ----
+0003c5a0: 2d2d 2d2d 2d2d 0a20 2020 202e 2e20 5b31  ------.    .. [1
+0003c5b0: 5d20 4475 7665 6e61 7564 2c20 4461 7669  ] Duvenaud, Davi
+0003c5c0: 6420 4b2e 2c20 6574 2061 6c2e 2022 436f  d K., et al. "Co
+0003c5d0: 6e76 6f6c 7574 696f 6e61 6c20 6e65 7477  nvolutional netw
+0003c5e0: 6f72 6b73 206f 6e20 6772 6170 6873 2066  orks on graphs f
+0003c5f0: 6f72 0a20 2020 2020 2020 206c 6561 726e  or.        learn
+0003c600: 696e 6720 6d6f 6c65 6375 6c61 7220 6669  ing molecular fi
+0003c610: 6e67 6572 7072 696e 7473 2e22 2041 6476  ngerprints." Adv
+0003c620: 616e 6365 7320 696e 206e 6575 7261 6c20  ances in neural 
+0003c630: 696e 666f 726d 6174 696f 6e20 7072 6f63  information proc
+0003c640: 6573 7369 6e67 0a20 2020 2020 2020 2073  essing.        s
+0003c650: 7973 7465 6d73 2e20 3230 3135 2e20 6874  ystems. 2015. ht
+0003c660: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+0003c670: 6162 732f 3135 3039 2e30 3932 3932 0a0a  abs/1509.09292..
+0003c680: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+0003c690: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0003c6a0: 6d69 6e5f 6465 6772 6565 3a20 696e 7420  min_degree: int 
+0003c6b0: 3d20 302c 206d 6178 5f64 6567 7265 653a  = 0, max_degree:
+0003c6c0: 2069 6e74 203d 2031 302c 202a 2a6b 7761   int = 10, **kwa
+0003c6d0: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
+0003c6e0: 2249 6e69 7469 616c 697a 6520 7468 6973  "Initialize this
+0003c6f0: 206c 6179 6572 0a0a 2020 2020 2020 2020   layer..        
+0003c700: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0003c710: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0003c720: 2020 2020 2020 6d69 6e5f 6465 673a 2069        min_deg: i
+0003c730: 6e74 2c20 6f70 7469 6f6e 616c 2028 6465  nt, optional (de
+0003c740: 6661 756c 7420 3029 0a20 2020 2020 2020  fault 0).       
+0003c750: 2020 2020 2054 6865 206d 696e 696d 756d       The minimum
+0003c760: 2061 6c6c 6f77 6564 2064 6567 7265 6520   allowed degree 
+0003c770: 666f 7220 6561 6368 2067 7261 7068 206e  for each graph n
+0003c780: 6f64 652e 0a20 2020 2020 2020 206d 6178  ode..        max
+0003c790: 5f64 6567 3a20 696e 742c 206f 7074 696f  _deg: int, optio
+0003c7a0: 6e61 6c20 2864 6566 6175 6c74 2031 3029  nal (default 10)
+0003c7b0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0003c7c0: 206d 6178 696d 756d 2061 6c6c 6f77 6564   maximum allowed
+0003c7d0: 2064 6567 7265 6520 666f 7220 6561 6368   degree for each
+0003c7e0: 2067 7261 7068 206e 6f64 652e 204e 6f74   graph node. Not
+0003c7f0: 6520 7468 6174 2074 6869 730a 2020 2020  e that this.    
+0003c800: 2020 2020 2020 2020 6973 2073 6574 2074          is set t
+0003c810: 6f20 3130 2074 6f20 6861 6e64 6c65 2063  o 10 to handle c
+0003c820: 6f6d 706c 6578 206d 6f6c 6563 756c 6573  omplex molecules
+0003c830: 2028 736f 6d65 206f 7267 616e 6f6d 6574   (some organomet
+0003c840: 616c 6c69 630a 2020 2020 2020 2020 2020  allic.          
+0003c850: 2020 636f 6d70 6f75 6e64 7320 6861 7665    compounds have
+0003c860: 2073 7472 616e 6765 2073 7472 7563 7475   strange structu
+0003c870: 7265 7329 2e20 4966 2079 6f75 2772 6520  res). If you're 
+0003c880: 7573 696e 6720 7468 6973 2066 6f72 0a20  using this for. 
+0003c890: 2020 2020 2020 2020 2020 206e 6f6e 2d6d             non-m
+0003c8a0: 6f6c 6563 756c 6172 2061 7070 6c69 6361  olecular applica
+0003c8b0: 7469 6f6e 732c 2079 6f75 206d 6179 206e  tions, you may n
+0003c8c0: 6565 6420 746f 2073 6574 2074 6869 7320  eed to set this 
+0003c8d0: 6d75 6368 2068 6967 6865 720a 2020 2020  much higher.    
+0003c8e0: 2020 2020 2020 2020 6465 7065 6e64 696e          dependin
+0003c8f0: 6720 6f6e 2079 6f75 7220 6461 7461 7365  g on your datase
+0003c900: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
+0003c910: 2020 2020 2020 2073 7570 6572 2847 7261         super(Gra
+0003c920: 7068 506f 6f6c 2c20 7365 6c66 292e 5f5f  phPool, self).__
+0003c930: 696e 6974 5f5f 282a 2a6b 7761 7267 7329  init__(**kwargs)
+0003c940: 0a20 2020 2020 2020 2073 656c 662e 6d69  .        self.mi
+0003c950: 6e5f 6465 6772 6565 3a20 696e 7420 3d20  n_degree: int = 
+0003c960: 6d69 6e5f 6465 6772 6565 0a20 2020 2020  min_degree.     
+0003c970: 2020 2073 656c 662e 6d61 785f 6465 6772     self.max_degr
+0003c980: 6565 3a20 696e 7420 3d20 6d61 785f 6465  ee: int = max_de
+0003c990: 6772 6565 0a0a 2020 2020 6465 6620 6765  gree..    def ge
+0003c9a0: 745f 636f 6e66 6967 2873 656c 6629 202d  t_config(self) -
+0003c9b0: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
+0003c9c0: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+0003c9d0: 6e73 2061 2073 7472 696e 6720 7265 7072  ns a string repr
+0003c9e0: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
+0003c9f0: 6520 6f62 6a65 6374 2e0a 0a20 2020 2020  e object...     
+0003ca00: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0003ca10: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0003ca20: 2020 2020 7374 723a 2041 2073 7472 696e      str: A strin
+0003ca30: 6720 7468 6174 2063 6f6e 7461 696e 7320  g that contains 
+0003ca40: 7468 6520 636c 6173 7320 6e61 6d65 2066  the class name f
+0003ca50: 6f6c 6c6f 7765 6420 6279 2074 6865 2076  ollowed by the v
+0003ca60: 616c 7565 7320 6f66 2069 7473 2069 6e73  alues of its ins
+0003ca70: 7461 6e63 6520 7661 7269 6162 6c65 2e0a  tance variable..
+0003ca80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0003ca90: 2020 2020 2320 666c 616b 6538 3a20 6e6f      # flake8: no
+0003caa0: 7161 0a20 2020 2020 2020 2072 6574 7572  qa.        retur
+0003cab0: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
+0003cac0: 6627 7b73 656c 662e 5f5f 636c 6173 735f  f'{self.__class_
+0003cad0: 5f2e 5f5f 6e61 6d65 5f5f 7d28 6d69 6e5f  _.__name__}(min_
+0003cae0: 6465 6772 6565 3a7b 7365 6c66 2e6d 696e  degree:{self.min
+0003caf0: 5f64 6567 7265 657d 2c6d 6178 5f64 6567  _degree},max_deg
+0003cb00: 7265 653a 7b73 656c 662e 6d61 785f 6465  ree:{self.max_de
+0003cb10: 6772 6565 7d29 270a 2020 2020 2020 2020  gree})'.        
+0003cb20: 290a 0a20 2020 2064 6566 2066 6f72 7761  )..    def forwa
+0003cb30: 7264 2873 656c 662c 2069 6e70 7574 733a  rd(self, inputs:
+0003cb40: 204c 6973 745b 6e70 2e6e 6461 7272 6179   List[np.ndarray
+0003cb50: 5d29 202d 3e20 746f 7263 682e 5465 6e73  ]) -> torch.Tens
+0003cb60: 6f72 3a0a 2020 2020 2020 2020 2222 220a  or:.        """.
+0003cb70: 2020 2020 2020 2020 5468 6520 666f 7277          The forw
+0003cb80: 6172 6420 7061 7373 2070 6572 666f 726d  ard pass perform
+0003cb90: 7320 6d61 782d 706f 6f6c 696e 6720 6f76  s max-pooling ov
+0003cba0: 6572 2074 6865 2066 6561 7475 7265 2076  er the feature v
+0003cbb0: 6563 746f 7273 206f 6620 6174 6f6d 7320  ectors of atoms 
+0003cbc0: 696e 2061 206e 6569 6768 626f 7268 6f6f  in a neighborhoo
+0003cbd0: 642e 0a0a 2020 2020 2020 2020 5061 7261  d...        Para
+0003cbe0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0003cbf0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0003cc00: 2020 696e 7075 7473 3a20 4c69 7374 5b6e    inputs: List[n
+0003cc10: 702e 6e64 6172 7261 795d 0a20 2020 2020  p.ndarray].     
+0003cc20: 2020 2053 686f 756c 6420 636f 6e74 6169     Should contai
+0003cc30: 6e20 6174 6f6d 2066 6561 7475 7265 7320  n atom features 
+0003cc40: 616e 6420 6172 7261 7973 2064 6573 6372  and arrays descr
+0003cc50: 6962 696e 6720 6772 6170 6820 746f 706f  ibing graph topo
+0003cc60: 6c6f 6779 2e0a 0a20 2020 2020 2020 2052  logy...        R
+0003cc70: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0003cc80: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0003cc90: 746f 7263 682e 5465 6e73 6f72 0a20 2020  torch.Tensor.   
+0003cca0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0003ccb0: 2061 746f 6d5f 6665 6174 7572 6573 203d   atom_features =
+0003ccc0: 2074 6f72 6368 2e74 656e 736f 7228 696e   torch.tensor(in
+0003ccd0: 7075 7473 5b30 5d29 0a20 2020 2020 2020  puts[0]).       
+0003cce0: 2064 6567 5f73 6c69 6365 3a20 6e70 2e6e   deg_slice: np.n
+0003ccf0: 6461 7272 6179 203d 2069 6e70 7574 735b  darray = inputs[
+0003cd00: 315d 0a20 2020 2020 2020 2064 6567 5f61  1].        deg_a
+0003cd10: 646a 5f6c 6973 7473 3a20 4c69 7374 5b6e  dj_lists: List[n
+0003cd20: 702e 6e64 6172 7261 795d 203d 2069 6e70  p.ndarray] = inp
+0003cd30: 7574 735b 333a 5d0a 0a20 2020 2020 2020  uts[3:]..       
+0003cd40: 2023 2050 6572 666f 726d 2074 6865 206d   # Perform the m
+0003cd50: 6f6c 2067 6174 6865 720a 2020 2020 2020  ol gather.      
+0003cd60: 2020 2320 6174 6f6d 5f66 6561 7475 7265    # atom_feature
+0003cd70: 7320 3d20 6772 6170 685f 706f 6f6c 2861  s = graph_pool(a
+0003cd80: 746f 6d5f 6665 6174 7572 6573 2c20 6465  tom_features, de
+0003cd90: 675f 6164 6a5f 6c69 7374 732c 2064 6567  g_adj_lists, deg
+0003cda0: 5f73 6c69 6365 2c0a 2020 2020 2020 2020  _slice,.        
+0003cdb0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0003cdc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0003cdd0: 662e 6d61 785f 6465 6772 6565 2c20 7365  f.max_degree, se
+0003cde0: 6c66 2e6d 696e 5f64 6567 7265 6529 0a0a  lf.min_degree)..
+0003cdf0: 2020 2020 2020 2020 2364 6567 5f6d 6178          #deg_max
+0003ce00: 6564 203d 2028 7365 6c66 2e6d 6178 5f64  ed = (self.max_d
+0003ce10: 6567 7265 6520 2b20 3120 2d20 7365 6c66  egree + 1 - self
+0003ce20: 2e6d 696e 5f64 6567 7265 6529 202a 205b  .min_degree) * [
+0003ce30: 4e6f 6e65 5d0a 2020 2020 2020 2020 6465  None].        de
+0003ce40: 675f 6d61 7865 6420 3d20 5b5d 0a0a 2020  g_maxed = []..  
+0003ce50: 2020 2020 2020 7370 6c69 745f 6665 6174        split_feat
+0003ce60: 7572 6573 3a20 5475 706c 655b 746f 7263  ures: Tuple[torc
+0003ce70: 682e 5465 6e73 6f72 2c0a 2020 2020 2020  h.Tensor,.      
+0003ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003ce90: 2020 2020 2020 2020 2e2e 2e5d 203d 2074          ...] = t
+0003cea0: 6f72 6368 2e73 706c 6974 2861 746f 6d5f  orch.split(atom_
+0003ceb0: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
+0003cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003cee0: 2020 2020 2020 2020 2020 2028 6465 675f             (deg_
+0003cef0: 736c 6963 655b 3a2c 2031 5d29 2e74 6f6c  slice[:, 1]).tol
+0003cf00: 6973 7428 2929 0a20 2020 2020 2020 2066  ist()).        f
+0003cf10: 6f72 2064 6567 2069 6e20 7261 6e67 6528  or deg in range(
+0003cf20: 312c 2073 656c 662e 6d61 785f 6465 6772  1, self.max_degr
+0003cf30: 6565 202b 2031 293a 0a20 2020 2020 2020  ee + 1):.       
+0003cf40: 2020 2020 2023 2047 6574 2073 656c 6620       # Get self 
+0003cf50: 6174 6f6d 730a 2020 2020 2020 2020 2020  atoms.          
+0003cf60: 2020 7365 6c66 5f61 746f 6d73 3a20 746f    self_atoms: to
+0003cf70: 7263 682e 5465 6e73 6f72 203d 2073 706c  rch.Tensor = spl
+0003cf80: 6974 5f66 6561 7475 7265 735b 6465 6720  it_features[deg 
+0003cf90: 2d20 7365 6c66 2e6d 696e 5f64 6567 7265  - self.min_degre
+0003cfa0: 655d 0a0a 2020 2020 2020 2020 2020 2020  e]..            
+0003cfb0: 6966 2064 6567 5f61 646a 5f6c 6973 7473  if deg_adj_lists
+0003cfc0: 5b64 6567 202d 2031 5d2e 7368 6170 655b  [deg - 1].shape[
+0003cfd0: 305d 203d 3d20 303a 0a20 2020 2020 2020  0] == 0:.       
+0003cfe0: 2020 2020 2020 2020 2023 2054 6865 7265           # There
+0003cff0: 2061 7265 206e 6f20 6e65 6967 6862 6f72   are no neighbor
+0003d000: 7320 6f66 2074 6869 7320 6465 6772 6565  s of this degree
+0003d010: 2c20 736f 206a 7573 7420 6372 6561 7465  , so just create
+0003d020: 2061 6e20 656d 7074 7920 7465 6e73 6f72   an empty tensor
+0003d030: 2064 6972 6563 746c 792e 0a20 2020 2020   directly..     
+0003d040: 2020 2020 2020 2020 2020 206d 6178 6564             maxed
+0003d050: 5f61 746f 6d73 3a20 746f 7263 682e 5465  _atoms: torch.Te
+0003d060: 6e73 6f72 203d 2074 6f72 6368 2e7a 6572  nsor = torch.zer
+0003d070: 6f73 280a 2020 2020 2020 2020 2020 2020  os(.            
+0003d080: 2020 2020 2020 2020 2830 2c20 7365 6c66          (0, self
+0003d090: 5f61 746f 6d73 2e73 6861 7065 5b2d 315d  _atoms.shape[-1]
+0003d0a0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0003d0b0: 2020 2064 6567 5f6d 6178 6564 2e61 7070     deg_maxed.app
+0003d0c0: 656e 6428 6d61 7865 645f 6174 6f6d 7329  end(maxed_atoms)
+0003d0d0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0003d0e0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0003d0f0: 2020 2023 2045 7870 616e 6420 6469 6d73     # Expand dims
+0003d100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003d110: 2073 656c 665f 6174 6f6d 7320 3d20 746f   self_atoms = to
+0003d120: 7263 682e 756e 7371 7565 657a 6528 7365  rch.unsqueeze(se
+0003d130: 6c66 5f61 746f 6d73 2c20 3129 0a0a 2020  lf_atoms, 1)..  
+0003d140: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0003d150: 616c 7761 7973 2064 6567 2d31 2066 6f72  always deg-1 for
+0003d160: 2064 6567 5f61 646a 5f6c 6973 7473 0a20   deg_adj_lists. 
+0003d170: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0003d180: 6174 6865 7265 645f 6174 6f6d 733a 2074  athered_atoms: t
+0003d190: 6f72 6368 2e54 656e 736f 7220 3d20 6174  orch.Tensor = at
+0003d1a0: 6f6d 5f66 6561 7475 7265 735b 6465 675f  om_features[deg_
+0003d1b0: 6164 6a5f 6c69 7374 735b 6465 6720 2d0a  adj_lists[deg -.
+0003d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d200: 2020 2020 2020 2020 2020 2031 5d5d 0a20             1]]. 
+0003d210: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0003d220: 6174 6865 7265 645f 6174 6f6d 7320 3d20  athered_atoms = 
+0003d230: 746f 7263 682e 636f 6e63 6174 285b 7365  torch.concat([se
+0003d240: 6c66 5f61 746f 6d73 2c20 6761 7468 6572  lf_atoms, gather
+0003d250: 6564 5f61 746f 6d73 5d2c 2031 290a 0a20  ed_atoms], 1).. 
+0003d260: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0003d270: 6178 5f61 746f 6d73 3a20 7475 706c 6520  ax_atoms: tuple 
+0003d280: 3d20 746f 7263 682e 6d61 7828 6761 7468  = torch.max(gath
+0003d290: 6572 6564 5f61 746f 6d73 2c20 3129 0a20  ered_atoms, 1). 
+0003d2a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0003d2b0: 6567 5f6d 6178 6564 2e61 7070 656e 6428  eg_maxed.append(
+0003d2c0: 6d61 785f 6174 6f6d 735b 305d 290a 0a20  max_atoms[0]).. 
+0003d2d0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+0003d2e0: 696e 5f64 6567 7265 6520 3d3d 2030 3a0a  in_degree == 0:.
+0003d2f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003d300: 5f61 746f 6d73 203d 2073 706c 6974 5f66  _atoms = split_f
+0003d310: 6561 7475 7265 735b 305d 0a20 2020 2020  eatures[0].     
+0003d320: 2020 2020 2020 2064 6567 5f6d 6178 6564         deg_maxed
+0003d330: 2e69 6e73 6572 7428 302c 2073 656c 665f  .insert(0, self_
+0003d340: 6174 6f6d 7329 0a0a 2020 2020 2020 2020  atoms)..        
+0003d350: 7265 7475 726e 2074 6f72 6368 2e63 6f6e  return torch.con
+0003d360: 6361 7428 6465 675f 6d61 7865 642c 2030  cat(deg_maxed, 0
+0003d370: 290a                                     ).
```

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/lcnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/mat.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/megnet.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/modular.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/molgan.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/mpnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/pagtn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/progressive_multitask.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/readout.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/scscore.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/seqtoseq.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/text_cnn.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/torch_model.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/unet.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/unet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/torch_models/weavemodel_pytorch.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/torch_models/weavemodel_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/trainer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/trainer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/models/wandblogger.py` & `deepchem-2.8.1.dev20240529195718/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/check_availability.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/defaults.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/dnasim.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/run_benchmark.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.8.1.dev20240529195718/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/rl/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/rl/a2c.py` & `deepchem-2.8.1.dev20240529195718/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.8.1.dev20240529195718/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/rl/envs/tictactoe.py` & `deepchem-2.8.1.dev20240529195718/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/rl/ppo.py` & `deepchem-2.8.1.dev20240529195718/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/rl/torch_rl/torch_a2c.py` & `deepchem-2.8.1.dev20240529195718/deepchem/rl/torch_rl/torch_a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/rl/torch_rl/torch_ppo.py` & `deepchem-2.8.1.dev20240529195718/deepchem/rl/torch_rl/torch_ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/splits/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/splits/splitters.py` & `deepchem-2.8.1.dev20240529195718/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/splits/task_splitter.py` & `deepchem-2.8.1.dev20240529195718/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/trans/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/trans/duplicate.py` & `deepchem-2.8.1.dev20240529195718/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/trans/transformers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/attribute_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/attribute_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/batch_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/conformers.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/data_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/debug_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/api/getxc.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/api/getxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/api/parser.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/api/parser.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/config.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/config.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/data/datastruct.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/data/datastruct.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/df/base_df.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/df/base_df.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/grid/base_grid.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/grid/base_grid.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/grid/radial_grid.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/grid/radial_grid.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/base_hamilton.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/base_hamilton.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/intor/lattice.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/intor/lattice.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/hamilton/orbparams.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/hamilton/orbparams.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/qccalc/base_qccalc.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/qccalc/base_qccalc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/qccalc/hf.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/qccalc/hf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/qccalc/scf_qccalc.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/qccalc/scf_qccalc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/system/base_system.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/system/base_system.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/xc/base_xc.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/xc/base_xc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/xc/libxc.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/xc/libxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dft_utils/xc/libxc_wrapper.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dft_utils/xc/libxc_wrapper.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/dftutils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/__init__.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/bcast.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/bcast.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/editable_module.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/editable_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/grad.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/grad.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/linop.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/linop.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/misc.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/misc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/equilibrium.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/equilibrium.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/jacobian.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/jacobian.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/minimizer.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/minimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/rootfinder.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/rootfinder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/optimize/rootsolver.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/optimize/rootsolver.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/pure_function.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/pure_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/solve.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/solve.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/differentiation_utils/symeig.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/differentiation_utils/symeig.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/docking_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/electron_sampler.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/equivariance_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/equivariance_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/evaluate.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/fake_data_generator.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/fragment_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/genomics_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/geometry_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/graph_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/grover.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/hash_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/misc_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/noncovalent_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/pdbqt_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/periodic_table_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/periodic_table_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/pytorch_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/rdkit_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/safeops_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/safeops_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/save.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/sequence_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_attribute_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_attribute_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_batch_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_batch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_data_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_dft_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_dft_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_dftutils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_differentiation_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_differentiation_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_equivariance_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_equivariance_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_evaluate.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_grover.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_periodic_table_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_periodic_table_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_pytorch_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_safe_ops_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_safe_ops_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/typing.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/vina_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem/utils/voxel_utils.py` & `deepchem-2.8.1.dev20240529195718/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem.egg-info/PKG-INFO` & `deepchem-2.8.1.dev20240529195718/deepchem.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.8.1.dev20240524164912
+Version: 2.8.1.dev20240529195718
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.8.1.dev20240524164912/deepchem.egg-info/SOURCES.txt` & `deepchem-2.8.1.dev20240529195718/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/setup.cfg` & `deepchem-2.8.1.dev20240529195718/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240524164912/setup.py` & `deepchem-2.8.1.dev20240529195718/setup.py`

 * *Files identical despite different names*

