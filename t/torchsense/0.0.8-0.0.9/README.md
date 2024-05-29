# Comparing `tmp/torchsense-0.0.8.tar.gz` & `tmp/torchsense-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchsense-0.0.8.tar", last modified: Mon May 20 06:25:05 2024, max compression
+gzip compressed data, was "torchsense-0.0.9.tar", last modified: Tue May 21 13:47:48 2024, max compression
```

## Comparing `torchsense-0.0.8.tar` & `torchsense-0.0.9.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.269107 torchsense-0.0.8/
--rw-rw-rw-   0        0        0     3568 2024-05-13 12:22:11.000000 torchsense-0.0.8/.gitignore
--rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1665 2024-05-20 06:25:05.267572 torchsense-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3904 2024-05-19 05:12:15.000000 torchsense-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.097691 torchsense-0.0.8/examples/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.079020 torchsense-0.0.8/examples/data1/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.079020 torchsense-0.0.8/examples/data1/hsm/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.127019 torchsense-0.0.8/examples/data1/hsm/1/
--rw-rw-rw-   0        0        0   696720 2024-04-30 08:25:03.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-1.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:32.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-10.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:32.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-2.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:33.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-3.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:33.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-4.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:34.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-5.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:34.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-6.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:35.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-7.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:35.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-8.mat
--rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:36.000000 torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-9.mat
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.080675 torchsense-0.0.8/examples/data2/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.131053 torchsense-0.0.8/examples/data2/1/
--rw-rw-rw-   0        0        0   361310 2024-05-12 13:57:33.000000 torchsense-0.0.8/examples/data2/1/test.mat
--rw-rw-rw-   0        0        0   361310 2024-05-12 13:57:33.000000 torchsense-0.0.8/examples/data2/1/test2.mat
--rw-rw-rw-   0        0        0     1420 2024-05-19 08:54:22.000000 torchsense-0.0.8/examples/run.py
--rw-rw-rw-   0        0        0     7646 2024-05-15 11:15:43.000000 torchsense-0.0.8/examples/train_fabric.py
--rw-rw-rw-   0        0        0      573 2024-05-20 06:25:00.000000 torchsense-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 06:25:05.269619 torchsense-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.134711 torchsense-0.0.8/tests/
--rw-rw-rw-   0        0        0     1445 2024-05-15 16:08:03.000000 torchsense-0.0.8/tests/test_model.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.136914 torchsense-0.0.8/torchsense/
--rw-rw-rw-   0        0        0        2 2024-05-16 08:20:27.000000 torchsense-0.0.8/torchsense/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.158340 torchsense-0.0.8/torchsense/datasets/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.8/torchsense/datasets/__init__.py
--rw-rw-rw-   0        0        0     4811 2024-05-18 11:16:08.000000 torchsense-0.0.8/torchsense/datasets/custom.py
--rw-rw-rw-   0        0        0     5076 2024-05-13 11:17:11.000000 torchsense-0.0.8/torchsense/datasets/dataset2.py
--rw-rw-rw-   0        0        0    11317 2024-05-18 15:57:09.000000 torchsense-0.0.8/torchsense/datasets/folder.py
--rw-rw-rw-   0        0        0     3433 2024-05-18 11:28:37.000000 torchsense-0.0.8/torchsense/datasets/utils.py
--rw-rw-rw-   0        0        0     4344 2024-05-18 09:04:23.000000 torchsense-0.0.8/torchsense/datasets/vision.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.237676 torchsense-0.0.8/torchsense/models/
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/Autoencode.py
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/Autoencoder.py
--rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/LSTM.py
--rw-rw-rw-   0        0        0      177 2024-05-19 14:11:42.000000 torchsense-0.0.8/torchsense/models/__init__.py
--rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/alexnet.py
--rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/attention.py
--rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/cct.py
--rw-rw-rw-   0        0        0      780 2024-05-15 11:05:37.000000 torchsense-0.0.8/torchsense/models/cnn4.py
--rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/deeplab.py
--rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/deeplabv3p.py
--rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/densenet.py
--rw-rw-rw-   0        0        0    11223 2024-05-17 10:48:08.000000 torchsense-0.0.8/torchsense/models/gan_g.py
--rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/googlenet.py
--rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/inceptionv3.py
--rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/inceptionv4.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.245162 torchsense-0.0.8/torchsense/models/lit_model/
--rw-rw-rw-   0        0        0      215 2024-05-17 13:37:52.000000 torchsense-0.0.8/torchsense/models/lit_model/__init__.py
--rw-rw-rw-   0        0        0     2345 2024-05-15 11:39:31.000000 torchsense-0.0.8/torchsense/models/lit_model/lit_classify.py
--rw-rw-rw-   0        0        0     2356 2024-05-19 14:11:42.000000 torchsense-0.0.8/torchsense/models/lit_model/lit_multimodal.py
--rw-rw-rw-   0        0        0     2347 2024-05-19 13:12:56.000000 torchsense-0.0.8/torchsense/models/lit_model/lit_regression.py
--rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/mobilenet.py
--rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/mobilenetv1.py
--rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/mobilenetv2.py
--rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/mobilenetv3.py
--rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/nasnet.py
--rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/preactresnet.py
--rw-rw-rw-   0        0        0     6796 2024-05-15 16:06:20.000000 torchsense-0.0.8/torchsense/models/resnet.py
--rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/resnext.py
--rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/rir.py
--rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/sealex.py
--rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/senet.py
--rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/shufflenet.py
--rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/shufflenetv2.py
--rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/simple_vit_1d.py
--rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/squeezenet.py
--rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/stochasticdepth.py
--rw-rw-rw-   0        0        0     4170 2024-05-14 01:33:19.000000 torchsense-0.0.8/torchsense/models/unet.py
--rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/vgg.py
--rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/vit.py
--rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/wideresidual.py
--rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.8/torchsense/models/xception.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.248770 torchsense-0.0.8/torchsense/trainer/
--rw-rw-rw-   0        0        0       48 2024-05-13 12:49:15.000000 torchsense-0.0.8/torchsense/trainer/__init__.py
--rw-rw-rw-   0        0        0     2197 2024-05-19 08:54:22.000000 torchsense-0.0.8/torchsense/trainer/trainer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.251856 torchsense-0.0.8/torchsense/transforms/
--rw-rw-rw-   0        0        0      261 2024-05-18 12:25:32.000000 torchsense-0.0.8/torchsense/transforms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.261928 torchsense-0.0.8/torchsense/transforms/augmentations/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.8/torchsense/transforms/augmentations/__init__.py
--rw-rw-rw-   0        0        0      713 2024-05-18 12:32:20.000000 torchsense-0.0.8/torchsense/transforms/augmentations/interpolate.py
--rw-rw-rw-   0        0        0      612 2024-05-18 11:19:22.000000 torchsense-0.0.8/torchsense/transforms/augmentations/normalize.py
--rw-rw-rw-   0        0        0      800 2024-05-18 11:31:59.000000 torchsense-0.0.8/torchsense/transforms/augmentations/to_tensor.py
--rw-rw-rw-   0        0        0      379 2024-05-18 12:29:31.000000 torchsense-0.0.8/torchsense/transforms/augmentations/utils.py
--rw-rw-rw-   0        0        0     6047 2024-05-18 07:44:50.000000 torchsense-0.0.8/torchsense/transforms/compose.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.263467 torchsense-0.0.8/torchsense/utils/
--rw-rw-rw-   0        0        0        0 2024-05-13 11:12:46.000000 torchsense-0.0.8/torchsense/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:25:05.265516 torchsense-0.0.8/torchsense.egg-info/
--rw-rw-rw-   0        0        0     1665 2024-05-20 06:25:04.000000 torchsense-0.0.8/torchsense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3229 2024-05-20 06:25:05.000000 torchsense-0.0.8/torchsense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 06:25:04.000000 torchsense-0.0.8/torchsense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 06:25:04.000000 torchsense-0.0.8/torchsense.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 06:25:04.000000 torchsense-0.0.8/torchsense.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.992769 torchsense-0.0.9/
+-rw-rw-rw-   0        0        0     3568 2024-05-13 12:22:11.000000 torchsense-0.0.9/.gitignore
+-rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1665 2024-05-21 13:47:48.991765 torchsense-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3904 2024-05-19 05:12:15.000000 torchsense-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.847914 torchsense-0.0.9/examples/
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.830933 torchsense-0.0.9/examples/data1/
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.832440 torchsense-0.0.9/examples/data1/hsm/
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.878507 torchsense-0.0.9/examples/data1/hsm/1/
+-rw-rw-rw-   0        0        0   696720 2024-04-30 08:25:03.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-1.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:32.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-10.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:32.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-2.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:33.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-3.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:33.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-4.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:34.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-5.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:34.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-6.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:35.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-7.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:35.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-8.mat
+-rw-rw-rw-   0        0        0   696720 2024-05-08 16:01:36.000000 torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-9.mat
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.833440 torchsense-0.0.9/examples/data2/
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.883520 torchsense-0.0.9/examples/data2/1/
+-rw-rw-rw-   0        0        0   361310 2024-05-12 13:57:33.000000 torchsense-0.0.9/examples/data2/1/test.mat
+-rw-rw-rw-   0        0        0   361310 2024-05-12 13:57:33.000000 torchsense-0.0.9/examples/data2/1/test2.mat
+-rw-rw-rw-   0        0        0     2037 2024-05-21 13:28:57.000000 torchsense-0.0.9/examples/run.py
+-rw-rw-rw-   0        0        0     7646 2024-05-15 11:15:43.000000 torchsense-0.0.9/examples/train_fabric.py
+-rw-rw-rw-   0        0        0      573 2024-05-21 13:47:42.000000 torchsense-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:47:48.993817 torchsense-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.886529 torchsense-0.0.9/tests/
+-rw-rw-rw-   0        0        0     1445 2024-05-15 16:08:03.000000 torchsense-0.0.9/tests/test_model.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.888534 torchsense-0.0.9/torchsense/
+-rw-rw-rw-   0        0        0        2 2024-05-16 08:20:27.000000 torchsense-0.0.9/torchsense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.903467 torchsense-0.0.9/torchsense/datasets/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.9/torchsense/datasets/__init__.py
+-rw-rw-rw-   0        0        0     6491 2024-05-21 13:03:43.000000 torchsense-0.0.9/torchsense/datasets/custom.py
+-rw-rw-rw-   0        0        0    11317 2024-05-18 15:57:09.000000 torchsense-0.0.9/torchsense/datasets/folder.py
+-rw-rw-rw-   0        0        0     3437 2024-05-21 08:37:00.000000 torchsense-0.0.9/torchsense/datasets/utils.py
+-rw-rw-rw-   0        0        0     4344 2024-05-18 09:04:23.000000 torchsense-0.0.9/torchsense/datasets/vision.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.962419 torchsense-0.0.9/torchsense/models/
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/Autoencode.py
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/Autoencoder.py
+-rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/LSTM.py
+-rw-rw-rw-   0        0        0      177 2024-05-19 14:11:42.000000 torchsense-0.0.9/torchsense/models/__init__.py
+-rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/alexnet.py
+-rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/attention.py
+-rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/cct.py
+-rw-rw-rw-   0        0        0      780 2024-05-15 11:05:37.000000 torchsense-0.0.9/torchsense/models/cnn4.py
+-rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/deeplab.py
+-rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/deeplabv3p.py
+-rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/densenet.py
+-rw-rw-rw-   0        0        0    11223 2024-05-17 10:48:08.000000 torchsense-0.0.9/torchsense/models/gan_g.py
+-rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/googlenet.py
+-rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/inceptionv3.py
+-rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/inceptionv4.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.969153 torchsense-0.0.9/torchsense/models/lit_model/
+-rw-rw-rw-   0        0        0      284 2024-05-21 08:07:25.000000 torchsense-0.0.9/torchsense/models/lit_model/__init__.py
+-rw-rw-rw-   0        0        0     2345 2024-05-15 11:39:31.000000 torchsense-0.0.9/torchsense/models/lit_model/lit_classify.py
+-rw-rw-rw-   0        0        0     2356 2024-05-21 12:45:50.000000 torchsense-0.0.9/torchsense/models/lit_model/lit_multimodal.py
+-rw-rw-rw-   0        0        0     2411 2024-05-21 13:27:45.000000 torchsense-0.0.9/torchsense/models/lit_model/lit_regression.py
+-rw-rw-rw-   0        0        0     3548 2024-05-21 12:39:48.000000 torchsense-0.0.9/torchsense/models/lit_model/lit_twostage.py
+-rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/mobilenet.py
+-rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/mobilenetv1.py
+-rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/mobilenetv2.py
+-rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/mobilenetv3.py
+-rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/nasnet.py
+-rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/preactresnet.py
+-rw-rw-rw-   0        0        0     6796 2024-05-15 16:06:20.000000 torchsense-0.0.9/torchsense/models/resnet.py
+-rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/resnext.py
+-rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/rir.py
+-rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/sealex.py
+-rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/senet.py
+-rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/shufflenet.py
+-rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/shufflenetv2.py
+-rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/simple_vit_1d.py
+-rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/squeezenet.py
+-rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/stochasticdepth.py
+-rw-rw-rw-   0        0        0     4170 2024-05-14 01:33:19.000000 torchsense-0.0.9/torchsense/models/unet.py
+-rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/vgg.py
+-rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/vit.py
+-rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/wideresidual.py
+-rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.9/torchsense/models/xception.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.972288 torchsense-0.0.9/torchsense/trainer/
+-rw-rw-rw-   0        0        0       48 2024-05-13 12:49:15.000000 torchsense-0.0.9/torchsense/trainer/__init__.py
+-rw-rw-rw-   0        0        0     2056 2024-05-21 12:34:20.000000 torchsense-0.0.9/torchsense/trainer/trainer.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.975626 torchsense-0.0.9/torchsense/transforms/
+-rw-rw-rw-   0        0        0      541 2024-05-21 12:02:31.000000 torchsense-0.0.9/torchsense/transforms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.986005 torchsense-0.0.9/torchsense/transforms/augmentations/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.9/torchsense/transforms/augmentations/__init__.py
+-rw-rw-rw-   0        0        0     4181 2024-05-21 11:37:17.000000 torchsense-0.0.9/torchsense/transforms/augmentations/griffinlim.py
+-rw-rw-rw-   0        0        0      713 2024-05-18 12:32:20.000000 torchsense-0.0.9/torchsense/transforms/augmentations/interpolate.py
+-rw-rw-rw-   0        0        0      612 2024-05-18 11:19:22.000000 torchsense-0.0.9/torchsense/transforms/augmentations/normalize.py
+-rw-rw-rw-   0        0        0      800 2024-05-18 11:31:59.000000 torchsense-0.0.9/torchsense/transforms/augmentations/to_tensor.py
+-rw-rw-rw-   0        0        0     2566 2024-05-21 12:23:35.000000 torchsense-0.0.9/torchsense/transforms/augmentations/utils.py
+-rw-rw-rw-   0        0        0     6047 2024-05-18 07:44:50.000000 torchsense-0.0.9/torchsense/transforms/compose.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.988447 torchsense-0.0.9/torchsense/utils/
+-rw-rw-rw-   0        0        0       60 2024-05-21 08:40:48.000000 torchsense-0.0.9/torchsense/utils/__init__.py
+-rw-rw-rw-   0        0        0      421 2024-05-21 08:40:48.000000 torchsense-0.0.9/torchsense/utils/load_from_ckpt.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:47:48.990656 torchsense-0.0.9/torchsense.egg-info/
+-rw-rw-rw-   0        0        0     1665 2024-05-21 13:47:48.000000 torchsense-0.0.9/torchsense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3326 2024-05-21 13:47:48.000000 torchsense-0.0.9/torchsense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:47:48.000000 torchsense-0.0.9/torchsense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:47:48.000000 torchsense-0.0.9/torchsense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-21 13:47:48.000000 torchsense-0.0.9/torchsense.egg-info/top_level.txt
```

### Comparing `torchsense-0.0.8/.gitignore` & `torchsense-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/LICENSE` & `torchsense-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/PKG-INFO` & `torchsense-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsense
-Version: 0.0.8
+Version: 0.0.9
 Summary: Torchsense is a library for sensor data processing with PyTorch
 Author-email: Xingwei Wang <wxwjkl123@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Xingwei Wang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `torchsense-0.0.8/README.md` & `torchsense-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-1.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-1.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-10.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-10.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-2.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-2.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-3.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-3.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-4.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-4.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-5.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-5.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-6.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-6.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-7.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-7.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-8.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-8.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-9.mat` & `torchsense-0.0.9/examples/data1/hsm/1/A cardboard pattern cut to fit inside holder will help to prevent warping-9.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data2/1/test.mat` & `torchsense-0.0.9/examples/data2/1/test.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/data2/1/test2.mat` & `torchsense-0.0.9/examples/data2/1/test2.mat`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/examples/run.py` & `torchsense-0.0.9/examples/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from torchsense.trainer import Trainer
 from torchsense.datasets.custom import SensorFolder
 from torch.utils.data import DataLoader
