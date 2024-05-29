# Comparing `tmp/kimm-0.2.1.tar.gz` & `tmp/kimm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimm-0.2.1.tar", last modified: Wed May 22 03:28:56 2024, max compression
+gzip compressed data, was "kimm-0.2.2.tar", last modified: Wed May 29 03:44:31 2024, max compression
```

## Comparing `kimm-0.2.1.tar` & `kimm-0.2.2.tar`

### file list

```diff
@@ -1,125 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 03:27:34.000000 kimm-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-22 03:28:56.581305 kimm-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-22 03:27:34.000000 kimm-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.565304 kimm-0.2.1/kimm/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.565304 kimm-0.2.1/kimm/_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.569305 kimm-0.2.1/kimm/_src/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/depthwise_separation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.569305 kimm-0.2.1/kimm/_src/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/export_onnx_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/export_tflite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/export_tflite_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/kimm_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.569305 kimm-0.2.1/kimm/_src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/layer_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/layer_scale_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/learnable_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/learnable_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/mobile_one_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/mobile_one_conv2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/rep_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/rep_conv2d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.573305 kimm-0.2.1/kimm/_src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/convmixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/ghostnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/hgnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/inception_next.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/mobileone.py
--rw-r--r--   0 runner    (1001) docker     (127)    26900 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/mobilevit.py
--rw-r--r--   0 runner    (1001) docker     (127)    22811 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/models_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18127 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/regnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/repvgg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/vgg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/_src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/make_divisble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/model_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/model_registry_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/model_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/timm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/export/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/base_model/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/base_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/convmixer/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/convmixer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/ghostnet/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/ghostnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/hgnet/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/hgnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/inception_next/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/inception_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/mobileone/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/mobileone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/mobilevit/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/mobilevit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/regnet/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/regnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/repvgg/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/repvgg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/vgg/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/vgg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/vision_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/vision_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/timm_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/timm_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-22 03:27:34.000000 kimm-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:28:56.581305 kimm-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.106458 kimm-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 03:43:11.000000 kimm-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-29 03:44:31.106458 kimm-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-29 03:43:11.000000 kimm-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.090458 kimm-0.2.2/kimm/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.090458 kimm-0.2.2/kimm/_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.094457 kimm-0.2.2/kimm/_src/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/blocks/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/blocks/depthwise_separation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/blocks/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/blocks/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.094457 kimm-0.2.2/kimm/_src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/export/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/export/export_onnx_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/export/export_tflite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/export/export_tflite_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/kimm_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.094457 kimm-0.2.2/kimm/_src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/layer_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/layer_scale_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/learnable_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/learnable_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/reparameterizable_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/layers/reparameterizable_conv2d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.098458 kimm-0.2.2/kimm/_src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/convmixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14179 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/ghostnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/ghostnet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/hgnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/inception_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/mobileone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26900 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23341 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18127 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/repvgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/models/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/_src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/utils/make_divisble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/utils/model_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/utils/model_registry_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/utils/model_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/utils/timm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/_src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/base_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/base_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/convmixer/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/convmixer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/ghostnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/ghostnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/hgnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/hgnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/inception_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/inception_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/mobileone/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/mobileone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/mobilevit/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/mobilevit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/regnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/regnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/repvgg/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/repvgg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/vgg/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/vgg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.102458 kimm-0.2.2/kimm/models/vision_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/vision_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.106458 kimm-0.2.2/kimm/models/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/models/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.106458 kimm-0.2.2/kimm/timm_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/timm_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.106458 kimm-0.2.2/kimm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 03:43:11.000000 kimm-0.2.2/kimm/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:44:31.106458 kimm-0.2.2/kimm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-29 03:44:31.000000 kimm-0.2.2/kimm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-29 03:44:31.000000 kimm-0.2.2/kimm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:44:31.000000 kimm-0.2.2/kimm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 03:44:31.000000 kimm-0.2.2/kimm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 03:44:31.000000 kimm-0.2.2/kimm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-29 03:43:11.000000 kimm-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:44:31.106458 kimm-0.2.2/setup.cfg
```

### Comparing `kimm-0.2.1/LICENSE` & `kimm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/PKG-INFO` & `kimm-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimm
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Keras model zoo with pretrained weights.
 Author-email: Hong-Yu Chiu <james77777778@gmail.com>
 Maintainer-email: Hong-Yu Chiu <james77777778@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/james77777778/keras-image-models
 Project-URL: Documentation, https://github.com/james77777778/keras-image-models
 Project-URL: Repository, https://github.com/james77777778/keras-image-models.git
