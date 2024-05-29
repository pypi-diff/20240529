# Comparing `tmp/castle_ai-0.0.6.tar.gz` & `tmp/castle_ai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castle_ai-0.0.6.tar", last modified: Tue May 28 04:55:34 2024, max compression
+gzip compressed data, was "castle_ai-0.0.8.tar", last modified: Wed May 29 09:32:41 2024, max compression
```

## Comparing `castle_ai-0.0.6.tar` & `castle_ai-0.0.8.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/
--rw-r--r--   0 raiso     (1000) raiso     (1000)     1904 2024-05-28 04:55:34.897531 castle_ai-0.0.6/PKG-INFO
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      993 2024-05-28 04:11:27.000000 castle_ai-0.0.6/README.md
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.893531 castle_ai-0.0.6/castle/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       20 2024-05-22 04:34:06.000000 castle_ai-0.0.6/castle/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.893531 castle_ai-0.0.6/castle/aot/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       31 2024-05-22 04:48:14.000000 castle_ai-0.0.6/castle/aot/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.893531 castle_ai-0.0.6/castle/aot/configs/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:30:16.000000 castle_ai-0.0.6/castle/aot/configs/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5566 2024-05-22 06:28:08.000000 castle_ai-0.0.6/castle/aot/configs/default.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/configs/models/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:32:03.000000 castle_ai-0.0.6/castle/aot/configs/models/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/aotb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/aots.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      174 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/aott.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/deaotb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/deaots.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      173 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/deaott.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      957 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/default.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      420 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/default_deaot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      545 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/r101_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/r50_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      410 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/r50_deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      585 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/rs101_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      645 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/swinb_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      451 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/models/swinb_deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      513 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/pre.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      690 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/pre_dav.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      611 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/pre_ytb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      668 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/pre_ytb_dav.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      251 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/configs/ytb.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/dataloaders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/dataloaders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    14300 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/dataloaders/eval_datasets.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    19828 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/dataloaders/image_transforms.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    24642 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/dataloaders/train_datasets.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    23561 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/dataloaders/video_transforms.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/networks/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:49:47.000000 castle_ai-0.0.6/castle/aot/networks/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/networks/decoders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      186 2024-05-22 05:12:26.000000 castle_ai-0.0.6/castle/aot/networks/decoders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2079 2024-05-22 05:13:06.000000 castle_ai-0.0.6/castle/aot/networks/decoders/fpn.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/networks/encoders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1307 2024-05-22 05:08:31.000000 castle_ai-0.0.6/castle/aot/networks/encoders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8427 2024-05-22 05:06:53.000000 castle_ai-0.0.6/castle/aot/networks/encoders/mobilenetv2.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     7907 2024-05-22 05:07:00.000000 castle_ai-0.0.6/castle/aot/networks/encoders/mobilenetv3.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/networks/encoders/resnest/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       23 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/encoders/resnest/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3343 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/encoders/resnest/resnest.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    16481 2024-05-22 05:10:30.000000 castle_ai-0.0.6/castle/aot/networks/encoders/resnest/resnet.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4467 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/encoders/resnest/splat.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6699 2024-05-22 05:07:30.000000 castle_ai-0.0.6/castle/aot/networks/encoders/resnet.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/networks/encoders/swin/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       35 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/encoders/swin/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      987 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/encoders/swin/build.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    27369 2024-05-22 05:10:57.000000 castle_ai-0.0.6/castle/aot/networks/encoders/swin/swin_transformer.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/networks/engines/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      653 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/engines/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    25206 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/engines/aot_engine.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5978 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/engines/deaot_engine.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/networks/layers/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/layers/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    32865 2024-05-22 05:11:50.000000 castle_ai-0.0.6/castle/aot/networks/layers/attention.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5111 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/layers/basic.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6698 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/layers/loss.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1700 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/networks/layers/normalization.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2834 2024-05-22 05:12:08.000000 castle_ai-0.0.6/castle/aot/networks/layers/position.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    24810 2024-05-22 05:11:35.000000 castle_ai-0.0.6/castle/aot/networks/layers/transformer.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/networks/models/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      358 2024-05-22 04:45:04.000000 castle_ai-0.0.6/castle/aot/networks/models/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4574 2024-05-22 05:03:48.000000 castle_ai-0.0.6/castle/aot/networks/models/aot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2109 2024-05-22 05:13:44.000000 castle_ai-0.0.6/castle/aot/networks/models/deaot.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/aot/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6233 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/checkpoint.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1358 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/cp_ckpt.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3561 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/ema.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      443 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/eval.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6075 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/image.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3454 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/learning.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      829 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/math.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      860 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/meters.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1102 2024-05-22 03:59:14.000000 castle_ai-0.0.6/castle/aot/utils/metric.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/sam/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/sam/segment_anything/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      427 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    15132 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2941 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/build_sam.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/sam/segment_anything/modeling/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      385 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/modeling/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1479 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/modeling/common.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    14407 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6614 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8594 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     7225 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/modeling/sam.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8396 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/modeling/transformer.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    11818 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/predictor.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/sam/segment_anything/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      197 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    12711 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/utils/amg.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5790 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/utils/onnx.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3968 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/segment_anything/utils/transforms.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 04:03:33.000000 castle_ai-0.0.6/castle/sam/setup.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/ui/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       30 2024-05-27 09:19:59.000000 castle_ai-0.0.6/castle/ui/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4051 2024-05-27 09:19:59.000000 castle_ai-0.0.6/castle/ui/cluster_input_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      793 2024-05-27 09:19:59.000000 castle_ai-0.0.6/castle/ui/cluster_page_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1402 2024-05-27 09:19:59.000000 castle_ai-0.0.6/castle/ui/dbscan_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4597 2024-05-27 09:19:59.000000 castle_ai-0.0.6/castle/ui/dimension_reduction_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3908 2024-05-28 02:46:14.000000 castle_ai-0.0.6/castle/ui/edit_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5686 2024-05-28 03:44:33.000000 castle_ai-0.0.6/castle/ui/extract_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4602 2024-05-28 04:03:20.000000 castle_ai-0.0.6/castle/ui/label_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2533 2024-05-28 04:44:40.000000 castle_ai-0.0.6/castle/ui/main_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2854 2024-05-28 02:07:22.000000 castle_ai-0.0.6/castle/ui/plot_mask_info.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     7897 2024-05-28 03:17:56.000000 castle_ai-0.0.6/castle/ui/post_track_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4589 2024-05-28 04:49:21.000000 castle_ai-0.0.6/castle/ui/project_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4048 2024-05-27 09:20:00.000000 castle_ai-0.0.6/castle/ui/source_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    10318 2024-05-28 03:47:34.000000 castle_ai-0.0.6/castle/ui/track_ui.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2126 2024-05-28 02:22:48.000000 castle_ai-0.0.6/castle/ui/view_ui.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      137 2024-05-24 08:01:14.000000 castle_ai-0.0.6/castle/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1002 2024-05-23 07:41:10.000000 castle_ai-0.0.6/castle/utils/download.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1357 2024-05-28 02:57:21.000000 castle_ai-0.0.6/castle/utils/h5_io.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6539 2024-05-28 02:15:58.000000 castle_ai-0.0.6/castle/utils/image_segment.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5637 2024-05-27 10:57:31.000000 castle_ai-0.0.6/castle/utils/latent_explorer.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1507 2024-05-28 02:25:32.000000 castle_ai-0.0.6/castle/utils/plot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3754 2024-05-28 03:44:17.000000 castle_ai-0.0.6/castle/utils/video_align.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2589 2024-05-28 02:20:08.000000 castle_ai-0.0.6/castle/utils/video_io.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8716 2024-05-28 02:16:40.000000 castle_ai-0.0.6/castle/utils/video_object_segment.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3677 2024-05-28 02:16:00.000000 castle_ai-0.0.6/castle/utils/visual_latent_extract.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-28 04:55:34.897531 castle_ai-0.0.6/castle_ai.egg-info/
--rw-r--r--   0 raiso     (1000) raiso     (1000)     1904 2024-05-28 04:55:34.000000 castle_ai-0.0.6/castle_ai.egg-info/PKG-INFO
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4101 2024-05-28 04:55:34.000000 castle_ai-0.0.6/castle_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-28 04:55:34.000000 castle_ai-0.0.6/castle_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-23 00:05:44.000000 castle_ai-0.0.6/castle_ai.egg-info/not-zip-safe
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       95 2024-05-28 04:55:34.000000 castle_ai-0.0.6/castle_ai.egg-info/requires.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        7 2024-05-28 04:55:34.000000 castle_ai-0.0.6/castle_ai.egg-info/top_level.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       38 2024-05-28 04:55:34.897531 castle_ai-0.0.6/setup.cfg
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2038 2024-05-28 04:55:22.000000 castle_ai-0.0.6/setup.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/
+-rw-r--r--   0 raiso     (1000) raiso     (1000)     1920 2024-05-29 09:32:41.496099 castle_ai-0.0.8/PKG-INFO
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      986 2024-05-28 09:04:38.000000 castle_ai-0.0.8/README.md
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.492099 castle_ai-0.0.8/castle/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       20 2024-05-22 04:34:06.000000 castle_ai-0.0.8/castle/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.492099 castle_ai-0.0.8/castle/aot/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       31 2024-05-22 04:48:14.000000 castle_ai-0.0.8/castle/aot/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.492099 castle_ai-0.0.8/castle/aot/configs/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:30:16.000000 castle_ai-0.0.8/castle/aot/configs/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5566 2024-05-22 06:28:08.000000 castle_ai-0.0.8/castle/aot/configs/default.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/configs/models/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:32:03.000000 castle_ai-0.0.8/castle/aot/configs/models/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/aotb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/aots.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      174 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/aott.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/deaotb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/deaots.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      173 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/deaott.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      957 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/default.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      420 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/default_deaot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      545 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/r101_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/r50_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      410 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/r50_deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      585 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/rs101_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      645 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/swinb_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      451 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/models/swinb_deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      513 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/pre.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      690 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/pre_dav.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      611 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/pre_ytb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      668 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/pre_ytb_dav.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      251 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/configs/ytb.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/dataloaders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/dataloaders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    14300 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/dataloaders/eval_datasets.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    19828 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/dataloaders/image_transforms.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    24642 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/dataloaders/train_datasets.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    23561 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/dataloaders/video_transforms.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/networks/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:49:47.000000 castle_ai-0.0.8/castle/aot/networks/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/networks/decoders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      186 2024-05-22 05:12:26.000000 castle_ai-0.0.8/castle/aot/networks/decoders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2079 2024-05-22 05:13:06.000000 castle_ai-0.0.8/castle/aot/networks/decoders/fpn.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/networks/encoders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1307 2024-05-22 05:08:31.000000 castle_ai-0.0.8/castle/aot/networks/encoders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8427 2024-05-22 05:06:53.000000 castle_ai-0.0.8/castle/aot/networks/encoders/mobilenetv2.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7907 2024-05-22 05:07:00.000000 castle_ai-0.0.8/castle/aot/networks/encoders/mobilenetv3.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/networks/encoders/resnest/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       23 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/encoders/resnest/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3343 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/encoders/resnest/resnest.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    16481 2024-05-22 05:10:30.000000 castle_ai-0.0.8/castle/aot/networks/encoders/resnest/resnet.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4467 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/encoders/resnest/splat.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6699 2024-05-22 05:07:30.000000 castle_ai-0.0.8/castle/aot/networks/encoders/resnet.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/networks/encoders/swin/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       35 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/encoders/swin/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      987 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/encoders/swin/build.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    27369 2024-05-22 05:10:57.000000 castle_ai-0.0.8/castle/aot/networks/encoders/swin/swin_transformer.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/networks/engines/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      653 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/engines/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    25206 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/engines/aot_engine.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5978 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/engines/deaot_engine.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/networks/layers/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/layers/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    32865 2024-05-22 05:11:50.000000 castle_ai-0.0.8/castle/aot/networks/layers/attention.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5111 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/layers/basic.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6698 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/layers/loss.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1700 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/networks/layers/normalization.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2834 2024-05-22 05:12:08.000000 castle_ai-0.0.8/castle/aot/networks/layers/position.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    24810 2024-05-22 05:11:35.000000 castle_ai-0.0.8/castle/aot/networks/layers/transformer.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/networks/models/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      358 2024-05-22 04:45:04.000000 castle_ai-0.0.8/castle/aot/networks/models/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4574 2024-05-22 05:03:48.000000 castle_ai-0.0.8/castle/aot/networks/models/aot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2109 2024-05-22 05:13:44.000000 castle_ai-0.0.8/castle/aot/networks/models/deaot.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/aot/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6233 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/checkpoint.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1358 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/cp_ckpt.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3561 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/ema.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      443 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/eval.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6075 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/image.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3454 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/learning.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      829 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/math.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      860 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/meters.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1102 2024-05-22 03:59:14.000000 castle_ai-0.0.8/castle/aot/utils/metric.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/sam/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/sam/segment_anything/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      427 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    15132 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2941 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/build_sam.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/sam/segment_anything/modeling/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      385 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1479 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/modeling/common.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    14407 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6614 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8594 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7225 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/modeling/sam.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8396 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    11818 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/predictor.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/sam/segment_anything/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      197 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    12711 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/utils/amg.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5790 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/utils/onnx.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3968 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/segment_anything/utils/transforms.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 04:03:33.000000 castle_ai-0.0.8/castle/sam/setup.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/ui/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       30 2024-05-27 09:19:59.000000 castle_ai-0.0.8/castle/ui/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4051 2024-05-27 09:19:59.000000 castle_ai-0.0.8/castle/ui/cluster_input_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    11005 2024-05-29 08:47:55.000000 castle_ai-0.0.8/castle/ui/cluster_page_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1402 2024-05-27 09:19:59.000000 castle_ai-0.0.8/castle/ui/dbscan_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4597 2024-05-27 09:19:59.000000 castle_ai-0.0.8/castle/ui/dimension_reduction_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3908 2024-05-29 06:39:46.000000 castle_ai-0.0.8/castle/ui/edit_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    10246 2024-05-29 09:21:48.000000 castle_ai-0.0.8/castle/ui/extract_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4602 2024-05-28 04:03:20.000000 castle_ai-0.0.8/castle/ui/label_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2521 2024-05-28 09:10:18.000000 castle_ai-0.0.8/castle/ui/main_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2854 2024-05-28 02:07:22.000000 castle_ai-0.0.8/castle/ui/plot_mask_info.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7897 2024-05-28 03:17:56.000000 castle_ai-0.0.8/castle/ui/post_track_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4691 2024-05-29 01:39:24.000000 castle_ai-0.0.8/castle/ui/project_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4048 2024-05-27 09:20:00.000000 castle_ai-0.0.8/castle/ui/source_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    10307 2024-05-28 13:02:37.000000 castle_ai-0.0.8/castle/ui/track_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2126 2024-05-28 02:22:48.000000 castle_ai-0.0.8/castle/ui/view_ui.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      137 2024-05-24 08:01:14.000000 castle_ai-0.0.8/castle/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1002 2024-05-23 07:41:10.000000 castle_ai-0.0.8/castle/utils/download.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1357 2024-05-28 02:57:21.000000 castle_ai-0.0.8/castle/utils/h5_io.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6539 2024-05-29 05:50:36.000000 castle_ai-0.0.8/castle/utils/image_segment.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7961 2024-05-29 06:34:38.000000 castle_ai-0.0.8/castle/utils/latent_explorer.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1507 2024-05-28 02:25:32.000000 castle_ai-0.0.8/castle/utils/plot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3754 2024-05-28 03:44:17.000000 castle_ai-0.0.8/castle/utils/video_align.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2589 2024-05-28 02:20:08.000000 castle_ai-0.0.8/castle/utils/video_io.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8716 2024-05-28 02:16:40.000000 castle_ai-0.0.8/castle/utils/video_object_segment.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3677 2024-05-28 02:16:00.000000 castle_ai-0.0.8/castle/utils/visual_latent_extract.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-29 09:32:41.496099 castle_ai-0.0.8/castle_ai.egg-info/
+-rw-r--r--   0 raiso     (1000) raiso     (1000)     1920 2024-05-29 09:32:41.000000 castle_ai-0.0.8/castle_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4101 2024-05-29 09:32:41.000000 castle_ai-0.0.8/castle_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-29 09:32:41.000000 castle_ai-0.0.8/castle_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-23 00:05:44.000000 castle_ai-0.0.8/castle_ai.egg-info/not-zip-safe
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      103 2024-05-29 09:32:41.000000 castle_ai-0.0.8/castle_ai.egg-info/requires.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        7 2024-05-29 09:32:41.000000 castle_ai-0.0.8/castle_ai.egg-info/top_level.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       38 2024-05-29 09:32:41.496099 castle_ai-0.0.8/setup.cfg
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2057 2024-05-29 09:32:26.000000 castle_ai-0.0.8/setup.py
```

### Comparing `castle_ai-0.0.6/PKG-INFO` & `castle_ai-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castle-ai
-Version: 0.0.6
+Version: 0.0.8
 Summary: Distinguish behavioral clusters Toolbox
 Maintainer: Raiso Liu
 Maintainer-email: rainsoon717@gmail.com
 License: AGPL-3.0 license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,15 @@
 Requires-Dist: torchvision
 Requires-Dist: matplotlib
 Requires-Dist: umap-learn
 Requires-Dist: h5py
 Requires-Dist: natsort
 Requires-Dist: gradio
 Requires-Dist: plotly