-from torchsense.models.gan_g import Generator
+from torchsense.models import Generator, UNet
 from torchsense import transforms as T
-from torchaudio.transforms import Spectrogram
+from torchaudio.transforms import Spectrogram,GriffinLim
+from torchsense.utils import load_from_ckpt
+import torchaudio
 
 
 def train():
     # data part
     data_path = "data1"
     transform1 = T.Compose([
         T.ToTensor(),
@@ -15,27 +17,40 @@
         Spectrogram(n_fft=512, hop_length=160, win_length=256, power=1),
     ])
     transform2 = T.Compose([
         T.ToTensor(),
         T.Interpolate(5000),
         Spectrogram(n_fft=100, hop_length=10, win_length=100, power=1),
     ])
+    target_transform = T.Compose([
+        T.ToTensor(),
+        T.Normalize(-1, 1),
+        Spectrogram(n_fft=512, hop_length=160, win_length=256, power=1),
+    ])
+    stage_transform = T.Compose([
+        # T.Normalize(-1, 1),
+        GriffinLim(n_fft=512, hop_length=160, win_length=256, power=1),
+    ])
+    stage1_model = Generator()
+    pre_model = load_from_ckpt(stage1_model, "epoch=19-val_loss=0.80.ckpt")
     data = SensorFolder(root=data_path,
                         params=(["acc[2]", "mix_mic"], ["mic"]),
+                        # pre_model=pre_model,
+                        # stage_transform=stage_transform,
                         transform=[transform2, transform1],
-                        target_transform=transform1)
+                        target_transform=target_transform)
     train_set, test_set = data.train_test_split(0.5)
     train_loader = DataLoader(train_set, batch_size=1, shuffle=True,
                               drop_last=True, num_workers=0, pin_memory=True)
     val_loader = DataLoader(test_set, batch_size=1, shuffle=False,
                             drop_last=True, num_workers=0)
 
     # model part