@@ -54,25 +54,33 @@
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/kimm/issues)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-image-models/actions.yml?label=tests)](https://github.com/james77777778/keras-image-models/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-image-models/graph/badge.svg?token=eEha1SR80D)](https://codecov.io/gh/james77777778/keras-image-models)
 </div>
 
 # Keras Image Models
 
+- [Latest Updates](#latest-updates)
 - [Introduction](#introduction)
 - [Usage](#usage)
 - [Installation](#installation)
 - [Quickstart](#quickstart)
   - [Image classification with ImageNet weights](#image-classification-using-the-model-pretrained-on-imagenet)
   - [An end-to-end fine-tuning example: cats vs. dogs dataset](#an-end-to-end-example-fine-tuning-an-image-classification-model-on-a-cats-vs-dogs-dataset)
   - [Grad-CAM](#grad-cam)
 - [Model Zoo](#model-zoo)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
 
+## Latest Updates
+
+2024/05/29:
+
+- Merge reparameterizable layers into 1 `ReparameterizableConv2D`
+- Add `GhostNetV3*` from [huawei-noah/Efficient-AI-Backbones](https://github.com/huawei-noah/Efficient-AI-Backbones)
+
 ## Introduction
 
 **K**eras **Im**age **M**odels (`kimm`) is a collection of image models, blocks and layers written in Keras 3. The goal is to offer SOTA models with pretrained weights in a user-friendly manner.
 
 **KIMM** is:
 
 - 🚀 A model zoo where almost all models come with **pre-trained weights on ImageNet**.
@@ -195,14 +203,15 @@
 |ConvNeXt|[CVPR 2022](https://arxiv.org/abs/2201.03545)|`timm`|`kimm.models.ConvNeXt*`|
 |DenseNet|[CVPR 2017](https://arxiv.org/abs/1608.06993)|`timm`|`kimm.models.DenseNet*`|
 |EfficientNet|[ICML 2019](https://arxiv.org/abs/1905.11946)|`timm`|`kimm.models.EfficientNet*`|
 |EfficientNetLite|[ICML 2019](https://arxiv.org/abs/1905.11946)|`timm`|`kimm.models.EfficientNetLite*`|
 |EfficientNetV2|[ICML 2021](https://arxiv.org/abs/2104.00298)|`timm`|`kimm.models.EfficientNetV2*`|
 |GhostNet|[CVPR 2020](https://arxiv.org/abs/1911.11907)|`timm`|`kimm.models.GhostNet*`|
 |GhostNetV2|[NeurIPS 2022](https://arxiv.org/abs/2211.12905)|`timm`|`kimm.models.GhostNetV2*`|
+|GhostNetV3|[arXiv 2024](https://arxiv.org/abs/2404.11202)|`github`|`kimm.models.GhostNetV3*`|
 |HGNet||`timm`|`kimm.models.HGNet*`|
 |HGNetV2||`timm`|`kimm.models.HGNetV2*`|
 |InceptionNeXt|[arXiv 2023](https://arxiv.org/abs/2303.16900)|`timm`|`kimm.models.InceptionNeXt*`|
 |InceptionV3|[CVPR 2016](https://arxiv.org/abs/1512.00567)|`timm`|`kimm.models.InceptionV3`|
 |LCNet|[arXiv 2021](https://arxiv.org/abs/2109.15099)|`timm`|`kimm.models.LCNet*`|
 |MobileNetV2|[CVPR 2018](https://arxiv.org/abs/1801.04381)|`timm`|`kimm.models.MobileNetV2*`|
 |MobileNetV3|[ICCV 2019](https://arxiv.org/abs/1905.02244)|`timm`|`kimm.models.MobileNetV3*`|
```

### Comparing `kimm-0.2.1/README.md` & `kimm-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,33 @@
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/kimm/issues)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-image-models/actions.yml?label=tests)](https://github.com/james77777778/keras-image-models/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-image-models/graph/badge.svg?token=eEha1SR80D)](https://codecov.io/gh/james77777778/keras-image-models)
 </div>
 
 # Keras Image Models
 
+- [Latest Updates](#latest-updates)
 - [Introduction](#introduction)
 - [Usage](#usage)
 - [Installation](#installation)
 - [Quickstart](#quickstart)
   - [Image classification with ImageNet weights](#image-classification-using-the-model-pretrained-on-imagenet)
   - [An end-to-end fine-tuning example: cats vs. dogs dataset](#an-end-to-end-example-fine-tuning-an-image-classification-model-on-a-cats-vs-dogs-dataset)
   - [Grad-CAM](#grad-cam)
 - [Model Zoo](#model-zoo)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
 
+## Latest Updates
+
+2024/05/29:
+
+- Merge reparameterizable layers into 1 `ReparameterizableConv2D`
+- Add `GhostNetV3*` from [huawei-noah/Efficient-AI-Backbones](https://github.com/huawei-noah/Efficient-AI-Backbones)
+
 ## Introduction
 
 **K**eras **Im**age **M**odels (`kimm`) is a collection of image models, blocks and layers written in Keras 3. The goal is to offer SOTA models with pretrained weights in a user-friendly manner.
 
 **KIMM** is:
 
 - 🚀 A model zoo where almost all models come with **pre-trained weights on ImageNet**.
@@ -150,14 +158,15 @@
 |ConvNeXt|[CVPR 2022](https://arxiv.org/abs/2201.03545)|`timm`|`kimm.models.ConvNeXt*`|
 |DenseNet|[CVPR 2017](https://arxiv.org/abs/1608.06993)|`timm`|`kimm.models.DenseNet*`|
 |EfficientNet|[ICML 2019](https://arxiv.org/abs/1905.11946)|`timm`|`kimm.models.EfficientNet*`|
 |EfficientNetLite|[ICML 2019](https://arxiv.org/abs/1905.11946)|`timm`|`kimm.models.EfficientNetLite*`|
 |EfficientNetV2|[ICML 2021](https://arxiv.org/abs/2104.00298)|`timm`|`kimm.models.EfficientNetV2*`|
 |GhostNet|[CVPR 2020](https://arxiv.org/abs/1911.11907)|`timm`|`kimm.models.GhostNet*`|
 |GhostNetV2|[NeurIPS 2022](https://arxiv.org/abs/2211.12905)|`timm`|`kimm.models.GhostNetV2*`|
+|GhostNetV3|[arXiv 2024](https://arxiv.org/abs/2404.11202)|`github`|`kimm.models.GhostNetV3*`|
 |HGNet||`timm`|`kimm.models.HGNet*`|
 |HGNetV2||`timm`|`kimm.models.HGNetV2*`|
 |InceptionNeXt|[arXiv 2023](https://arxiv.org/abs/2303.16900)|`timm`|`kimm.models.InceptionNeXt*`|
 |InceptionV3|[CVPR 2016](https://arxiv.org/abs/1512.00567)|`timm`|`kimm.models.InceptionV3`|
 |LCNet|[arXiv 2021](https://arxiv.org/abs/2109.15099)|`timm`|`kimm.models.LCNet*`|
 |MobileNetV2|[CVPR 2018](https://arxiv.org/abs/1801.04381)|`timm`|`kimm.models.MobileNetV2*`|
 |MobileNetV3|[ICCV 2019](https://arxiv.org/abs/1905.02244)|`timm`|`kimm.models.MobileNetV3*`|
```

### Comparing `kimm-0.2.1/kimm/_src/blocks/conv2d.py` & `kimm-0.2.2/kimm/_src/blocks/conv2d.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/blocks/depthwise_separation.py` & `kimm-0.2.2/kimm/_src/blocks/depthwise_separation.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/blocks/inverted_residual.py` & `kimm-0.2.2/kimm/_src/blocks/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/blocks/squeeze_and_excitation.py` & `kimm-0.2.2/kimm/_src/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/blocks/transformer.py` & `kimm-0.2.2/kimm/_src/blocks/transformer.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/export/export_onnx.py` & `kimm-0.2.2/kimm/_src/export/export_onnx.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/export/export_onnx_test.py` & `kimm-0.2.2/kimm/_src/export/export_onnx_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/export/export_tflite.py` & `kimm-0.2.2/kimm/_src/export/export_tflite.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/export/export_tflite_test.py` & `kimm-0.2.2/kimm/_src/export/export_tflite_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/kimm_export.py` & `kimm-0.2.2/kimm/_src/kimm_export.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/layers/attention.py` & `kimm-0.2.2/kimm/_src/layers/attention.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/layers/attention_test.py` & `kimm-0.2.2/kimm/_src/layers/attention_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/layers/layer_scale.py` & `kimm-0.2.2/kimm/_src/layers/layer_scale.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/layers/layer_scale_test.py` & `kimm-0.2.2/kimm/_src/layers/layer_scale_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/layers/learnable_affine.py` & `kimm-0.2.2/kimm/_src/layers/learnable_affine.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/layers/learnable_affine_test.py` & `kimm-0.2.2/kimm/_src/layers/learnable_affine_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/layers/mobile_one_conv2d.py` & `kimm-0.2.2/kimm/_src/layers/reparameterizable_conv2d.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,172 +10,173 @@
 from keras.src.utils.argument_validation import standardize_tuple
 
 from kimm._src.kimm_export import kimm_export
 
 
 @kimm_export(parent_path=["kimm.layers"])
 @keras.saving.register_keras_serializable(package="kimm")
-class MobileOneConv2D(Layer):
+class ReparameterizableConv2D(Layer):
     def __init__(
         self,
         filters,
         kernel_size,
         strides=(1, 1),
         padding=None,
         has_skip: bool = True,
+        has_scale: bool = True,
         use_depthwise: bool = False,
         branch_size: int = 1,
         reparameterized: bool = False,
         data_format=None,
         activation=None,
+        name=None,
         **kwargs,
     ):
-        super().__init__(**kwargs)
+        super().__init__(name=name, **kwargs)
         self.filters = filters
         self.kernel_size = standardize_tuple(kernel_size, 2, "kernel_size")
         self.strides = standardize_tuple(strides, 2, "strides")
         self.padding = padding
         self.has_skip = has_skip
+        self.has_scale = has_scale
         self.use_depthwise = use_depthwise
         self.branch_size = branch_size
-        self._reparameterized = reparameterized
+        self.reparameterized = reparameterized
         self.data_format = standardize_data_format(data_format)
         self.activation = activation
 
         if self.kernel_size[0] != self.kernel_size[1]:
             raise ValueError(
-                "The value of kernel_size must be the same. "
+                "The values of `kernel_size` must be the same. "
                 f"Received: kernel_size={kernel_size}"
             )
         if self.strides[0] != self.strides[1]:
             raise ValueError(
-                "The value of strides must be the same. "
+                "The values of `strides` must be the same. "
                 f"Received: strides={strides}"
             )
-        if has_skip is True and (self.strides[0] != 1 or self.strides[1] != 1):
+        if has_skip is True and self.strides[0] != 1:
             raise ValueError(
-                "strides must be `1` when `has_skip=True`. "
+                "When `has_skip=True`, `strides` must be `1`. "
                 f"Received: has_skip={has_skip}, strides={strides}"
             )
 
-        self.zero_padding = layers.Identity(dtype=self.dtype_policy)
-        if padding is None:
-            padding = "same"
-            if self.strides[0] > 1:
-                padding = "valid"
+        # Configure zero padding
+        self.zero_padding: typing.Optional[layers.ZeroPadding2D] = None
+        if self.padding is None:
+            if self.strides[0] > 1 and self.kernel_size[0] > 1:
+                self.padding = "valid"
                 self.zero_padding = layers.ZeroPadding2D(
-                    (self.kernel_size[0] // 2, self.kernel_size[1] // 2),
+                    self.kernel_size[0] // 2,
                     data_format=self.data_format,
                     dtype=self.dtype_policy,
                     name=f"{self.name}_pad",
                 )
-            self.padding = padding
-        else:
-            self.padding = padding
+            else:
+                self.padding = "same"
+
+        # Configure filters_axis
+        self.filters_axis = -1 if self.data_format == "channels_last" else -3
 
-        channel_axis = -1 if self.data_format == "channels_last" else -3
+        # Build layers
+        bn_momentum, bn_epsilon = 0.9, 1e-5  # Defaults to torch's default
 
-        # Build layers (rep_conv2d, identity, conv_kxk, conv_scale)
-        self.rep_conv2d: typing.Optional[layers.Conv2D] = None
-        self.identity: typing.Optional[layers.BatchNormalization] = None
-        self.conv_kxk: typing.Optional[typing.List[Sequential]] = None
+        self.reparameterized_conv2d: typing.Optional[layers.Conv2D] = None
+        self.skip: typing.Optional[layers.BatchNormalization] = None
         self.conv_scale: typing.Optional[Sequential] = None
-        if self._reparameterized:
-            self.rep_conv2d = self._get_conv2d(
-                use_depthwise,
+        self.conv_kxk: typing.List[Sequential] = []
+        self.act: typing.Optional[layers.Activation] = None
+
+        if self.reparameterized:
+            self.reparameterized_conv2d = self._get_conv2d_layer(
+                self.use_depthwise,
                 self.filters,
                 self.kernel_size,
                 self.strides,
                 self.padding,
                 use_bias=True,
                 name=f"{self.name}_reparam_conv",
             )
         else:
-            # Skip connection
+            # Skip branch
             if self.has_skip:
-                self.identity = layers.BatchNormalization(
-                    axis=channel_axis,
-                    momentum=0.9,
-                    epsilon=1e-5,
+                self.skip = layers.BatchNormalization(
+                    axis=self.filters_axis,
+                    momentum=bn_momentum,
+                    epsilon=bn_epsilon,
                     dtype=self.dtype_policy,
-                    name=f"{self.name}_identity",
+                    name=f"{self.name}_skip",
                 )
-            else:
-                self.identity = None
-
-            # Convoluation branches
-            self.conv_kxk = []
+            # Scale branch
+            if self.has_scale:
+                self.conv_scale = Sequential(
+                    [
+                        self._get_conv2d_layer(
+                            self.use_depthwise,
+                            self.filters,
+                            1,
+                            self.strides,
+                            self.padding,
+                            use_bias=False,
+                        ),
+                        layers.BatchNormalization(
+                            axis=self.filters_axis,
+                            momentum=bn_momentum,
+                            epsilon=bn_epsilon,
+                            dtype=self.dtype_policy,
+                        ),
+                    ],
+                    name=f"{self.name}_conv_scale",
+                )
+            # Overparameterized branch
             for i in range(self.branch_size):
                 self.conv_kxk.append(
                     Sequential(
                         [
-                            self._get_conv2d(
+                            self._get_conv2d_layer(
                                 self.use_depthwise,
                                 self.filters,
                                 self.kernel_size,
                                 self.strides,
                                 self.padding,
                                 use_bias=False,
                             ),
                             layers.BatchNormalization(
-                                axis=channel_axis,
-                                momentum=0.9,
-                                epsilon=1e-5,
+                                axis=self.filters_axis,
+                                momentum=bn_momentum,
+                                epsilon=bn_epsilon,
                                 dtype=self.dtype_policy,
                             ),
                         ],
                         name=f"{self.name}_conv_kxk_{i}",
                     )
                 )
-
-            # Scale branch
-            self.conv_scale = None
-            if self.kernel_size[0] > 1:
-                self.conv_scale = Sequential(
-                    [
-                        self._get_conv2d(
-                            self.use_depthwise,
-                            self.filters,
-                            1,
-                            self.strides,
-                            self.padding,
-                            use_bias=False,
-                        ),
-                        layers.BatchNormalization(
-                            axis=channel_axis,
-                            momentum=0.9,
-                            epsilon=1e-5,
-                            dtype=self.dtype_policy,
-                        ),
-                    ],
-                    name=f"{self.name}_conv_scale",
-                )
-
-        if activation is None:
-            self.act = layers.Identity(dtype=self.dtype_policy)
-        else:
+        if activation is not None:
             self.act = layers.Activation(activation, dtype=self.dtype_policy)
 
-        # Internal parameters for `_get_reparameterized_weights_from_layer`
-        self._input_channels = None
-        self._rep_kernel_shape = None
-
-        # Attach extra layers
-        self.extra_layers = []
-        if self.rep_conv2d is not None:
-            self.extra_layers.append(self.rep_conv2d)
-        if self.identity is not None:
-            self.extra_layers.append(self.identity)
-        if self.conv_kxk is not None:
-            self.extra_layers.extend(self.conv_kxk)
+    @property
+    def _sublayers(self):
+        """An internal api for weights exporting.
+
+        Generally, you don't need this.
+        """
+        sublayers = []
+        if self.reparameterized_conv2d is not None:
+            sublayers.append(self.reparameterized_conv2d)
+        if self.skip is not None:
+            sublayers.append(self.skip)
         if self.conv_scale is not None:
-            self.extra_layers.append(self.conv_scale)
-        self.extra_layers.append(self.act)
+            sublayers.append(self.conv_scale)
+        if self.conv_kxk is not None:
+            sublayers.extend(self.conv_kxk)
+        if self.act is not None:
+            sublayers.append(self.act)
+        return sublayers
 
-    def _get_conv2d(
+    def _get_conv2d_layer(
         self,
         use_depthwise,
         filters,
         kernel_size,
         strides,
         padding,
         use_bias,
@@ -200,93 +201,99 @@
                 data_format=self.data_format,
                 use_bias=use_bias,
                 dtype=self.dtype_policy,
                 name=name,
             )
 
     def build(self, input_shape):
-        channel_axis = -1 if self.data_format == "channels_last" else -3
+        input_filters = input_shape[self.filters_axis]
+        if self.use_depthwise and input_filters != self.filters:
+            raise ValueError(
+                "When `use_depthwise=True`, `filters` must be the same as "
+                f"input filters. Received: input_shape={input_shape}, "
+                f"filters={self.filters}"
+            )
 
         if isinstance(self.zero_padding, layers.ZeroPadding2D):
-            padded_shape = self.zero_padding.compute_output_shape(input_shape)
-        else:
-            padded_shape = input_shape
+            input_shape = self.zero_padding.compute_output_shape(input_shape)
 
-        if self.rep_conv2d is not None:
-            self.rep_conv2d.build(padded_shape)
-        if self.identity is not None:
-            self.identity.build(input_shape)
-        if self.conv_kxk is not None:
-            for layer in self.conv_kxk:
-                layer.build(padded_shape)
+        if self.reparameterized_conv2d is not None:
+            self.reparameterized_conv2d.build(input_shape)
+
+        if self.skip is not None:
+            self.skip.build(input_shape)
         if self.conv_scale is not None:
             self.conv_scale.build(input_shape)
+        for layer in self.conv_kxk:
+            layer.build(input_shape)
 
         # Update internal parameters
-        self._input_channels = input_shape[channel_axis]
-        if self.conv_kxk is not None:
-            self._rep_kernel_shape = self.conv_kxk[0].layers[0].kernel.shape
+        self.input_filters = input_filters
 
         self.built = True
 
-    def call(self, inputs, **kwargs):
-        x = ops.cast(inputs, self.compute_dtype)
-        padded_x = self.zero_padding(x)
-
-        # Shortcut for reparameterized mode
-        if self._reparameterized:
-            return self.act(self.rep_conv2d(padded_x, **kwargs))
-
-        # Skip connection
-        identity_outputs = None
-        if self.identity is not None:
-            identity_outputs = self.identity(x, **kwargs)
-
+    def call(self, inputs, training=None, **kwargs):
+        x = inputs
+        padded_x = x
+
+        if self.zero_padding is not None:
+            padded_x = self.zero_padding(x)
+
+        # Shortcut for reparameterized=True
+        if self.reparameterized:
+            y = self.reparameterized_conv2d(padded_x)
+            if self.act is not None:
+                y = self.act(y)
+            return y
+
+        # Skip branch
+        y = None
+        if self.skip is not None:
+            y = self.skip(x, training=training)
         # Scale branch
-        scale_outputs = None
         if self.conv_scale is not None:
-            scale_outputs = self.conv_scale(x, **kwargs)
-
-        # Conv branch
-        conv_outputs = scale_outputs
-        for layer in self.conv_kxk:
-            if conv_outputs is None:
-                conv_outputs = layer(padded_x, **kwargs)
+            scale_y = self.conv_scale(x, training=training)
+            if y is None:
+                y = scale_y
             else:
-                conv_outputs = layers.Add()(
-                    [conv_outputs, layer(padded_x, **kwargs)]
-                )
-
-        if identity_outputs is not None:
-            outputs = layers.Add()([conv_outputs, identity_outputs])
-        else:
-            outputs = conv_outputs
-        return self.act(outputs)
+                y = layers.Add(dtype=self.dtype_policy)([y, scale_y])
+        # Overparameterized bracnh
+        for idx in range(self.branch_size):
+            over_y = self.conv_kxk[idx](padded_x, training=training)
+            if y is None:
+                y = over_y
+            else:
+                y = layers.Add(dtype=self.dtype_policy)([y, over_y])
+        if self.act is not None:
+            y = self.act(y)
+        return y
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "filters": self.filters,
                 "kernel_size": self.kernel_size,
                 "strides": self.strides,
                 "padding": self.padding,
                 "has_skip": self.has_skip,
+                "has_scale": self.has_scale,
                 "use_depthwise": self.use_depthwise,
                 "branch_size": self.branch_size,
-                "reparameterized": self._reparameterized,
+                "reparameterized": self.reparameterized,
                 "data_format": self.data_format,
                 "activation": self.activation,
                 "name": self.name,
             }
         )
         return config
 
     def _get_reparameterized_weights_from_layer(self, layer):
         if isinstance(layer, Sequential):
+            # Check
             if not isinstance(
                 layer.layers[0], (layers.Conv2D, layers.DepthwiseConv2D)
             ):
                 raise ValueError
             if not isinstance(layer.layers[1], layers.BatchNormalization):
                 raise ValueError
             kernel = ops.convert_to_numpy(layer.layers[0].kernel)
@@ -294,40 +301,29 @@
                 kernel = np.swapaxes(kernel, -2, -1)
             gamma = ops.convert_to_numpy(layer.layers[1].gamma)
             beta = ops.convert_to_numpy(layer.layers[1].beta)
             running_mean = ops.convert_to_numpy(layer.layers[1].moving_mean)
             running_var = ops.convert_to_numpy(layer.layers[1].moving_variance)
             eps = layer.layers[1].epsilon
         elif isinstance(layer, layers.BatchNormalization):
-            if self._rep_kernel_shape is None:
-                raise ValueError(
-                    "Remember to build the layer before performing"
-                    "reparameterization. Failed to get valid "
-                    "`self._rep_kernel_shape`."
-                )
-            # Calculate identity tensor
-            kernel_value = ops.convert_to_numpy(
-                ops.zeros(self._rep_kernel_shape)
+            k = self.kernel_size[0]
+            input_filters = 1 if self.use_depthwise else self.input_filters
+            kernel = np.zeros(
+                shape=[k, k, input_filters, self.filters], dtype="float64"
             )
-            kernel = kernel_value.copy()
-            if self.use_depthwise:
-                kernel = np.swapaxes(kernel, -2, -1)
-            for i in range(self._input_channels):
+            for i in range(self.input_filters):
                 group_i = 0 if self.use_depthwise else i
-                kernel[
-                    self.kernel_size[0] // 2,
-                    self.kernel_size[1] // 2,
-                    group_i,
-                    i,
-                ] = 1
+                kernel[k // 2, k // 2, group_i, i] = 1
             gamma = ops.convert_to_numpy(layer.gamma)
             beta = ops.convert_to_numpy(layer.beta)
             running_mean = ops.convert_to_numpy(layer.moving_mean)
             running_var = ops.convert_to_numpy(layer.moving_variance)
             eps = layer.epsilon
+        else:
+            raise NotImplementedError
 
         # use float64 for better precision
         kernel = kernel.astype("float64")
         gamma = gamma.astype("float64")
         beta = beta.astype("float64")
         running_var = running_var.astype("float64")
         running_var = running_var.astype("float64")
@@ -337,37 +333,37 @@
 
         kernel_final = kernel * t
         if self.use_depthwise:
             kernel_final = np.swapaxes(kernel_final, -2, -1)
         return kernel_final, beta - running_mean * gamma / std
 
     def get_reparameterized_weights(self):
+        # Get kernels and bias from skip branch
+        kernel_identity = 0.0
+        bias_identity = 0.0
+        if self.skip is not None:
+            (
+                kernel_identity,
+                bias_identity,
+            ) = self._get_reparameterized_weights_from_layer(self.skip)
+
         # Get kernels and bias from scale branch
         kernel_scale = 0.0
         bias_scale = 0.0
         if self.conv_scale is not None:
             (
                 kernel_scale,
                 bias_scale,
             ) = self._get_reparameterized_weights_from_layer(self.conv_scale)
             pad = self.kernel_size[0] // 2
             kernel_scale = np.pad(
                 kernel_scale, [[pad, pad], [pad, pad], [0, 0], [0, 0]]
             )
 
-        # Get kernels and bias from skip branch
-        kernel_identity = 0.0
-        bias_identity = 0.0
-        if self.identity is not None:
-            (
-                kernel_identity,
-                bias_identity,
-            ) = self._get_reparameterized_weights_from_layer(self.identity)
-
-        # Get kernels and bias from conv branch
+        # Get kernels and bias from overparameterized branch
         kernel_conv = 0.0
         bias_conv = 0.0
         for i in range(self.branch_size):
             (
                 _kernel_conv,
                 _bias_conv,
             ) = self._get_reparameterized_weights_from_layer(self.conv_kxk[i])
```

### Comparing `kimm-0.2.1/kimm/_src/layers/mobile_one_conv2d_test.py` & `kimm-0.2.2/kimm/_src/layers/reparameterizable_conv2d_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,119 @@
 import pytest
 from absl.testing import parameterized
 from keras import backend
 from keras import random
 from keras.src import testing
 
-from kimm._src.layers.mobile_one_conv2d import MobileOneConv2D
+from kimm._src.layers.reparameterizable_conv2d import ReparameterizableConv2D
 
 TEST_CASES = [
     {
         "filters": 16,
         "kernel_size": 3,
         "has_skip": True,
+        "has_scale": True,
         "use_depthwise": False,
         "branch_size": 2,
         "data_format": "channels_last",
         "input_shape": (1, 4, 4, 16),
         "output_shape": (1, 4, 4, 16),
         "num_trainable_weights": 11,
         "num_non_trainable_weights": 8,
     },
     {
         "filters": 16,
         "kernel_size": 3,
         "has_skip": True,
+        "has_scale": True,
         "use_depthwise": True,
         "branch_size": 3,
         "data_format": "channels_last",
         "input_shape": (1, 4, 4, 16),
         "output_shape": (1, 4, 4, 16),
         "num_trainable_weights": 14,
         "num_non_trainable_weights": 10,
     },
     {
         "filters": 16,
         "kernel_size": 3,
         "has_skip": False,
+        "has_scale": True,
         "use_depthwise": False,
         "branch_size": 2,
         "data_format": "channels_last",
         "input_shape": (1, 4, 4, 8),
         "output_shape": (1, 4, 4, 16),
         "num_trainable_weights": 9,
         "num_non_trainable_weights": 6,
     },
     {
         "filters": 16,
         "kernel_size": 5,
         "has_skip": True,
+        "has_scale": True,
         "use_depthwise": False,
         "branch_size": 2,
         "data_format": "channels_last",
         "input_shape": (1, 4, 4, 16),
         "output_shape": (1, 4, 4, 16),
         "num_trainable_weights": 11,
         "num_non_trainable_weights": 8,
     },
     {
         "filters": 16,
         "kernel_size": 3,
         "has_skip": True,
+        "has_scale": True,
         "use_depthwise": False,
         "branch_size": 2,
         "data_format": "channels_first",
         "input_shape": (1, 16, 4, 4),
         "output_shape": (1, 16, 4, 4),
         "num_trainable_weights": 11,
         "num_non_trainable_weights": 8,
     },
+    {
+        "filters": 16,
+        "kernel_size": 1,
+        "has_skip": True,
+        "has_scale": False,
+        "use_depthwise": False,
+        "branch_size": 2,
+        "data_format": "channels_last",
+        "input_shape": (1, 4, 4, 16),
+        "output_shape": (1, 4, 4, 16),
+        "num_trainable_weights": 8,
+        "num_non_trainable_weights": 6,
+    },
+    {
+        "filters": 16,
+        "kernel_size": 1,
+        "has_skip": False,
+        "has_scale": False,
+        "use_depthwise": True,
+        "branch_size": 3,
+        "data_format": "channels_last",
+        "input_shape": (1, 4, 4, 16),
+        "output_shape": (1, 4, 4, 16),
+        "num_trainable_weights": 9,
+        "num_non_trainable_weights": 6,
+    },
 ]
 
 
-class MobileOneConv2DTest(testing.TestCase, parameterized.TestCase):
+class ReparameterizableConv2DTest(testing.TestCase, parameterized.TestCase):
     @parameterized.parameters(TEST_CASES)
     @pytest.mark.requires_trainable_backend
     def test_basic(
         self,
         filters,
         kernel_size,
         has_skip,
+        has_scale,
         use_depthwise,
         branch_size,
         data_format,
         input_shape,
         output_shape,
         num_trainable_weights,
         num_non_trainable_weights,
@@ -91,19 +123,20 @@
             and data_format == "channels_first"
         ):
             self.skipTest(
                 "Conv2D in tensorflow backend with 'channels_first' is limited "
                 "to be supported"
             )
         self.run_layer_test(
-            MobileOneConv2D,
+            ReparameterizableConv2D,
             init_kwargs={
                 "filters": filters,
                 "kernel_size": kernel_size,
                 "has_skip": has_skip,
+                "has_scale": has_scale,
                 "use_depthwise": use_depthwise,
                 "branch_size": branch_size,
                 "data_format": data_format,
             },
             input_shape=input_shape,
             expected_output_shape=output_shape,
             expected_num_trainable_weights=num_trainable_weights,
@@ -114,14 +147,15 @@
 
     @parameterized.parameters(TEST_CASES)
     def test_get_reparameterized_weights(
         self,
         filters,
         kernel_size,
         has_skip,
+        has_scale,
         use_depthwise,
         branch_size,
         data_format,
         input_shape,
         output_shape,
         num_trainable_weights,
         num_non_trainable_weights,
@@ -130,35 +164,50 @@
             backend.backend() == "tensorflow"
             and data_format == "channels_first"
         ):
             self.skipTest(
                 "Conv2D in tensorflow backend with 'channels_first' is limited "
                 "to be supported"
             )
-        layer = MobileOneConv2D(
+        layer = ReparameterizableConv2D(
             filters=filters,
             kernel_size=kernel_size,
             has_skip=has_skip,
+            has_scale=has_scale,
             use_depthwise=use_depthwise,
             branch_size=branch_size,
             data_format=data_format,
         )
         layer.build(input_shape)
-        reparameterized_layer = MobileOneConv2D(
+        reparameterized_layer = ReparameterizableConv2D(
             filters=filters,
             kernel_size=kernel_size,
             has_skip=has_skip,
+            has_scale=has_scale,
             use_depthwise=use_depthwise,
             branch_size=branch_size,
             reparameterized=True,
             data_format=data_format,
         )
         reparameterized_layer.build(input_shape)
         x = random.uniform(input_shape)
 
         kernel, bias = layer.get_reparameterized_weights()
-        reparameterized_layer.rep_conv2d.kernel.assign(kernel)
-        reparameterized_layer.rep_conv2d.bias.assign(bias)
+        reparameterized_layer.reparameterized_conv2d.kernel.assign(kernel)
+        reparameterized_layer.reparameterized_conv2d.bias.assign(bias)
         y1 = layer(x, training=False)
         y2 = reparameterized_layer(x, training=False)
 
         self.assertAllClose(y1, y2, atol=1e-3)
+
+    def test_invalid_args(self):
+        layer = ReparameterizableConv2D(
+            filters=4,
+            kernel_size=3,
+            has_skip=False,
+            has_scale=False,
+            use_depthwise=True,
+            branch_size=1,
+            data_format="channels_last",
+        )
+        with self.assertRaisesRegex(ValueError, "must be the same as"):
+            layer.build([1, 4, 4, 8])
```

### Comparing `kimm-0.2.1/kimm/_src/layers/position_embedding.py` & `kimm-0.2.2/kimm/_src/layers/position_embedding.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/layers/position_embedding_test.py` & `kimm-0.2.2/kimm/_src/layers/position_embedding_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/__init__.py` & `kimm-0.2.2/kimm/_src/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from kimm._src.models import convmixer
 from kimm._src.models import convnext
 from kimm._src.models import densenet
 from kimm._src.models import efficientnet
 from kimm._src.models import ghostnet
+from kimm._src.models import ghostnet_v3
 from kimm._src.models import hgnet
 from kimm._src.models import inception_next
 from kimm._src.models import inception_v3
 from kimm._src.models import mobilenet_v2
 from kimm._src.models import mobilenet_v3
 from kimm._src.models import mobileone
 from kimm._src.models import mobilevit
```

### Comparing `kimm-0.2.1/kimm/_src/models/base_model.py` & `kimm-0.2.2/kimm/_src/models/base_model.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/convmixer.py` & `kimm-0.2.2/kimm/_src/models/convmixer.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/convnext.py` & `kimm-0.2.2/kimm/_src/models/convnext.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/densenet.py` & `kimm-0.2.2/kimm/_src/models/densenet.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/efficientnet.py` & `kimm-0.2.2/kimm/_src/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/ghostnet.py` & `kimm-0.2.2/kimm/_src/models/ghostnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,25 +427,25 @@
             weights=weights,
             name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
-class GhostNet050(GhostNetVariant):
+class GhostNetW050(GhostNetVariant):
     available_weights = []
 
     # Parameters
     width = 0.5
     config = "default"
     version = "v1"
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
-class GhostNet100(GhostNetVariant):
+class GhostNetW100(GhostNetVariant):
     available_weights = [
         (
             "imagenet",
             GhostNet.default_origin,
             "ghostnet100_ghostnet_100.keras",
         )
     ]
@@ -453,25 +453,25 @@
     # Parameters
     width = 1.0
     config = "default"
     version = "v1"
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
-class GhostNet130(GhostNetVariant):
+class GhostNetW130(GhostNetVariant):
     available_weights = []
 
     # Parameters
     width = 1.3
     config = "default"
     version = "v1"
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
-class GhostNet100V2(GhostNetVariant):
+class GhostNetV2W100(GhostNetVariant):
     available_weights = [
         (
             "imagenet",
             GhostNet.default_origin,
             "ghostnet100v2_ghostnetv2_100.keras",
         )
     ]
@@ -479,15 +479,15 @@
     # Parameters
     width = 1.0
     config = "default"
     version = "v2"
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
-class GhostNet130V2(GhostNetVariant):
+class GhostNetV2W130(GhostNetVariant):
     available_weights = [
         (
             "imagenet",
             GhostNet.default_origin,
             "ghostnet130v2_ghostnetv2_130.keras",
         )
     ]
@@ -495,28 +495,28 @@
     # Parameters
     width = 1.3
     config = "default"
     version = "v2"
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
-class GhostNet160V2(GhostNetVariant):
+class GhostNetV2W160(GhostNetVariant):
     available_weights = [
         (
             "imagenet",
             GhostNet.default_origin,
             "ghostnet160v2_ghostnetv2_160.keras",
         )
     ]
 
     # Parameters
     width = 1.6
     config = "default"
     version = "v2"
 
 
-add_model_to_registry(GhostNet050)
-add_model_to_registry(GhostNet100, "imagenet")
-add_model_to_registry(GhostNet130)
-add_model_to_registry(GhostNet100V2, "imagenet")
-add_model_to_registry(GhostNet130V2, "imagenet")
-add_model_to_registry(GhostNet160V2, "imagenet")
+add_model_to_registry(GhostNetW050)
+add_model_to_registry(GhostNetW100, "imagenet")
+add_model_to_registry(GhostNetW130)
+add_model_to_registry(GhostNetV2W100, "imagenet")
+add_model_to_registry(GhostNetV2W130, "imagenet")
+add_model_to_registry(GhostNetV2W160, "imagenet")
```

### Comparing `kimm-0.2.1/kimm/_src/models/hgnet.py` & `kimm-0.2.2/kimm/_src/models/hgnet.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/inception_next.py` & `kimm-0.2.2/kimm/_src/models/inception_next.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/inception_v3.py` & `kimm-0.2.2/kimm/_src/models/inception_v3.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/mobilenet_v2.py` & `kimm-0.2.2/kimm/_src/models/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/mobilenet_v3.py` & `kimm-0.2.2/kimm/_src/models/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/mobileone.py` & `kimm-0.2.2/kimm/_src/models/mobileone.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import typing
 
 import keras
 from keras import backend
 
 from kimm._src.kimm_export import kimm_export
-from kimm._src.layers.mobile_one_conv2d import MobileOneConv2D
+from kimm._src.layers.reparameterizable_conv2d import ReparameterizableConv2D
 from kimm._src.models.base_model import BaseModel
 from kimm._src.utils.model_registry import add_model_to_registry
 
 
 @keras.saving.register_keras_serializable(package="kimm")
 class MobileOne(BaseModel):
+    # Updated weights: use ReparameterizableConv2D
+    default_origin = "https://github.com/james77777778/keras-image-models/releases/download/0.1.2/"
     available_feature_keys = [
         "STEM_S2",
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
     ]
 
     def __init__(
         self,
@@ -49,19 +51,20 @@
 
         x = self.build_preprocessing(x, "imagenet")
 
         # Prepare feature extraction
         features = {}
 
         # stem
-        x = MobileOneConv2D(
+        x = ReparameterizableConv2D(
             stem_channels,
             3,
             2,
             has_skip=False,
+            branch_size=1,
             reparameterized=reparameterized,
             activation="relu",
             name="stem",
         )(x)
         features["STEM_S2"] = x
 
         # stages
@@ -77,31 +80,32 @@
                 strides = strides if current_block_idx == 0 else 1
                 input_channels = x.shape[channels_axis]
                 has_skip1 = strides == 1
                 has_skip2 = input_channels == c
                 name1 = f"stages_{current_stage_idx}_{current_block_idx}"
                 name2 = f"stages_{current_stage_idx}_{current_block_idx+1}"
                 # Depthwise
-                x = MobileOneConv2D(
+                x = ReparameterizableConv2D(
                     input_channels,
                     3,
                     strides,
                     has_skip=has_skip1,
                     use_depthwise=True,
                     branch_size=branch_size,
                     reparameterized=reparameterized,
                     activation="relu",
                     name=name1,
                 )(x)
                 # Pointwise
-                x = MobileOneConv2D(
+                x = ReparameterizableConv2D(
                     c,
                     1,
                     1,
                     has_skip=has_skip2,
+                    has_scale=False,
                     use_depthwise=False,
                     branch_size=branch_size,
                     reparameterized=reparameterized,
                     activation="relu",
                     name=name2,
                 )(x)
                 current_block_idx += 2
@@ -146,22 +150,22 @@
         return config
 
     def get_reparameterized_model(self):
         config = self.get_config()
         config["reparameterized"] = True
         config["weights"] = None
         model = MobileOne(**config)
-        for layer, reparameterized_layer in zip(self.layers, model.layers):
+        for layer, rep_layer in zip(self.layers, model.layers):
             if hasattr(layer, "get_reparameterized_weights"):
                 kernel, bias = layer.get_reparameterized_weights()
-                reparameterized_layer.rep_conv2d.kernel.assign(kernel)
-                reparameterized_layer.rep_conv2d.bias.assign(bias)
+                rep_layer.reparameterized_conv2d.kernel.assign(kernel)
+                rep_layer.reparameterized_conv2d.bias.assign(bias)
             else:
                 for weight, target_weight in zip(
-                    layer.weights, reparameterized_layer.weights
+                    layer.weights, rep_layer.weights
                 ):
                     target_weight.assign(weight)
         return model
 
 
 # Model Definition
```

### Comparing `kimm-0.2.1/kimm/_src/models/mobilevit.py` & `kimm-0.2.2/kimm/_src/models/mobilevit.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/models_test.py` & `kimm-0.2.2/kimm/_src/models/models_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,28 +243,40 @@
             ("BLOCK2_S8", [1, 14, 14, make_divisible(40 * 0.51)]),
             ("BLOCK3_S16", [1, 7, 7, make_divisible(80 * 0.51)]),
             ("BLOCK5_S32", [1, 4, 4, make_divisible(192 * 0.51)]),
         ],
     ),
     # ghostnet
     (
-        kimm_models.ghostnet.GhostNet100.__name__,
-        kimm_models.ghostnet.GhostNet100,
+        kimm_models.ghostnet.GhostNetW100.__name__,
+        kimm_models.ghostnet.GhostNetV2W100,
         224,
         [
             ("STEM_S2", [1, 112, 112, 16]),
             ("BLOCK1_S4", [1, 56, 56, 24]),
             ("BLOCK3_S8", [1, 28, 28, 40]),
             ("BLOCK5_S16", [1, 14, 14, 80]),
             ("BLOCK7_S32", [1, 7, 7, 160]),
         ],
     ),
     (
-        kimm_models.ghostnet.GhostNet100V2.__name__,
-        kimm_models.ghostnet.GhostNet100V2,
+        kimm_models.ghostnet.GhostNetV2W100.__name__,
+        kimm_models.ghostnet.GhostNetV2W100,
+        224,
+        [
+            ("STEM_S2", [1, 112, 112, 16]),
+            ("BLOCK1_S4", [1, 56, 56, 24]),
+            ("BLOCK3_S8", [1, 28, 28, 40]),
+            ("BLOCK5_S16", [1, 14, 14, 80]),
+            ("BLOCK7_S32", [1, 7, 7, 160]),
+        ],
+    ),
+    (
+        kimm_models.ghostnet_v3.GhostNetV3W100.__name__,
+        kimm_models.ghostnet_v3.GhostNetV3W100,
         224,
         [
             ("STEM_S2", [1, 112, 112, 16]),
             ("BLOCK1_S4", [1, 56, 56, 24]),
             ("BLOCK3_S8", [1, 28, 28, 40]),
             ("BLOCK5_S16", [1, 14, 14, 80]),
             ("BLOCK7_S32", [1, 7, 7, 160]),
@@ -595,14 +607,19 @@
             # Test correct label is in top 3 (weak correctness test).
             self.assertIn("African_elephant", names[:3])
         elif weights is None:
             self.assertEqual(list(y.shape), [1, 1000])
 
     @parameterized.named_parameters(
         (
+            kimm_models.ghostnet_v3.GhostNetV3W050.__name__,
+            kimm_models.ghostnet_v3.GhostNetV3W050,
+            224,
+        ),
+        (
             kimm_models.repvgg.RepVGGA0.__name__,
             kimm_models.repvgg.RepVGGA0,
             224,
         ),
         (
             kimm_models.mobileone.MobileOneS0.__name__,
             kimm_models.mobileone.MobileOneS0,
```

### Comparing `kimm-0.2.1/kimm/_src/models/regnet.py` & `kimm-0.2.2/kimm/_src/models/regnet.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/repvgg.py` & `kimm-0.2.2/kimm/_src/models/repvgg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import typing
 
 import keras
 from keras import backend
 
 from kimm._src.kimm_export import kimm_export
-from kimm._src.layers.rep_conv2d import RepConv2D
+from kimm._src.layers.reparameterizable_conv2d import ReparameterizableConv2D
 from kimm._src.models.base_model import BaseModel
 from kimm._src.utils.model_registry import add_model_to_registry
 
 
 @keras.saving.register_keras_serializable(package="kimm")
 class RepVGG(BaseModel):
+    # Updated weights: use ReparameterizableConv2D
+    default_origin = "https://github.com/james77777778/keras-image-models/releases/download/0.1.2/"
     available_feature_keys = [
         "STEM_S2",
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
     ]
 
     def __init__(
         self,
@@ -49,19 +51,20 @@
 
         x = self.build_preprocessing(x, "imagenet")
 
         # Prepare feature extraction
         features = {}
 
         # stem
-        x = RepConv2D(
+        x = ReparameterizableConv2D(
             stem_channels,
             3,
             2,
             has_skip=False,
+            branch_size=1,
             reparameterized=reparameterized,
             activation="relu",
             name="stem",
         )(x)
         features["STEM_S2"] = x
 
         # stages
@@ -73,19 +76,20 @@
             current_strides *= strides
             # blocks
             for current_block_idx in range(n):
                 strides = strides if current_block_idx == 0 else 1
                 input_channels = x.shape[channels_axis]
                 has_skip = input_channels == c and strides == 1
                 name = f"stages_{current_stage_idx}_{current_block_idx}"
-                x = RepConv2D(
+                x = ReparameterizableConv2D(
                     c,
                     3,
                     strides,
                     has_skip=has_skip,
+                    branch_size=1,
                     reparameterized=reparameterized,
                     activation="relu",
                     name=name,
                 )(x)
 
             # add feature
             features[f"BLOCK{current_stage_idx}_S{current_strides}"] = x
@@ -124,22 +128,22 @@
         return config
 
     def get_reparameterized_model(self):
         config = self.get_config()
         config["reparameterized"] = True
         config["weights"] = None
         model = RepVGG(**config)
-        for layer, reparameterized_layer in zip(self.layers, model.layers):
+        for layer, rep_layer in zip(self.layers, model.layers):
             if hasattr(layer, "get_reparameterized_weights"):
                 kernel, bias = layer.get_reparameterized_weights()
-                reparameterized_layer.rep_conv2d.kernel.assign(kernel)
-                reparameterized_layer.rep_conv2d.bias.assign(bias)
+                rep_layer.reparameterized_conv2d.kernel.assign(kernel)
+                rep_layer.reparameterized_conv2d.bias.assign(bias)
             else:
                 for weight, target_weight in zip(
-                    layer.weights, reparameterized_layer.weights
+                    layer.weights, rep_layer.weights
                 ):
                     target_weight.assign(weight)
         return model
 
 
 # Model Definition
 
@@ -283,15 +287,15 @@
     # Parameters
     num_blocks = [4, 6, 16, 1]
     num_channels = [160, 320, 640, 2560]
     stem_channels = 64
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.repvgg"])
-class RepVGGB3(RepVGG):
+class RepVGGB3(RepVGGVariant):
     available_weights = [
         (
             "imagenet",
             RepVGG.default_origin,
             "repvggb3_repvgg_b3.rvgg_in1k.keras",
         )
     ]
```

### Comparing `kimm-0.2.1/kimm/_src/models/resnet.py` & `kimm-0.2.2/kimm/_src/models/resnet.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/vgg.py` & `kimm-0.2.2/kimm/_src/models/vgg.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/vision_transformer.py` & `kimm-0.2.2/kimm/_src/models/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/models/xception.py` & `kimm-0.2.2/kimm/_src/models/xception.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/utils/model_registry.py` & `kimm-0.2.2/kimm/_src/utils/model_registry.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/utils/model_registry_test.py` & `kimm-0.2.2/kimm/_src/utils/model_registry_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/utils/model_utils_test.py` & `kimm-0.2.2/kimm/_src/utils/model_utils_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/_src/utils/timm_utils.py` & `kimm-0.2.2/kimm/_src/utils/timm_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
 
 @kimm_export(parent_path=["kimm.timm_utils"])
 def separate_keras_weights(keras_model: keras.Model):
     trainable_weights = []
     non_trainable_weights = []
     for layer in keras_model.layers:
-        if hasattr(layer, "extra_layers"):
-            for sub_layer in layer.extra_layers:
+        if hasattr(layer, "_sublayers"):
+            for sub_layer in layer._sublayers:
                 sub_layer: keras.Layer
                 for weight in sub_layer.trainable_weights:
                     trainable_weights.append(
                         (weight, sub_layer.name + "_" + weight.name)
                     )
                 for weight in sub_layer.non_trainable_weights:
                     non_trainable_weights.append(
```

### Comparing `kimm-0.2.1/kimm/blocks/__init__.py` & `kimm-0.2.2/kimm/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/models/__init__.py` & `kimm-0.2.2/kimm/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,24 @@
 from kimm._src.models.efficientnet import EfficientNetV2S
 from kimm._src.models.efficientnet import EfficientNetV2XL
 from kimm._src.models.efficientnet import TinyNetA
 from kimm._src.models.efficientnet import TinyNetB
 from kimm._src.models.efficientnet import TinyNetC
 from kimm._src.models.efficientnet import TinyNetD
 from kimm._src.models.efficientnet import TinyNetE
-from kimm._src.models.ghostnet import GhostNet050
-from kimm._src.models.ghostnet import GhostNet100
-from kimm._src.models.ghostnet import GhostNet100V2
-from kimm._src.models.ghostnet import GhostNet130
-from kimm._src.models.ghostnet import GhostNet130V2
-from kimm._src.models.ghostnet import GhostNet160V2
+from kimm._src.models.ghostnet import GhostNetV2W100
+from kimm._src.models.ghostnet import GhostNetV2W130
+from kimm._src.models.ghostnet import GhostNetV2W160
+from kimm._src.models.ghostnet import GhostNetW050
+from kimm._src.models.ghostnet import GhostNetW100
+from kimm._src.models.ghostnet import GhostNetW130
+from kimm._src.models.ghostnet_v3 import GhostNetV3W050
+from kimm._src.models.ghostnet_v3 import GhostNetV3W100
+from kimm._src.models.ghostnet_v3 import GhostNetV3W130
+from kimm._src.models.ghostnet_v3 import GhostNetV3W160
 from kimm._src.models.hgnet import HGNetBase
 from kimm._src.models.hgnet import HGNetSmall
 from kimm._src.models.hgnet import HGNetTiny
 from kimm._src.models.hgnet import HGNetV2B0
 from kimm._src.models.hgnet import HGNetV2B1
 from kimm._src.models.hgnet import HGNetV2B2
 from kimm._src.models.hgnet import HGNetV2B3
```

### Comparing `kimm-0.2.1/kimm/models/convnext/__init__.py` & `kimm-0.2.2/kimm/models/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/models/efficientnet/__init__.py` & `kimm-0.2.2/kimm/models/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/models/hgnet/__init__.py` & `kimm-0.2.2/kimm/models/hgnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/models/mobilenet_v3/__init__.py` & `kimm-0.2.2/kimm/models/mobilenet_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/models/mobilevit/__init__.py` & `kimm-0.2.2/kimm/models/mobilevit/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/models/regnet/__init__.py` & `kimm-0.2.2/kimm/models/regnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm/models/vision_transformer/__init__.py` & `kimm-0.2.2/kimm/models/vision_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.1/kimm.egg-info/PKG-INFO` & `kimm-0.2.2/kimm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimm
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Keras model zoo with pretrained weights.
 Author-email: Hong-Yu Chiu <james77777778@gmail.com>
 Maintainer-email: Hong-Yu Chiu <james77777778@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/james77777778/keras-image-models
 Project-URL: Documentation, https://github.com/james77777778/keras-image-models
 Project-URL: Repository, https://github.com/james77777778/keras-image-models.git
@@ -54,25 +54,33 @@
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/kimm/issues)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-image-models/actions.yml?label=tests)](https://github.com/james77777778/keras-image-models/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-image-models/graph/badge.svg?token=eEha1SR80D)](https://codecov.io/gh/james77777778/keras-image-models)
 </div>
 
 # Keras Image Models
 
+- [Latest Updates](#latest-updates)
 - [Introduction](#introduction)
 - [Usage](#usage)
 - [Installation](#installation)
 - [Quickstart](#quickstart)
   - [Image classification with ImageNet weights](#image-classification-using-the-model-pretrained-on-imagenet)
   - [An end-to-end fine-tuning example: cats vs. dogs dataset](#an-end-to-end-example-fine-tuning-an-image-classification-model-on-a-cats-vs-dogs-dataset)
   - [Grad-CAM](#grad-cam)
 - [Model Zoo](#model-zoo)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
 
+## Latest Updates
+
+2024/05/29:
+
+- Merge reparameterizable layers into 1 `ReparameterizableConv2D`
+- Add `GhostNetV3*` from [huawei-noah/Efficient-AI-Backbones](https://github.com/huawei-noah/Efficient-AI-Backbones)
+
 ## Introduction
 
 **K**eras **Im**age **M**odels (`kimm`) is a collection of image models, blocks and layers written in Keras 3. The goal is to offer SOTA models with pretrained weights in a user-friendly manner.
 
 **KIMM** is:
 
 - 🚀 A model zoo where almost all models come with **pre-trained weights on ImageNet**.
@@ -195,14 +203,15 @@
 |ConvNeXt|[CVPR 2022](https://arxiv.org/abs/2201.03545)|`timm`|`kimm.models.ConvNeXt*`|
 |DenseNet|[CVPR 2017](https://arxiv.org/abs/1608.06993)|`timm`|`kimm.models.DenseNet*`|
 |EfficientNet|[ICML 2019](https://arxiv.org/abs/1905.11946)|`timm`|`kimm.models.EfficientNet*`|
 |EfficientNetLite|[ICML 2019](https://arxiv.org/abs/1905.11946)|`timm`|`kimm.models.EfficientNetLite*`|
 |EfficientNetV2|[ICML 2021](https://arxiv.org/abs/2104.00298)|`timm`|`kimm.models.EfficientNetV2*`|
 |GhostNet|[CVPR 2020](https://arxiv.org/abs/1911.11907)|`timm`|`kimm.models.GhostNet*`|
 |GhostNetV2|[NeurIPS 2022](https://arxiv.org/abs/2211.12905)|`timm`|`kimm.models.GhostNetV2*`|
+|GhostNetV3|[arXiv 2024](https://arxiv.org/abs/2404.11202)|`github`|`kimm.models.GhostNetV3*`|
 |HGNet||`timm`|`kimm.models.HGNet*`|
 |HGNetV2||`timm`|`kimm.models.HGNetV2*`|
 |InceptionNeXt|[arXiv 2023](https://arxiv.org/abs/2303.16900)|`timm`|`kimm.models.InceptionNeXt*`|
 |InceptionV3|[CVPR 2016](https://arxiv.org/abs/1512.00567)|`timm`|`kimm.models.InceptionV3`|
 |LCNet|[arXiv 2021](https://arxiv.org/abs/2109.15099)|`timm`|`kimm.models.LCNet*`|
 |MobileNetV2|[CVPR 2018](https://arxiv.org/abs/1801.04381)|`timm`|`kimm.models.MobileNetV2*`|
 |MobileNetV3|[ICCV 2019](https://arxiv.org/abs/1905.02244)|`timm`|`kimm.models.MobileNetV3*`|
```

### Comparing `kimm-0.2.1/kimm.egg-info/SOURCES.txt` & `kimm-0.2.2/kimm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,26 @@
 kimm/_src/layers/__init__.py
 kimm/_src/layers/attention.py
 kimm/_src/layers/attention_test.py
 kimm/_src/layers/layer_scale.py
 kimm/_src/layers/layer_scale_test.py
 kimm/_src/layers/learnable_affine.py
 kimm/_src/layers/learnable_affine_test.py
-kimm/_src/layers/mobile_one_conv2d.py
-kimm/_src/layers/mobile_one_conv2d_test.py
 kimm/_src/layers/position_embedding.py
 kimm/_src/layers/position_embedding_test.py
-kimm/_src/layers/rep_conv2d.py
-kimm/_src/layers/rep_conv2d_test.py
+kimm/_src/layers/reparameterizable_conv2d.py
+kimm/_src/layers/reparameterizable_conv2d_test.py
 kimm/_src/models/__init__.py
 kimm/_src/models/base_model.py
 kimm/_src/models/convmixer.py
 kimm/_src/models/convnext.py
 kimm/_src/models/densenet.py
 kimm/_src/models/efficientnet.py
 kimm/_src/models/ghostnet.py
+kimm/_src/models/ghostnet_v3.py
 kimm/_src/models/hgnet.py
 kimm/_src/models/inception_next.py
 kimm/_src/models/inception_v3.py
 kimm/_src/models/mobilenet_v2.py
 kimm/_src/models/mobilenet_v3.py
 kimm/_src/models/mobileone.py
 kimm/_src/models/mobilevit.py
```

### Comparing `kimm-0.2.1/pyproject.toml` & `kimm-0.2.2/pyproject.toml`

 * *Files identical despite different names*

