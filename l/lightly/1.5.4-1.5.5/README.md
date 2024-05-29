# Comparing `tmp/lightly-1.5.4.tar.gz` & `tmp/lightly-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightly-1.5.4.tar", last modified: Thu May 16 12:54:12 2024, max compression
+gzip compressed data, was "lightly-1.5.5.tar", last modified: Wed May 29 13:06:17 2024, max compression
```

## Comparing `lightly-1.5.4.tar` & `lightly-1.5.5.tar`

### file list

```diff
@@ -1,472 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.207729 lightly-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 12:54:00.000000 lightly-1.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 12:54:00.000000 lightly-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    25843 2024-05-16 12:54:12.207729 lightly-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24261 2024-05-16 12:54:00.000000 lightly-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.139728 lightly-1.5.4/lightly/
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.139728 lightly-1.5.4/lightly/active_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/active_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.139728 lightly-1.5.4/lightly/active_learning/config/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/active_learning/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/active_learning/config/selection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.143728 lightly-1.5.4/lightly/api/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/_version_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_collaboration.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_compute_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    20194 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    36969 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_download_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13415 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_upload_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/bitmask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/swagger_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/swagger_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.143728 lightly-1.5.4/lightly/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/_cli_simclr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.147728 lightly-1.5.4/lightly/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/config/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/config/lightly-serve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/crop_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/download_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/embed_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/lightly_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/serve_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/train_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/version_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.147728 lightly-1.5.4/lightly/data/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_image_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25874 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)    55856 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/lightly_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/multi_view_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.147728 lightly-1.5.4/lightly/embedding/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/embedding/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/embedding/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/embedding/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.151728 lightly-1.5.4/lightly/loss/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/dcl_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/dino_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/emp_ssl_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/hypersphere_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/mmcr_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/msn_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/negative_cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/ntx_ent_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/pmsn_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.151728 lightly-1.5.4/lightly/loss/regularizer/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/regularizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/regularizer/co2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/swav_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/sym_neg_cos_sim_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/tico_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/vicreg_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    17701 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/vicregl_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/wmse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.151728 lightly-1.5.4/lightly/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/_momentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/byol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/moco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.155728 lightly-1.5.4/lightly/models/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/heads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/heads_timm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/ijepa.py
--rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_autoencoder_timm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_causal_vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_vision_transformer_timm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_vision_transformer_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/nn_memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/nnclr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/simclr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (127)    25558 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.155728 lightly-1.5.4/lightly/openapi_generated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.155728 lightly-1.5.4/lightly/openapi_generated/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (127)    31348 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.159728 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22634 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/collaboration_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    98546 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   136811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/datasources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   308272 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/docker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24023 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    52405 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/embeddings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/mappings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30243 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    61239 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/predictions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/quota_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    81340 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/samples_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/samplings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    51643 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/scores_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   160366 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/versioning_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.199729 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    29144 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_types_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/api_error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/api_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/async_task_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_cf_bucket_activity_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_entity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_team_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/crop_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_base_full_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_local_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/delegated_access_external_ids_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_authorization_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_authorization_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_license_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_storage_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_create_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_docker_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_task_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_authorization_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_datasource_input_expiration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/expiry_handling_strategy_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/file_name_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/file_output_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/internal_debug_latency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/internal_debug_latency_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_result_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/jobs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_studio_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_docker_selection_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_me_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_me_data_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/s3_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sama_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sama_task_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_input_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/service_account_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/task_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/update_team_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/video_frame_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.203729 lightly-1.5.4/lightly/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/aim_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/byol_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/dino_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/fast_siam_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/ijepa_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/image_grid_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/mae_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/mmcr_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/moco_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/msn_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/multi_crop_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/multi_view_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/pirl_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/random_crop_and_flip_with_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/simclr_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/simsiam_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/smog_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/solarize.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/swav_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/vicreg_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/vicregl_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/wmse_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.203729 lightly-1.5.4/lightly/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.207729 lightly-1.5.4/lightly/utils/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/benchmark_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/knn_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/linear_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/metric_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/online_linear_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/topk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/bounding_box.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.207729 lightly-1.5.4/lightly/utils/cropping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/cropping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/cropping/crop_image_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/cropping/read_yolo_label_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/embeddings_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/hipify.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/lars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/reordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.139728 lightly-1.5.4/lightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25843 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 12:54:00.000000 lightly-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:54:12.207729 lightly-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-16 12:54:00.000000 lightly-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.947157 lightly-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 13:06:08.000000 lightly-1.5.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 13:06:08.000000 lightly-1.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25843 2024-05-29 13:06:17.947157 lightly-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24261 2024-05-29 13:06:08.000000 lightly-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.883157 lightly-1.5.5/lightly/
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.887157 lightly-1.5.5/lightly/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/active_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.887157 lightly-1.5.5/lightly/active_learning/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/active_learning/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/active_learning/config/selection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.887157 lightly-1.5.5/lightly/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/_version_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_compute_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20194 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36969 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_download_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13415 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_upload_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/api_workflow_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/bitmask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/swagger_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/swagger_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.891157 lightly-1.5.5/lightly/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/_cli_simclr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.891157 lightly-1.5.5/lightly/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/config/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/config/lightly-serve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/crop_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/download_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/embed_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/lightly_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/serve_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/train_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/cli/version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.891157 lightly-1.5.5/lightly/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/_image_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25874 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55856 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/lightly_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/data/multi_view_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.891157 lightly-1.5.5/lightly/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/embedding/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/embedding/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/embedding/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.895157 lightly-1.5.5/lightly/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/dcl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/dino_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/emp_ssl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/hypersphere_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/mmcr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/msn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/negative_cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/ntx_ent_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/pmsn_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.895157 lightly-1.5.5/lightly/loss/regularizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/regularizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/regularizer/co2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/swav_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/sym_neg_cos_sim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/tico_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/vicreg_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17701 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/vicregl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/loss/wmse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.895157 lightly-1.5.5/lightly/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/byol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/moco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.899157 lightly-1.5.5/lightly/models/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/heads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/heads_timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/ijepa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/masked_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/masked_autoencoder_timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/masked_causal_vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/masked_vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/masked_vision_transformer_timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/masked_vision_transformer_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/modules/nn_memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/nnclr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26487 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/models/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.899157 lightly-1.5.5/lightly/openapi_generated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.899157 lightly-1.5.5/lightly/openapi_generated/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    31348 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.903157 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22634 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/collaboration_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98546 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136811 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/datasources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   308272 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/docker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24023 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52405 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/embeddings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/mappings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30243 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61239 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/predictions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/quota_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81340 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/samples_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/samplings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51643 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/scores_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   160366 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api/versioning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.939157 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    29144 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/active_learning_score_types_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/active_learning_score_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/api_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/api_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/async_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/configuration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/configuration_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_cf_bucket_activity_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_team_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_azure_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_base_full_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_gcs_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_local_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_obs_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/delegated_access_external_ids_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_authorization_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_authorization_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_license_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_storage_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_create_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_docker_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_task_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_authorization_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_datasource_input_expiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/expiry_handling_strategy_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/file_name_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/file_output_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/internal_debug_latency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/internal_debug_latency_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_status_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/jobs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/label_studio_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_docker_selection_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/profile_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/profile_me_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/profile_me_data_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/s3_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sama_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sama_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sampling_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sampling_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/service_account_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/shared_access_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/team_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/team_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/team_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/update_team_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/video_frame_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/openapi_generated/swagger_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.943157 lightly-1.5.5/lightly/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/aim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/byol_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/dino_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/fast_siam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/ijepa_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/image_grid_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/mae_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/mmcr_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/moco_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/msn_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/multi_crop_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/multi_view_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/pirl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/random_crop_and_flip_with_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/simclr_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/simsiam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/smog_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/swav_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/vicreg_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/vicregl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/transforms/wmse_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.947157 lightly-1.5.5/lightly/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.947157 lightly-1.5.5/lightly/utils/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/benchmarking/benchmark_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/benchmarking/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/benchmarking/knn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/benchmarking/linear_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/benchmarking/metric_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/benchmarking/online_linear_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/benchmarking/topk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.947157 lightly-1.5.5/lightly/utils/cropping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/cropping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/cropping/crop_image_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/cropping/read_yolo_label_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/embeddings_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/hipify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/lars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/reordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-29 13:06:08.000000 lightly-1.5.5/lightly/utils/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:06:17.887157 lightly-1.5.5/lightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25843 2024-05-29 13:06:17.000000 lightly-1.5.5/lightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-05-29 13:06:17.000000 lightly-1.5.5/lightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:06:17.000000 lightly-1.5.5/lightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-29 13:06:17.000000 lightly-1.5.5/lightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-29 13:06:17.000000 lightly-1.5.5/lightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 13:06:17.000000 lightly-1.5.5/lightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 13:06:08.000000 lightly-1.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:06:17.947157 lightly-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-29 13:06:08.000000 lightly-1.5.5/setup.py
```

### Comparing `lightly-1.5.4/LICENSE.txt` & `lightly-1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/PKG-INFO` & `lightly-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.5.4
+Version: 1.5.5
 Summary: A deep learning package for self-supervised learning
 Author: Lightly Team
 Author-email: team@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.5.4/README.md` & `lightly-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/__init__.py` & `lightly-1.5.5/lightly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 __name__ = "lightly"
