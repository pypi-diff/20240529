# Comparing `tmp/sae_lens-2.1.3.tar.gz` & `tmp/sae_lens-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-2.1.3.tar", max compression
+gzip compressed data, was "sae_lens-3.0.0.tar", max compression
```

## Comparing `sae_lens-2.1.3.tar` & `sae_lens-3.0.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     1069 2024-05-15 20:51:54.662037 sae_lens-2.1.3/LICENSE
--rw-r--r--   0        0        0     3381 2024-05-15 20:51:54.662037 sae_lens-2.1.3/README.md
--rw-r--r--   0        0        0     2041 2024-05-15 20:51:56.206061 sae_lens-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     1098 2024-05-15 20:51:56.206061 sae_lens-2.1.3/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6844 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    20340 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     4052 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/batching.py
--rw-r--r--   0        0        0     6065 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    16237 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/config.py
--rw-r--r--   0        0        0     8229 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     4377 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1280 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     5574 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/optim.py
--rw-r--r--   0        0        0     5401 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/pretokenize_runner.py
--rw-r--r--   0        0        0     8403 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2424 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    20000 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     1932 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    18456 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    31427 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0      423 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/utils.py
--rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 15:48:37.244262 sae_lens-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3381 2024-05-28 15:48:37.244262 sae_lens-3.0.0/README.md
+-rw-r--r--   0        0        0     2068 2024-05-28 15:48:38.976267 sae_lens-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-05-28 15:48:38.976267 sae_lens-3.0.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0     3320 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    12561 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/analysis/hooked_sae_transformer.py
+-rw-r--r--   0        0        0    17062 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20406 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     4052 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/batching.py
+-rw-r--r--   0        0        0     6047 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/cache_activations_runner.py
+-rw-r--r--   0        0        0    24486 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/config.py
+-rw-r--r--   0        0        0    16161 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/dashboard_runner.py
+-rw-r--r--   0        0        0     7216 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/evals.py
+-rw-r--r--   0        0        0     1320 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/load_model.py
+-rw-r--r--   0        0        0     5383 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/pretokenize_runner.py
+-rw-r--r--   0        0        0     4833 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0    15121 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/sae.py
+-rw-r--r--   0        0        0     6972 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/sae_training_runner.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     6506 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     4752 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0     1783 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/toy_model_runner.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    21723 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     3779 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     5585 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0    16114 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/training/sae.py
+-rw-r--r--   0        0        0    14674 2024-05-28 15:48:37.256262 sae_lens-3.0.0/sae_lens/training/sae_trainer.py
+-rw-r--r--   0        0        0    18456 2024-05-28 15:48:37.260262 sae_lens-3.0.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0     4850 2024-05-28 15:48:37.260262 sae_lens-3.0.0/sae_lens/training/train_toy_sae.py
+-rw-r--r--   0        0        0    15532 2024-05-28 15:48:37.260262 sae_lens-3.0.0/sae_lens/training/training_sae.py
+-rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-3.0.0/PKG-INFO
```

### Comparing `sae_lens-2.1.3/LICENSE` & `sae_lens-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.3/README.md` & `sae_lens-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.3/pyproject.toml` & `sae_lens-3.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "2.1.3"
+version = "3.0.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
@@ -46,14 +46,15 @@
 flake8 = "7.0.0"
 isort = "5.13.2"
 pyright = "^1.1.351"
 mamba-lens = "^0.0.4"
 ansible-lint = { version = "^24.2.3", markers = "platform_system != 'Windows'" }
 botocore = "^1.34.101"
 boto3 = "^1.34.101"
+docstr-coverage = "^2.3.2"
 
 [tool.poetry.extras]
 mamba = ["mamba-lens"]
 
 
 [tool.isort]
 profile = "black"
```

### Comparing `sae_lens-2.1.3/sae_lens/analysis/dashboard_runner.py` & `sae_lens-3.0.0/sae_lens/dashboard_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,414 +1,409 @@
-import os
-from typing import Any, Optional, cast
+# this code is stale. We may revive it soon.
+# import os
+# from typing import Any, Optional, cast
+
+# # set TOKENIZERS_PARALLELISM to false to avoid warnings
+# os.environ["TOKENIZERS_PARALLELISM"] = "false"
+# import shutil
+# import time
+# import uuid
+
+# import pandas as pd
+# import plotly
+# import plotly.express as px
+# import torch
+# import wandb
+# from sae_vis.data_config_classes import (
+#     ActsHistogramConfig,
+#     Column,
+#     FeatureTablesConfig,
+#     SaeVisConfig,
+#     SaeVisLayoutConfig,
+#     SequencesConfig,
+# )
+# from sae_vis.data_fetching_fns import get_feature_data
+# from torch.nn.functional import cosine_similarity
+# from tqdm import tqdm
+# from transformer_lens import HookedTransformer
+
+# from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
+
+
+# class DashboardRunner:
+
+#     model: HookedTransformer | None = None
+
+#     def __init__(
+#         self,
+#         sae_path: Optional[str] = None,
+#         dashboard_parent_folder: str = "./feature_dashboards",
+#         wandb_artifact_path: Optional[str] = None,
+#         init_session: bool = True,
+#         # token pars
+#         n_batches_to_sample_from: int = 2**12,
+#         n_prompts_to_select: int = 4096 * 6,
+#         # sampling pars
+#         n_features_at_a_time: int = 1024,
+#         max_batch_size: int = 256,
+#         buffer_tokens: int = 8,
+#         # util pars
+#         use_wandb: bool = False,
+#         continue_existing_dashboard: bool = True,
+#         final_index: Optional[int] = None,
+#     ):
+#         """ """
+
+#         if wandb_artifact_path is not None:
+#             artifact_dir = f"artifacts/{wandb_artifact_path.split('/')[2]}"
+#             if not os.path.exists(artifact_dir):
+#                 print("Downloading artifact")
+#                 run = wandb.init()
+#                 assert run is not None  # keep pyright happy
+#                 artifact = run.use_artifact(wandb_artifact_path)
+#                 artifact_dir = artifact.download()
+#                 path_to_artifact = f"{artifact_dir}/{os.listdir(artifact_dir)[0]}"
+#                 # feature sparsity
+#                 feature_sparsity_path = self.get_feature_sparsity_path(
+#                     wandb_artifact_path
+#                 )
+#                 artifact = run.use_artifact(feature_sparsity_path)
+#                 artifact_dir = artifact.download()
+#                 # add it as a property
+#                 self.feature_sparsity = torch.load(
+#                     f"{artifact_dir}/{os.listdir(artifact_dir)[0]}"
+#                 )
+#             else:
+#                 print("Artifact already downloaded")
+#                 path_to_artifact = f"{artifact_dir}/{os.listdir(artifact_dir)[0]}"
+
+#                 feature_sparsity_path = self.get_feature_sparsity_path(
+#                     wandb_artifact_path
+#                 )
+#                 artifact_dir = f"artifacts/{feature_sparsity_path.split('/')[2]}"
+#                 feature_sparsity_file = os.listdir(artifact_dir)[0]
+#                 self.feature_sparsity = torch.load(
+#                     f"{artifact_dir}/{feature_sparsity_file}"
+#                 )
+
+#             self.sae_path = path_to_artifact
+#         else:
+#             assert sae_path is not None
+#             self.sae_path = sae_path
+#             self.feature_sparsity = None
+
+#         if init_session:
+#             self.init_sae_session()
+
+#         self.n_features_at_a_time = n_features_at_a_time
+#         self.max_batch_size = max_batch_size
+#         self.buffer_tokens = buffer_tokens
+#         self.use_wandb = use_wandb
+#         self.final_index = (
+#             final_index
+#             if final_index is not None
+#             else self.sparse_autoencoder.cfg.d_sae
+#         )
+#         self.n_batches_to_sample_from = n_batches_to_sample_from
+#         self.n_prompts_to_select = n_prompts_to_select
+
+#         # Deal with file structure
+#         if not os.path.exists(dashboard_parent_folder):
+#             os.makedirs(dashboard_parent_folder)
+
+#         self.dashboard_folder = (
+#             f"{dashboard_parent_folder}/{self.get_dashboard_folder_name()}"
+#         )
+#         if not os.path.exists(self.dashboard_folder):
+#             os.makedirs(self.dashboard_folder)
+
+#         if not continue_existing_dashboard:
+#             # check if there are files there and if so abort
+#             if len(os.listdir(self.dashboard_folder)) > 0:
+#                 raise ValueError("Dashboard folder not empty. Aborting.")
+
+#     def get_feature_sparsity_path(self, wandb_artifact_path: str):
+#         prefix = wandb_artifact_path.split(":")[0]
+#         return f"{prefix}_log_feature_sparsity:v9"
+
+#     def get_dashboard_folder_name(self):
+#         model = self.sparse_autoencoder.cfg.model_name
+#         hook_point = self.sparse_autoencoder.cfg.hook_point
+#         d_sae = self.sparse_autoencoder.cfg.d_sae
+#         dashboard_folder_name = f"{model}_{hook_point}_{d_sae}"
+
+#         return dashboard_folder_name
+
+#     def init_sae_session(self):
+#         (
+#             self.model,  # type: ignore
+#             self.sparse_autoencoder,
+#             self.activation_store,
+#         ) = LMSparseAutoencoderSessionloader.load_pretrained_sae(self.sae_path)
+
+#     def get_tokens(
+#         self, n_batches_to_sample_from: int = 2**12, n_prompts_to_select: int = 4096 * 6
+#     ):
+#         """
+#         Get the tokens needed for dashboard generation.
+#         """
+
+#         all_tokens_list = []
+#         pbar = tqdm(range(n_batches_to_sample_from))
+#         for _ in pbar:
+#             batch_tokens = self.activation_store.get_batch_tokens()
+#             batch_tokens = batch_tokens[torch.randperm(batch_tokens.shape[0])][
+#                 : batch_tokens.shape[0]
+#             ]
+#             all_tokens_list.append(batch_tokens)
+
+#         all_tokens = torch.cat(all_tokens_list, dim=0)
+#         all_tokens = all_tokens[torch.randperm(all_tokens.shape[0])]
+#         return all_tokens[:n_prompts_to_select]
+
+#     def get_index_to_resume_from(self):
+#         i = 0
+#         assert self.n_features is not None  # keep pyright happy
+#         for i in range(self.n_features):
+#             if not os.path.exists(f"{self.dashboard_folder}/data_{i:04}.html"):
+#                 break
+
+#         assert self.sparse_autoencoder.cfg.d_sae is not None  # keep pyright happy
+#         assert self.final_index is not None  # keep pyright happy
+#         n_features = self.sparse_autoencoder.cfg.d_sae
+#         n_features_at_a_time = self.n_features_at_a_time
+#         id_of_last_feature_without_dashboard = i
+#         n_features_remaining = self.final_index - id_of_last_feature_without_dashboard
+#         n_batches_to_do = n_features_remaining // n_features_at_a_time
+#         if self.final_index == n_features:
+#             id_to_start_from = max(
+#                 0, n_features - (n_batches_to_do + 1) * n_features_at_a_time
+#             )
+#         else:
+#             id_to_start_from = 0  # testing purposes only
+
+#         print(f"File {i} does not exist")
+#         print(f"features left to do: {n_features_remaining}")
+#         print(f"id_to_start_from: {id_to_start_from}")
+#         print(
+#             f"number of batches to do: {(n_features - id_to_start_from) // n_features_at_a_time}"
+#         )
+
+#         return id_to_start_from
+
+#     @torch.no_grad()
+#     def get_feature_property_df(self):
+#         sparse_autoencoder = self.sparse_autoencoder
+#         feature_sparsity = (
+#             self.feature_sparsity
+#             if self.feature_sparsity is not None
+#             else torch.tensor(0)
+#         )
+
+#         W_dec_normalized = (
+#             sparse_autoencoder.W_dec.cpu()
+#         )  # / sparse_autoencoder.W_dec.cpu().norm(dim=-1, keepdim=True)
+#         W_enc_normalized = (
+#             sparse_autoencoder.W_enc.cpu()
+#             / sparse_autoencoder.W_enc.cpu().norm(dim=-1, keepdim=True)
+#         )
+#         d_e_projection = cosine_similarity(W_dec_normalized, W_enc_normalized.T)
+
+#         assert sparse_autoencoder.cfg.d_sae is not None  # keep pyright happy
+#         temp_df = pd.DataFrame(
+#             {
+#                 "log_feature_sparsity": feature_sparsity + 1e-10,
+#                 "d_e_projection": d_e_projection,
+#                 # "d_e_projection_normalized": d_e_projection_normalized,
+#                 "b_enc": sparse_autoencoder.b_enc.detach().cpu(),
+#                 "feature": [
+#                     f"feature_{i}" for i in range(sparse_autoencoder.cfg.d_sae)
+#                 ],
+#                 "index": torch.arange(sparse_autoencoder.cfg.d_sae),
+#                 "dead_neuron": (feature_sparsity < -9).cpu(),
+#             }
+#         )
+
+#         return temp_df
+
+#     def run(self):
+#         """
+#         Generate the dashboard.
+#         """
+
+#         run = None
+#         if self.use_wandb:
+#             # get name from wandb
+#             random_suffix = str(uuid.uuid4())[:8]
+#             name = f"{self.get_dashboard_folder_name()}_{random_suffix}"
+#             run = wandb.init(
+#                 project="feature_dashboards",
+#                 config=cast(Any, self.sparse_autoencoder.cfg),
+#                 name=name,
+#                 tags=[
+#                     f"model_{self.sparse_autoencoder.cfg.model_name}",
+#                     f"hook_point_{self.sparse_autoencoder.cfg.hook_point}",
+#                 ],
+#             )
+
+#         if self.model is None:
+#             self.init_sae_session()
+
+#         # generate all the plots
+#         if self.use_wandb and self.feature_sparsity is not None:
+#             feature_property_df = self.get_feature_property_df()
+
+#             fig = px.histogram(
+#                 self.feature_sparsity + 1e-10,
+#                 nbins=100,
+#                 log_x=False,
+#                 title="Feature sparsity",
+#             )
+#             wandb.log(
+#                 {"plots/feature_density_histogram": wandb.Html(plotly.io.to_html(fig))}
+#             )
+
+#             fig = px.histogram(
+#                 self.sparse_autoencoder.b_enc.detach().cpu(), title="b_enc", nbins=100
+#             )
+#             wandb.log({"plots/b_enc_histogram": wandb.Html(plotly.io.to_html(fig))})
+
+#             fig = px.histogram(
+#                 feature_property_df.d_e_projection, nbins=100, title="D/E projection"
+#             )
+#             wandb.log(
+#                 {"plots/d_e_projection_histogram": wandb.Html(plotly.io.to_html(fig))}
+#             )
+
+#             fig = px.histogram(
+#                 self.sparse_autoencoder.b_dec.detach().cpu(),
+#                 nbins=100,
+#                 title="b_dec projection onto W_dec",
+#             )
+#             wandb.log(
+#                 {"plots/b_dec_projection_histogram": wandb.Html(plotly.io.to_html(fig))}
+#             )
+
+#             fig = px.scatter_matrix(
+#                 feature_property_df,
+#                 dimensions=["log_feature_sparsity", "d_e_projection", "b_enc"],
+#                 color="dead_neuron",
+#                 hover_name="feature",
+#                 opacity=0.2,
+#                 height=800,
+#                 width=1400,
+#             )
+#             wandb.log({"plots/scatter_matrix": wandb.Html(plotly.io.to_html(fig))})
+
+#         self.n_features = self.sparse_autoencoder.cfg.d_sae
+#         id_to_start_from = self.get_index_to_resume_from()
+#         id_to_end_at = self.n_features if self.final_index is None else self.final_index
+#         assert id_to_end_at is not None  # keep pyright happy
+
+#         # divide into batches
+#         feature_idx = torch.tensor(range(id_to_start_from, id_to_end_at))
+#         feature_idx = feature_idx.reshape(-1, self.n_features_at_a_time)
+#         feature_idx = [x.tolist() for x in feature_idx]
+
+#         print(f"Hook Point Layer: {self.sparse_autoencoder.cfg.hook_point_layer}")
+#         print(f"Hook Point: {self.sparse_autoencoder.cfg.hook_point}")
+#         print(f"Writing files to: {self.dashboard_folder}")
+
+#         # get tokens:
+#         start = time.time()
+#         tokens = self.get_tokens(
+#             self.n_batches_to_sample_from, self.n_prompts_to_select
+#         )
+#         end = time.time()
+#         print(f"Time to get tokens: {end - start}")
+#         if self.use_wandb:
+#             wandb.log({"time/time_to_get_tokens": end - start})
+
+#         assert self.model is not None
+#         vocab_dict = cast(Any, self.model.tokenizer).vocab
+#         vocab_dict = {
+#             v: k.replace("Ġ", " ").replace("\n", "\\n") for k, v in vocab_dict.items()
+#         }
+
+#         with torch.no_grad():
+#             for interesting_features in tqdm(feature_idx):
+#                 print(interesting_features)
+
+#                 layout = SaeVisLayoutConfig(
+#                     columns=[
+#                         Column(
+#                             SequencesConfig(
+#                                 stack_mode="stack-all",
+#                                 buffer=(self.buffer_tokens, self.buffer_tokens),
+#                                 compute_buffer=False,
+#                                 n_quantiles=10,
+#                                 top_acts_group_size=20,
+#                                 quantile_group_size=5,
+#                             ),
+#                             width=650,
+#                         ),
+#                         Column(
+#                             ActsHistogramConfig(),
+#                             FeatureTablesConfig(n_rows=5),
+#                             width=500,
+#                         ),
+#                     ],
+#                     height=1000,
+#                 )
+#                 feature_vis_params = SaeVisConfig(
+#                     hook_point=self.sparse_autoencoder.cfg.hook_point,
+#                     minibatch_size_features=256,
+#                     minibatch_size_tokens=64,
+#                     features=interesting_features,
+#                     verbose=True,
+#                     feature_centric_layout=layout,
+#                 )
+
+#                 feature_data = get_feature_data(
+#                     encoder=self.sparse_autoencoder,  # type: ignore
+#                     model=self.model,
+#                     tokens=tokens,
+#                     cfg=feature_vis_params,
+#                 )
+
+#                 for i, test_idx in enumerate(feature_data.feature_data_dict.keys()):
+#                     feature_data.save_feature_centric_vis(
+#                         f"{self.dashboard_folder}/data_{test_idx:04}.html",
+#                         feature_idx=test_idx,
+#                     )
+
+#                     if i < 10 and self.use_wandb:
+#                         # upload the html as an artifact
+#                         artifact = wandb.Artifact(f"feature_{test_idx}", type="feature")
+#                         artifact.add_file(
+#                             f"{self.dashboard_folder}/data_{test_idx:04}.html"
+#                         )
+#                         assert run is not None  # keep pyright happy
+#                         run.log_artifact(artifact)
+
+#                         # also upload as html to dashboard
+#                         wandb.log(
+#                             {
+#                                 "features/feature_dashboard": wandb.Html(
+#                                     f"{self.dashboard_folder}/data_{test_idx:04}.html"
+#                                 )
+#                             },
+#                             step=test_idx,
+#                         )
+
+#         if self.use_wandb:
+#             # when done zip the folder
+#             shutil.make_archive(self.dashboard_folder, "zip", self.dashboard_folder)
+
+#             # then upload the zip as an artifact
+#             artifact = wandb.Artifact("dashboard", type="zipped_feature_dashboards")
+#             artifact.add_file(f"{self.dashboard_folder}.zip")
+#             assert run is not None  # keep pyright happy
+#             run.log_artifact(artifact)
 