-    model = Generator()
 
+    model = Generator()
     # training part
-    trainer = Trainer(model, max_epochs=5, task="m",)
+    trainer = Trainer(model,  max_epochs=5, task="r", )
     trainer.fit(train_loader, val_loader)
 
 
 if __name__ == "__main__":
     train()
```

### Comparing `torchsense-0.0.8/examples/train_fabric.py` & `torchsense-0.0.9/examples/train_fabric.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/pyproject.toml` & `torchsense-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torchsense"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     {name = "Xingwei Wang", email = "wxwjkl123@gmail.com"},
 ]
 description = "Torchsense is a library for sensor data processing with PyTorch"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `torchsense-0.0.8/tests/test_model.py` & `torchsense-0.0.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/datasets/custom.py` & `torchsense-0.0.9/torchsense/datasets/custom.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .utils import load_file
 from .folder import DatasetFolder
 from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
-
+from torchsense.transforms import (tensor_has_valid_audio_batch_dimension,
+                                   add_audio_batch_dimension, remove_audio_batch_dimension)
 IMG_EXTENSIONS = (".mat", ".jpeg", ".npz")
 
 
 def default_loader(path: str, params: list) -> Any:
     return load_file(path, params)
 
 
@@ -41,14 +42,16 @@
         imgs (list): List of (image path, class_index) tuples
     """
 
     def __init__(
             self,
             root: str,
             params: Tuple[List[str], Optional[List[str]]],
+            pre_model=None,
+            stage_transform: Optional[Callable] = None,
             transform: Union[Optional[Callable], List[Callable]] = None,
             target_transform: Optional[Callable] = None,
             loader: Callable[[str, Any], Any] = default_loader,
             is_valid_file: Optional[Callable[[str], bool]] = None,
             allow_empty: bool = False,
     ):
         super().__init__(
@@ -58,14 +61,46 @@
             IMG_EXTENSIONS if is_valid_file is None else None,
             transform=transform,
             target_transform=target_transform,
             is_valid_file=is_valid_file,
             allow_empty=allow_empty,
         )
         self.imgs = self.samples
+        if pre_model is None:
+            self.pre_model = None
+            self.stage_transform = None
+
+    def __getitem__(self, index: int) -> Tuple[Any, Any, Any]:
+        """
+        Args:
+            index (int): Index
+
+        Returns:
+            tuple: (sample, target) where target is class_index of the target class.
+        """
+        path, labels = self.samples[index]
+        sample, target = self.loader(path, self.params)
+        if len(sample) == 1:
+            sample = sample[0]
+        if len(target) == 1:
+            target = target[0]
+        if self.transform is not None:
+            for i in range(len(self.transform)):
+                sample[i] = self.transform[i](sample[i])
+        if self.pre_model is not None:
+            if tensor_has_valid_audio_batch_dimension(sample):
+                sample = add_audio_batch_dimension(sample)
+            stage_out = self.pre_model(tuple(sample))
+            stage_out = remove_audio_batch_dimension(stage_out)
+            if self.stage_transform is not None:
+                sample = self.stage_transform(stage_out)
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return sample, target, labels
 
 
 class AudioFolder(DatasetFolder):
     """A generic data1 loader where the images are arranged in this way by default: ::
 
         root/dog/xxx.png
         root/dog/xxy.png
@@ -96,14 +131,16 @@
         imgs (list): List of (image path, class_index) tuples
     """
 
     def __init__(
             self,
             root: str,
             params: Tuple[List[str], Optional[List[str]]] = None,
+            pre_model=None,
+            stage_transform: Optional[Callable] = None,
             transform: Optional[Callable] = None,
             target_transform: Optional[Callable] = None,
             loader: Callable[[str, Any], Any] = default_loader,
             is_valid_file: Optional[Callable[[str], bool]] = None,
             allow_empty: bool = False,
     ):
         super().__init__(
@@ -113,7 +150,9 @@
             IMG_EXTENSIONS if is_valid_file is None else None,
             transform=transform,
             target_transform=target_transform,
             is_valid_file=is_valid_file,
             allow_empty=allow_empty,
         )
         self.imgs = self.samples
+        self.pre_model = pre_model
+        self.stage_transform = stage_transform
```

