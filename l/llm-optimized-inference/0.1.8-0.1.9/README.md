# Comparing `tmp/llm_optimized_inference-0.1.8-py3-none-any.whl.zip` & `tmp/llm_optimized_inference-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,38 @@
-Zip file size: 67541 bytes, number of entries: 36
--rw-rw-r--  2.0 unx      249 b- defN 24-May-15 20:55 llm/__init__.py
--rw-rw-r--  2.0 unx      249 b- defN 24-May-15 20:55 llm/optimized/__init__.py
--rw-rw-r--  2.0 unx      703 b- defN 24-May-15 20:55 llm/optimized/inference/__init__.py
--rw-rw-r--  2.0 unx      204 b- defN 24-May-15 20:55 llm/optimized/inference/_version.py
--rw-rw-r--  2.0 unx    28831 b- defN 24-May-15 20:55 llm/optimized/inference/api_server.py
--rw-rw-r--  2.0 unx     3203 b- defN 24-May-15 20:55 llm/optimized/inference/configs.py
--rw-rw-r--  2.0 unx     7172 b- defN 24-May-15 20:55 llm/optimized/inference/constants.py
--rw-rw-r--  2.0 unx     3255 b- defN 24-May-15 20:55 llm/optimized/inference/conversation.py
--rw-rw-r--  2.0 unx     5802 b- defN 24-May-15 20:55 llm/optimized/inference/fm_score.py
--rw-rw-r--  2.0 unx      664 b- defN 24-May-15 20:55 llm/optimized/inference/logging_config.py
--rw-rw-r--  2.0 unx     9420 b- defN 24-May-15 20:55 llm/optimized/inference/managed_inference.py
--rw-rw-r--  2.0 unx     1369 b- defN 24-May-15 20:55 llm/optimized/inference/model_config_factory.py
--rw-rw-r--  2.0 unx     6814 b- defN 24-May-15 20:55 llm/optimized/inference/model_utils.py
--rw-rw-r--  2.0 unx     1575 b- defN 24-May-15 20:55 llm/optimized/inference/prompt_formatter.py
--rw-rw-r--  2.0 unx    12420 b- defN 24-May-15 20:55 llm/optimized/inference/replica_manager.py
--rw-rw-r--  2.0 unx    18786 b- defN 24-May-15 20:55 llm/optimized/inference/score.py
--rw-rw-r--  2.0 unx     4731 b- defN 24-May-15 20:55 llm/optimized/inference/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-May-15 20:55 llm/optimized/inference/api_server_setup/__init__.py
--rw-rw-r--  2.0 unx     9502 b- defN 24-May-15 20:55 llm/optimized/inference/api_server_setup/openapi.json
--rw-rw-r--  2.0 unx     1878 b- defN 24-May-15 20:55 llm/optimized/inference/api_server_setup/protocol.py
--rw-rw-r--  2.0 unx      131 b- defN 24-May-15 20:55 llm/optimized/inference/custom_model_configurations/__init__.py
--rw-rw-r--  2.0 unx     2725 b- defN 24-May-15 20:55 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
--rw-rw-r--  2.0 unx     8806 b- defN 24-May-15 20:55 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
--rw-rw-r--  2.0 unx     1047 b- defN 24-May-15 20:55 llm/optimized/inference/custom_model_configurations/schema_output.py
--rw-rw-r--  2.0 unx      259 b- defN 24-May-15 20:55 llm/optimized/inference/engine/__init__.py
--rw-rw-r--  2.0 unx    38577 b- defN 24-May-15 20:55 llm/optimized/inference/engine/_hf_predictors.py
--rw-rw-r--  2.0 unx     4673 b- defN 24-May-15 20:55 llm/optimized/inference/engine/engine.py
--rw-rw-r--  2.0 unx     8617 b- defN 24-May-15 20:55 llm/optimized/inference/engine/hf_engine.py
--rw-rw-r--  2.0 unx    10797 b- defN 24-May-15 20:55 llm/optimized/inference/engine/mii_engine.py
--rw-rw-r--  2.0 unx     7971 b- defN 24-May-15 20:55 llm/optimized/inference/engine/mii_engine_v2.py
--rw-rw-r--  2.0 unx    16449 b- defN 24-May-15 20:55 llm/optimized/inference/engine/vllm_engine.py
--rw-rw-r--  2.0 unx        0 b- defN 24-May-15 20:58 llm_optimized_inference-0.1.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3107 b- defN 24-May-15 20:58 llm_optimized_inference-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-15 20:58 llm_optimized_inference-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 24-May-15 20:58 llm_optimized_inference-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3599 b- defN 24-May-15 20:58 llm_optimized_inference-0.1.8.dist-info/RECORD
-36 files, 223681 bytes uncompressed, 61557 bytes compressed:  72.5%
+Zip file size: 67547 bytes, number of entries: 36
+-rw-rw-r--  2.0 unx      249 b- defN 24-May-29 17:29 llm/__init__.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-May-29 17:29 llm/optimized/__init__.py
+-rw-rw-r--  2.0 unx      703 b- defN 24-May-29 17:29 llm/optimized/inference/__init__.py
+-rw-rw-r--  2.0 unx      204 b- defN 24-May-29 17:29 llm/optimized/inference/_version.py
+-rw-rw-r--  2.0 unx    28831 b- defN 24-May-29 17:29 llm/optimized/inference/api_server.py
+-rw-rw-r--  2.0 unx     3203 b- defN 24-May-29 17:29 llm/optimized/inference/configs.py
+-rw-rw-r--  2.0 unx     7172 b- defN 24-May-29 17:29 llm/optimized/inference/constants.py
+-rw-rw-r--  2.0 unx     3255 b- defN 24-May-29 17:29 llm/optimized/inference/conversation.py
+-rw-rw-r--  2.0 unx     5802 b- defN 24-May-29 17:29 llm/optimized/inference/fm_score.py
+-rw-rw-r--  2.0 unx      664 b- defN 24-May-29 17:29 llm/optimized/inference/logging_config.py
+-rw-rw-r--  2.0 unx     9420 b- defN 24-May-29 17:29 llm/optimized/inference/managed_inference.py
+-rw-rw-r--  2.0 unx     1369 b- defN 24-May-29 17:29 llm/optimized/inference/model_config_factory.py
+-rw-rw-r--  2.0 unx     6814 b- defN 24-May-29 17:29 llm/optimized/inference/model_utils.py
+-rw-rw-r--  2.0 unx     1575 b- defN 24-May-29 17:29 llm/optimized/inference/prompt_formatter.py
+-rw-rw-r--  2.0 unx    12420 b- defN 24-May-29 17:29 llm/optimized/inference/replica_manager.py
+-rw-rw-r--  2.0 unx    18786 b- defN 24-May-29 17:29 llm/optimized/inference/score.py
+-rw-rw-r--  2.0 unx     4731 b- defN 24-May-29 17:29 llm/optimized/inference/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-29 17:29 llm/optimized/inference/api_server_setup/__init__.py
+-rw-rw-r--  2.0 unx     9502 b- defN 24-May-29 17:29 llm/optimized/inference/api_server_setup/openapi.json
+-rw-rw-r--  2.0 unx     1878 b- defN 24-May-29 17:29 llm/optimized/inference/api_server_setup/protocol.py
+-rw-rw-r--  2.0 unx      131 b- defN 24-May-29 17:29 llm/optimized/inference/custom_model_configurations/__init__.py
+-rw-rw-r--  2.0 unx     2725 b- defN 24-May-29 17:29 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
+-rw-rw-r--  2.0 unx     8806 b- defN 24-May-29 17:29 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-May-29 17:29 llm/optimized/inference/custom_model_configurations/schema_output.py
+-rw-rw-r--  2.0 unx      259 b- defN 24-May-29 17:29 llm/optimized/inference/engine/__init__.py
+-rw-rw-r--  2.0 unx    38577 b- defN 24-May-29 17:29 llm/optimized/inference/engine/_hf_predictors.py
+-rw-rw-r--  2.0 unx     4673 b- defN 24-May-29 17:29 llm/optimized/inference/engine/engine.py
+-rw-rw-r--  2.0 unx     8617 b- defN 24-May-29 17:29 llm/optimized/inference/engine/hf_engine.py
+-rw-rw-r--  2.0 unx    10797 b- defN 24-May-29 17:29 llm/optimized/inference/engine/mii_engine.py
+-rw-rw-r--  2.0 unx     7971 b- defN 24-May-29 17:29 llm/optimized/inference/engine/mii_engine_v2.py
+-rw-rw-r--  2.0 unx    16449 b- defN 24-May-29 17:29 llm/optimized/inference/engine/vllm_engine.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-29 17:32 llm_optimized_inference-0.1.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3137 b- defN 24-May-29 17:32 llm_optimized_inference-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-29 17:32 llm_optimized_inference-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 24-May-29 17:32 llm_optimized_inference-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3599 b- defN 24-May-29 17:32 llm_optimized_inference-0.1.9.dist-info/RECORD
+36 files, 223711 bytes uncompressed, 61563 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -87,23 +87,23 @@
 
 Filename: llm/optimized/inference/engine/mii_engine_v2.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/vllm_engine.py
 Comment: 
 