-__version__ = "1.5.4"
+__version__ = "1.5.5"
 
 
 import os
 
 if os.getenv("LIGHTLY_DID_VERSION_CHECK", "False") == "False":
     os.environ["LIGHTLY_DID_VERSION_CHECK"] = "True"
     import multiprocessing
```

### Comparing `lightly-1.5.4/lightly/active_learning/config/selection_config.py` & `lightly-1.5.5/lightly/active_learning/config/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/__init__.py` & `lightly-1.5.5/lightly/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/_version_checking.py` & `lightly-1.5.5/lightly/api/_version_checking.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_artifacts.py` & `lightly-1.5.5/lightly/api/api_workflow_artifacts.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_client.py` & `lightly-1.5.5/lightly/api/api_workflow_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_collaboration.py` & `lightly-1.5.5/lightly/api/api_workflow_collaboration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_compute_worker.py` & `lightly-1.5.5/lightly/api/api_workflow_compute_worker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_datasets.py` & `lightly-1.5.5/lightly/api/api_workflow_datasets.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_datasources.py` & `lightly-1.5.5/lightly/api/api_workflow_datasources.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_download_dataset.py` & `lightly-1.5.5/lightly/api/api_workflow_download_dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_export.py` & `lightly-1.5.5/lightly/api/api_workflow_export.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_predictions.py` & `lightly-1.5.5/lightly/api/api_workflow_predictions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_selection.py` & `lightly-1.5.5/lightly/api/api_workflow_selection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_tags.py` & `lightly-1.5.5/lightly/api/api_workflow_tags.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_upload_embeddings.py` & `lightly-1.5.5/lightly/api/api_workflow_upload_embeddings.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/api_workflow_upload_metadata.py` & `lightly-1.5.5/lightly/api/api_workflow_upload_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/bitmask.py` & `lightly-1.5.5/lightly/api/bitmask.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/download.py` & `lightly-1.5.5/lightly/api/download.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/patch.py` & `lightly-1.5.5/lightly/api/patch.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/serve.py` & `lightly-1.5.5/lightly/api/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from http.server import HTTPServer, SimpleHTTPRequestHandler
+from http.server import SimpleHTTPRequestHandler, ThreadingHTTPServer
 from pathlib import Path
 from typing import Sequence
 from urllib import parse
 
 from lightly.data import _helpers
 
 