-# set TOKENIZERS_PARALLELISM to false to avoid warnings
-os.environ["TOKENIZERS_PARALLELISM"] = "false"
-import shutil
-import time
-import uuid
-
-import pandas as pd
-import plotly
-import plotly.express as px
-import torch
-import wandb
-from sae_vis.data_config_classes import (
-    ActsHistogramConfig,
-    Column,
-    FeatureTablesConfig,
-    SaeVisConfig,
-    SaeVisLayoutConfig,
-    SequencesConfig,
-)
-from sae_vis.data_fetching_fns import get_feature_data
-from torch.nn.functional import cosine_similarity
-from tqdm import tqdm
-from transformer_lens import HookedTransformer
-
-from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
-
-
-class DashboardRunner:
-
-    model: HookedTransformer | None = None
-
-    def __init__(
-        self,
-        sae_path: Optional[str] = None,
-        dashboard_parent_folder: str = "./feature_dashboards",
-        wandb_artifact_path: Optional[str] = None,
-        init_session: bool = True,
-        # token pars
-        n_batches_to_sample_from: int = 2**12,
-        n_prompts_to_select: int = 4096 * 6,
-        # sampling pars
-        n_features_at_a_time: int = 1024,
-        max_batch_size: int = 256,
-        buffer_tokens: int = 8,
-        # util pars
-        use_wandb: bool = False,
-        continue_existing_dashboard: bool = True,
-        final_index: Optional[int] = None,
-    ):
-        """ """
-
-        if wandb_artifact_path is not None:
-            artifact_dir = f"artifacts/{wandb_artifact_path.split('/')[2]}"
-            if not os.path.exists(artifact_dir):
-                print("Downloading artifact")
-                run = wandb.init()
-                assert run is not None  # keep pyright happy
-                artifact = run.use_artifact(wandb_artifact_path)
-                artifact_dir = artifact.download()
-                path_to_artifact = f"{artifact_dir}/{os.listdir(artifact_dir)[0]}"
-                # feature sparsity
-                feature_sparsity_path = self.get_feature_sparsity_path(
-                    wandb_artifact_path
-                )
-                artifact = run.use_artifact(feature_sparsity_path)
-                artifact_dir = artifact.download()
-                # add it as a property
-                self.feature_sparsity = torch.load(
-                    f"{artifact_dir}/{os.listdir(artifact_dir)[0]}"
-                )
-            else:
-                print("Artifact already downloaded")
-                path_to_artifact = f"{artifact_dir}/{os.listdir(artifact_dir)[0]}"
-
-                feature_sparsity_path = self.get_feature_sparsity_path(
-                    wandb_artifact_path
-                )
-                artifact_dir = f"artifacts/{feature_sparsity_path.split('/')[2]}"
-                feature_sparsity_file = os.listdir(artifact_dir)[0]
-                self.feature_sparsity = torch.load(
-                    f"{artifact_dir}/{feature_sparsity_file}"
-                )
-
-            self.sae_path = path_to_artifact
-        else:
-            assert sae_path is not None
-            self.sae_path = sae_path
-            self.feature_sparsity = None
-
-        if init_session:
-            self.init_sae_session()
-
-        self.n_features_at_a_time = n_features_at_a_time
-        self.max_batch_size = max_batch_size
-        self.buffer_tokens = buffer_tokens
-        self.use_wandb = use_wandb
-        self.final_index = (
-            final_index
-            if final_index is not None
-            else self.sparse_autoencoder.cfg.d_sae
-        )
-        self.n_batches_to_sample_from = n_batches_to_sample_from
-        self.n_prompts_to_select = n_prompts_to_select
-
-        # Deal with file structure
-        if not os.path.exists(dashboard_parent_folder):
-            os.makedirs(dashboard_parent_folder)
-
-        self.dashboard_folder = (
-            f"{dashboard_parent_folder}/{self.get_dashboard_folder_name()}"
-        )
-        if not os.path.exists(self.dashboard_folder):
-            os.makedirs(self.dashboard_folder)
-
-        if not continue_existing_dashboard:
-            # check if there are files there and if so abort
-            if len(os.listdir(self.dashboard_folder)) > 0:
-                raise ValueError("Dashboard folder not empty. Aborting.")
-
-    def get_feature_sparsity_path(self, wandb_artifact_path: str):
-        prefix = wandb_artifact_path.split(":")[0]
-        return f"{prefix}_log_feature_sparsity:v9"
-
-    def get_dashboard_folder_name(self):
-        model = self.sparse_autoencoder.cfg.model_name
-        hook_point = self.sparse_autoencoder.cfg.hook_point
-        d_sae = self.sparse_autoencoder.cfg.d_sae
-        dashboard_folder_name = f"{model}_{hook_point}_{d_sae}"
-
-        return dashboard_folder_name
-
-    def init_sae_session(self):
-        (
-            model,
-            sae_group,
-            self.activation_store,
-        ) = LMSparseAutoencoderSessionloader.load_pretrained_sae(self.sae_path)
-        assert isinstance(
-            model, HookedTransformer
-        )  # only HookedTransformer is allowed to be used in the dashboard
-        self.model = model
-        # TODO: handle multiple autoencoders
-        self.sparse_autoencoder = next(iter(sae_group))[1]
-
-    def get_tokens(
-        self, n_batches_to_sample_from: int = 2**12, n_prompts_to_select: int = 4096 * 6
-    ):
-        """
-        Get the tokens needed for dashboard generation.
-        """
-
-        all_tokens_list = []
-        pbar = tqdm(range(n_batches_to_sample_from))
-        for _ in pbar:
-            batch_tokens = self.activation_store.get_batch_tokens()
-            batch_tokens = batch_tokens[torch.randperm(batch_tokens.shape[0])][
-                : batch_tokens.shape[0]
-            ]
-            all_tokens_list.append(batch_tokens)
-
-        all_tokens = torch.cat(all_tokens_list, dim=0)
-        all_tokens = all_tokens[torch.randperm(all_tokens.shape[0])]
-        return all_tokens[:n_prompts_to_select]
-
-    def get_index_to_resume_from(self):
-        i = 0
-        assert self.n_features is not None  # keep pyright happy
-        for i in range(self.n_features):
-            if not os.path.exists(f"{self.dashboard_folder}/data_{i:04}.html"):
-                break
-
-        assert self.sparse_autoencoder.cfg.d_sae is not None  # keep pyright happy
-        assert self.final_index is not None  # keep pyright happy
-        n_features = self.sparse_autoencoder.cfg.d_sae
-        n_features_at_a_time = self.n_features_at_a_time
-        id_of_last_feature_without_dashboard = i
-        n_features_remaining = self.final_index - id_of_last_feature_without_dashboard
-        n_batches_to_do = n_features_remaining // n_features_at_a_time
-        if self.final_index == n_features:
-            id_to_start_from = max(
-                0, n_features - (n_batches_to_do + 1) * n_features_at_a_time
-            )
-        else:
-            id_to_start_from = 0  # testing purposes only
-
-        print(f"File {i} does not exist")
-        print(f"features left to do: {n_features_remaining}")
-        print(f"id_to_start_from: {id_to_start_from}")
-        print(
-            f"number of batches to do: {(n_features - id_to_start_from) // n_features_at_a_time}"
-        )
-
-        return id_to_start_from
-
-    @torch.no_grad()
-    def get_feature_property_df(self):
-        sparse_autoencoder = self.sparse_autoencoder
-        feature_sparsity = (
-            self.feature_sparsity
-            if self.feature_sparsity is not None
-            else torch.tensor(0)
-        )
-
-        W_dec_normalized = (
-            sparse_autoencoder.W_dec.cpu()
-        )  # / sparse_autoencoder.W_dec.cpu().norm(dim=-1, keepdim=True)
-        W_enc_normalized = (
-            sparse_autoencoder.W_enc.cpu()
-            / sparse_autoencoder.W_enc.cpu().norm(dim=-1, keepdim=True)
-        )
-        d_e_projection = cosine_similarity(W_dec_normalized, W_enc_normalized.T)
-
-        assert sparse_autoencoder.cfg.d_sae is not None  # keep pyright happy
-        temp_df = pd.DataFrame(
-            {
-                "log_feature_sparsity": feature_sparsity + 1e-10,
-                "d_e_projection": d_e_projection,
-                # "d_e_projection_normalized": d_e_projection_normalized,
-                "b_enc": sparse_autoencoder.b_enc.detach().cpu(),
-                "feature": [
-                    f"feature_{i}" for i in range(sparse_autoencoder.cfg.d_sae)
-                ],
-                "index": torch.arange(sparse_autoencoder.cfg.d_sae),
-                "dead_neuron": (feature_sparsity < -9).cpu(),
-            }
-        )
-
-        return temp_df
-
-    def run(self):
-        """
-        Generate the dashboard.
-        """
-
-        run = None
-        if self.use_wandb:
-            # get name from wandb
-            random_suffix = str(uuid.uuid4())[:8]
-            name = f"{self.get_dashboard_folder_name()}_{random_suffix}"
-            run = wandb.init(
-                project="feature_dashboards",
-                config=cast(Any, self.sparse_autoencoder.cfg),
-                name=name,
-                tags=[
-                    f"model_{self.sparse_autoencoder.cfg.model_name}",
-                    f"hook_point_{self.sparse_autoencoder.cfg.hook_point}",
-                ],
-            )
-
-        if self.model is None:
-            self.init_sae_session()
-
-        # generate all the plots
-        if self.use_wandb and self.feature_sparsity is not None:
-            feature_property_df = self.get_feature_property_df()
-
-            fig = px.histogram(
-                self.feature_sparsity + 1e-10,
-                nbins=100,
-                log_x=False,
-                title="Feature sparsity",
-            )
-            wandb.log(
-                {"plots/feature_density_histogram": wandb.Html(plotly.io.to_html(fig))}
-            )
-
-            fig = px.histogram(
-                self.sparse_autoencoder.b_enc.detach().cpu(), title="b_enc", nbins=100
-            )
-            wandb.log({"plots/b_enc_histogram": wandb.Html(plotly.io.to_html(fig))})
-
-            fig = px.histogram(
-                feature_property_df.d_e_projection, nbins=100, title="D/E projection"
-            )
-            wandb.log(
-                {"plots/d_e_projection_histogram": wandb.Html(plotly.io.to_html(fig))}
-            )
-
-            fig = px.histogram(
-                self.sparse_autoencoder.b_dec.detach().cpu(),
-                nbins=100,
-                title="b_dec projection onto W_dec",
-            )
-            wandb.log(
-                {"plots/b_dec_projection_histogram": wandb.Html(plotly.io.to_html(fig))}
-            )
-
-            fig = px.scatter_matrix(
-                feature_property_df,
-                dimensions=["log_feature_sparsity", "d_e_projection", "b_enc"],
-                color="dead_neuron",
-                hover_name="feature",
-                opacity=0.2,
-                height=800,
-                width=1400,
-            )
-            wandb.log({"plots/scatter_matrix": wandb.Html(plotly.io.to_html(fig))})
-
-        self.n_features = self.sparse_autoencoder.cfg.d_sae
-        id_to_start_from = self.get_index_to_resume_from()
-        id_to_end_at = self.n_features if self.final_index is None else self.final_index
-        assert id_to_end_at is not None  # keep pyright happy
-
-        # divide into batches
-        feature_idx = torch.tensor(range(id_to_start_from, id_to_end_at))
-        feature_idx = feature_idx.reshape(-1, self.n_features_at_a_time)
-        feature_idx = [x.tolist() for x in feature_idx]
-
-        print(f"Hook Point Layer: {self.sparse_autoencoder.cfg.hook_point_layer}")
-        print(f"Hook Point: {self.sparse_autoencoder.cfg.hook_point}")
-        print(f"Writing files to: {self.dashboard_folder}")
-
-        # get tokens:
-        start = time.time()
-        tokens = self.get_tokens(
-            self.n_batches_to_sample_from, self.n_prompts_to_select
-        )
-        end = time.time()
-        print(f"Time to get tokens: {end - start}")
-        if self.use_wandb:
-            wandb.log({"time/time_to_get_tokens": end - start})
-
-        assert self.model is not None
-        vocab_dict = cast(Any, self.model.tokenizer).vocab
-        vocab_dict = {
-            v: k.replace("Ġ", " ").replace("\n", "\\n") for k, v in vocab_dict.items()
-        }
-
-        with torch.no_grad():
-            for interesting_features in tqdm(feature_idx):
-                print(interesting_features)
-
-                layout = SaeVisLayoutConfig(
-                    columns=[
-                        Column(
-                            SequencesConfig(
-                                stack_mode="stack-all",
-                                buffer=(self.buffer_tokens, self.buffer_tokens),
-                                compute_buffer=False,
-                                n_quantiles=10,
-                                top_acts_group_size=20,
-                                quantile_group_size=5,
-                            ),
-                            width=650,
-                        ),
-                        Column(
-                            ActsHistogramConfig(),
-                            FeatureTablesConfig(n_rows=5),
-                            width=500,
-                        ),
-                    ],
-                    height=1000,
-                )
-                feature_vis_params = SaeVisConfig(
-                    hook_point=self.sparse_autoencoder.cfg.hook_point,
-                    minibatch_size_features=256,
-                    minibatch_size_tokens=64,
-                    features=interesting_features,
-                    verbose=True,
-                    feature_centric_layout=layout,
-                )
-
-                feature_data = get_feature_data(
-                    encoder=self.sparse_autoencoder,  # type: ignore
-                    model=self.model,
-                    tokens=tokens,
-                    cfg=feature_vis_params,
-                )
-
-                for i, test_idx in enumerate(feature_data.feature_data_dict.keys()):
-                    feature_data.save_feature_centric_vis(
-                        f"{self.dashboard_folder}/data_{test_idx:04}.html",
-                        feature_idx=test_idx,
-                    )
-
-                    if i < 10 and self.use_wandb:
-                        # upload the html as an artifact
-                        artifact = wandb.Artifact(f"feature_{test_idx}", type="feature")
-                        artifact.add_file(
-                            f"{self.dashboard_folder}/data_{test_idx:04}.html"
-                        )
-                        assert run is not None  # keep pyright happy
-                        run.log_artifact(artifact)
-
-                        # also upload as html to dashboard
-                        wandb.log(
-                            {
-                                "features/feature_dashboard": wandb.Html(
-                                    f"{self.dashboard_folder}/data_{test_idx:04}.html"
-                                )
-                            },
-                            step=test_idx,
-                        )
-
-        if self.use_wandb:
-            # when done zip the folder
-            shutil.make_archive(self.dashboard_folder, "zip", self.dashboard_folder)
-
-            # then upload the zip as an artifact
-            artifact = wandb.Artifact("dashboard", type="zipped_feature_dashboards")
-            artifact.add_file(f"{self.dashboard_folder}.zip")
-            assert run is not None  # keep pyright happy
-            run.log_artifact(artifact)
+#             # terminate the run
+#             run.finish()
 
-            # terminate the run
-            run.finish()
+#             # delete the dashboard folder
+#             shutil.rmtree(self.dashboard_folder)
 
-            # delete the dashboard folder
-            shutil.rmtree(self.dashboard_folder)
-
-        return
+#         return
```

### Comparing `sae_lens-2.1.3/sae_lens/analysis/feature_statistics.py` & `sae_lens-3.0.0/sae_lens/analysis/feature_statistics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 import pandas as pd
 import torch
 from tqdm import tqdm
 from transformer_lens import HookedTransformer
 
-from sae_lens.training.sparse_autoencoder import SparseAutoencoder
+from sae_lens.sae import SAE
 
 
 @torch.no_grad()