-Filename: llm_optimized_inference-0.1.8.dist-info/LICENSE
+Filename: llm_optimized_inference-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: llm_optimized_inference-0.1.8.dist-info/METADATA
+Filename: llm_optimized_inference-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: llm_optimized_inference-0.1.8.dist-info/WHEEL
+Filename: llm_optimized_inference-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: llm_optimized_inference-0.1.8.dist-info/top_level.txt
+Filename: llm_optimized_inference-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_optimized_inference-0.1.8.dist-info/RECORD
+Filename: llm_optimized_inference-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llm/optimized/inference/_version.py

```diff
@@ -1,5 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
```

## Comparing `llm_optimized_inference-0.1.8.dist-info/METADATA` & `llm_optimized_inference-0.1.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-optimized-inference
-Version: 0.1.8
+Version: 0.1.9
 Home-page: 
 Author: Microsoft
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -27,14 +27,15 @@
 Requires-Dist: azureml-inference-server-http
 Requires-Dist: azureml-mlflow
 Requires-Dist: requests ~=2.31.0
 Requires-Dist: aiohttp ~=3.9.1
 Requires-Dist: torch ~=2.3.0
 Requires-Dist: scipy
 Requires-Dist: accelerate >=0.20.3
+Requires-Dist: Jinja2 >=3.1.4
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 
 # Foundation Model Inferencing
 
 
 ### Setting up Pre-commit for this Repository