@@ -45,15 +45,15 @@
         def send_response_only(self, code, message=None):
             super().send_response_only(code, message)
             self.send_header(
                 "Cache-Control", "no-store, must-revalidate, no-cache, max-age=-1"
             )
             self.send_header("Expires", "0")
 
-    return HTTPServer((host, port), _LocalDatasourceRequestHandler)
+    return ThreadingHTTPServer((host, port), _LocalDatasourceRequestHandler)
 
 
 def validate_input_mount(input_mount: Path) -> None:
     """Validates that the input mount is a directory and contains files."""
     input_mount = input_mount.resolve()
     if not input_mount.exists():
         raise ValueError(
```

### Comparing `lightly-1.5.4/lightly/api/swagger_api_client.py` & `lightly-1.5.5/lightly/api/swagger_api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/swagger_rest_client.py` & `lightly-1.5.5/lightly/api/swagger_rest_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/api/utils.py` & `lightly-1.5.5/lightly/api/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/_cli_simclr.py` & `lightly-1.5.5/lightly/cli/_cli_simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/_helpers.py` & `lightly-1.5.5/lightly/cli/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/config/config.yaml` & `lightly-1.5.5/lightly/cli/config/config.yaml`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/crop_cli.py` & `lightly-1.5.5/lightly/cli/crop_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/download_cli.py` & `lightly-1.5.5/lightly/cli/download_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/embed_cli.py` & `lightly-1.5.5/lightly/cli/embed_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/lightly_cli.py` & `lightly-1.5.5/lightly/cli/lightly_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/serve_cli.py` & `lightly-1.5.5/lightly/cli/serve_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,12 +57,15 @@
     )
     print(
         f"Serving files in '{bcolors.OKBLUE}{cfg.input_mount}{bcolors.ENDC}' and '{bcolors.OKBLUE}{cfg.lightly_mount}{bcolors.ENDC}'"
     )
     print(
         f"Please follow our docs if you are facing any issues: https://docs.lightly.ai/docs/local-storage#optional-after-run-view-local-data-in-lightly-platform"
     )
-    httpd.serve_forever()
+    try:
+        httpd.serve_forever()
+    finally:
+        httpd.server_close()
 
 
 def entry() -> None:
     lightly_serve()
```

### Comparing `lightly-1.5.4/lightly/cli/train_cli.py` & `lightly-1.5.5/lightly/cli/train_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/cli/version_cli.py` & `lightly-1.5.5/lightly/cli/version_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/core.py` & `lightly-1.5.5/lightly/core.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/__init__.py` & `lightly-1.5.5/lightly/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/_helpers.py` & `lightly-1.5.5/lightly/data/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/_image.py` & `lightly-1.5.5/lightly/data/_image.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/_image_loaders.py` & `lightly-1.5.5/lightly/data/_image_loaders.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/_utils.py` & `lightly-1.5.5/lightly/data/_utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/_video.py` & `lightly-1.5.5/lightly/data/_video.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/collate.py` & `lightly-1.5.5/lightly/data/collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/dataset.py` & `lightly-1.5.5/lightly/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/lightly_subset.py` & `lightly-1.5.5/lightly/data/lightly_subset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/data/multi_view_collate.py` & `lightly-1.5.5/lightly/data/multi_view_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/embedding/_base.py` & `lightly-1.5.5/lightly/embedding/_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/embedding/callbacks.py` & `lightly-1.5.5/lightly/embedding/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/embedding/embedding.py` & `lightly-1.5.5/lightly/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/__init__.py` & `lightly-1.5.5/lightly/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/barlow_twins_loss.py` & `lightly-1.5.5/lightly/loss/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/dcl_loss.py` & `lightly-1.5.5/lightly/loss/dcl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/dino_loss.py` & `lightly-1.5.5/lightly/loss/dino_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/emp_ssl_loss.py` & `lightly-1.5.5/lightly/loss/emp_ssl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/hypersphere_loss.py` & `lightly-1.5.5/lightly/loss/hypersphere_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/mmcr_loss.py` & `lightly-1.5.5/lightly/loss/mmcr_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/msn_loss.py` & `lightly-1.5.5/lightly/loss/msn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/negative_cosine_similarity.py` & `lightly-1.5.5/lightly/loss/negative_cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/ntx_ent_loss.py` & `lightly-1.5.5/lightly/loss/ntx_ent_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/pmsn_loss.py` & `lightly-1.5.5/lightly/loss/pmsn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/regularizer/co2.py` & `lightly-1.5.5/lightly/loss/regularizer/co2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/swav_loss.py` & `lightly-1.5.5/lightly/loss/swav_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/sym_neg_cos_sim_loss.py` & `lightly-1.5.5/lightly/loss/sym_neg_cos_sim_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/tico_loss.py` & `lightly-1.5.5/lightly/loss/tico_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/vicreg_loss.py` & `lightly-1.5.5/lightly/loss/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/vicregl_loss.py` & `lightly-1.5.5/lightly/loss/vicregl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/loss/wmse_loss.py` & `lightly-1.5.5/lightly/loss/wmse_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/__init__.py` & `lightly-1.5.5/lightly/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/_momentum.py` & `lightly-1.5.5/lightly/models/_momentum.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/barlowtwins.py` & `lightly-1.5.5/lightly/models/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/batchnorm.py` & `lightly-1.5.5/lightly/models/batchnorm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/byol.py` & `lightly-1.5.5/lightly/models/byol.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/moco.py` & `lightly-1.5.5/lightly/models/moco.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/__init__.py` & `lightly-1.5.5/lightly/models/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/heads.py` & `lightly-1.5.5/lightly/models/modules/heads.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/heads_timm.py` & `lightly-1.5.5/lightly/models/modules/heads_timm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/ijepa.py` & `lightly-1.5.5/lightly/models/modules/ijepa.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/masked_autoencoder.py` & `lightly-1.5.5/lightly/models/modules/masked_autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/masked_autoencoder_timm.py` & `lightly-1.5.5/lightly/models/modules/masked_autoencoder_timm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/masked_causal_vision_transformer.py` & `lightly-1.5.5/lightly/models/modules/masked_causal_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/masked_vision_transformer.py` & `lightly-1.5.5/lightly/models/modules/masked_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/masked_vision_transformer_timm.py` & `lightly-1.5.5/lightly/models/modules/masked_vision_transformer_timm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/masked_vision_transformer_torchvision.py` & `lightly-1.5.5/lightly/models/modules/masked_vision_transformer_torchvision.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/memory_bank.py` & `lightly-1.5.5/lightly/models/modules/memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/modules/nn_memory_bank.py` & `lightly-1.5.5/lightly/models/modules/nn_memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/nnclr.py` & `lightly-1.5.5/lightly/models/nnclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/resnet.py` & `lightly-1.5.5/lightly/models/resnet.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/simclr.py` & `lightly-1.5.5/lightly/models/simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/simsiam.py` & `lightly-1.5.5/lightly/models/simsiam.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/models/utils.py` & `lightly-1.5.5/lightly/models/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -430,14 +430,41 @@
     num_patches = patch_h * patch_w
     patches = images.reshape(shape=(N, C, patch_h, patch_size, patch_w, patch_size))
     patches = torch.einsum("nchpwq->nhwpqc", patches)
     patches = patches.reshape(shape=(N, num_patches, patch_size**2 * C))
     return patches
 
 
+def unpatchify(
+    patches: torch.Tensor, patch_size: int, channels: int = 3
+) -> torch.Tensor:
+    """
+    Reconstructs images from their patches.
+
+     Args:
+         patches:
+             Patches tensor with shape (batch_size, num_patches, channels * patch_size ** 2).
+         patch_size:
+             The patch size in pixels used to create the patches.
+         channels:
+             The number of channels the image must have
+
+     Returns:
+         Reconstructed images tensor with shape (batch_size, channels, height, width).
+    """
+    N, C = patches.shape[0], channels
+    patch_h = patch_w = int(patches.shape[1] ** 0.5)
+    assert patch_h * patch_w == patches.shape[1]
+
+    images = patches.reshape(shape=(N, patch_h, patch_w, patch_size, patch_size, C))
+    images = torch.einsum("nhwpqc->nchpwq", images)
+    images = images.reshape(shape=(N, C, patch_h * patch_size, patch_h * patch_size))
+    return images
+
+
 def random_token_mask(
     size: Tuple[int, int],
     mask_ratio: float = 0.6,
     mask_class_token: bool = False,
     device: Optional[Union[torch.device, str]] = None,
 ) -> torch.Tensor:
     """Creates random token masks.
```

### Comparing `lightly-1.5.4/lightly/models/zoo.py` & `lightly-1.5.5/lightly/models/zoo.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/__init__.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/__init__.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/collaboration_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/collaboration_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/datasets_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/datasources_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/datasources_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/docker_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/docker_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/embeddings_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/jobs_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/mappings_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/mappings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/predictions_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/predictions_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/quota_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/quota_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/samples_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/samples_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/samplings_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/samplings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/scores_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/scores_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/tags_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/teams_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/versioning_api.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api/versioning_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api_client.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/api_response.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/api_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/configuration.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/exceptions.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/__init__.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_types_v2_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/active_learning_score_types_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_v2_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/active_learning_score_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/api_error_code.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/api_error_code.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/api_error_response.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/async_task_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/async_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request_user.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request_user.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/configuration_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_entry.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/configuration_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_set_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/configuration_set_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_cf_bucket_activity_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_cf_bucket_activity_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_entity_response.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_entity_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_team_membership_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/create_team_membership_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/creator.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/crop_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/crop_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_creator.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_update_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dataset_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_azure_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_base.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_base_full_path.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_base_full_path.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_gcs_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_local.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_local.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_local_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_local_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_obs_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_purpose.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_purpose.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/delegated_access_external_ids_inner.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/delegated_access_external_ids_inner.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_authorization_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_authorization_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_authorization_response.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_authorization_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_license_information.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_license_information.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_storage_location.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_storage_location.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_create_entry_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_create_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_docker_load.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_docker_load.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data_base.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_state.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_task_description.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_task_description.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_user_stats.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_user_stats.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_authorization_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_authorization_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request_base.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_datasource.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_datasource.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_datasource_input_expiration.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_datasource_input_expiration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_docker.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data_base.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_state.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/docker_worker_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding2d_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/embedding2d_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/expiry_handling_strategy_v3.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/expiry_handling_strategy_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/file_name_format.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/file_name_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/file_output_format.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/file_output_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/image_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/image_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/internal_debug_latency.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/internal_debug_latency.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/internal_debug_latency_mongodb.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/internal_debug_latency_mongodb.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_result_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_result_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_state.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_status_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_data_result.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_status_data_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_meta.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_status_meta.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/jobs_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/jobs_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_box_data_row.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/label_box_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_studio_task.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/label_studio_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_docker_selection_method.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_docker_selection_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_base.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schemas.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/prediction_task_schemas.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_basic_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/profile_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_me_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/profile_me_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_me_data_settings.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/profile_me_data_settings.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/questionnaire_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/questionnaire_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/s3_region.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/s3_region.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sama_task.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sama_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sama_task_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sama_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_data_modes.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_data_modes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_meta_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_sort_by.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_sort_by.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_update_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_write_urls.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sample_write_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_config.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sampling_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sampling_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_method.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sampling_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sector.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/sector.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_base.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_input.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy_all_of.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_input_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_input_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/service_account_basic_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/service_account_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/shared_access_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_entry.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_change_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_create_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_creator.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_update_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/task_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/task_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_basic_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/team_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/team_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_role.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/team_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/update_team_membership_request.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/update_team_membership_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/user_type.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/user_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/video_frame_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/video_frame_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/openapi_generated/swagger_client/rest.py` & `lightly-1.5.5/lightly/openapi_generated/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/__init__.py` & `lightly-1.5.5/lightly/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/aim_transform.py` & `lightly-1.5.5/lightly/transforms/aim_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/byol_transform.py` & `lightly-1.5.5/lightly/transforms/byol_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/dino_transform.py` & `lightly-1.5.5/lightly/transforms/dino_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/fast_siam_transform.py` & `lightly-1.5.5/lightly/transforms/fast_siam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/gaussian_blur.py` & `lightly-1.5.5/lightly/transforms/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/ijepa_transform.py` & `lightly-1.5.5/lightly/transforms/ijepa_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/image_grid_transform.py` & `lightly-1.5.5/lightly/transforms/image_grid_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/jigsaw.py` & `lightly-1.5.5/lightly/transforms/jigsaw.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/mae_transform.py` & `lightly-1.5.5/lightly/transforms/mae_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/mmcr_transform.py` & `lightly-1.5.5/lightly/transforms/mmcr_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/moco_transform.py` & `lightly-1.5.5/lightly/transforms/moco_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/msn_transform.py` & `lightly-1.5.5/lightly/transforms/msn_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/multi_crop_transform.py` & `lightly-1.5.5/lightly/transforms/multi_crop_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/multi_view_transform.py` & `lightly-1.5.5/lightly/transforms/multi_view_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/pirl_transform.py` & `lightly-1.5.5/lightly/transforms/pirl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/random_crop_and_flip_with_grid.py` & `lightly-1.5.5/lightly/transforms/random_crop_and_flip_with_grid.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/rotation.py` & `lightly-1.5.5/lightly/transforms/rotation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/simclr_transform.py` & `lightly-1.5.5/lightly/transforms/simclr_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/simsiam_transform.py` & `lightly-1.5.5/lightly/transforms/simsiam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/smog_transform.py` & `lightly-1.5.5/lightly/transforms/smog_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/solarize.py` & `lightly-1.5.5/lightly/transforms/solarize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/swav_transform.py` & `lightly-1.5.5/lightly/transforms/swav_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/vicreg_transform.py` & `lightly-1.5.5/lightly/transforms/vicreg_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/vicregl_transform.py` & `lightly-1.5.5/lightly/transforms/vicregl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/transforms/wmse_transform.py` & `lightly-1.5.5/lightly/transforms/wmse_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/benchmarking/benchmark_module.py` & `lightly-1.5.5/lightly/utils/benchmarking/benchmark_module.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/benchmarking/knn.py` & `lightly-1.5.5/lightly/utils/benchmarking/knn.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/benchmarking/knn_classifier.py` & `lightly-1.5.5/lightly/utils/benchmarking/knn_classifier.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/benchmarking/linear_classifier.py` & `lightly-1.5.5/lightly/utils/benchmarking/linear_classifier.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/benchmarking/metric_callback.py` & `lightly-1.5.5/lightly/utils/benchmarking/metric_callback.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/benchmarking/online_linear_classifier.py` & `lightly-1.5.5/lightly/utils/benchmarking/online_linear_classifier.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/benchmarking/topk.py` & `lightly-1.5.5/lightly/utils/benchmarking/topk.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/bounding_box.py` & `lightly-1.5.5/lightly/utils/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/cropping/crop_image_by_bounding_boxes.py` & `lightly-1.5.5/lightly/utils/cropping/crop_image_by_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/cropping/read_yolo_label_file.py` & `lightly-1.5.5/lightly/utils/cropping/read_yolo_label_file.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/debug.py` & `lightly-1.5.5/lightly/utils/debug.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/dependency.py` & `lightly-1.5.5/lightly/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/dist.py` & `lightly-1.5.5/lightly/utils/dist.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/embeddings_2d.py` & `lightly-1.5.5/lightly/utils/embeddings_2d.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/hipify.py` & `lightly-1.5.5/lightly/utils/hipify.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/io.py` & `lightly-1.5.5/lightly/utils/io.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/lars.py` & `lightly-1.5.5/lightly/utils/lars.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/reordering.py` & `lightly-1.5.5/lightly/utils/reordering.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/scheduler.py` & `lightly-1.5.5/lightly/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly/utils/version_compare.py` & `lightly-1.5.5/lightly/utils/version_compare.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly.egg-info/PKG-INFO` & `lightly-1.5.5/lightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.5.4
+Version: 1.5.5
 Summary: A deep learning package for self-supervised learning
 Author: Lightly Team
 Author-email: team@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.5.4/lightly.egg-info/SOURCES.txt` & `lightly-1.5.5/lightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/lightly.egg-info/requires.txt` & `lightly-1.5.5/lightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.5.4/setup.py` & `lightly-1.5.5/setup.py`

 * *Files identical despite different names*