### Comparing `torchsense-0.0.8/torchsense/datasets/folder.py` & `torchsense-0.0.9/torchsense/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/datasets/utils.py` & `torchsense-0.0.9/torchsense/datasets/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,11 +104,13 @@
         return input_values, target_values
 
 
 def load_npz_file(path, keys):
     npz_data = np.load(path)
     return tuple(npz_data[key] for key in keys if key in npz_data)
 
+
+
 # 使用示例
 # file_path = 'example.txt'
 # data1 = load_file(file_path)
 # print(data1)
```

### Comparing `torchsense-0.0.8/torchsense/datasets/vision.py` & `torchsense-0.0.9/torchsense/datasets/vision.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/Autoencode.py` & `torchsense-0.0.9/torchsense/models/Autoencode.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/Autoencoder.py` & `torchsense-0.0.9/torchsense/models/Autoencoder.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/LSTM.py` & `torchsense-0.0.9/torchsense/models/LSTM.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/alexnet.py` & `torchsense-0.0.9/torchsense/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/attention.py` & `torchsense-0.0.9/torchsense/models/attention.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/cct.py` & `torchsense-0.0.9/torchsense/models/cct.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/cnn4.py` & `torchsense-0.0.9/torchsense/models/cnn4.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/deeplab.py` & `torchsense-0.0.9/torchsense/models/deeplab.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/deeplabv3p.py` & `torchsense-0.0.9/torchsense/models/deeplabv3p.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/densenet.py` & `torchsense-0.0.9/torchsense/models/densenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/gan_g.py` & `torchsense-0.0.9/torchsense/models/gan_g.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/googlenet.py` & `torchsense-0.0.9/torchsense/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/inceptionv3.py` & `torchsense-0.0.9/torchsense/models/inceptionv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/inceptionv4.py` & `torchsense-0.0.9/torchsense/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/lit_model/lit_classify.py` & `torchsense-0.0.9/torchsense/models/lit_model/lit_classify.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/lit_model/lit_multimodal.py` & `torchsense-0.0.9/torchsense/models/lit_model/lit_multimodal.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def _calculate_loss(self, batch, mode="train"):
         x = tuple(batch[0])
         y = batch[1]
         preds = self.model(x)
 
         loss = self.loss_fn(preds.flatten(), y.flatten())
 