```

## Comparing `llm_optimized_inference-0.1.8.dist-info/RECORD` & `llm_optimized_inference-0.1.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 llm/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/inference/__init__.py,sha256=rGZODP-qE2NOlUgdbmxhfuS3svmx9gM-kU97d9-jb50,703
-llm/optimized/inference/_version.py,sha256=G_1k2TLqowK_zt3JaZz-RckEg4KB-WZ7qW2KjBZdnYg,204
+llm/optimized/inference/_version.py,sha256=N7SHKKTjgQIjG18Oe14wOa5X1DU9-SzR7n1bpqkTY_k,204
 llm/optimized/inference/api_server.py,sha256=lmBc6LVx06CenPskU28atubBg7zO2Ca2hKATL1Umr7w,28831
 llm/optimized/inference/configs.py,sha256=d5NKbQlfYVkUQ4SL03KVBQekdOG4VrcD0xGxVeHESeQ,3203
 llm/optimized/inference/constants.py,sha256=rjbacKgwUqTWeDb1YVRXjfhjB9L0smWvMwwirz9BbRE,7172
 llm/optimized/inference/conversation.py,sha256=cBrHv1sI1hrOQB57sSZKAarplKRgqQWqmYxT-wkZHLM,3255
 llm/optimized/inference/fm_score.py,sha256=7z7ZbLMXUXH6gp1-G_l3rOus9r9vSpIm5-wOj5X17aQ,5802
 llm/optimized/inference/logging_config.py,sha256=egtAiGCNVNoU8E_JPhp2aGJVIJ_QkTwLhkNjpVKjICI,664
 llm/optimized/inference/managed_inference.py,sha256=TXQmdPHla_U2exzXv_17AFMvUORQVT7a54CZroSURqo,9420
@@ -25,12 +25,12 @@
 llm/optimized/inference/engine/__init__.py,sha256=8GqGW53dbRlGShwO11h5HQH4KjnUzoW0t0cChUUFDPY,259
 llm/optimized/inference/engine/_hf_predictors.py,sha256=AwQTIpmOHb7h31H2DF2Jx-9b03lcB5DOrgSbXGpamIk,38577
 llm/optimized/inference/engine/engine.py,sha256=WohAsPpFbD6LMAiE_2Sn8gp6ybVmF22qLKjc6roO25s,4673
 llm/optimized/inference/engine/hf_engine.py,sha256=4rRldNod-pMDJ_-3q0RDWEkigCTr6I62HyJspb01lAs,8617
 llm/optimized/inference/engine/mii_engine.py,sha256=TBfc_wt4-NKTzkjHCie5YpqRGS6pvBNigyYpTHt_jII,10797
 llm/optimized/inference/engine/mii_engine_v2.py,sha256=rI4tjRyj-dCZBDAiN0YNPKMBtkD3MXxcbucuSlHg6lI,7971
 llm/optimized/inference/engine/vllm_engine.py,sha256=h43ePEzUvf2psVzgzN7wZ9dpXJZPeXUW7N6NjXLzQiQ,16449
-llm_optimized_inference-0.1.8.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-llm_optimized_inference-0.1.8.dist-info/METADATA,sha256=wNFyDrY_xDUwN3DjKtuKKi7hWIDuSVooon6Rv8iMjiw,3107
-llm_optimized_inference-0.1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-llm_optimized_inference-0.1.8.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
-llm_optimized_inference-0.1.8.dist-info/RECORD,,
+llm_optimized_inference-0.1.9.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+llm_optimized_inference-0.1.9.dist-info/METADATA,sha256=SJH5vDIPTlWUGnsTskT_nWzVYSje34VfR5fgHB0I_n8,3137
+llm_optimized_inference-0.1.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+llm_optimized_inference-0.1.9.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
+llm_optimized_inference-0.1.9.dist-info/RECORD,,
```