+Requires-Dist: hdbscan
 
 # CASTLE
 
 
 [![PyPI version](https://badge.fury.io/py/castle-ai.svg)](https://badge.fury.io/py/castle-ai)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CASTLE-ai/castle-ai/blob/main/notebooks/colab.ipynb)
 
@@ -41,15 +42,15 @@
 ```
 pip install castle-ai
 ```
 
 # Open
 
 ```
-python web_ui/app.py
+python app.py
 ```
 
 # Reference
 
 [Segment Anything](https://github.com/facebookresearch/segment-anything.git)
 
 [DeAOT](https://github.com/z-x-yang/Segment-and-Track-Anything.git)
```

### Comparing `castle_ai-0.0.6/README.md` & `castle_ai-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 pip install castle-ai
 ```
 
 # Open
 
 ```
-python web_ui/app.py
+python app.py
 ```
 
 # Reference
 
 [Segment Anything](https://github.com/facebookresearch/segment-anything.git)
 
 [DeAOT](https://github.com/z-x-yang/Segment-and-Track-Anything.git)
```

### Comparing `castle_ai-0.0.6/castle/aot/configs/default.py` & `castle_ai-0.0.8/castle/aot/configs/default.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/models/default.py` & `castle_ai-0.0.8/castle/aot/configs/models/default.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/models/r101_aotl.py` & `castle_ai-0.0.8/castle/aot/configs/models/r101_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/models/r50_aotl.py` & `castle_ai-0.0.8/castle/aot/configs/models/r50_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/models/rs101_aotl.py` & `castle_ai-0.0.8/castle/aot/configs/models/rs101_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/models/swinb_aotl.py` & `castle_ai-0.0.8/castle/aot/configs/models/swinb_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/pre.py` & `castle_ai-0.0.8/castle/aot/configs/pre.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/pre_dav.py` & `castle_ai-0.0.8/castle/aot/configs/pre_dav.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/pre_ytb.py` & `castle_ai-0.0.8/castle/aot/configs/pre_ytb.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/configs/pre_ytb_dav.py` & `castle_ai-0.0.8/castle/aot/configs/pre_ytb_dav.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/dataloaders/eval_datasets.py` & `castle_ai-0.0.8/castle/aot/dataloaders/eval_datasets.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/dataloaders/image_transforms.py` & `castle_ai-0.0.8/castle/aot/dataloaders/image_transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/dataloaders/train_datasets.py` & `castle_ai-0.0.8/castle/aot/dataloaders/train_datasets.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/dataloaders/video_transforms.py` & `castle_ai-0.0.8/castle/aot/dataloaders/video_transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/decoders/fpn.py` & `castle_ai-0.0.8/castle/aot/networks/decoders/fpn.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/__init__.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/mobilenetv2.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/mobilenetv3.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/resnest/resnest.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/resnest/resnest.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/resnest/resnet.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/resnest/resnet.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/resnest/splat.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/resnest/splat.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/resnet.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/swin/build.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/swin/build.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/encoders/swin/swin_transformer.py` & `castle_ai-0.0.8/castle/aot/networks/encoders/swin/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/engines/__init__.py` & `castle_ai-0.0.8/castle/aot/networks/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/engines/aot_engine.py` & `castle_ai-0.0.8/castle/aot/networks/engines/aot_engine.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/engines/deaot_engine.py` & `castle_ai-0.0.8/castle/aot/networks/engines/deaot_engine.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/layers/attention.py` & `castle_ai-0.0.8/castle/aot/networks/layers/attention.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/layers/basic.py` & `castle_ai-0.0.8/castle/aot/networks/layers/basic.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/layers/loss.py` & `castle_ai-0.0.8/castle/aot/networks/layers/loss.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/layers/normalization.py` & `castle_ai-0.0.8/castle/aot/networks/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/layers/position.py` & `castle_ai-0.0.8/castle/aot/networks/layers/position.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/layers/transformer.py` & `castle_ai-0.0.8/castle/aot/networks/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/models/aot.py` & `castle_ai-0.0.8/castle/aot/networks/models/aot.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/networks/models/deaot.py` & `castle_ai-0.0.8/castle/aot/networks/models/deaot.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/utils/checkpoint.py` & `castle_ai-0.0.8/castle/aot/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/utils/cp_ckpt.py` & `castle_ai-0.0.8/castle/aot/utils/cp_ckpt.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/utils/ema.py` & `castle_ai-0.0.8/castle/aot/utils/ema.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/utils/image.py` & `castle_ai-0.0.8/castle/aot/utils/image.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/utils/learning.py` & `castle_ai-0.0.8/castle/aot/utils/learning.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/utils/math.py` & `castle_ai-0.0.8/castle/aot/utils/math.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/utils/meters.py` & `castle_ai-0.0.8/castle/aot/utils/meters.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/aot/utils/metric.py` & `castle_ai-0.0.8/castle/aot/utils/metric.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/automatic_mask_generator.py` & `castle_ai-0.0.8/castle/sam/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/build_sam.py` & `castle_ai-0.0.8/castle/sam/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/modeling/common.py` & `castle_ai-0.0.8/castle/sam/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/modeling/image_encoder.py` & `castle_ai-0.0.8/castle/sam/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/modeling/mask_decoder.py` & `castle_ai-0.0.8/castle/sam/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/modeling/prompt_encoder.py` & `castle_ai-0.0.8/castle/sam/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/modeling/sam.py` & `castle_ai-0.0.8/castle/sam/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/modeling/transformer.py` & `castle_ai-0.0.8/castle/sam/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/predictor.py` & `castle_ai-0.0.8/castle/sam/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/utils/amg.py` & `castle_ai-0.0.8/castle/sam/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/utils/onnx.py` & `castle_ai-0.0.8/castle/sam/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/segment_anything/utils/transforms.py` & `castle_ai-0.0.8/castle/sam/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/sam/setup.py` & `castle_ai-0.0.8/castle/sam/setup.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/cluster_input_ui.py` & `castle_ai-0.0.8/castle/ui/cluster_input_ui.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/dbscan_ui.py` & `castle_ai-0.0.8/castle/ui/dbscan_ui.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/dimension_reduction_ui.py` & `castle_ai-0.0.8/castle/ui/dimension_reduction_ui.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/edit_ui.py` & `castle_ai-0.0.8/castle/ui/edit_ui.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/label_ui.py` & `castle_ai-0.0.8/castle/ui/label_ui.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/main_ui.py` & `castle_ai-0.0.8/castle/ui/main_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import gradio as gr
 
 
 from .project_ui import create_project_ui
 from .source_ui import create_source_ui
 from .edit_ui import create_edit_ui
 from .extract_ui import create_extract_ui
-# from .cluster_page_ui import create_cluster_page_ui
+from .cluster_page_ui import create_cluster_page_ui
 
 def show_ui(project_name, object_count):
     if not project_name == None:
         return [gr.update(visible=True) for i in range(object_count)]
     else:
         return [gr.update(visible=False) for i in range(object_count)]
 
@@ -47,22 +47,22 @@
             extract_tab.select(
                 fn=show_ui, 
                 inputs=[project_ui['project_name'], extract_ui_object_count], 
                 outputs=[v for k, v in extract_ui.items()]
             )
             pass
 
-        # with gr.Tab(label='Cluster') as cluster_page_tab:
-        #     cluster_ui = create_cluster_page_ui(storage_path, project_name, cluster_page_tab)
-        #     cluster_ui_object_count = gr.State(len(cluster_ui))
-        #     cluster_page_tab.select(
-        #         fn=show_ui, 
-        #         inputs=[project_ui['project_name'], cluster_ui_object_count], 
-        #         outputs=[v for k, v in cluster_ui.items()]
-        #     )
-        #     pass
+        with gr.Tab(label='Latent Explorer') as cluster_page_tab:
+            cluster_ui = create_cluster_page_ui(storage_path, project_name, cluster_page_tab)
+            cluster_ui_object_count = gr.State(len(cluster_ui))
+            cluster_page_tab.select(
+                fn=show_ui, 
+                inputs=[project_ui['project_name'], cluster_ui_object_count], 
+                outputs=[v for k, v in cluster_ui.items()]
+            )
+            pass
 
         # with gr.Tab(label='Export'):
         #     pass
 
     return app
```

### Comparing `castle_ai-0.0.6/castle/ui/plot_mask_info.py` & `castle_ai-0.0.8/castle/ui/plot_mask_info.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/post_track_ui.py` & `castle_ai-0.0.8/castle/ui/post_track_ui.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/project_ui.py` & `castle_ai-0.0.8/castle/ui/project_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,18 +45,22 @@
         print("Deleted")
     else:
         print("No such folder")
 
 
 
 def create_project_ui(OS_SYS, root=''):
-    if len(root) == 0:
-        root = 'projects/'
-    if not root[-1] == '/':
-        root += '/'
+    if root == None:
+        root = os.path.join('projects','')
+    sep = os.sep
+    if not root.endswith(sep):
+        root += sep
+    if not os.path.exists(root):
+        os.makedirs(root)
+        
     ui = dict()
     DEFAULT_DEVICE = 'mps' if OS_SYS == 'Darwin' else 'cuda'
     ui['device'] = gr.Textbox(label='Device',
                               info='For example: mps, cpu, cuda, or cuda:x',
                               value=DEFAULT_DEVICE,
                               interactive=False, visible=False)
```

### Comparing `castle_ai-0.0.6/castle/ui/source_ui.py` & `castle_ai-0.0.8/castle/ui/source_ui.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/ui/track_ui.py` & `castle_ai-0.0.8/castle/ui/track_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
 
     def write_mask(self, index, mask):
         mask_list_path = os.path.join(self.track_dir_path, f'mask_list.h5')            
         mode = 'a' if os.path.isfile(mask_list_path) else 'w'
         with h5py.File(mask_list_path, mode) as f:
             if f"{index}" in f:
-                dset = f[f"{index}"]
+                dset = f[f"{index}"][:]
                 dset[:] = mask
             else:
                 dset = f.create_dataset(f"{index}", mask.shape, dtype='uint8', compression="gzip", compression_opts=9)
                 dset[:] = mask
 
 
     def set_cancel(self):
@@ -202,15 +202,15 @@
 def create_track_ui(storage_path, project_name, source_video, track_tab):
     ui = dict()
 
     label_list = gr.State(None)
     interfence = gr.State(None)
     with gr.Accordion('ROIs Knowledge', visible=False) as ui['gallery_accordion']:
         ui['gallery'] = gr.Gallery(
-            label="Label Frame", show_label=True, allow_preview=True, height="auto", object_fit="contain", columns=3)
+            label="Label Frame", show_label=True, allow_preview=False, object_fit="contain", columns=3)
 
     with gr.Accordion('Inference', open=True, visible=False) as ui['inference_accordion']:
         with gr.Row(visible=True):
             with gr.Column(scale=2):
                 # ui['start_frame'] = gr.Textbox(
                 #     label="Start Frame", interactive=False, visible=False)
                 ui['start_frame'] = gr.Slider(
```

### Comparing `castle_ai-0.0.6/castle/ui/view_ui.py` & `castle_ai-0.0.8/castle/ui/view_ui.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/utils/download.py` & `castle_ai-0.0.8/castle/utils/download.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/utils/h5_io.py` & `castle_ai-0.0.8/castle/utils/h5_io.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/utils/image_segment.py` & `castle_ai-0.0.8/castle/utils/image_segment.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/utils/plot.py` & `castle_ai-0.0.8/castle/utils/plot.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/utils/video_align.py` & `castle_ai-0.0.8/castle/utils/video_align.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/utils/video_io.py` & `castle_ai-0.0.8/castle/utils/video_io.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/utils/video_object_segment.py` & `castle_ai-0.0.8/castle/utils/video_object_segment.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle/utils/visual_latent_extract.py` & `castle_ai-0.0.8/castle/utils/visual_latent_extract.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/castle_ai.egg-info/PKG-INFO` & `castle_ai-0.0.8/castle_ai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castle-ai
-Version: 0.0.6
+Version: 0.0.8
 Summary: Distinguish behavioral clusters Toolbox
 Maintainer: Raiso Liu
 Maintainer-email: rainsoon717@gmail.com
 License: AGPL-3.0 license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,15 @@
 Requires-Dist: torchvision
 Requires-Dist: matplotlib
 Requires-Dist: umap-learn
 Requires-Dist: h5py
 Requires-Dist: natsort
 Requires-Dist: gradio
 Requires-Dist: plotly
+Requires-Dist: hdbscan
 
 # CASTLE
 
 
 [![PyPI version](https://badge.fury.io/py/castle-ai.svg)](https://badge.fury.io/py/castle-ai)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CASTLE-ai/castle-ai/blob/main/notebooks/colab.ipynb)
 
@@ -41,15 +42,15 @@
 ```
 pip install castle-ai
 ```
 
 # Open
 
 ```
-python web_ui/app.py
+python app.py
 ```
 
 # Reference
 
 [Segment Anything](https://github.com/facebookresearch/segment-anything.git)
 
 [DeAOT](https://github.com/z-x-yang/Segment-and-Track-Anything.git)
```

### Comparing `castle_ai-0.0.6/castle_ai.egg-info/SOURCES.txt` & `castle_ai-0.0.8/castle_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.6/setup.py` & `castle_ai-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         with io.open("README.md", encoding="UTF-8") as readme_file:
             return readme_file.read()
 
 
 
 configuration = {
     "name": "castle-ai",
-    "version": "0.0.6",
+    "version": "0.0.8",
     "description": "Distinguish behavioral clusters Toolbox",
     "long_description": readme(),
     "long_description_content_type": "text/markdown",
     "classifiers": [
         "Development Status :: 1 - Planning",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
@@ -45,14 +45,15 @@
         "torchvision",
         "matplotlib",
         "umap-learn",
         "h5py",
         "natsort",
         "gradio",
         "plotly",
+        "hdbscan",
     ],
     # "extras_require": {
     #     "cu11": [
     #         "pandas",
     #         "matplotlib",
     #         "datashader",
     #         "bokeh",
```