-        self.log("%s_loss" % mode, loss, prog_bar=True, on_step=mode is "train", on_epoch=mode is "val")
+        self.log("%s_loss" % mode, loss, prog_bar=True, on_step=mode == "train", on_epoch=mode == "val")
 
         return loss
 
     def configure_optimizers(self):
         optimizer = optim.AdamW(self.model.parameters(), lr=self.hparams.lr)
         scheduler = optim.lr_scheduler.MultiStepLR(optimizer, milestones=[5, 10], gamma=0.1)
         # optimizer = optim.Adadelta(self.parameters(), lr=self.hparams.lr)
```

### Comparing `torchsense-0.0.8/torchsense/models/lit_model/lit_regression.py` & `torchsense-0.0.9/torchsense/models/lit_model/lit_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,23 @@
         self.model.apply(self.weights_init)
         self.loss_fn = MeanSquaredError()
 
     def forward(self, x: torch.Tensor):
         return self.model(x)
 
     def _calculate_loss(self, batch, mode="train"):
-        x = tuple(batch[0])
+        x = batch[0]
         y = batch[1]
+        if not isinstance(x, torch.Tensor):
+            x = tuple(x)
         preds = self.model(x)
 
         loss = self.loss_fn(preds.flatten(), y.flatten())
 
-        self.log("%s_loss" % mode, loss, prog_bar=True, on_step=mode is "train", on_epoch=mode is "val")
+        self.log("%s_loss" % mode, loss, prog_bar=True, on_step=mode == "train", on_epoch=mode == "val")
 
         return loss
 
     def configure_optimizers(self):
         optimizer = optim.AdamW(self.parameters(), lr=self.hparams.lr)
         scheduler = optim.lr_scheduler.MultiStepLR(optimizer, milestones=[5, 10], gamma=0.1)
         # optimizer = optim.Adadelta(self.parameters(), lr=self.hparams.lr)