-def get_feature_property_df(
-    sparse_autoencoder: SparseAutoencoder, feature_sparsity: torch.Tensor
-):
+def get_feature_property_df(sae: SAE, feature_sparsity: torch.Tensor):
     """
-    feature_property_df = get_feature_property_df(sparse_autoencoder, log_feature_density.cpu())
+    feature_property_df = get_feature_property_df(sae, log_feature_density.cpu())
     """
 
     W_dec_normalized = (
-        sparse_autoencoder.W_dec.cpu()
+        sae.W_dec.cpu()
     )  # / sparse_autoencoder.W_dec.cpu().norm(dim=-1, keepdim=True)
-    W_enc_normalized = (
-        sparse_autoencoder.W_enc.cpu()
-        / sparse_autoencoder.W_enc.cpu().norm(dim=-1, keepdim=True)
-    ).T
+    W_enc_normalized = (sae.W_enc.cpu() / sae.W_enc.cpu().norm(dim=-1, keepdim=True)).T
 
     d_e_projection = (W_dec_normalized * W_enc_normalized).sum(-1)
-    b_dec_projection = sparse_autoencoder.b_dec.cpu() @ W_dec_normalized.T
+    b_dec_projection = sae.b_dec.cpu() @ W_dec_normalized.T
 
     temp_df = pd.DataFrame(
         {
             "log_feature_sparsity": feature_sparsity + 1e-10,
             "d_e_projection": d_e_projection,
             # "d_e_projection_normalized": d_e_projection_normalized,
-            "b_enc": sparse_autoencoder.b_enc.detach().cpu(),
+            "b_enc": sae.b_enc.detach().cpu(),
             "b_dec_projection": b_dec_projection,
-            "feature": list(range(sparse_autoencoder.cfg.d_sae)),  # type: ignore
+            "feature": list(range(sae.cfg.d_sae)),  # type: ignore
             "dead_neuron": (feature_sparsity < -9).cpu(),
         }
     )
 
     return temp_df
 
 
@@ -64,25 +59,25 @@
     )
 
     return stats_df
 
 
 @torch.no_grad()
 def get_all_stats_dfs(
-    gpt2_small_sparse_autoencoders: dict[str, SparseAutoencoder],  # [hook_point, sae]
+    gpt2_small_sparse_autoencoders: dict[str, SAE],  # [hook_point, sae]
     gpt2_small_sae_sparsities: dict[str, torch.Tensor],  # [hook_point, sae]
     model: HookedTransformer,
     cosine_sim: bool = False,
 ):
     stats_dfs = []
     pbar = tqdm(gpt2_small_sparse_autoencoders.keys())
     for key in pbar:
         layer = int(key.split(".")[1])
         sparse_autoencoder = gpt2_small_sparse_autoencoders[key]
-        pbar.set_description(f"Processing layer {sparse_autoencoder.cfg.hook_point}")
+        pbar.set_description(f"Processing layer {sparse_autoencoder.cfg.hook_name}")
         W_U_stats_df_dec, _ = get_W_U_W_dec_stats_df(
             sparse_autoencoder.W_dec.cpu(), model, cosine_sim
         )
         log_feature_sparsity = gpt2_small_sae_sparsities[key].detach().cpu()
         W_U_stats_df_dec["log_feature_sparsity"] = log_feature_sparsity
         W_U_stats_df_dec["layer"] = layer + (1 if "post" in key else 0)
         stats_dfs.append(W_U_stats_df_dec)
```

### Comparing `sae_lens-2.1.3/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-3.0.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.3/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-3.0.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,19 @@
     SaeVisLayoutConfig,
     SequencesConfig,
 )
 from sae_vis.data_storing_fns import SaeVisData
 from tqdm import tqdm
 from transformer_lens import HookedTransformer
 
+from sae_lens.config import LanguageModelSAERunnerConfig
+from sae_lens.load_model import load_model
+from sae_lens.sae import SAE
 from sae_lens.toolkit.pretrained_saes import load_sparsity
-from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
-from sae_lens.training.sparse_autoencoder import SparseAutoencoder
+from sae_lens.training.activations_store import ActivationsStore
 
 OUT_OF_RANGE_TOKEN = "<|outofrange|>"
 
 BG_COLOR_MAP = colors.LinearSegmentedColormap.from_list(
     "bg_color_map", ["white", "darkorange"]
 )
 
@@ -63,14 +65,16 @@
 
     def __init__(
         self,
         sae_id: str,
         sae_path: str,
         outputs_dir: str,
         sparsity_threshold: int = DEFAULT_SPARSITY_THRESHOLD,
+        # ACTIVATION STORE PARAMATERS
+        ## SAE VIS PARAMETERS
         # token pars
         n_batches_to_sample_from: int = 2**12,
         n_prompts_to_select: int = 4096 * 6,
         # batching
         n_features_at_a_time: int = 128,
         start_batch_inclusive: int = 0,
         end_batch_inclusive: Optional[int] = None,
@@ -83,21 +87,29 @@
         self.device = "cpu"
         if torch.backends.mps.is_available():
             self.device = "mps"
         elif torch.cuda.is_available():
             self.device = "cuda"
 
         self.sae_path = sae_path
-        self.sparse_autoencoder = SparseAutoencoder.load_from_pretrained(
-            self.sae_path, device=self.device
+        self.sae = SAE.load_from_pretrained(self.sae_path, device=self.device)
+        self.model = load_model(
+            model_class_name="HookedTransformer",
+            model_name=self.sae.model_name,
+            device=self.device,
         )
-        loader = LMSparseAutoencoderSessionloader(self.sparse_autoencoder.cfg)
-        self.model, _, self.activation_store = loader.load_sae_training_group_session()
-        self.model_id = self.sparse_autoencoder.cfg.model_name
-        self.layer = self.sparse_autoencoder.cfg.hook_point_layer
+
+        # temporarily, load config seperately
+        cfg = LanguageModelSAERunnerConfig.from_json(sae_path)
+
+        # currently this script assumes we are loading an SAE trained using SAE Lens.
+        self.activation_store = ActivationsStore.from_config(model=self.model, cfg=cfg)
+
+        self.model_id = self.sae.cfg.model_name
+        self.layer = self.sae.cfg.hook_layer
         self.sae_id = sae_id
         self.sparsity_threshold = sparsity_threshold
         self.n_features_at_a_time = n_features_at_a_time
         self.n_batches_to_sample_from = n_batches_to_sample_from
         self.n_prompts_to_select = n_prompts_to_select
         self.start_batch = start_batch_inclusive
         self.end_batch = end_batch_inclusive
@@ -156,15 +168,15 @@
             for t in tokens.flatten().tolist()
         ]
 
         # Reshape
         return np.reshape(str_tokens, tokens.shape).tolist()
 
     def run(self):
-        self.n_features = self.sparse_autoencoder.cfg.d_sae
+        self.n_features = self.sae.cfg.d_sae
         assert self.n_features is not None
 
         # if we have feature sparsity, then use it to only generate outputs for non-dead features
         self.target_feature_indexes: list[int] = []
         sparsity = load_sparsity(self.sae_path)
         # convert sparsity to logged sparsity if it's not
         # TODO: standardize the sparsity file format
@@ -269,23 +281,23 @@
                             LogitsHistogramConfig(),
                             LogitsTableConfig(),
                             FeatureTablesConfig(n_rows=3),
                         )
                     ]
                 )
                 feature_vis_params = SaeVisConfig(
-                    hook_point=self.sparse_autoencoder.cfg.hook_point,
+                    hook_point=self.sae.cfg.hook_name,
                     minibatch_size_features=128,
                     minibatch_size_tokens=64,
                     features=features_to_process,
                     verbose=True,
                     feature_centric_layout=layout,
                 )
                 feature_data = SaeVisData.create(
-                    encoder=self.sparse_autoencoder,  # type: ignore
+                    encoder=self.sae,  # type: ignore
                     model=cast(HookedTransformer, self.model),
                     tokens=tokens,
                     cfg=feature_vis_params,
                 )
 
                 features_outputs = []
                 for _, feat_index in enumerate(feature_data.feature_data_dict.keys()):
```

### Comparing `sae_lens-2.1.3/sae_lens/analysis/tsea.py` & `sae_lens-3.0.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.3/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-3.0.0/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.3/sae_lens/training/activations_store.py` & `sae_lens-3.0.0/sae_lens/training/activations_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+import contextlib
 import os
-from typing import Any, Iterator, Literal, TypeVar, cast
+from typing import Any, Iterator, Literal, cast
 
 import torch
 import tqdm
 from datasets import (
     Dataset,
     DatasetDict,
     IterableDataset,
@@ -13,35 +14,41 @@
     load_dataset,
 )
 from safetensors import safe_open
 from safetensors.torch import load_file, save_file
 from torch.utils.data import DataLoader
 from transformer_lens.hook_points import HookedRootModule
 