```

### Comparing `torchsense-0.0.8/torchsense/models/mobilenet.py` & `torchsense-0.0.9/torchsense/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/mobilenetv1.py` & `torchsense-0.0.9/torchsense/models/mobilenetv1.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/mobilenetv2.py` & `torchsense-0.0.9/torchsense/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/mobilenetv3.py` & `torchsense-0.0.9/torchsense/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/nasnet.py` & `torchsense-0.0.9/torchsense/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/preactresnet.py` & `torchsense-0.0.9/torchsense/models/preactresnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/resnet.py` & `torchsense-0.0.9/torchsense/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/resnext.py` & `torchsense-0.0.9/torchsense/models/resnext.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/rir.py` & `torchsense-0.0.9/torchsense/models/rir.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/rnn.py` & `torchsense-0.0.9/torchsense/models/rnn.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/senet.py` & `torchsense-0.0.9/torchsense/models/senet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/shufflenet.py` & `torchsense-0.0.9/torchsense/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/shufflenetv2.py` & `torchsense-0.0.9/torchsense/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/simple_vit_1d.py` & `torchsense-0.0.9/torchsense/models/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/squeezenet.py` & `torchsense-0.0.9/torchsense/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/stochasticdepth.py` & `torchsense-0.0.9/torchsense/models/stochasticdepth.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/unet.py` & `torchsense-0.0.9/torchsense/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/vgg.py` & `torchsense-0.0.9/torchsense/models/vgg.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/vit.py` & `torchsense-0.0.9/torchsense/models/vit.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/wideresidual.py` & `torchsense-0.0.9/torchsense/models/wideresidual.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/models/xception.py` & `torchsense-0.0.9/torchsense/models/xception.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/trainer/trainer.py` & `torchsense-0.0.9/torchsense/trainer/trainer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-from torchsense.models.lit_model import (LitRegressModel,
-                                         LitClassModel,
-                                         LitMultimodalModel)
+from torchsense.models.lit_model import *
 import lightning as L
 import os
 from lightning.pytorch.callbacks import LearningRateMonitor, ModelCheckpoint
 import torch
 from lightning.pytorch.tuner import Tuner
 
 L.seed_everything(42)
 CHECKPOINT_PATH = os.environ.get("PATH_CHECKPOINT", "saved_models/base")
 print(CHECKPOINT_PATH)
 os.makedirs(CHECKPOINT_PATH, exist_ok=True)
 torch.set_float32_matmul_precision("medium")
 
 
 class Trainer:
-    def __init__(self, model, task="r",
-                 precision="32", max_epochs=5,
-                 accelerator="auto",
+    def __init__(self, model,task="r", precision="32", max_epochs=5,
                  lr=0.001, *args):
         if task == "r":
             self.model = LitRegressModel(model, lr=lr)
         elif task == "c":
             self.model = LitClassModel(model, lr=lr)
         elif task == "m":
             self.model = LitMultimodalModel(model, lr=lr)
+        elif task == "two" or task == "t":
+            self.model = LitTwoStageModel(model, lr=lr)
         else:
             raise ValueError("task must be either 'r' or 'c'")
         self.max_epochs = max_epochs
-        self.accelerator = accelerator
         self.precision = precision
         self.trainer = L.Trainer(
             default_root_dir=CHECKPOINT_PATH,
             precision=self.precision,
-            accelerator=self.accelerator,
+            accelerator="auto",
             max_epochs=self.max_epochs,
             callbacks=[
                 ModelCheckpoint(save_weights_only=True, mode="min", monitor="val_loss",
                                 save_last=True, save_top_k=3, filename='{epoch}-{val_loss:.2f}'),
                 # Save the best checkpoint based on the maximum val_acc recorded. Saves only weights and not optimizer
 
             ], *args,
```

### Comparing `torchsense-0.0.8/torchsense/transforms/augmentations/interpolate.py` & `torchsense-0.0.9/torchsense/transforms/augmentations/interpolate.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/transforms/augmentations/normalize.py` & `torchsense-0.0.9/torchsense/transforms/augmentations/normalize.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/transforms/augmentations/to_tensor.py` & `torchsense-0.0.9/torchsense/transforms/augmentations/to_tensor.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense/transforms/compose.py` & `torchsense-0.0.9/torchsense/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.8/torchsense.egg-info/PKG-INFO` & `torchsense-0.0.9/torchsense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsense
-Version: 0.0.8
+Version: 0.0.9
 Summary: Torchsense is a library for sensor data processing with PyTorch
 Author-email: Xingwei Wang <wxwjkl123@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Xingwei Wang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `torchsense-0.0.8/torchsense.egg-info/SOURCES.txt` & `torchsense-0.0.9/torchsense.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 torchsense.egg-info/PKG-INFO
 torchsense.egg-info/SOURCES.txt
 torchsense.egg-info/dependency_links.txt
 torchsense.egg-info/requires.txt
 torchsense.egg-info/top_level.txt
 torchsense/datasets/__init__.py
 torchsense/datasets/custom.py
-torchsense/datasets/dataset2.py
 torchsense/datasets/folder.py
 torchsense/datasets/utils.py
 torchsense/datasets/vision.py
 torchsense/models/Autoencode.py
 torchsense/models/Autoencoder.py
 torchsense/models/LSTM.py
 torchsense/models/__init__.py
@@ -66,17 +65,20 @@
 torchsense/models/vit.py
 torchsense/models/wideresidual.py
 torchsense/models/xception.py
 torchsense/models/lit_model/__init__.py
 torchsense/models/lit_model/lit_classify.py
 torchsense/models/lit_model/lit_multimodal.py
 torchsense/models/lit_model/lit_regression.py
+torchsense/models/lit_model/lit_twostage.py
 torchsense/trainer/__init__.py
 torchsense/trainer/trainer.py
 torchsense/transforms/__init__.py
 torchsense/transforms/compose.py
 torchsense/transforms/augmentations/__init__.py
+torchsense/transforms/augmentations/griffinlim.py
 torchsense/transforms/augmentations/interpolate.py
 torchsense/transforms/augmentations/normalize.py
 torchsense/transforms/augmentations/to_tensor.py
 torchsense/transforms/augmentations/utils.py
-torchsense/utils/__init__.py
+torchsense/utils/__init__.py
+torchsense/utils/load_from_ckpt.py
```