-from sae_lens.training.config import (
+from sae_lens.config import (
+    DTYPE_MAP,
     CacheActivationsRunnerConfig,
     LanguageModelSAERunnerConfig,
 )
+from sae_lens.sae import SAE
 
 HfDataset = DatasetDict | Dataset | IterableDatasetDict | IterableDataset
 
 
+# TODO: Make an activation store config class to be consistent with the rest of the code.
 class ActivationsStore:
     """
     Class for streaming tokens and generating and storing activations
     while training SAEs.
     """
 
     model: HookedRootModule
     dataset: HfDataset
     cached_activations_path: str | None
     tokens_column: Literal["tokens", "input_ids", "text"]
-    hook_point_head_index: int | None
+    hook_name: str
+    hook_layer: int
+    hook_head_index: int | None
     _dataloader: Iterator[Any] | None = None
     _storage_buffer: torch.Tensor | None = None
+    device: torch.device
 
     @classmethod
     def from_config(
         cls,
         model: HookedRootModule,
         cfg: LanguageModelSAERunnerConfig | CacheActivationsRunnerConfig,
         dataset: HfDataset | None = None,
@@ -53,75 +60,110 @@
             and not cfg.use_cached_activations
         ):
             cached_activations_path = None
         return cls(
             model=model,
             dataset=dataset or cfg.dataset_path,
             streaming=cfg.streaming,
-            hook_point=cfg.hook_point,
-            hook_point_layers=listify(cfg.hook_point_layer),
-            hook_point_head_index=cfg.hook_point_head_index,
+            hook_name=cfg.hook_name,
+            hook_layer=cfg.hook_layer,
+            hook_head_index=cfg.hook_head_index,
             context_size=cfg.context_size,
             d_in=cfg.d_in,
             n_batches_in_buffer=cfg.n_batches_in_buffer,
             total_training_tokens=cfg.training_tokens,
             store_batch_size_prompts=cfg.store_batch_size_prompts,
             train_batch_size_tokens=cfg.train_batch_size_tokens,
             prepend_bos=cfg.prepend_bos,
             normalize_activations=cfg.normalize_activations,
-            device=cfg.device,
+            device=torch.device(cfg.act_store_device),
             dtype=cfg.dtype,
             cached_activations_path=cached_activations_path,
             model_kwargs=cfg.model_kwargs,
+            autocast_lm=cfg.autocast_lm,
+        )
+
+    @classmethod
+    def from_sae(
+        cls,
+        model: HookedRootModule,
+        sae: SAE,
+        streaming: bool = True,
+        store_batch_size_prompts: int = 8,
+        n_batches_in_buffer: int = 8,
+        train_batch_size_tokens: int = 4096,
+        total_tokens: int = 10**9,
+        device: str = "cpu",
+    ) -> "ActivationsStore":
+
+        return cls(
+            model=model,
+            dataset=sae.cfg.dataset_path,
+            d_in=sae.cfg.d_in,
+            hook_name=sae.cfg.hook_name,
+            hook_layer=sae.cfg.hook_layer,
+            hook_head_index=sae.cfg.hook_head_index,
+            context_size=sae.cfg.context_size,
+            prepend_bos=sae.cfg.prepend_bos,
+            streaming=streaming,
+            store_batch_size_prompts=store_batch_size_prompts,
+            train_batch_size_tokens=train_batch_size_tokens,
+            n_batches_in_buffer=n_batches_in_buffer,
+            total_training_tokens=total_tokens,
+            normalize_activations=sae.cfg.normalize_activations,
+            dtype=sae.cfg.dtype,
+            device=torch.device(device),
         )
 
     def __init__(
         self,
         model: HookedRootModule,
         dataset: HfDataset | str,
         streaming: bool,
-        hook_point: str,
-        hook_point_layers: list[int],
-        hook_point_head_index: int | None,
+        hook_name: str,
+        hook_layer: int,
+        hook_head_index: int | None,
         context_size: int,
         d_in: int,
         n_batches_in_buffer: int,
         total_training_tokens: int,
         store_batch_size_prompts: int,
         train_batch_size_tokens: int,
         prepend_bos: bool,
         normalize_activations: bool,
-        device: str | torch.device,
-        dtype: str | torch.dtype,
+        device: torch.device,
+        dtype: str,
         cached_activations_path: str | None = None,
         model_kwargs: dict[str, Any] | None = None,
+        autocast_lm: bool = False,
     ):
         self.model = model
         if model_kwargs is None:
             model_kwargs = {}
         self.model_kwargs = model_kwargs
         self.dataset = (
             load_dataset(dataset, split="train", streaming=streaming)
             if isinstance(dataset, str)
             else dataset
         )
-        self.hook_point = hook_point
-        self.hook_point_layers = hook_point_layers
-        self.hook_point_head_index = hook_point_head_index
+        self.hook_name = hook_name
+        self.hook_layer = hook_layer
+        self.hook_head_index = hook_head_index
         self.context_size = context_size
         self.d_in = d_in
         self.n_batches_in_buffer = n_batches_in_buffer
         self.total_training_tokens = total_training_tokens
         self.store_batch_size_prompts = store_batch_size_prompts
         self.train_batch_size_tokens = train_batch_size_tokens
         self.prepend_bos = prepend_bos
         self.normalize_activations = normalize_activations
-        self.device = device
-        self.dtype = dtype
+        self.device = torch.device(device)
+        self.dtype = DTYPE_MAP[dtype]
         self.cached_activations_path = cached_activations_path
+        self.autocast_lm = autocast_lm
 
         self.n_dataset_processed = 0
         self.iterable_dataset = iter(self.dataset)
 
         self.estimated_norm_scaling_factor = 1.0
 
         # Check if dataset is tokenized
@@ -270,55 +312,59 @@
 
     def get_activations(self, batch_tokens: torch.Tensor):
         """
         Returns activations of shape (batches, context, num_layers, d_in)
 
         d_in may result from a concatenated head dimension.
         """
-        layers = self.hook_point_layers
-        act_names = [self.hook_point.format(layer=layer) for layer in layers]
-        hook_point_max_layer = max(layers)
-
-        layerwise_activations = self.model.run_with_cache(
-            batch_tokens,
-            names_filter=act_names,
-            stop_at_layer=hook_point_max_layer + 1,
-            prepend_bos=self.prepend_bos,
-            **self.model_kwargs,
-        )[1]
 
-        n_batches, n_context = batch_tokens.shape
+        # Setup autocast if using
+        if self.autocast_lm:
+            autocast_if_enabled = torch.autocast(
+                device_type="cuda",
+                dtype=torch.bfloat16,
+                enabled=self.autocast_lm,
+            )
+        else:
+            autocast_if_enabled = contextlib.nullcontext()
 
-        stacked_activations = torch.zeros(
-            (n_batches, n_context, len(layers), self.d_in)
-        )
+        with autocast_if_enabled:
+            layerwise_activations = self.model.run_with_cache(
+                batch_tokens,
+                names_filter=[self.hook_name],
+                stop_at_layer=self.hook_layer + 1,
+                prepend_bos=self.prepend_bos,
+                **self.model_kwargs,
+            )[1]
 
-        for i, act_name in enumerate(act_names):
+        n_batches, n_context = batch_tokens.shape
 
-            if self.hook_point_head_index is not None:
-                stacked_activations[:, :, i] = layerwise_activations[act_name][
-                    :, :, self.hook_point_head_index
-                ]
-            elif (
-                layerwise_activations[act_names[0]].ndim > 3
-            ):  # if we have a head dimension
-                stacked_activations[:, :, i] = layerwise_activations[act_name].view(
-                    n_batches, n_context, -1
-                )
-            else:
-                stacked_activations[:, :, i] = layerwise_activations[act_name]
+        stacked_activations = torch.zeros((n_batches, n_context, 1, self.d_in))
+
+        if self.hook_head_index is not None:
+            stacked_activations[:, :, 0] = layerwise_activations[self.hook_name][
+                :, :, self.hook_head_index
+            ]
+        elif (
+            layerwise_activations[self.hook_name].ndim > 3
+        ):  # if we have a head dimension
+            stacked_activations[:, :, 0] = layerwise_activations[self.hook_name].view(
+                n_batches, n_context, -1
+            )
+        else:
+            stacked_activations[:, :, 0] = layerwise_activations[self.hook_name]
 
         return stacked_activations
 
     def get_buffer(self, n_batches_in_buffer: int) -> torch.Tensor:
         context_size = self.context_size
         batch_size = self.store_batch_size_prompts
         d_in = self.d_in
         total_size = batch_size * n_batches_in_buffer
-        num_layers = len(self.hook_point_layers)  # Number of hook points or layers
+        num_layers = 1
 
         if self.cached_activations_path is not None:
             # Load the activations from disk
             buffer_size = total_size * context_size
             # Initialize an empty tensor with an additional dimension for layers
             new_buffer = torch.zeros(
                 (buffer_size, num_layers, d_in),
@@ -374,29 +420,30 @@
         new_buffer = torch.zeros(
             (total_size, context_size, num_layers, d_in),
             dtype=self.dtype,  # type: ignore
             device=self.device,
         )
 
         for refill_batch_idx_start in refill_iterator:
-            refill_batch_tokens = self.get_batch_tokens()
+            # move batch toks to gpu for model
+            refill_batch_tokens = self.get_batch_tokens().to(self.model.cfg.device)
             refill_activations = self.get_activations(refill_batch_tokens)
+            # move acts back to cpu
+            refill_activations.to(self.device)
             new_buffer[
                 refill_batch_idx_start : refill_batch_idx_start + batch_size, ...
             ] = refill_activations
 
             # pbar.update(1)
 
         new_buffer = new_buffer.reshape(-1, num_layers, d_in)
         new_buffer = new_buffer[torch.randperm(new_buffer.shape[0])]
 
         # every buffer should be normalized:
         if self.normalize_activations:
-            if self.estimated_norm_scaling_factor == 1:
-                print("WARNING: no normalisation is being applied, scaling factor = 1")
             new_buffer = self.apply_norm_scaling_factor(new_buffer)
 
         return new_buffer
 
     def save_buffer(self, buffer: torch.Tensor, path: str):
         """
         Used by cached activations runner to save a buffer to disk.
@@ -497,20 +544,24 @@
     def save(self, file_path: str):
         save_file(self.state_dict(), file_path)
 
     def _get_next_dataset_tokens(self) -> torch.Tensor:
         device = self.device
         if not self.is_dataset_tokenized:
             s = next(self.iterable_dataset)[self.tokens_column]
-            tokens = self.model.to_tokens(
-                s,
-                truncate=True,
-                move_to_device=True,
-                prepend_bos=self.prepend_bos,
-            ).squeeze(0)
+            tokens = (
+                self.model.to_tokens(
+                    s,
+                    truncate=True,
+                    move_to_device=True,
+                    prepend_bos=self.prepend_bos,
+                )
+                .squeeze(0)
+                .to(device)
+            )
             assert (
                 len(tokens.shape) == 1
             ), f"tokens.shape should be 1D but was {tokens.shape}"
         else:
             tokens = torch.tensor(
                 next(self.iterable_dataset)[self.tokens_column],
                 dtype=torch.long,
@@ -520,16 +571,7 @@
             if (
                 not self.prepend_bos
                 and tokens[0] == self.model.tokenizer.bos_token_id  # type: ignore
             ):
                 tokens = tokens[1:]
         self.n_dataset_processed += 1
         return tokens
-
-
-T = TypeVar("T")
-
-
-def listify(x: T | list[T]) -> list[T]:
-    if isinstance(x, list):
-        return x
-    return [x]
```

### Comparing `sae_lens-2.1.3/sae_lens/training/batching.py` & `sae_lens-3.0.0/sae_lens/batching.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.3/sae_lens/training/cache_activations_runner.py` & `sae_lens-3.0.0/sae_lens/cache_activations_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import math
 import os
 from typing import Tuple
 
 import torch
 from tqdm import tqdm
 
+from sae_lens.config import DTYPE_MAP, CacheActivationsRunnerConfig
+from sae_lens.load_model import load_model
 from sae_lens.training.activations_store import ActivationsStore
-from sae_lens.training.config import DTYPE_MAP, CacheActivationsRunnerConfig
-from sae_lens.training.load_model import load_model
 
 
 class CacheActivationsRunner:
 
     def __init__(self, cfg: CacheActivationsRunnerConfig):
         self.cfg = cfg
         self.model = load_model(
```

### Comparing `sae_lens-2.1.3/sae_lens/training/config.py` & `sae_lens-3.0.0/sae_lens/sae.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,440 +1,420 @@
+"""Most of this is just copied over from Arthur's code and slightly simplified:
+https://github.com/ArthurConmy/sae/blob/main/sae/model.py
+"""
+
+import json
 import os
-from dataclasses import dataclass, field
-from typing import Any, Literal, Optional, cast
+from dataclasses import dataclass
+from typing import Any, Callable, Optional, Tuple
 
+import einops
 import torch
-import wandb
-
-from sae_lens import __version__
-
-DTYPE_MAP = {
-    "torch.float32": torch.float32,
-    "torch.float64": torch.float64,
-    "torch.float16": torch.float16,
-    "torch.bfloat16": torch.bfloat16,
-}
+from jaxtyping import Float
+from safetensors.torch import save_file
+from torch import nn
+from transformer_lens.hook_points import HookedRootModule, HookPoint
+
+from sae_lens.config import DTYPE_MAP
+from sae_lens.toolkit.pretrained_sae_loaders import (
+    NAMED_PRETRAINED_SAE_LOADERS,
+    load_pretrained_sae_lens_sae_components,
+)
+from sae_lens.toolkit.pretrained_saes_directory import get_pretrained_saes_directory
+
+SPARSITY_PATH = "sparsity.safetensors"
+SAE_WEIGHTS_PATH = "sae_weights.safetensors"
+SAE_CFG_PATH = "cfg.json"
 
 
 @dataclass
-class LanguageModelSAERunnerConfig:
-    """
-    Configuration for training a sparse autoencoder on a language model.
-    """
-
-    # Data Generating Function (Model + Training Distibuion)
-    model_name: str = "gelu-2l"
-    model_class_name: str = "HookedTransformer"
-    hook_point: str = "blocks.{layer}.hook_mlp_out"
-    hook_point_eval: str = "blocks.{layer}.attn.pattern"
-    hook_point_layer: int | list[int] = 0
-    hook_point_head_index: Optional[int] = None
-    dataset_path: str = "NeelNanda/c4-tokenized-2b"
-    streaming: bool = True
-    is_dataset_tokenized: bool = True
-    context_size: int = 128
-    use_cached_activations: bool = False
-    cached_activations_path: Optional[str] = (
-        None  # Defaults to "activations/{dataset}/{model}/{full_hook_name}_{hook_point_head_index}"
-    )
-
-    # SAE Parameters
-    d_in: int = 512
-    d_sae: Optional[int] = None
-    b_dec_init_method: str = "geometric_median"
-    expansion_factor: int | list[int] = 4
-    activation_fn: str = "relu"  # relu, tanh-relu
-    normalize_sae_decoder: bool = True
-    noise_scale: float = 0.0
-    from_pretrained_path: Optional[str] = None
-    apply_b_dec_to_input: bool = True
-    decoder_orthogonal_init: bool = False
-    decoder_heuristic_init: bool = False
-    init_encoder_as_decoder_transpose: bool = False
-
-    # Activation Store Parameters
-    n_batches_in_buffer: int = 20
-    training_tokens: int = 2_000_000
-    finetuning_tokens: int = 0
-    store_batch_size_prompts: int = 32
-    train_batch_size_tokens: int = 4096
-    normalize_activations: bool = False
-
-    # Misc
-    device: str | torch.device = "cpu"
-    seed: int = 42
-    dtype: str | torch.dtype = "float32"  # type: ignore #
-    prepend_bos: bool = True
-
-    # Performance - see compilation section of lm_runner.py for info
-    autocast: bool = False  # autocast to autocast_dtype during training
-    compile_llm: bool = False  # use torch.compile on the LLM
-    llm_compilation_mode: str | None = None  # which torch.compile mode to use
-    compile_sae: bool = False  # use torch.compile on the SAE
-    sae_compilation_mode: str | None = None
-
-    # Training Parameters
-
-    ## Batch size
-    train_batch_size_tokens: int = 4096
-
-    ## Adam
-    adam_beta1: float | list[float] = 0
-    adam_beta2: float | list[float] = 0.999
-
-    ## Loss Function
-    mse_loss_normalization: Optional[str] = None
-    l1_coefficient: float | list[float] = 1e-3
-    lp_norm: float | list[float] = 1
-    scale_sparsity_penalty_by_decoder_norm: bool = False
-    l1_warm_up_steps: int | list[int] = 0
-
-    ## Learning Rate Schedule
-    lr: float | list[float] = 3e-4
-    lr_scheduler_name: str | list[str] = (
-        "constant"  # constant, cosineannealing, cosineannealingwarmrestarts
-    )
-    lr_warm_up_steps: int | list[int] = 0
-    lr_end: float | list[float] | None = (
-        None  # only used for cosine annealing, default is lr / 10
-    )
-    lr_decay_steps: int | list[int] = 0
-    n_restart_cycles: int | list[int] = 1  # used only for cosineannealingwarmrestarts
-
-    ## FineTuning
-    finetuning_method: Optional[str] = None  # scale, decoder or unrotated_decoder
-
-    # Resampling protocol args
-    use_ghost_grads: bool | list[bool] = (
-        False  # want to change this to true on some timeline.
-    )
-    feature_sampling_window: int = 2000
-    dead_feature_window: int = 1000  # unless this window is larger feature sampling,
-
-    dead_feature_threshold: float = 1e-8
-
-    # Evals
-    n_eval_batches: int = 10
-    eval_batch_size_prompts: int | None = None  # useful if evals cause OOM
-
-    # WANDB
-    log_to_wandb: bool = True
-    log_activations_store_to_wandb: bool = False
-    log_optimizer_state_to_wandb: bool = False
-    wandb_project: str = "mats_sae_training_language_model"
-    wandb_id: Optional[str] = None
-    run_name: Optional[str] = None
-    wandb_entity: Optional[str] = None
-    wandb_log_frequency: int = 10
-    eval_every_n_wandb_logs: int = 100  # logs every 1000 steps.
-
-    # Misc
-    resume: bool = False
-    n_checkpoints: int = 0
-    checkpoint_path: str = "checkpoints"
-    verbose: bool = True
-    model_kwargs: dict[str, Any] = field(default_factory=dict)
-    model_from_pretrained_kwargs: dict[str, Any] = field(default_factory=dict)
-    sae_lens_version: str = field(default_factory=lambda: __version__)
-    sae_lens_training_version: str = field(default_factory=lambda: __version__)
-
-    def __post_init__(self):
-        if self.use_cached_activations and self.cached_activations_path is None:
-            self.cached_activations_path = _default_cached_activations_path(
-                self.dataset_path,
-                self.model_name,
-                self.hook_point,
-                self.hook_point_head_index,
+class SAEConfig:
+
+    # forward pass details.
+    d_in: int
+    d_sae: int
+    activation_fn_str: str
+    apply_b_dec_to_input: bool
+    finetuning_scaling_factor: bool
+
+    # dataset it was trained on details.
+    context_size: int
+    model_name: str
+    hook_name: str
+    hook_layer: int
+    hook_head_index: Optional[int]
+    prepend_bos: bool
+    dataset_path: str
+    normalize_activations: bool
+
+    # misc
+    dtype: str
+    device: str
+    sae_lens_training_version: Optional[str]
+
+    @classmethod
+    def from_dict(cls, config_dict: dict[str, Any]) -> "SAEConfig":
+
+        # rename dict:
+        rename_dict = {  # old : new
+            "hook_point": "hook_name",
+            "hook_point_head_index": "hook_head_index",
+            "hook_point_layer": "hook_layer",
+            "activation_fn": "activation_fn_str",
+        }
+        config_dict = {rename_dict.get(k, k): v for k, v in config_dict.items()}
+
+        # use only config terms that are in the dataclass
+        config_dict = {
+            k: v for k, v in config_dict.items() if k in cls.__dataclass_fields__  # type: ignore
+        }
+        return cls(**config_dict)
+
+    # def __post_init__(self):
+
+    def to_dict(self) -> dict[str, Any]:
+        return {
+            "d_in": self.d_in,
+            "d_sae": self.d_sae,
+            "dtype": self.dtype,
+            "device": self.device,
+            "model_name": self.model_name,
+            "hook_name": self.hook_name,
+            "hook_layer": self.hook_layer,
+            "hook_head_index": self.hook_head_index,
+            "activation_fn_str": self.activation_fn_str,  # use string for serialization
+            "apply_b_dec_to_input": self.apply_b_dec_to_input,
+            "finetuning_scaling_factor": self.finetuning_scaling_factor,
+            "sae_lens_training_version": self.sae_lens_training_version,
+            "prepend_bos": self.prepend_bos,
+            "dataset_path": self.dataset_path,
+            "context_size": self.context_size,
+            "normalize_activations": self.normalize_activations,
+        }
+
+
+class SAE(HookedRootModule):
+    """ """
+
+    cfg: SAEConfig
+    dtype: torch.dtype
+    device: torch.device
+
+    # analysis
+    use_error_term: bool
+
+    def __init__(
+        self,
+        cfg: SAEConfig,
+        use_error_term: bool = False,
+    ):
+        super().__init__()
+
+        self.cfg = cfg
+        self.activation_fn = get_activation_fn(cfg.activation_fn_str)
+        self.dtype = DTYPE_MAP[cfg.dtype]
+        self.device = torch.device(cfg.device)
+        self.use_error_term = use_error_term
+
+        self.initialize_weights_basic()
+
+        # handle presence / absence of scaling factor.
+        if self.cfg.finetuning_scaling_factor:
+            self.apply_finetuning_scaling_factor = (
+                lambda x: x * self.finetuning_scaling_factor
             )
+        else:
+            self.apply_finetuning_scaling_factor = lambda x: x
 
-        if not isinstance(self.expansion_factor, list):
-            self.d_sae = self.d_in * self.expansion_factor
-        self.tokens_per_buffer = (
-            self.train_batch_size_tokens * self.context_size * self.n_batches_in_buffer
+        # set up hooks
+        self.hook_sae_input = HookPoint()
+        self.hook_sae_acts_pre = HookPoint()
+        self.hook_sae_acts_post = HookPoint()
+        self.hook_sae_output = HookPoint()
+        self.hook_sae_recons = HookPoint()
+        self.hook_sae_error = HookPoint()
+
+        # handle hook_z reshaping if needed.
+        # this is very cursed and should be refactored. it exists so that we can reshape out
+        # the z activations for hook_z SAEs. but don't know d_head if we split up the forward pass
+        # into a separate encode and decode function.
+        # this will cause errors if we call decode before encode.
+        self.reshape_fn_in = lambda x: x
+        self.reshape_fn_out = lambda x, d_head: x
+        self.d_head = None
+        if self.cfg.hook_name.endswith("_z"):
+
+            def reshape_fn_in(x: torch.Tensor):
+                self.d_head = x.shape[-1]  # type: ignore
+                self.reshape_fn_in = lambda x: einops.rearrange(
+                    x, "... n_heads d_head -> ... (n_heads d_head)"
+                )
+                return einops.rearrange(x, "... n_heads d_head -> ... (n_heads d_head)")
+
+            self.reshape_fn_in = reshape_fn_in
+
+        if self.cfg.hook_name.endswith("_z"):
+            self.reshape_fn_out = lambda x, d_head: einops.rearrange(
+                x, "... (n_heads d_head) -> ... n_heads d_head", d_head=d_head
+            )
+
+        self.setup()  # Required for `HookedRootModule`s
+
+    def initialize_weights_basic(self):
+
+        # no config changes encoder bias init for now.
+        self.b_enc = nn.Parameter(
+            torch.zeros(self.cfg.d_sae, dtype=self.dtype, device=self.device)
         )
 
-        if self.run_name is None:
-            self.run_name = f"{self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
-
-        if self.b_dec_init_method not in ["geometric_median", "mean", "zeros"]:
-            raise ValueError(
-                f"b_dec_init_method must be geometric_median, mean, or zeros. Got {self.b_dec_init_method}"
+        # Start with the default init strategy:
+        self.W_dec = nn.Parameter(
+            torch.nn.init.kaiming_uniform_(
+                torch.empty(
+                    self.cfg.d_sae, self.cfg.d_in, dtype=self.dtype, device=self.device
+                )
             )
+        )
 
-        if self.normalize_sae_decoder and self.decoder_heuristic_init:
-            raise ValueError(
-                "You can't normalize the decoder and use heuristic initialization."
+        self.W_enc = nn.Parameter(
+            torch.nn.init.kaiming_uniform_(
+                torch.empty(
+                    self.cfg.d_in, self.cfg.d_sae, dtype=self.dtype, device=self.device
+                )
             )
+        )
 
-        if self.normalize_sae_decoder and self.scale_sparsity_penalty_by_decoder_norm:
-            raise ValueError(
-                "Weighting loss by decoder norm makes no sense if you are normalizing the decoder weight norms to 1"
-            )
+        # methdods which change b_dec as a function of the dataset are implemented after init.
+        self.b_dec = nn.Parameter(
+            torch.zeros(self.cfg.d_in, dtype=self.dtype, device=self.device)
+        )
 
-        if isinstance(self.dtype, str) and self.dtype not in DTYPE_MAP:
-            raise ValueError(
-                f"dtype must be one of {list(DTYPE_MAP.keys())}. Got {self.dtype}"
-            )
-        elif isinstance(self.dtype, str):
-            self.dtype: torch.dtype = DTYPE_MAP[self.dtype]
+        # scaling factor for fine-tuning (not to be used in initial training)
+        # TODO: Make this optional and not included with all SAEs by default (but maintain backwards compatibility)
+        if self.cfg.finetuning_scaling_factor:
+            self.finetuning_scaling_factor = nn.Parameter(
+                torch.ones(self.cfg.d_sae, dtype=self.dtype, device=self.device)
+            )
+
+    # Basic Forward Pass Functionality.
+    def forward(
+        self,
+        x: torch.Tensor,
+    ) -> torch.Tensor:
+
+        feature_acts = self.encode(x)
+        sae_out = self.decode(feature_acts)
+
+        if self.use_error_term:
+            with torch.no_grad():
+                # Recompute everything without hooks to get true error term
+                # Otherwise, the output with error term will always equal input, even for causal interventions that affect x_reconstruct
+                # This is in a no_grad context to detach the error, so we can compute SAE feature gradients (eg for attribution patching). See A.3 in https://arxiv.org/pdf/2403.19647.pdf for more detail
+                # NOTE: we can't just use `sae_error = input - x_reconstruct.detach()` or something simpler, since this would mean intervening on features would mean ablating features still results in perfect reconstruction.
+
+                # move x to correct dtype
+                x = x.to(self.dtype)
+
+                # handle hook z reshaping if needed.
+                sae_in = self.reshape_fn_in(x)  # type: ignore
+
+                # apply b_dec_to_input if using that method.
+                sae_in_cent = sae_in - (self.b_dec * self.cfg.apply_b_dec_to_input)
+
+                # "... d_in, d_in d_sae -> ... d_sae",
+                hidden_pre = sae_in_cent @ self.W_enc + self.b_enc
+                feature_acts = self.activation_fn(hidden_pre)
+                x_reconstruct_clean = self.reshape_fn_out(
+                    self.apply_finetuning_scaling_factor(feature_acts) @ self.W_dec
+                    + self.b_dec,
+                    d_head=self.d_head,
+                )
+
+                sae_error = self.hook_sae_error(x - x_reconstruct_clean)
+
+            return self.hook_sae_output(sae_out + sae_error)
+
+        return self.hook_sae_output(sae_out)
+
+    def encode(
+        self, x: Float[torch.Tensor, "... d_in"]
+    ) -> Float[torch.Tensor, "... d_sae"]:
+
+        # move x to correct dtype
+        x = x.to(self.dtype)
+
+        # handle hook z reshaping if needed.
+        x = self.reshape_fn_in(x)  # type: ignore
+
+        # apply b_dec_to_input if using that method.
+        sae_in = self.hook_sae_input(x - (self.b_dec * self.cfg.apply_b_dec_to_input))
+
+        # "... d_in, d_in d_sae -> ... d_sae",
+        hidden_pre = self.hook_sae_acts_pre(sae_in @ self.W_enc + self.b_enc)
+        feature_acts = self.hook_sae_acts_post(self.activation_fn(hidden_pre))
+
+        return feature_acts
+
+    def decode(
+        self, feature_acts: Float[torch.Tensor, "... d_sae"]
+    ) -> Float[torch.Tensor, "... d_in"]:
+        """Decodes SAE feature activation tensor into a reconstructed input activation tensor."""
+        # "... d_sae, d_sae d_in -> ... d_in",
+        sae_out = self.hook_sae_recons(
+            self.apply_finetuning_scaling_factor(feature_acts) @ self.W_dec + self.b_dec
+        )
 
-        # if we use decoder fine tuning, we can't be applying b_dec to the input
-        if (self.finetuning_method == "decoder") and (self.apply_b_dec_to_input):
-            raise ValueError(
-                "If we are fine tuning the decoder, we can't be applying b_dec to the input.\nSet apply_b_dec_to_input to False."
-            )
+        # handle hook z reshaping if needed.
+        sae_out = self.reshape_fn_out(sae_out, self.d_head)  # type: ignore
 
-        self.device: str | torch.device = torch.device(self.device)
+        return sae_out
 
-        if self.lr_end is None:
-            if isinstance(self.lr, list):
-                self.lr_end = [lr / 10 for lr in self.lr]
-            else:
-                self.lr_end = self.lr / 10
-        unique_id = self.wandb_id
-        if unique_id is None:
-            unique_id = cast(
-                Any, wandb
-            ).util.generate_id()  # not sure why this type is erroring
-        self.checkpoint_path = f"{self.checkpoint_path}/{unique_id}"
-
-        if self.verbose:
-            print(
-                f"Run name: {self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
-            )
-            # Print out some useful info:
-            n_tokens_per_buffer = (
-                self.store_batch_size_prompts
-                * self.context_size
-                * self.n_batches_in_buffer
-            )
-            print(f"n_tokens_per_buffer (millions): {n_tokens_per_buffer / 10 ** 6}")
-            n_contexts_per_buffer = (
-                self.store_batch_size_prompts * self.n_batches_in_buffer
-            )
-            print(
-                f"Lower bound: n_contexts_per_buffer (millions): {n_contexts_per_buffer / 10 ** 6}"
-            )
+    def save_model(self, path: str, sparsity: Optional[torch.Tensor] = None):
 
-            total_training_steps = (
-                self.training_tokens + self.finetuning_tokens
-            ) // self.train_batch_size_tokens
-            print(f"Total training steps: {total_training_steps}")
-
-            total_wandb_updates = total_training_steps // self.wandb_log_frequency
-            print(f"Total wandb updates: {total_wandb_updates}")
-
-            # how many times will we sample dead neurons?
-            # assert self.dead_feature_window <= self.feature_sampling_window, "dead_feature_window must be smaller than feature_sampling_window"
-            n_feature_window_samples = (
-                total_training_steps // self.feature_sampling_window
-            )
-            print(
-                f"n_tokens_per_feature_sampling_window (millions): {(self.feature_sampling_window * self.context_size * self.train_batch_size_tokens) / 10 ** 6}"
-            )
-            print(
-                f"n_tokens_per_dead_feature_window (millions): {(self.dead_feature_window * self.context_size * self.train_batch_size_tokens) / 10 ** 6}"
-            )
-            print(
-                f"We will reset the sparsity calculation {n_feature_window_samples} times."
-            )
-            # print("Number tokens in dead feature calculation window: ", self.dead_feature_window * self.train_batch_size_tokens)
-            print(
-                f"Number tokens in sparsity calculation window: {self.feature_sampling_window * self.train_batch_size_tokens:.2e}"
-            )
+        if not os.path.exists(path):
+            os.mkdir(path)
 
-        if not isinstance(self.use_ghost_grads, list) and self.use_ghost_grads:
-            print("Using Ghost Grads.")
+        # generate the weights
+        save_file(self.state_dict(), f"{path}/{SAE_WEIGHTS_PATH}")
 
-    def get_checkpoints_by_step(self) -> tuple[dict[int, str], bool]:
-        """
-        Returns (dict, is_done)
-        where dict is [steps] = path
-        for each checkpoint, and
-        is_done is True if there is a "final_{steps}" checkpoint
-        """
-        is_done = False
-        checkpoints = [
-            f
-            for f in os.listdir(self.checkpoint_path)
-            if os.path.isdir(os.path.join(self.checkpoint_path, f))
-        ]
-        mapped_to_steps = {}
-        for c in checkpoints:
-            try:
-                steps = int(c)
-            except ValueError:
-                if c.startswith("final"):
-                    steps = int(c.split("_")[1])
-                    is_done = True
-                else:
-                    continue  # ignore this directory
-            full_path = os.path.join(self.checkpoint_path, c)
-            mapped_to_steps[steps] = full_path
-        return mapped_to_steps, is_done
+        # save the config
+        config = self.cfg.to_dict()
+
+        with open(f"{path}/{SAE_CFG_PATH}", "w") as f:
+            json.dump(config, f)
+
+        if sparsity is not None:
+            sparsity_in_dict = {"sparsity": sparsity}
+            save_file(sparsity_in_dict, f"{path}/{SPARSITY_PATH}")  # type: ignore
+
+    @classmethod
+    def load_from_pretrained(
+        cls, path: str, device: str = "cpu", dtype: str = "float32"
+    ) -> "SAE":
+
+        config_path = os.path.join(path, "cfg.json")
+        weight_path = os.path.join(path, "sae_weights.safetensors")
+
+        cfg_dict, state_dict, _ = load_pretrained_sae_lens_sae_components(
+            config_path, weight_path, device, dtype
+        )
+
+        sae_cfg = SAEConfig.from_dict(cfg_dict)
+
+        sae = cls(sae_cfg)
+        sae.load_state_dict(state_dict)
+
+        return sae
 
-    def get_resume_checkpoint_path(self) -> str:
+    @classmethod
+    def from_pretrained(
+        cls,
+        release: str,
+        sae_id: str,
+        device: str = "cpu",
+    ) -> Tuple["SAE", dict[str, Any], Optional[torch.Tensor]]:
         """
-        Gets the checkpoint path with the most steps
-        raises StopIteration if the model is done (there is a final_{steps} directoryh
-        raises FileNotFoundError if there are no checkpoints found
+
+        Load a pretrained SAE from the Hugging Face model hub.
+
+        Args:
+            release: The release name. This will be mapped to a huggingface repo id based on the pretrained_saes.yaml file.
+            id: The id of the SAE to load. This will be mapped to a path in the huggingface repo.
+            device: The device to load the SAE on.
+            return_sparsity_if_present: If True, will return the log sparsity tensor if it is present in the model directory in the Hugging Face model hub.
         """
-        mapped_to_steps, is_done = self.get_checkpoints_by_step()
-        if is_done:
-            raise StopIteration("Finished training model")
-        if len(mapped_to_steps) == 0:
-            raise FileNotFoundError("no checkpoints available to resume from")
-        else:
-            max_step = max(list(mapped_to_steps.keys()))
-            checkpoint_dir = mapped_to_steps[max_step]
-            print(f"resuming from step {max_step} at path {checkpoint_dir}")
-            return mapped_to_steps[max_step]
 
+        # get sae directory
+        sae_directory = get_pretrained_saes_directory()
 
-@dataclass
-class CacheActivationsRunnerConfig:
-    """
-    Configuration for caching activations of an LLM.
-    """
-
-    # Data Generating Function (Model + Training Distibuion)
-    model_name: str = "gelu-2l"
-    model_class_name: str = "HookedTransformer"
-    hook_point: str = "blocks.{layer}.hook_mlp_out"
-    hook_point_layer: int | list[int] = 0
-    hook_point_head_index: Optional[int] = None
-    dataset_path: str = "NeelNanda/c4-tokenized-2b"
-    streaming: bool = True
-    is_dataset_tokenized: bool = True
-    context_size: int = 128
-    new_cached_activations_path: Optional[str] = (
-        None  # Defaults to "activations/{dataset}/{model}/{full_hook_name}_{hook_point_head_index}"
-    )
-    # dont' specify this since you don't want to load from disk with the cache runner.
-    cached_activations_path: Optional[str] = None
-    # SAE Parameters
-    d_in: int = 512
-
-    # Activation Store Parameters
-    n_batches_in_buffer: int = 20
-    training_tokens: int = 2_000_000
-    store_batch_size_prompts: int = 32
-    train_batch_size_tokens: int = 4096
-    normalize_activations: bool = False
-
-    # Misc
-    device: str | torch.device = "cpu"
-    seed: int = 42
-    dtype: str | torch.dtype = "float32"
-    prepend_bos: bool = True
-
-    # Activation caching stuff
-    shuffle_every_n_buffers: int = 10
-    n_shuffles_with_last_section: int = 10
-    n_shuffles_in_entire_dir: int = 10
-    n_shuffles_final: int = 100
-    model_kwargs: dict[str, Any] = field(default_factory=dict)
-    model_from_pretrained_kwargs: dict[str, Any] = field(default_factory=dict)
-
-    def __post_init__(self):
-        # Autofill cached_activations_path unless the user overrode it
-        if self.new_cached_activations_path is None:
-            self.new_cached_activations_path = _default_cached_activations_path(
-                self.dataset_path,
-                self.model_name,
-                self.hook_point,
-                self.hook_point_head_index,
+        # get the repo id and path to the SAE
+        if release not in sae_directory:
+            raise ValueError(
+                f"Release {release} not found in pretrained SAEs directory."
             )
+        if sae_id not in sae_directory[release].saes_map:
+            raise ValueError(f"ID {sae_id} not found in release {release}.")
+        sae_info = sae_directory[release]
+        hf_repo_id = sae_info.repo_id
+        hf_path = sae_info.saes_map[sae_id]
 
+        conversion_loader_name = sae_info.conversion_func or "sae_lens"
+        if conversion_loader_name not in NAMED_PRETRAINED_SAE_LOADERS:
+            raise ValueError(
+                f"Conversion func {conversion_loader_name} not found in NAMED_PRETRAINED_SAE_LOADERS."
+            )
+        conversion_loader = NAMED_PRETRAINED_SAE_LOADERS[conversion_loader_name]
 
-@dataclass
-class ToyModelSAERunnerConfig:
-    # ReLu Model Parameters
-    n_features: int = 5
-    n_hidden: int = 2
-    n_correlated_pairs: int = 0
-    n_anticorrelated_pairs: int = 0
-    feature_probability: float = 0.025
-    model_training_steps: int = 10_000
-
-    # SAE Parameters
-    d_sae: int = 5
-
-    # Training Parameters
-    l1_coefficient: float = 1e-3
-    lr: float = 3e-4
-    train_batch_size: int = 1024
-    b_dec_init_method: str = "geometric_median"
-
-    # Sparsity / Dead Feature Handling
-    use_ghost_grads: bool = (
-        False  # not currently implemented, but SAE class expects it.
-    )
-    feature_sampling_window: int = 100
-    dead_feature_window: int = 100  # unless this window is larger feature sampling,
-    dead_feature_threshold: float = 1e-8
-
-    # Activation Store Parameters
-    total_training_tokens: int = 25_000
-
-    # WANDB
-    log_to_wandb: bool = True
-    wandb_project: str = "mats_sae_training_toy_model"
-    wandb_entity: str | None = None
-    wandb_log_frequency: int = 50
-
-    # Misc
-    device: str | torch.device = "cuda" if torch.cuda.is_available() else "cpu"
-    seed: int = 42
-    checkpoint_path: str = "checkpoints"
-    dtype: str | torch.dtype = "float32"
+        cfg_dict, state_dict, log_sparsities = conversion_loader(
+            repo_id=hf_repo_id,
+            folder_name=hf_path,
+            device=device,
+            force_download=False,
+        )
+
+        if "prepend_bos" not in cfg_dict:
+            # default to True for backwards compatibility
+            cfg_dict["prepend_bos"] = True
+
+        if "apply_b_dec_to_input" not in cfg_dict:
+            # default to True for backwards compatibility
+            cfg_dict["apply_b_dec_to_input"] = True
+
+        if "finetuning_scaling_factor" not in cfg_dict:
+            # default to False for backwards compatibility
+            cfg_dict["finetuning_scaling_factor"] = False
+
+        if "sae_lens_training_version" not in cfg_dict:
+            cfg_dict["sae_lens_training_version"] = None
+
+        if "activation_fn" not in cfg_dict:
+            cfg_dict["activation_fn_str"] = "relu"
+
+        if "normalize_activations" not in cfg_dict:
+            cfg_dict["normalize_activations"] = False
+
+        if "scaling_factor" in state_dict:
+            # we were adding it anyway for a period of time but are no longer doing so.
+            # so we should delete it if
+            if torch.allclose(
+                state_dict["scaling_factor"],
+                torch.ones_like(state_dict["scaling_factor"]),
+            ):
+                del state_dict["scaling_factor"]
+                cfg_dict["finetuning_scaling_factor"] = False
+            else:
+                assert cfg_dict[
+                    "finetuning_scaling_factor"
+                ], "Scaling factor is present but finetuning_scaling_factor is False."
+                state_dict["finetuning_scaling_factor"] = state_dict["scaling_factor"]
+                del state_dict["scaling_factor"]
+        else:
+            # it's there and it's not all 1's, we should use it.
+            cfg_dict["finetuning_scaling_factor"] = False
 
-    def __post_init__(self):
-        self.d_in = self.n_hidden  # hidden for the ReLu model is the input for the SAE
+        sae = cls(SAEConfig.from_dict(cfg_dict))
+        sae.load_state_dict(state_dict)
 
-        if isinstance(self.dtype, str) and self.dtype not in DTYPE_MAP:
-            raise ValueError(
-                f"dtype must be one of {list(DTYPE_MAP.keys())}. Got {self.dtype}"
-            )
-        elif isinstance(self.dtype, str):
-            self.dtype = DTYPE_MAP[self.dtype]
+        return sae, cfg_dict, log_sparsities
 
+    def get_name(self):
+        sae_name = f"sae_{self.cfg.model_name}_{self.cfg.hook_name}_{self.cfg.d_sae}"
+        return sae_name
 
-def _default_cached_activations_path(
-    dataset_path: str,
-    model_name: str,
-    hook_point: str,
-    hook_point_head_index: int | None,
-) -> str:
-    path = f"activations/{dataset_path.replace('/', '_')}/{model_name.replace('/', '_')}/{hook_point}"
-    if hook_point_head_index is not None:
-        path += f"_{hook_point_head_index}"
-    return path
+    @classmethod
+    def from_dict(cls, config_dict: dict[str, Any]) -> "SAE":
+        return cls(SAEConfig.from_dict(config_dict))
 
 
-@dataclass
-class PretokenizeRunnerConfig:
-    tokenizer_name: str = "gpt2"
-    dataset_path: str = "NeelNanda/c4-10k"
-    split: str | None = "train"
-    data_files: list[str] | None = None
-    data_dir: str | None = None
-    num_proc: int = 4
-    context_size: int = 128
-    column_name: str = "text"
-    shuffle: bool = True
-    seed: int | None = None
-    streaming: bool = False
-
-    # special tokens
-    begin_batch_token: int | Literal["bos", "eos", "sep"] | None = "bos"
-    begin_sequence_token: int | Literal["bos", "eos", "sep"] | None = None
-    sequence_separator_token: int | Literal["bos", "eos", "sep"] | None = "eos"
-
-    # if saving locally, set save_path
-    save_path: str | None = None
-
-    # if saving to huggingface, set hf_repo_id
-    hf_repo_id: str | None = None
-    hf_num_shards: int = 64
-    hf_revision: str = "main"
-    hf_is_private_repo: bool = False
+def get_activation_fn(activation_fn: str) -> Callable[[torch.Tensor], torch.Tensor]:
+    if activation_fn == "relu":
+        return torch.nn.ReLU()
+    elif activation_fn == "tanh-relu":
+
+        def tanh_relu(input: torch.Tensor) -> torch.Tensor:
+            input = torch.relu(input)
+            input = torch.tanh(input)
+            return input
+
+        return tanh_relu
+    else:
+        raise ValueError(f"Unknown activation function: {activation_fn}")
```

### Comparing `sae_lens-2.1.3/sae_lens/training/evals.py` & `sae_lens-3.0.0/sae_lens/evals.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 from functools import partial
 from typing import Any, Mapping, cast
 
 import pandas as pd
 import torch
-import wandb
 from transformer_lens.hook_points import HookedRootModule
 
+from sae_lens.sae import SAE
 from sae_lens.training.activations_store import ActivationsStore
-from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
 @torch.no_grad()
 def run_evals(
-    sparse_autoencoder: SparseAutoencoder,
+    sae: SAE,
     activation_store: ActivationsStore,
     model: HookedRootModule,
-    n_training_steps: int,
-    suffix: str = "",
     n_eval_batches: int = 10,
     eval_batch_size_prompts: int | None = None,
+    model_kwargs: Mapping[str, Any] = {},
 ) -> Mapping[str, Any]:
-    hook_point = sparse_autoencoder.cfg.hook_point
-    hook_point_layer = sparse_autoencoder.hook_point_layer
-    hook_point_head_index = sparse_autoencoder.cfg.hook_point_head_index
-    hook_point_eval = sparse_autoencoder.cfg.hook_point_eval.format(
-        layer=hook_point_layer
-    )
+    hook_name = sae.cfg.hook_name
+    hook_head_index = sae.cfg.hook_head_index
     ### Evals
     eval_tokens = activation_store.get_batch_tokens(eval_batch_size_prompts)
 
     # Get Reconstruction Score
     losses_df = recons_loss_batched(
-        sparse_autoencoder,
+        sae,
         model,
         activation_store,
         n_batches=n_eval_batches,
         eval_batch_size_prompts=eval_batch_size_prompts,
     )
 
     recons_score = losses_df["score"].mean()
@@ -43,79 +37,69 @@
     recons_loss = losses_df["recons_loss"].mean()
     zero_abl_loss = losses_df["zero_abl_loss"].mean()
 
     # get cache
     _, cache = model.run_with_cache(
         eval_tokens,
         prepend_bos=False,
-        names_filter=[hook_point_eval, hook_point],
-        **sparse_autoencoder.cfg.model_kwargs,
+        names_filter=[hook_name],
+        **model_kwargs,
     )
 
-    has_head_dim_key_substrings = ["hook_q", "hook_k", "hook_v", "hook_z"]
-    if hook_point_head_index is not None:
-        original_act = cache[hook_point][:, :, hook_point_head_index]
-    elif any(substring in hook_point for substring in has_head_dim_key_substrings):
-        original_act = cache[hook_point].flatten(-2, -1)
+    # we would include hook z, except that we now have base SAE's
+    # which will do their own reshaping for hook z.
+    has_head_dim_key_substrings = ["hook_q", "hook_k", "hook_v"]
+    if hook_head_index is not None:
+        original_act = cache[hook_name][:, :, hook_head_index]
+    elif any(substring in hook_name for substring in has_head_dim_key_substrings):
+        original_act = cache[hook_name].flatten(-2, -1)
     else:
-        original_act = cache[hook_point]
+        original_act = cache[hook_name]
 
     # normalise if necessary
     if activation_store.normalize_activations:
         original_act = activation_store.apply_norm_scaling_factor(original_act)
 
     # send the (maybe normalised) activations into the SAE
-    sae_out, _, _, _, _, _ = sparse_autoencoder(original_act)
+    sae_out = sae.decode(sae.encode(original_act))
     del cache
 
     l2_norm_in = torch.norm(original_act, dim=-1)
     l2_norm_out = torch.norm(sae_out, dim=-1)
     l2_norm_in_for_div = l2_norm_in.clone()
     l2_norm_in_for_div[torch.abs(l2_norm_in_for_div) < 0.0001] = 1
     l2_norm_ratio = l2_norm_out / l2_norm_in_for_div
 
-    W_dec_norm_dist = sparse_autoencoder.W_dec.norm(dim=1).detach().cpu().numpy()
-    b_e_dist = sparse_autoencoder.b_enc.detach().cpu().numpy()
-
     metrics = {
         # l2 norms
-        f"metrics/l2_norm{suffix}": l2_norm_out.mean().item(),
-        f"metrics/l2_ratio{suffix}": l2_norm_ratio.mean().item(),
-        f"metrics/l2_norm_in{suffix}": l2_norm_in.mean().item(),
-        # More detail on loss.
-        f"weights/W_dec_norms{suffix}": wandb.Histogram(W_dec_norm_dist),
-        f"weights/b_e{suffix}": wandb.Histogram(b_e_dist),
+        "metrics/l2_norm": l2_norm_out.mean().item(),
+        "metrics/l2_ratio": l2_norm_ratio.mean().item(),
+        "metrics/l2_norm_in": l2_norm_in.mean().item(),
         # CE Loss
-        f"metrics/CE_loss_score{suffix}": recons_score,
-        f"metrics/ce_loss_without_sae{suffix}": ntp_loss,
-        f"metrics/ce_loss_with_sae{suffix}": recons_loss,
-        f"metrics/ce_loss_with_ablation{suffix}": zero_abl_loss,
+        "metrics/CE_loss_score": recons_score,
+        "metrics/ce_loss_without_sae": ntp_loss,
+        "metrics/ce_loss_with_sae": recons_loss,
+        "metrics/ce_loss_with_ablation": zero_abl_loss,
     }
 
-    if wandb.run is not None:
-        wandb.log(
-            metrics,
-            step=n_training_steps,
-        )
-
     return metrics
 
 
 def recons_loss_batched(
-    sparse_autoencoder: SparseAutoencoder,
+    sae: SAE,
     model: HookedRootModule,
     activation_store: ActivationsStore,
     n_batches: int = 100,
     eval_batch_size_prompts: int | None = None,
 ):
     losses = []
     for _ in range(n_batches):
         batch_tokens = activation_store.get_batch_tokens(eval_batch_size_prompts)
         score, loss, recons_loss, zero_abl_loss = get_recons_loss(
-            sparse_autoencoder,
+            sae,
             model,
             batch_tokens,
             activation_store,
         )
         losses.append(
             (
                 score.mean().item(),
@@ -130,107 +114,101 @@
     )
 
     return losses
 
 
 @torch.no_grad()
 def get_recons_loss(
-    sparse_autoencoder: SparseAutoencoder,
+    sae: SAE,
     model: HookedRootModule,
     batch_tokens: torch.Tensor,
     activation_store: ActivationsStore,
+    model_kwargs: Mapping[str, Any] = {},
 ):
-    hook_point = sparse_autoencoder.cfg.hook_point
-    loss = model(
-        batch_tokens, return_type="loss", **sparse_autoencoder.cfg.model_kwargs
-    )
-    head_index = sparse_autoencoder.cfg.hook_point_head_index
+    hook_name = sae.cfg.hook_name
+    head_index = sae.cfg.hook_head_index
+
+    loss = model(batch_tokens, return_type="loss", **model_kwargs)
 
     # TODO(tomMcGrath): the rescaling below is a bit of a hack and could probably be tidied up
     def standard_replacement_hook(activations: torch.Tensor, hook: Any):
         # Handle rescaling if SAE expects it
         if activation_store.normalize_activations:
             activations = activation_store.apply_norm_scaling_factor(activations)
 
-        activations = sparse_autoencoder.forward(activations).sae_out.to(
-            activations.dtype
-        )
+        # SAE class agnost forward forward pass.
+        activations = sae.decode(sae.encode(activations)).to(activations.dtype)
 
         # Unscale if activations were scaled prior to going into the SAE
         if activation_store.normalize_activations:
             activations = activation_store.unscale(activations)
         return activations
 
     def all_head_replacement_hook(activations: torch.Tensor, hook: Any):
         # Handle rescaling if SAE expects it
         if activation_store.normalize_activations:
             activations = activation_store.apply_norm_scaling_factor(activations)
 
-        new_activations = sparse_autoencoder.forward(
-            activations.flatten(-2, -1)
-        ).sae_out.to(activations.dtype)
+        # SAE class agnost forward forward pass.
+        new_activations = sae.decode(sae.encode(activations.flatten(-2, -1))).to(
+            activations.dtype
+        )
+
         new_activations = new_activations.reshape(
             activations.shape
         )  # reshape to match original shape
 
         # Unscale if activations were scaled prior to going into the SAE
         if activation_store.normalize_activations:
             new_activations = activation_store.unscale(new_activations)
         return new_activations
 
     def single_head_replacement_hook(activations: torch.Tensor, hook: Any):
         # Handle rescaling if SAE expects it
         if activation_store.normalize_activations:
             activations = activation_store.apply_norm_scaling_factor(activations)
 
-        new_activations = sparse_autoencoder.forward(
-            activations[:, :, head_index]
-        ).sae_out.to(activations.dtype)
+        new_activations = sae.decoder(sae.encode(activations[:, :, head_index])).to(
+            activations.dtype
+        )
         activations[:, :, head_index] = new_activations
 
         # Unscale if activations were scaled prior to going into the SAE
         if activation_store.normalize_activations:
             activations = activation_store.unscale(activations)
         return activations
 
-    has_head_dim_key_substrings = ["hook_q", "hook_k", "hook_v", "hook_z"]
-    if any(substring in hook_point for substring in has_head_dim_key_substrings):
+    def zero_ablate_hook(activations: torch.Tensor, hook: Any):
+        activations = torch.zeros_like(activations)
+        return activations
+
+    # we would include hook z, except that we now have base SAE's
+    # which will do their own reshaping for hook z.
+    has_head_dim_key_substrings = ["hook_q", "hook_k", "hook_v"]
+    if any(substring in hook_name for substring in has_head_dim_key_substrings):
         if head_index is None:
             replacement_hook = all_head_replacement_hook
         else:
             replacement_hook = single_head_replacement_hook
     else:
         replacement_hook = standard_replacement_hook
 
     recons_loss = model.run_with_hooks(
         batch_tokens,
         return_type="loss",
-        fwd_hooks=[(hook_point, partial(replacement_hook))],
-        **sparse_autoencoder.cfg.model_kwargs,
+        fwd_hooks=[(hook_name, partial(replacement_hook))],
+        **model_kwargs,
     )
 
     zero_abl_loss = model.run_with_hooks(
         batch_tokens,
         return_type="loss",
-        fwd_hooks=[(hook_point, zero_ablate_hook)],
-        **sparse_autoencoder.cfg.model_kwargs,
+        fwd_hooks=[(hook_name, zero_ablate_hook)],
+        **model_kwargs,
     )
 
     div_val = zero_abl_loss - loss
     div_val[torch.abs(div_val) < 0.0001] = 1.0
 
     score = (zero_abl_loss - recons_loss) / div_val
 
     return score, loss, recons_loss, zero_abl_loss
-
-
-def zero_ablate_hook(activations: torch.Tensor, hook: Any):
-    activations = torch.zeros_like(activations)
-    return activations
-
-
-def kl_divergence_attention(y_true: torch.Tensor, y_pred: torch.Tensor):
-    # Compute log probabilities for KL divergence
-    log_y_true = torch.log2(y_true + 1e-10)
-    log_y_pred = torch.log2(y_pred + 1e-10)
-
-    return y_true * (log_y_true - log_y_pred)
```

### Comparing `sae_lens-2.1.3/sae_lens/training/geometric_median.py` & `sae_lens-3.0.0/sae_lens/training/geometric_median.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 @torch.no_grad()
 def geometric_median_objective(
     median: torch.Tensor, points: torch.Tensor, weights: torch.Tensor
 ) -> torch.Tensor:
 
-    norms = torch.linalg.norm(points - median.view(1, -1), dim=1)
+    norms = torch.linalg.norm(points - median.view(1, -1), dim=1)  # type: ignore
 
     return (norms * weights).sum()
 
 
 def compute_geometric_median(
     points: torch.Tensor,
     weights: Optional[torch.Tensor] = None,
@@ -56,15 +56,15 @@
 
         # Weiszfeld iterations
         early_termination = False
         pbar = tqdm.tqdm(range(maxiter))
         for _ in pbar:
             prev_obj_value = objective_value
 
-            norms = torch.linalg.norm(points - median.view(1, -1), dim=1)
+            norms = torch.linalg.norm(points - median.view(1, -1), dim=1)  # type: ignore
             new_weights = weights / torch.clamp(norms, min=eps)
             median = weighted_average(points, new_weights)
             objective_value = geometric_median_objective(median, points, weights)
 
             if logs is not None:
                 logs.append(objective_value)
             if abs(prev_obj_value - objective_value) <= ftol * objective_value:
```

### Comparing `sae_lens-2.1.3/sae_lens/training/load_model.py` & `sae_lens-3.0.0/sae_lens/load_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,20 +16,20 @@
     if model_class_name == "HookedTransformer":
         return HookedTransformer.from_pretrained(
             model_name=model_name, device=device, **model_from_pretrained_kwargs
         )
     elif model_class_name == "HookedMamba":
         try:
             from mamba_lens import HookedMamba
-        except ImportError:
+        except ImportError:  # pragma: no cover
             raise ValueError(
                 "mamba-lens must be installed to work with mamba models. This can be added with `pip install sae-lens[mamba]`"
             )
         # HookedMamba has incorrect typing information, so we need to cast the type here
         return cast(
             HookedRootModule,
             HookedMamba.from_pretrained(
                 model_name, device=cast(Any, device), **model_from_pretrained_kwargs
             ),
         )
-    else:
+    else:  # pragma: no cover
         raise ValueError(f"Unknown model class: {model_class_name}")
```

### Comparing `sae_lens-2.1.3/sae_lens/training/optim.py` & `sae_lens-3.0.0/sae_lens/training/optim.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 """
 
 from typing import Any
 
 import torch.optim as optim
 import torch.optim.lr_scheduler as lr_scheduler
 
-from sae_lens.training.sparse_autoencoder import SparseAutoencoder
-
 
 #  Constant
 #  Cosine Annealing with Warmup
 #  Cosine Annealing with Warmup / Restarts
 #  No default values specified so the type-checker can verify we don't forget any arguments.
 def get_lr_scheduler(
     scheduler_name: str,
@@ -104,55 +102,58 @@
 
 class L1Scheduler:
 
     def __init__(
         self,
         l1_warm_up_steps: float,
         total_steps: int,
-        sparse_autoencoder: SparseAutoencoder,
+        final_l1_coefficient: float,
     ):
 
         self.l1_warmup_steps = l1_warm_up_steps
-        self.total_steps = total_steps
-        self.sparse_autoencoder = sparse_autoencoder
-        self.final_l1_value = sparse_autoencoder.cfg.l1_coefficient
-        self.current_step = 0
-        assert isinstance(self.final_l1_value, float | int)
-
         # assume using warm-up
         if self.l1_warmup_steps != 0:
-            sparse_autoencoder.l1_coefficient = 0.0
+            self.current_l1_coefficient = 0.0
+        else:
+            self.current_l1_coefficient = final_l1_coefficient
+
+        self.final_l1_coefficient = final_l1_coefficient
+
+        self.current_step = 0
+        self.total_steps = total_steps
+        assert isinstance(self.final_l1_coefficient, float | int)
 
     def __repr__(self) -> str:
         return (
-            f"L1Scheduler(final_l1_value={self.final_l1_value}, "
+            f"L1Scheduler(final_l1_value={self.final_l1_coefficient}, "
             f"l1_warmup_steps={self.l1_warmup_steps}, "
             f"total_steps={self.total_steps})"
         )
 
     def step(self):
         """
         Updates the l1 coefficient of the sparse autoencoder.
         """
         step = self.current_step
         if step < self.l1_warmup_steps:
-            self.sparse_autoencoder.l1_coefficient = self.final_l1_value * (
+            self.current_l1_coefficient = self.final_l1_coefficient * (
                 (1 + step) / self.l1_warmup_steps
             )  # type: ignore
         else:
-            self.sparse_autoencoder.l1_coefficient = self.final_l1_value  # type: ignore
+            self.current_l1_coefficient = self.final_l1_coefficient  # type: ignore
 
         self.current_step += 1
 
     def state_dict(self):
         """State dict for serializing as part of an SAETrainContext."""
         return {
             "l1_warmup_steps": self.l1_warmup_steps,
             "total_steps": self.total_steps,
-            "final_l1_value": self.final_l1_value,
+            "current_l1_coefficient": self.current_l1_coefficient,
+            "final_l1_coefficient": self.final_l1_coefficient,
             "current_step": self.current_step,
         }
 
     def load_state_dict(self, state_dict: dict[str, Any]):
         """Loads all state apart from attached SAE."""
         for k in state_dict:
             setattr(self, k, state_dict[k])
```

### Comparing `sae_lens-2.1.3/sae_lens/training/pretokenize_runner.py` & `sae_lens-3.0.0/sae_lens/pretokenize_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import torch
 from datasets import Dataset, DatasetDict, load_dataset
 from huggingface_hub import HfApi
 from transformers import AutoTokenizer, PreTrainedTokenizerBase
 
 from sae_lens import __version__
-from sae_lens.training.batching import concat_and_batch_sequences
-from sae_lens.training.config import PretokenizeRunnerConfig
+from sae_lens.batching import concat_and_batch_sequences
+from sae_lens.config import PretokenizeRunnerConfig
 
 
 @dataclass
 class PretokenizedDatasetMetadata:
     """
     This metadata will be saved along with the pretokenized dataset as a JSON file.
     """
```

### Comparing `sae_lens-2.1.3/sae_lens/training/sparse_autoencoder.py` & `sae_lens-3.0.0/sae_lens/training/sae.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,283 +1,378 @@
 """Most of this is just copied over from Arthur's code and slightly simplified:
 https://github.com/ArthurConmy/sae/blob/main/sae/model.py
 """
 
-import gzip
-import json
 import os
-import pickle
-from typing import Callable, NamedTuple, Optional
+from dataclasses import dataclass
+from typing import Any, Callable, Optional
 
 import einops
 import torch
 from jaxtyping import Float
-from safetensors.torch import save_file
 from torch import nn
-from transformer_lens.hook_points import HookedRootModule, HookPoint
 
+from sae_lens.config import LanguageModelSAERunnerConfig
+from sae_lens.sae import SAE, SAEConfig
 from sae_lens.toolkit.pretrained_sae_loaders import (
-    NAMED_PRETRAINED_SAE_LOADERS,
     load_pretrained_sae_lens_sae_components,
 )
-from sae_lens.toolkit.pretrained_saes_directory import get_pretrained_saes_directory
-from sae_lens.training.activation_functions import get_activation_fn
-from sae_lens.training.config import LanguageModelSAERunnerConfig
-from sae_lens.training.utils import BackwardsCompatiblePickleClass
 
 SPARSITY_PATH = "sparsity.safetensors"
 SAE_WEIGHTS_PATH = "sae_weights.safetensors"
 SAE_CFG_PATH = "cfg.json"
 
 
-class ForwardOutput(NamedTuple):
+@dataclass
+class TrainStepOutput:
+    sae_in: torch.Tensor
     sae_out: torch.Tensor
     feature_acts: torch.Tensor
-    loss: torch.Tensor
-    mse_loss: torch.Tensor
-    l1_loss: torch.Tensor
-    ghost_grad_loss: torch.Tensor | float
+    loss: torch.Tensor  # we need to call backwards on this
+    mse_loss: float
+    l1_loss: float
+    ghost_grad_loss: float
 
 
-class SparseAutoencoder(HookedRootModule):
-    """ """
+@dataclass
+class TrainingSAEConfig(SAEConfig):
 
+    # Sparsity Loss Calculations
     l1_coefficient: float
     lp_norm: float
-    d_sae: int
     use_ghost_grads: bool
     normalize_sae_decoder: bool
-    hook_point_layer: int
-    dtype: torch.dtype
-    device: str | torch.device
     noise_scale: float
-    activation_fn: Callable[[torch.Tensor], torch.Tensor]
-
-    def __init__(
-        self,
-        cfg: LanguageModelSAERunnerConfig,
-    ):
-        super().__init__()
-        self.cfg = cfg
-        self.d_in = cfg.d_in
-        if not isinstance(self.d_in, int):
-            raise ValueError(
-                f"d_in must be an int but was {self.d_in=}; {type(self.d_in)=}"
-            )
-        assert cfg.d_sae is not None  # keep pyright happy
-        # lists are valid only for SAEGroup cfg, not SAE cfg vals
-        assert not isinstance(cfg.l1_coefficient, list)
-        assert not isinstance(cfg.lp_norm, list)
-        assert not isinstance(cfg.lr, list)
-        assert not isinstance(cfg.lr_scheduler_name, list)
-        assert not isinstance(cfg.lr_warm_up_steps, list)
-        assert not isinstance(cfg.use_ghost_grads, list)
-        assert not isinstance(cfg.hook_point_layer, list)
-        assert (
-            "{layer}" not in cfg.hook_point
-        ), "{layer} must be replaced with the actual layer number in SAE cfg"
-
-        self.d_sae = cfg.d_sae
-        self.l1_coefficient = cfg.l1_coefficient
-        self.lp_norm = cfg.lp_norm
-        self.dtype = cfg.dtype
-        self.device = cfg.device
-        self.use_ghost_grads = cfg.use_ghost_grads
-        self.normalize_sae_decoder = cfg.normalize_sae_decoder
-        self.hook_point_layer = cfg.hook_point_layer
-        self.noise_scale = cfg.noise_scale
-        self.activation_fn = get_activation_fn(cfg.activation_fn)
+    decoder_orthogonal_init: bool
+    mse_loss_normalization: Optional[str]
+    decoder_heuristic_init: bool = False
+    init_encoder_as_decoder_transpose: bool = False
+    scale_sparsity_penalty_by_decoder_norm: bool = False
 
-        if self.cfg.scale_sparsity_penalty_by_decoder_norm:
-            self.get_sparsity_loss_term = self.get_sparsity_loss_term_decoder_norm
-        else:
-            self.get_sparsity_loss_term = self.get_sparsity_loss_term_standard
-
-        self.initialize_weights()
-
-        self.hook_sae_in = HookPoint()
-        self.hook_hidden_pre = HookPoint()
-        self.hook_hidden_post = HookPoint()
-        self.hook_sae_out = HookPoint()
+    @classmethod
+    def from_sae_runner_config(
+        cls, cfg: LanguageModelSAERunnerConfig
+    ) -> "TrainingSAEConfig":
+
+        return cls(
+            # base confg
+            d_in=cfg.d_in,
+            d_sae=cfg.d_sae,  # type: ignore
+            dtype=cfg.dtype,
+            device=cfg.device,
+            model_name=cfg.model_name,
+            hook_name=cfg.hook_name,
+            hook_layer=cfg.hook_layer,
+            hook_head_index=cfg.hook_head_index,
+            activation_fn_str=cfg.activation_fn,
+            apply_b_dec_to_input=cfg.apply_b_dec_to_input,
+            finetuning_scaling_factor=cfg.finetuning_method is not None,
+            sae_lens_training_version=cfg.sae_lens_training_version,
+            context_size=cfg.context_size,
+            dataset_path=cfg.dataset_path,
+            prepend_bos=cfg.prepend_bos,
+            # Training cfg
+            l1_coefficient=cfg.l1_coefficient,
+            lp_norm=cfg.lp_norm,
+            use_ghost_grads=cfg.use_ghost_grads,
+            normalize_sae_decoder=cfg.normalize_sae_decoder,
+            noise_scale=cfg.noise_scale,
+            decoder_orthogonal_init=cfg.decoder_orthogonal_init,
+            mse_loss_normalization=cfg.mse_loss_normalization,
+            decoder_heuristic_init=cfg.decoder_heuristic_init,
+            init_encoder_as_decoder_transpose=cfg.init_encoder_as_decoder_transpose,
+            scale_sparsity_penalty_by_decoder_norm=cfg.scale_sparsity_penalty_by_decoder_norm,
+            normalize_activations=cfg.normalize_activations,
+        )
 
-        self.setup()  # Required for `HookedRootModule`s
+    @classmethod
+    def from_dict(cls, config_dict: dict[str, Any]) -> "TrainingSAEConfig":
+        return TrainingSAEConfig(**config_dict)
 
-    def initialize_weights(self):
-        """
-        Wrapped around weight initialization code to make init cleaner.
+    def to_dict(self) -> dict[str, Any]:
+        return {
+            **super().to_dict(),
+            "l1_coefficient": self.l1_coefficient,
+            "lp_norm": self.lp_norm,
+            "use_ghost_grads": self.use_ghost_grads,
+            "normalize_sae_decoder": self.normalize_sae_decoder,
+            "noise_scale": self.noise_scale,
+            "decoder_orthogonal_init": self.decoder_orthogonal_init,
+            "init_encoder_as_decoder_transpose": self.init_encoder_as_decoder_transpose,
+            "mse_loss_normalization": self.mse_loss_normalization,
+            "decoder_heuristic_init": self.decoder_heuristic_init,
+            "scale_sparsity_penalty_by_decoder_norm": self.scale_sparsity_penalty_by_decoder_norm,
+            "normalize_activations": self.normalize_activations,
+        }
 
-        """
+    # this needs to exist so we can initialize the parent sae cfg without the training specific
+    # parameters. Maybe there's a cleaner way to do this
+    def get_base_sae_cfg_dict(self) -> dict[str, Any]:
+        return {
+            "d_in": self.d_in,
+            "d_sae": self.d_sae,
+            "activation_fn_str": self.activation_fn_str,
+            "apply_b_dec_to_input": self.apply_b_dec_to_input,
+            "dtype": self.dtype,
+            "model_name": self.model_name,
+            "hook_name": self.hook_name,
+            "hook_layer": self.hook_layer,
+            "hook_head_index": self.hook_head_index,
+            "device": self.device,
+            "context_size": self.context_size,
+            "prepend_bos": self.prepend_bos,
+            "finetuning_scaling_factor": self.finetuning_scaling_factor,
+            "normalize_activations": self.normalize_activations,
+            "dataset_path": self.dataset_path,
+            "sae_lens_training_version": self.sae_lens_training_version,
+        }
 
-        # no config changes encoder bias init for now.
-        self.b_enc = nn.Parameter(
-            torch.zeros(self.d_sae, dtype=self.dtype, device=self.device)
-        )
 
-        # Start with the default init strategy:
-        self.W_dec = nn.Parameter(
-            torch.nn.init.kaiming_uniform_(
-                torch.empty(self.d_sae, self.d_in, dtype=self.dtype, device=self.device)
-            )
-        )
-        if self.cfg.decoder_orthogonal_init:
-            self.W_dec.data = nn.init.orthogonal_(self.W_dec.data.T).T
+class TrainingSAE(SAE):
 
-        elif self.cfg.decoder_heuristic_init:
-            self.W_dec = nn.Parameter(
-                torch.rand(self.d_sae, self.d_in, dtype=self.dtype, device=self.device)
-            )
-            self.initialize_decoder_norm_constant_norm()
+    cfg: TrainingSAEConfig  # type: ignore
+    use_error_term: bool
+    dtype: torch.dtype
+    device: torch.device
 
-        elif self.cfg.normalize_sae_decoder:
-            self.set_decoder_norm_to_unit_norm()
+    def __init__(self, cfg: TrainingSAEConfig, use_error_term: bool = False):
 
-        self.W_enc = nn.Parameter(
-            torch.nn.init.kaiming_uniform_(
-                torch.empty(self.d_in, self.d_sae, dtype=self.dtype, device=self.device)
-            )
-        )
+        base_sae_cfg = SAEConfig.from_dict(cfg.get_base_sae_cfg_dict())
+        super().__init__(base_sae_cfg)
+        self.cfg = cfg  # type: ignore
+        self.use_error_term = use_error_term
 
-        # Then we intialize the encoder weights (either as the transpose of decoder or not)
-        if self.cfg.init_encoder_as_decoder_transpose:
-            self.W_enc.data = self.W_dec.data.T.clone().contiguous()
-        else:
-            self.W_enc = nn.Parameter(
-                torch.nn.init.kaiming_uniform_(
-                    torch.empty(
-                        self.d_in, self.d_sae, dtype=self.dtype, device=self.device
-                    )
-                )
-            )
+        self.initialize_weights_complex()
 
-        if self.normalize_sae_decoder:
-            with torch.no_grad():
-                # Anthropic normalize this to have unit columns
-                self.set_decoder_norm_to_unit_norm()
+        # The training SAE will assume that the activation store handles
+        # reshaping.
+        self.reshape_fn_in = lambda x: x
+        self.reshape_fn_out = lambda x, d_head: x
 
-        # methdods which change b_dec as a function of the dataset are implemented after init.
-        self.b_dec = nn.Parameter(
-            torch.zeros(self.d_in, dtype=self.dtype, device=self.device)
-        )
+        self.mse_loss_fn = self._get_mse_loss_fn()
 
-        # scaling factor for fine-tuning (not to be used in initial training)
-        self.scaling_factor = nn.Parameter(
-            torch.ones(self.d_sae, dtype=self.dtype, device=self.device)
-        )
+    @classmethod
+    def from_dict(cls, config_dict: dict[str, Any]) -> "TrainingSAE":
+        return cls(TrainingSAEConfig.from_dict(config_dict))
 
     def encode(
         self, x: Float[torch.Tensor, "... d_in"]
     ) -> Float[torch.Tensor, "... d_sae"]:
-        feature_acts, _ = self._encode_with_hidden_pre(x)
+        feature_acts, _ = self.encode_with_hidden_pre(x)
         return feature_acts
 
-    def _encode_with_hidden_pre(
+    def encode_with_hidden_pre(
         self, x: Float[torch.Tensor, "... d_in"]
     ) -> tuple[Float[torch.Tensor, "... d_sae"], Float[torch.Tensor, "... d_sae"]]:
-        """Encodes input activation tensor x into an SAE feature activation tensor."""
+
         # move x to correct dtype
         x = x.to(self.dtype)
-        sae_in = self.hook_sae_in(
-            x - (self.b_dec * self.cfg.apply_b_dec_to_input)
-        )  # Remove decoder bias as per Anthropic
-
-        hidden_pre = self.hook_hidden_pre(
-            einops.einsum(
-                sae_in,
-                self.W_enc,
-                "... d_in, d_in d_sae -> ... d_sae",
-            )
-            + self.b_enc
-        )
-        noisy_hidden_pre = hidden_pre
-        if self.noise_scale > 0:
-            noise = torch.randn_like(hidden_pre) * self.noise_scale
-            noisy_hidden_pre = hidden_pre + noise
-        feature_acts = self.hook_hidden_post(self.activation_fn(noisy_hidden_pre))
 
-        return feature_acts, hidden_pre
+        # handle hook z reshaping if needed.
+        x = self.reshape_fn_in(x)  # type: ignore
 
-    def decode(
-        self, feature_acts: Float[torch.Tensor, "... d_sae"]
-    ) -> Float[torch.Tensor, "... d_in"]:
-        """Decodes SAE feature activation tensor into a reconstructed input activation tensor."""
-        sae_out = self.hook_sae_out(
-            einops.einsum(
-                feature_acts
-                * self.scaling_factor,  # need to make sure this handled when loading old models.
-                self.W_dec,
-                "... d_sae, d_sae d_in -> ... d_in",
-            )
-            + self.b_dec
-        )
-        return sae_out
+        # apply b_dec_to_input if using that method.
+        sae_in = self.hook_sae_input(x - (self.b_dec * self.cfg.apply_b_dec_to_input))
 
-    def get_sparsity_loss_term_standard(
-        self, feature_acts: torch.Tensor
-    ) -> torch.Tensor:
-        """
-        Sparsity loss term calculated as the L1 norm of the feature activations.
-        """
-        sparsity = feature_acts.norm(p=self.lp_norm, dim=-1)
-        return sparsity
+        # "... d_in, d_in d_sae -> ... d_sae",
+        hidden_pre = self.hook_sae_acts_pre(sae_in @ self.W_enc + self.b_enc)
+        hidden_pre_noised = hidden_pre + (
+            torch.randn_like(hidden_pre) * self.cfg.noise_scale * self.training
+        )
+        feature_acts = self.hook_sae_acts_post(self.activation_fn(hidden_pre_noised))
 
-    def get_sparsity_loss_term_decoder_norm(
-        self, feature_acts: torch.Tensor
-    ) -> torch.Tensor:
-        """
-        Sparsity loss term for decoder norm regularization.
-        """
-        weighted_feature_acts = feature_acts * self.W_dec.norm(dim=1)
-        sparsity = weighted_feature_acts.norm(
-            p=self.lp_norm, dim=-1
-        )  # sum over the feature dimension
-        return sparsity
+        return feature_acts, hidden_pre_noised
 
     def forward(
-        self, x: torch.Tensor, dead_neuron_mask: torch.Tensor | None = None
-    ) -> ForwardOutput:
+        self,
+        x: Float[torch.Tensor, "... d_in"],
+    ) -> Float[torch.Tensor, "... d_in"]:
 
-        feature_acts, hidden_pre = self._encode_with_hidden_pre(x)
+        feature_acts, _ = self.encode_with_hidden_pre(x)
         sae_out = self.decode(feature_acts)
 
-        # add config for whether l2 is normalized:
-        per_item_mse_loss = _per_item_mse_loss_with_target_norm(
-            sae_out, x, self.cfg.mse_loss_normalization
-        )
+        return sae_out
+
+    def training_forward_pass(
+        self,
+        sae_in: torch.Tensor,
+        current_l1_coefficient: float,
+        dead_neuron_mask: Optional[torch.Tensor] = None,
+    ) -> TrainStepOutput:  # type: ignore
+
+        # do a forward pass to get SAE out, but we also need the
+        # hidden pre.
+        feature_acts, _ = self.encode_with_hidden_pre(sae_in)
+        sae_out = self.decode(feature_acts)
 
-        # gate on config and training so evals is not slowed down.
-        if (
-            self.use_ghost_grads
-            and self.training
-            and dead_neuron_mask is not None
-            and dead_neuron_mask.sum() > 0
-        ):
+        # MSE LOSS
+        per_item_mse_loss = self.mse_loss_fn(sae_out, sae_in)
+        mse_loss = per_item_mse_loss.sum(dim=-1).mean()
+
+        # GHOST GRADS
+        if self.cfg.use_ghost_grads and self.training and dead_neuron_mask is not None:
+
+            # first half of second forward pass
+            _, hidden_pre = self.encode_with_hidden_pre(sae_in)
             ghost_grad_loss = self.calculate_ghost_grad_loss(
-                x=x,
+                x=sae_in,
                 sae_out=sae_out,
                 per_item_mse_loss=per_item_mse_loss,
                 hidden_pre=hidden_pre,
                 dead_neuron_mask=dead_neuron_mask,
             )
         else:
-            ghost_grad_loss = 0
+            ghost_grad_loss = 0.0
+
+        # SPARSITY LOSS
+        # either the W_dec norms are 1 and this won't do anything or they are not 1
+        # and we're using their norm in the loss function.
+        weighted_feature_acts = feature_acts * self.W_dec.norm(dim=1)
+        sparsity = weighted_feature_acts.norm(
+            p=self.cfg.lp_norm, dim=-1
+        )  # sum over the feature dimension
+
+        l1_loss = (current_l1_coefficient * sparsity).mean()
 
-        mse_loss = per_item_mse_loss.sum(dim=-1).mean()
-        sparsity = self.get_sparsity_loss_term(feature_acts)
-        l1_loss = (self.l1_coefficient * sparsity).mean()
         loss = mse_loss + l1_loss + ghost_grad_loss
 
-        return ForwardOutput(
+        return TrainStepOutput(
+            sae_in=sae_in,
             sae_out=sae_out,
             feature_acts=feature_acts,
             loss=loss,
-            mse_loss=mse_loss,
-            l1_loss=l1_loss,
-            ghost_grad_loss=ghost_grad_loss,
+            mse_loss=mse_loss.item(),
+            l1_loss=l1_loss.item(),
+            ghost_grad_loss=(
+                ghost_grad_loss.item()
+                if isinstance(ghost_grad_loss, torch.Tensor)
+                else ghost_grad_loss
+            ),
+        )
+
+    def calculate_ghost_grad_loss(
+        self,
+        x: torch.Tensor,
+        sae_out: torch.Tensor,
+        per_item_mse_loss: torch.Tensor,
+        hidden_pre: torch.Tensor,
+        dead_neuron_mask: torch.Tensor,
+    ) -> torch.Tensor:
+
+        # 1.
+        residual = x - sae_out
+        l2_norm_residual = torch.norm(residual, dim=-1)
+
+        # 2.
+        # ghost grads use an exponentional activation function, ignoring whatever
+        # the activation function is in the SAE. The forward pass uses the dead neurons only.
+        feature_acts_dead_neurons_only = torch.exp(hidden_pre[:, dead_neuron_mask])
+        ghost_out = feature_acts_dead_neurons_only @ self.W_dec[dead_neuron_mask, :]
+        l2_norm_ghost_out = torch.norm(ghost_out, dim=-1)
+        norm_scaling_factor = l2_norm_residual / (1e-6 + l2_norm_ghost_out * 2)
+        ghost_out = ghost_out * norm_scaling_factor[:, None].detach()
+
+        # 3. There is some fairly complex rescaling here to make sure that the loss
+        # is comparable to the original loss. This is because the ghost grads are
+        # only calculated for the dead neurons, so we need to rescale the loss to
+        # make sure that the loss is comparable to the original loss.
+        # There have been methodological improvements that are not implemented here yet
+        # see here: https://www.lesswrong.com/posts/C5KAZQib3bzzpeyrg/full-post-progress-update-1-from-the-gdm-mech-interp-team#Improving_ghost_grads
+        per_item_mse_loss_ghost_resid = self.mse_loss_fn(ghost_out, residual.detach())
+        mse_rescaling_factor = (
+            per_item_mse_loss / (per_item_mse_loss_ghost_resid + 1e-6)
+        ).detach()
+        per_item_mse_loss_ghost_resid = (
+            mse_rescaling_factor * per_item_mse_loss_ghost_resid
+        )
+
+        return per_item_mse_loss_ghost_resid.mean()
+
+    @torch.no_grad()
+    def _get_mse_loss_fn(self) -> Any:
+
+        def standard_mse_loss_fn(
+            preds: torch.Tensor, target: torch.Tensor
+        ) -> torch.Tensor:
+            return torch.nn.functional.mse_loss(preds, target, reduction="none")
+
+        def batch_norm_mse_loss_fn(
+            preds: torch.Tensor, target: torch.Tensor
+        ) -> torch.Tensor:
+            target_centered = target - target.mean(dim=0, keepdim=True)
+            normalization = target_centered.norm(dim=-1, keepdim=True)
+            return torch.nn.functional.mse_loss(preds, target, reduction="none") / (
+                normalization + 1e-6
+            )
+
+        if self.cfg.mse_loss_normalization == "dense_batch":
+            return batch_norm_mse_loss_fn
+        else:
+            return standard_mse_loss_fn
+
+    @classmethod
+    def load_from_pretrained(  # type: ignore
+        cls,
+        path: str,
+        device: str = "cpu",
+        dtype: str = "float32",
+    ) -> "TrainingSAE":
+
+        config_path = os.path.join(path, "cfg.json")
+        weight_path = os.path.join(path, "sae_weights.safetensors")
+
+        cfg_dict, state_dict, _ = load_pretrained_sae_lens_sae_components(
+            config_path, weight_path, device, dtype
         )
 
+        sae_cfg = TrainingSAEConfig.from_dict(cfg_dict)
+
+        sae = cls(sae_cfg)
+        sae.load_state_dict(state_dict)
+
+        return sae
+
+    def initialize_weights_complex(self):
+        """ """
+
+        if self.cfg.decoder_orthogonal_init:
+            self.W_dec.data = nn.init.orthogonal_(self.W_dec.data.T).T
+
+        elif self.cfg.decoder_heuristic_init:
+            self.W_dec = nn.Parameter(
+                torch.rand(
+                    self.cfg.d_sae, self.cfg.d_in, dtype=self.dtype, device=self.device
+                )
+            )
+            self.initialize_decoder_norm_constant_norm()
+
+        elif self.cfg.normalize_sae_decoder:
+            self.set_decoder_norm_to_unit_norm()
+
+        # Then we intialize the encoder weights (either as the transpose of decoder or not)
+        if self.cfg.init_encoder_as_decoder_transpose:
+            self.W_enc.data = self.W_dec.data.T.clone().contiguous()
+        else:
+            self.W_enc = nn.Parameter(
+                torch.nn.init.kaiming_uniform_(
+                    torch.empty(
+                        self.cfg.d_in,
+                        self.cfg.d_sae,
+                        dtype=self.dtype,
+                        device=self.device,
+                    )
+                )
+            )
+
+        if self.cfg.normalize_sae_decoder:
+            with torch.no_grad():
+                # Anthropic normalize this to have unit columns
+                self.set_decoder_norm_to_unit_norm()
+
+    ## Initialization Methods
     @torch.no_grad()
     def initialize_b_dec_with_precalculated(self, origin: torch.Tensor):
         out = torch.tensor(origin, dtype=self.dtype, device=self.device)
         self.b_dec.data = out
 
     @torch.no_grad()
     def initialize_b_dec_with_mean(self, all_activations: torch.Tensor):
@@ -291,29 +386,30 @@
         print(
             f"Previous distances: {previous_distances.median(0).values.mean().item()}"
         )
         print(f"New distances: {distances.median(0).values.mean().item()}")
 
         self.b_dec.data = out.to(self.dtype).to(self.device)
 
+    ## Training Utils
     @torch.no_grad()
     def set_decoder_norm_to_unit_norm(self):
         self.W_dec.data /= torch.norm(self.W_dec.data, dim=1, keepdim=True)
 
     @torch.no_grad()
     def initialize_decoder_norm_constant_norm(self, norm: float = 0.1):
         """
         A heuristic proceedure inspired by:
         https://transformer-circuits.pub/2024/april-update/index.html#training-saes
         """
         # TODO: Parameterise this as a function of m and n
 
         # ensure W_dec norms at unit norm
         self.W_dec.data /= torch.norm(self.W_dec.data, dim=1, keepdim=True)
-        self.W_dec.data *= 0.1  # will break tests but do this for now.
+        self.W_dec.data *= norm  # will break tests but do this for now.
 
     @torch.no_grad()
     def remove_gradient_parallel_to_decoder_directions(self):
         """
         Update grads so that they remove the parallel component
             (d_sae, d_in) shape
         """
@@ -326,233 +422,21 @@
         )
         self.W_dec.grad -= einops.einsum(
             parallel_component,
             self.W_dec.data,
             "d_sae, d_sae d_in -> d_sae d_in",
         )
 
-    def save_model_legacy(self, path: str):
-        """
-        Basic save function for the model. Saves the model's state_dict and the config used to train it.
-        """
-
-        # check if path exists
-        folder = os.path.dirname(path)
-        os.makedirs(folder, exist_ok=True)
-
-        state_dict = {"cfg": self.cfg, "state_dict": self.state_dict()}
-
-        if path.endswith(".pt"):
-            torch.save(state_dict, path)
-        else:
-            raise ValueError(
-                f"Unexpected file extension: {path}, supported extensions are .pt and .pkl.gz"
-            )
-
-        print(f"Saved model to {path}")
-
-    def save_model(self, path: str, sparsity: Optional[torch.Tensor] = None):
-
-        if not os.path.exists(path):
-            os.mkdir(path)
-
-        # generate the weights
-        save_file(self.state_dict(), f"{path}/{SAE_WEIGHTS_PATH}")
-
-        # save the config
-        config = {
-            **self.cfg.__dict__,
-            # some args may not be serializable by default
-            "dtype": str(self.cfg.dtype),
-            "device": str(self.cfg.device),
-        }
-
-        with open(f"{path}/{SAE_CFG_PATH}", "w") as f:
-            json.dump(config, f)
-
-        if sparsity is not None:
-            sparsity_in_dict = {"sparsity": sparsity}
-            save_file(sparsity_in_dict, f"{path}/{SPARSITY_PATH}")  # type: ignore
-
-    @classmethod
-    def load_from_pretrained_legacy(cls, path: str):
-        """
-        Load function for the model. Loads the model's state_dict and the config used to train it.
-        This method can be called directly on the class, without needing an instance.
-        """
-
-        # Ensure the file exists
-        if not os.path.isfile(path):
-            raise FileNotFoundError(f"No file found at specified path: {path}")
-
-        # Load the state dictionary
-        if path.endswith(".pt"):
-            try:
-                if torch.backends.mps.is_available():
-                    state_dict = torch.load(
-                        path,
-                        map_location="mps",
-                        pickle_module=BackwardsCompatiblePickleClass,
-                    )
-                    state_dict["cfg"].device = "mps"
-                else:
-                    state_dict = torch.load(
-                        path, pickle_module=BackwardsCompatiblePickleClass
-                    )
-            except Exception as e:
-                raise IOError(f"Error loading the state dictionary from .pt file: {e}")
-        elif path.endswith(".pkl.gz"):
-            try:
-                with gzip.open(path, "rb") as f:
-                    state_dict = pickle.load(f)
-            except Exception as e:
-                raise IOError(
-                    f"Error loading the state dictionary from .pkl.gz file: {e}"
-                )
-        elif path.endswith(".pkl"):
-            try:
-                with open(path, "rb") as f:
-                    state_dict = pickle.load(f)
-            except Exception as e:
-                raise IOError(f"Error loading the state dictionary from .pkl file: {e}")
-        else:
-            raise ValueError(
-                f"Unexpected file extension: {path}, supported extensions are .pt, .pkl, and .pkl.gz"
-            )
-
-        # Ensure the loaded state contains both 'cfg' and 'state_dict'
-        if "cfg" not in state_dict or "state_dict" not in state_dict:
-            raise ValueError(
-                "The loaded state dictionary must contain 'cfg' and 'state_dict' keys"
-            )
-
-        # Create an instance of the class using the loaded configuration
-        instance = cls(cfg=state_dict["cfg"])
-        if "scaling_factor" not in state_dict["state_dict"]:
-            assert isinstance(instance.cfg.d_sae, int)
-            state_dict["state_dict"]["scaling_factor"] = torch.ones(
-                instance.cfg.d_sae, dtype=instance.cfg.dtype, device=instance.cfg.device
-            )
-        instance.load_state_dict(state_dict["state_dict"], strict=True)
-
-        return instance
-
-    @classmethod
-    def load_from_pretrained(
-        cls, path: str, device: str = "cpu"
-    ) -> "SparseAutoencoder":
-
-        config_path = os.path.join(path, "cfg.json")
-        weight_path = os.path.join(path, "sae_weights.safetensors")
-
-        cfg, state_dict = load_pretrained_sae_lens_sae_components(
-            config_path, weight_path, device
-        )
-
-        sae = cls(cfg)
-        sae.load_state_dict(state_dict)
-
-        return sae
-
-    @classmethod
-    def from_pretrained(
-        cls, release: str, sae_id: str, device: str = "cpu"
-    ) -> "SparseAutoencoder":
-        """
-
-        Load a pretrained SAE from the Hugging Face model hub.
-
-        Args:
-            release: The release name. This will be mapped to a huggingface repo id based on the pretrained_saes.yaml file.
-            id: The id of the SAE to load. This will be mapped to a path in the huggingface repo.
-            device: The device to load the SAE on.
-
-        """
-
-        # get sae directory
-        sae_directory = get_pretrained_saes_directory()
-
-        # get the repo id and path to the SAE
-        if release not in sae_directory:
-            raise ValueError(
-                f"Release {release} not found in pretrained SAEs directory."
-            )
-        if sae_id not in sae_directory[release].saes_map:
-            raise ValueError(f"ID {sae_id} not found in release {release}.")
-        sae_info = sae_directory[release]
-        hf_repo_id = sae_info.repo_id
-        hf_path = sae_info.saes_map[sae_id]
-
-        conversion_loader_name = sae_info.conversion_func or "sae_lens"
-        if conversion_loader_name not in NAMED_PRETRAINED_SAE_LOADERS:
-            raise ValueError(
-                f"Conversion func {conversion_loader_name} not found in NAMED_PRETRAINED_SAE_LOADERS."
-            )
-        conversion_loader = NAMED_PRETRAINED_SAE_LOADERS[conversion_loader_name]
-
-        cfg, state_dict = conversion_loader(
-            repo_id=hf_repo_id,
-            folder_name=hf_path,
-            device=device,
-            force_download=False,
-        )
-
-        sae = cls(cfg)
-        sae.load_state_dict(state_dict)
-
-        return sae
-
-    def get_name(self):
-        sae_name = f"sparse_autoencoder_{self.cfg.model_name}_{self.cfg.hook_point}_{self.cfg.d_sae}"
-        return sae_name
-
-    def calculate_ghost_grad_loss(
-        self,
-        x: torch.Tensor,
-        sae_out: torch.Tensor,
-        per_item_mse_loss: torch.Tensor,
-        hidden_pre: torch.Tensor,
-        dead_neuron_mask: torch.Tensor,
-    ) -> torch.Tensor:
-        # 1.
-        residual = x - sae_out
-        l2_norm_residual = torch.norm(residual, dim=-1)
-
-        # 2.
-        feature_acts_dead_neurons_only = torch.exp(hidden_pre[:, dead_neuron_mask])
-        ghost_out = feature_acts_dead_neurons_only @ self.W_dec[dead_neuron_mask, :]
-        l2_norm_ghost_out = torch.norm(ghost_out, dim=-1)
-        norm_scaling_factor = l2_norm_residual / (1e-6 + l2_norm_ghost_out * 2)
-        ghost_out = ghost_out * norm_scaling_factor[:, None].detach()
-
-        # 3.
-        per_item_mse_loss_ghost_resid = _per_item_mse_loss_with_target_norm(
-            ghost_out, residual.detach(), self.cfg.mse_loss_normalization
-        )
-        mse_rescaling_factor = (
-            per_item_mse_loss / (per_item_mse_loss_ghost_resid + 1e-6)
-        ).detach()
-        per_item_mse_loss_ghost_resid = (
-            mse_rescaling_factor * per_item_mse_loss_ghost_resid
-        )
-
-        return per_item_mse_loss_ghost_resid.mean()
 
+def get_activation_fn(activation_fn: str) -> Callable[[torch.Tensor], torch.Tensor]:
+    if activation_fn == "relu":
+        return torch.nn.ReLU()
+    elif activation_fn == "tanh-relu":
+
+        def tanh_relu(input: torch.Tensor) -> torch.Tensor:
+            input = torch.relu(input)
+            input = torch.tanh(input)
+            return input
 
-def _per_item_mse_loss_with_target_norm(
-    preds: torch.Tensor,
-    target: torch.Tensor,
-    mse_loss_normalization: Optional[str] = None,
-) -> torch.Tensor:
-    """
-    Calculate MSE loss per item in the batch, without taking a mean.
-    Then, optionally, normalizes by the L2 norm of the centered target.
-    This normalization seems to improve performance.
-    """
-    if mse_loss_normalization == "dense_batch":
-        target_centered = target - target.mean(dim=0, keepdim=True)
-        normalization = target_centered.norm(dim=-1, keepdim=True)
-        return torch.nn.functional.mse_loss(preds, target, reduction="none") / (
-            normalization + 1e-6
-        )
+        return tanh_relu
     else:
-        return torch.nn.functional.mse_loss(preds, target, reduction="none")
+        raise ValueError(f"Unknown activation function: {activation_fn}")
```

### Comparing `sae_lens-2.1.3/sae_lens/training/toy_models.py` & `sae_lens-3.0.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.3/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-3.0.0/sae_lens/training/train_toy_sae.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Any, cast
 
 import torch
 import wandb
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-from sae_lens.training.sparse_autoencoder import SparseAutoencoder
+from sae_lens.sae import SAE
 
 
 def train_toy_sae(
-    sparse_autoencoder: SparseAutoencoder,
+    sparse_autoencoder: SAE,
     activation_store: torch.Tensor,  # TODO: this type seems strange / wrong
     batch_size: int = 1024,
     feature_sampling_window: int = 100,  # how many training steps between resampling the features / considiring neurons dead
-    dead_feature_window: int = 2000,  # how many training steps before a feature is considered dead
     dead_feature_threshold: float = 1e-8,  # how infrequently a feature has to be active to be considered dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
 ):
     """
     Takes an SAE and a bunch of activations and does a bunch of training steps
     """
```

### Comparing `sae_lens-2.1.3/PKG-INFO` & `sae_lens-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 2.1.3
+Version: 3.0.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

