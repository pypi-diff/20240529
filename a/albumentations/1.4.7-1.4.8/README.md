# Comparing `tmp/albumentations-1.4.7.tar.gz` & `tmp/albumentations-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albumentations-1.4.7.tar", last modified: Tue May 14 00:43:18 2024, max compression
+gzip compressed data, was "albumentations-1.4.8.tar", last modified: Tue May 28 23:52:26 2024, max compression
```

## Comparing `albumentations-1.4.7.tar` & `albumentations-1.4.8.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.726340 albumentations-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-14 00:43:09.000000 albumentations-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 00:43:09.000000 albumentations-1.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    37567 2024-05-14 00:43:18.726340 albumentations-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35779 2024-05-14 00:43:09.000000 albumentations-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.714340 albumentations-1.4.7/albumentations/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.718340 albumentations-1.4.7/albumentations/augmentations/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.718340 albumentations-1.4.7/albumentations/augmentations/blur/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/blur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/blur/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22830 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/blur/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.718340 albumentations-1.4.7/albumentations/augmentations/crops/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/crops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/crops/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    50508 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/crops/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/domain_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/domain_adaptation_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/augmentations/dropout/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/channel_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/grid_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/mask_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/xy_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    51636 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/augmentations/geometric/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43397 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/resize.py
--rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    80815 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/augmentations/mixing/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/mixing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/mixing/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/mixing/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)   126628 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/check_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/bbox_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/keypoints_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/transforms_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/pytorch/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.726340 albumentations-1.4.7/albumentations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    37567 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-14 00:43:09.000000 albumentations-1.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 00:43:18.726340 albumentations-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-14 00:43:09.000000 albumentations-1.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.726340 albumentations-1.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    40331 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_blur.py
--rw-r--r--   0 runner    (1001) docker     (127)    21637 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    52457 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_functional_cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_functional_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_keypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    38359 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    59111 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.448691 albumentations-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-28 23:52:16.000000 albumentations-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 23:52:16.000000 albumentations-1.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37601 2024-05-28 23:52:26.448691 albumentations-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35779 2024-05-28 23:52:16.000000 albumentations-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.436691 albumentations-1.4.8/albumentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.440691 albumentations-1.4.8/albumentations/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.440691 albumentations-1.4.8/albumentations/augmentations/blur/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/blur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/blur/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/blur/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.440691 albumentations-1.4.8/albumentations/augmentations/crops/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/crops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/crops/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52021 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/crops/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/domain_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/domain_adaptation_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.440691 albumentations-1.4.8/albumentations/augmentations/dropout/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/dropout/channel_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/dropout/coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/dropout/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/dropout/grid_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/dropout/mask_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/dropout/xy_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51901 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.444691 albumentations-1.4.8/albumentations/augmentations/geometric/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/geometric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43920 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/geometric/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/geometric/resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/geometric/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82127 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/geometric/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.444691 albumentations-1.4.8/albumentations/augmentations/mixing/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/mixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/mixing/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/mixing/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130858 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/augmentations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/check_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.444691 albumentations-1.4.8/albumentations/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/bbox_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25637 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/keypoints_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14996 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/transforms_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/core/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.444691 albumentations-1.4.8/albumentations/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/pytorch/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-28 23:52:16.000000 albumentations-1.4.8/albumentations/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.448691 albumentations-1.4.8/albumentations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37601 2024-05-28 23:52:26.000000 albumentations-1.4.8/albumentations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-28 23:52:26.000000 albumentations-1.4.8/albumentations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:52:26.000000 albumentations-1.4.8/albumentations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 23:52:26.000000 albumentations-1.4.8/albumentations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 23:52:26.000000 albumentations-1.4.8/albumentations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-28 23:52:16.000000 albumentations-1.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:52:26.448691 albumentations-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-28 23:52:16.000000 albumentations-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:52:26.448691 albumentations-1.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    40249 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_blur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_check_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50348 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_functional_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_functional_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38359 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66188 2024-05-28 23:52:16.000000 albumentations-1.4.8/tests/test_transforms.py
```

### Comparing `albumentations-1.4.7/LICENSE` & `albumentations-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/PKG-INFO` & `albumentations-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.7
+Version: 1.4.8
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,16 @@
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: PyYAML
 Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: pydantic>=2.7.0
-Requires-Dist: opencv-python-headless>=4.9.0
+Requires-Dist: albucore>=0.0.4
+Requires-Dist: opencv-python-headless>=4.9.0.80
 
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/albumentations.svg?label=PyPI%20downloads)](
 https://pypi.org/project/albumentations/)
```

### Comparing `albumentations-1.4.7/README.md` & `albumentations-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/albumentations/augmentations/__init__.py` & `albumentations-1.4.8/albumentations/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/albumentations/augmentations/blur/functional.py` & `albumentations-1.4.8/albumentations/augmentations/blur/functional.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from itertools import product
 from math import ceil
 from typing import Sequence, Union
 
 import cv2
 import numpy as np
+from albucore.utils import clipped, maybe_process_in_chunks, preserve_channel_dim
 
 from albumentations.augmentations.functional import convolve
 from albumentations.augmentations.geometric.functional import scale
-from albumentations.augmentations.utils import (
-    _maybe_process_in_chunks,
-    clipped,
-    preserve_channel_dim,
-)
 
 __all__ = ["blur", "median_blur", "gaussian_blur", "glass_blur", "defocus", "central_zoom", "zoom_blur"]
 
 TWO = 2
 EIGHT = 8
 
 
 @preserve_channel_dim
 def blur(img: np.ndarray, ksize: int) -> np.ndarray:
-    blur_fn = _maybe_process_in_chunks(cv2.blur, ksize=(ksize, ksize))
+    blur_fn = maybe_process_in_chunks(cv2.blur, ksize=(ksize, ksize))
     return blur_fn(img)
 
 
 @preserve_channel_dim
 def median_blur(img: np.ndarray, ksize: int) -> np.ndarray:
     if img.dtype == np.float32 and ksize not in {3, 5}:
         raise ValueError(f"Invalid ksize value {ksize}. For a float32 image the only valid ksize values are 3 and 5")
 
-    blur_fn = _maybe_process_in_chunks(cv2.medianBlur, ksize=ksize)
+    blur_fn = maybe_process_in_chunks(cv2.medianBlur, ksize=ksize)
     return blur_fn(img)
 
 
 @preserve_channel_dim
 def gaussian_blur(img: np.ndarray, ksize: int, sigma: float = 0) -> np.ndarray:
     # When sigma=0, it is computed as `sigma = 0.3*((ksize-1)*0.5 - 1) + 0.8`
-    blur_fn = _maybe_process_in_chunks(cv2.GaussianBlur, ksize=(ksize, ksize), sigmaX=sigma)
+    blur_fn = maybe_process_in_chunks(cv2.GaussianBlur, ksize=(ksize, ksize), sigmaX=sigma)
     return blur_fn(img)
 
 
 @preserve_channel_dim
 def glass_blur(
     img: np.ndarray,
     sigma: float,
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/blur/transforms.py` & `albumentations-1.4.8/albumentations/augmentations/blur/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 import cv2
 import numpy as np
 from pydantic import Field, ValidationInfo, field_validator, model_validator
 from typing_extensions import Self
 
 from albumentations import random_utils
-from albumentations.augmentations import functional as FMain
+from albumentations.augmentations import functional as fmain
 from albumentations.augmentations.utils import check_range
 from albumentations.core.pydantic import (
     NonNegativeFloatRangeType,
     OnePlusFloatRangeType,
     OnePlusIntRangeType,
     SymmetricRangeType,
 )
 from albumentations.core.transforms_interface import BaseTransformInitSchema, ImageOnlyTransform
 from albumentations.core.types import ScaleFloatType, ScaleIntType
 from albumentations.core.utils import to_tuple
 
-from . import functional as F
+from . import functional as fblur
 
 __all__ = ["Blur", "MotionBlur", "GaussianBlur", "GlassBlur", "AdvancedBlur", "MedianBlur", "Defocus", "ZoomBlur"]
 
 
 HALF = 0.5
 TWO = 2
 
@@ -69,15 +69,15 @@
         pass
 
     def __init__(self, blur_limit: ScaleIntType = 7, always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply, p)
         self.blur_limit = cast(Tuple[int, int], blur_limit)
 
     def apply(self, img: np.ndarray, kernel: int, **params: Any) -> np.ndarray:
-        return F.blur(img, kernel)
+        return fblur.blur(img, kernel)
 
     def get_params(self) -> Dict[str, Any]:
         return {"kernel": random_utils.choice(list(range(self.blur_limit[0], self.blur_limit[1] + 1, 2)))}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("blur_limit",)
 
@@ -130,15 +130,15 @@
         self.allow_shifted = allow_shifted
         self.blur_limit = cast(Tuple[int, int], blur_limit)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (*super().get_transform_init_args_names(), "allow_shifted")
 
     def apply(self, img: np.ndarray, kernel: np.ndarray, **params: Any) -> np.ndarray:
-        return FMain.convolve(img, kernel=kernel)
+        return fmain.convolve(img, kernel=kernel)
 
     def get_params(self) -> Dict[str, Any]:
         ksize = random.choice(list(range(self.blur_limit[0], self.blur_limit[1] + 1, 2)))
         if ksize <= TWO:
             raise ValueError(f"ksize must be > 2. Got: {ksize}")
         kernel = np.zeros((ksize, ksize), dtype=np.uint8)
         x1, x2 = random.randint(0, ksize - 1), random.randint(0, ksize - 1)
@@ -191,15 +191,15 @@
 
     """
 
     def __init__(self, blur_limit: ScaleIntType = 7, always_apply: bool = False, p: float = 0.5):
         super().__init__(blur_limit, always_apply, p)
 
     def apply(self, img: np.ndarray, kernel: int, **params: Any) -> np.ndarray:
-        return F.median_blur(img, kernel)
+        return fblur.median_blur(img, kernel)
 
 
 class GaussianBlur(ImageOnlyTransform):
     """Blur the input image using a Gaussian filter with a random kernel size.
 
     Args:
         blur_limit (int, (int, int)): maximum Gaussian kernel size for blurring the input image.
@@ -236,14 +236,15 @@
                 and isinstance(self.sigma_limit, (tuple, list))
                 and self.sigma_limit[0] == 0
             ):
                 self.blur_limit = 3, max(3, self.blur_limit[1])
                 warnings.warn(
                     "blur_limit and sigma_limit minimum value can not be both equal to 0. "
                     "blur_limit minimum value changed to 3.",
+                    stacklevel=2,
                 )
 
             if isinstance(self.blur_limit, tuple):
                 for v in self.blur_limit:
                     if v != 0 and v % 2 != 1:
                         raise ValueError(f"Blur limit must be 0 or odd. Got: {self.blur_limit}")
 
@@ -257,15 +258,15 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.blur_limit = cast(Tuple[int, int], blur_limit)
         self.sigma_limit = cast(Tuple[float, float], sigma_limit)
 
     def apply(self, img: np.ndarray, ksize: int, sigma: float, **params: Any) -> np.ndarray:
-        return F.gaussian_blur(img, ksize, sigma=sigma)
+        return fblur.gaussian_blur(img, ksize, sigma=sigma)
 
     def get_params(self) -> Dict[str, float]:
         ksize = random.randrange(self.blur_limit[0], self.blur_limit[1] + 1)
         if ksize != 0 and ksize % 2 != 1:
             ksize = (ksize + 1) % (self.blur_limit[1] + 1)
 
         return {"ksize": ksize, "sigma": random.uniform(*self.sigma_limit)}
@@ -319,15 +320,15 @@
         self.mode = mode
 
     def apply(self, img: np.ndarray, *args: Any, dxy: np.ndarray, **params: Any) -> np.ndarray:
         if dxy is None:
             msg = "dxy is None"
             raise ValueError(msg)
 
-        return F.glass_blur(img, self.sigma, self.max_delta, self.iterations, dxy, self.mode)
+        return fblur.glass_blur(img, self.sigma, self.max_delta, self.iterations, dxy, self.mode)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
         img = params["image"]
 
         height, width = img.shape[:2]
 
         # generate array containing all necessary values for transformations
@@ -432,30 +433,30 @@
         noise_limit: ScaleFloatType = (0.9, 1.1),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
 
         if sigmaX_limit is not None:
-            warnings.warn("sigmaX_limit is deprecated; use sigma_x_limit instead.", DeprecationWarning)
+            warnings.warn("sigmaX_limit is deprecated; use sigma_x_limit instead.", DeprecationWarning, stacklevel=2)
             sigma_x_limit = sigmaX_limit
 
         if sigmaY_limit is not None:
-            warnings.warn("sigmaY_limit is deprecated; use sigma_y_limit instead.", DeprecationWarning)
+            warnings.warn("sigmaY_limit is deprecated; use sigma_y_limit instead.", DeprecationWarning, stacklevel=2)
             sigma_y_limit = sigmaY_limit
 
         self.blur_limit = cast(Tuple[int, int], blur_limit)
         self.sigma_x_limit = cast(Tuple[float, float], sigma_x_limit)
         self.sigma_y_limit = cast(Tuple[float, float], sigma_y_limit)
         self.rotate_limit = cast(Tuple[int, int], rotate_limit)
         self.beta_limit = cast(Tuple[float, float], beta_limit)
         self.noise_limit = cast(Tuple[float, float], noise_limit)
 
     def apply(self, img: np.ndarray, kernel: np.ndarray, **params: Any) -> np.ndarray:
-        return FMain.convolve(img, kernel=kernel)
+        return fmain.convolve(img, kernel=kernel)
 
     def get_params(self) -> Dict[str, np.ndarray]:
         ksize = random.randrange(self.blur_limit[0], self.blur_limit[1] + 1, 2)
         sigma_x = random_utils.uniform(*self.sigma_x_limit)
         sigma_y = random_utils.uniform(*self.sigma_y_limit)
         angle = np.deg2rad(random.uniform(*self.rotate_limit))
 
@@ -529,15 +530,15 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.radius = cast(Tuple[int, int], radius)
         self.alias_blur = cast(Tuple[float, float], alias_blur)
 
     def apply(self, img: np.ndarray, radius: int, alias_blur: float, **params: Any) -> np.ndarray:
-        return F.defocus(img, radius, alias_blur)
+        return fblur.defocus(img, radius, alias_blur)
 
     def get_params(self) -> Dict[str, Any]:
         return {
             "radius": random_utils.randint(self.radius[0], self.radius[1] + 1),
             "alias_blur": random_utils.uniform(self.alias_blur[0], self.alias_blur[1]),
         }
 
@@ -579,15 +580,15 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.max_factor = cast(Tuple[float, float], max_factor)
         self.step_factor = cast(Tuple[float, float], step_factor)
 
     def apply(self, img: np.ndarray, zoom_factors: np.ndarray, **params: Any) -> np.ndarray:
-        return F.zoom_blur(img, zoom_factors)
+        return fblur.zoom_blur(img, zoom_factors)
 
     def get_params(self) -> Dict[str, Any]:
         max_factor = random.uniform(self.max_factor[0], self.max_factor[1])
         step_factor = random.uniform(self.step_factor[0], self.step_factor[1])
         return {"zoom_factors": np.arange(1.0, max_factor, step_factor)}
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/crops/functional.py` & `albumentations-1.4.8/albumentations/augmentations/crops/functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from typing import Optional, Sequence, Tuple, cast
 
 import cv2
 import numpy as np
+from albucore.utils import maybe_process_in_chunks, preserve_channel_dim
 
-from albumentations.augmentations.geometric import functional as FGeometric
-from albumentations.augmentations.utils import (
-    _maybe_process_in_chunks,
-    preserve_channel_dim,
-)
+from albumentations.augmentations.geometric import functional as fgeometric
 from albumentations.core.bbox_utils import denormalize_bbox, normalize_bbox
 from albumentations.core.types import BoxInternalType, KeypointInternalType
 
 __all__ = [
     "get_random_crop_coords",
     "random_crop",
     "crop_bbox_by_coords",
@@ -63,28 +60,26 @@
     bbox: BoxInternalType,
     crop_coords: Tuple[int, int, int, int],
     crop_height: int,
     crop_width: int,
     rows: int,
     cols: int,
 ) -> BoxInternalType:
-    """Crop a bounding box using the provided coordinates of bottom-left and top-right corners in pixels and the
-    required height and width of the crop.
+    """Crop a bounding box using the provided coordinates of the crop area and the original image dimensions.
 
     Args:
-        bbox: A cropped box `(x_min, y_min, x_max, y_max)`.
-        crop_coords: Crop coordinates `(x1, y1, x2, y2)`.
-        crop_height:
-        crop_width:
-        rows: Image rows.
-        cols: Image cols.
+        bbox (BoxInternalType): A bounding box in the format `(x_min, y_min, x_max, y_max)`.
+        crop_coords (Tuple[int, int, int, int]): The coordinates of the crop area in the format `(x1, y1, x2, y2)`.
+        crop_height (int): The height of the crop area in pixels.
+        crop_width (int): The width of the crop area in pixels.
+        rows (int): The number of rows (height) in the original image.
+        cols (int): The number of columns (width) in the original image.
 
     Returns:
-        A cropped bounding box `(x_min, y_min, x_max, y_max)`.
-
+        BoxInternalType: A cropped bounding box in the format `(x_min, y_min, x_max, y_max)`.
     """
     normalized_bbox = denormalize_bbox(bbox, rows, cols)
     x_min, y_min, x_max, y_max = normalized_bbox[:4]
     x1, y1 = crop_coords[:2]
     cropped_bbox = x_min - x1, y_min - y1, x_max - x1, y_max - y1
     return cast(BoxInternalType, normalize_bbox(cropped_bbox, crop_height, crop_width))
 
@@ -220,28 +215,27 @@
     x_min: int,
     y_min: int,
     x_max: int,
     y_max: int,
     rows: int,
     cols: int,
 ) -> BoxInternalType:
-    """Crop a bounding box.
+    """Crop a bounding box using the provided coordinates.
 
     Args:
-        bbox: A bounding box `(x_min, y_min, x_max, y_max)`.
-        x_min:
-        y_min:
-        x_max:
-        y_max:
-        rows: Image rows.
-        cols: Image cols.
+        bbox (BoxInternalType): A bounding box in the format `(x_min, y_min, x_max, y_max)`.
+        x_min (int): The minimum x-coordinate of the crop area.
+        y_min (int): The minimum y-coordinate of the crop area.
+        x_max (int): The maximum x-coordinate of the crop area.
+        y_max (int): The maximum y-coordinate of the crop area.
+        rows (int): The number of rows (height) in the original image.
+        cols (int): The number of columns (width) in the original image.
 
     Returns:
-        A cropped bounding box `(x_min, y_min, x_max, y_max)`.
-
+        BoxInternalType: A cropped bounding box in the format `(x_min, y_min, x_max, y_max)`.
     """
     crop_coords = x_min, y_min, x_max, y_max
     crop_height = y_max - y_min
     crop_width = x_max - x_min
     return crop_bbox_by_coords(bbox, crop_coords, crop_height, crop_width, rows, cols)
 
 
@@ -269,26 +263,26 @@
     interpolation: int,
     pad_mode: int,
     keep_size: bool,
 ) -> np.ndarray:
     if crop_params is not None and any(i != 0 for i in crop_params):
         img = crop(img, *crop_params)
     if pad_params is not None and any(i != 0 for i in pad_params):
-        img = FGeometric.pad_with_params(
+        img = fgeometric.pad_with_params(
             img,
             pad_params[0],
             pad_params[1],
             pad_params[2],
             pad_params[3],
             border_mode=pad_mode,
             value=pad_value,
         )
 
     if keep_size:
-        resize_fn = _maybe_process_in_chunks(cv2.resize, dsize=(cols, rows), interpolation=interpolation)
+        resize_fn = maybe_process_in_chunks(cv2.resize, dsize=(cols, rows), interpolation=interpolation)
         return resize_fn(img)
 
     return img
 
 
 def crop_and_pad_bbox(
     bbox: BoxInternalType,
@@ -342,10 +336,10 @@
 
         x += left
         y += top
 
     if keep_size and (result_cols != cols or result_rows != rows):
         scale_x = cols / result_cols
         scale_y = rows / result_rows
-        return FGeometric.keypoint_scale((x, y, angle, scale), scale_x, scale_y)
+        return fgeometric.keypoint_scale((x, y, angle, scale), scale_x, scale_y)
 
     return x, y, angle, scale
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/crops/transforms.py` & `albumentations-1.4.8/albumentations/augmentations/crops/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import math
 import random
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
 from warnings import warn
 
 import cv2
 import numpy as np
-from pydantic import Field, field_validator, model_validator
+from pydantic import AfterValidator, Field, field_validator, model_validator
 from typing_extensions import Annotated, Self
 
 from albumentations import random_utils
-from albumentations.augmentations.geometric import functional as FGeometric
+from albumentations.augmentations.geometric import functional as fgeometric
 from albumentations.core.bbox_utils import union_of_bboxes
 from albumentations.core.pydantic import (
     BorderModeType,
     InterpolationType,
-    NonNegativeFloatRangeType,
     OnePlusIntRangeType,
     ProbabilityType,
     ZeroOneRangeType,
+    check_0plus,
+    check_01,
 )
-from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
+from albumentations.core.transforms_interface import PAIR, BaseTransformInitSchema, DualTransform
 from albumentations.core.types import (
     NUM_MULTI_CHANNEL_DIMENSIONS,
     BoxInternalType,
-    ColorType,
     KeypointInternalType,
+    PercentType,
+    PxType,
+    ScalarType,
     ScaleFloatType,
     ScaleIntType,
     Targets,
 )
 
-from . import functional as F
+from . import functional as fcrops
 
 __all__ = [
     "RandomCrop",
     "CenterCrop",
     "Crop",
     "CropNonEmptyMaskIfExists",
     "RandomSizedCrop",
@@ -42,16 +45,14 @@
     "RandomCropNearBBox",
     "RandomSizedBBoxSafeCrop",
     "CropAndPad",
     "RandomCropFromBorders",
     "BBoxSafeRandomCrop",
 ]
 
-TWO = 2
-
 
 class CropInitSchema(BaseTransformInitSchema):
     height: Optional[int] = Field(description="Height of the crop", ge=1)
     width: Optional[int] = Field(description="Width of the crop", ge=1)
     p: ProbabilityType = 1
 
 
@@ -78,24 +79,24 @@
 
     def __init__(self, height: int, width: int, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.height = height
         self.width = width
 
     def apply(self, img: np.ndarray, h_start: int, w_start: int, **params: Any) -> np.ndarray:
-        return F.random_crop(img, self.height, self.width, h_start, w_start)
+        return fcrops.random_crop(img, self.height, self.width, h_start, w_start)
 
     def get_params(self) -> Dict[str, float]:
         return {"h_start": random.random(), "w_start": random.random()}
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_random_crop(bbox, self.height, self.width, **params)
+        return fcrops.bbox_random_crop(bbox, self.height, self.width, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
-        return F.keypoint_random_crop(keypoint, self.height, self.width, **params)
+        return fcrops.keypoint_random_crop(keypoint, self.height, self.width, **params)
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("height", "width")
 
 
 class CenterCrop(DualTransform):
     """Crop the central part of the input.
@@ -120,21 +121,21 @@
 
     def __init__(self, height: int, width: int, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.height = height
         self.width = width
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        return F.center_crop(img, self.height, self.width)
+        return fcrops.center_crop(img, self.height, self.width)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_center_crop(bbox, self.height, self.width, **params)
+        return fcrops.bbox_center_crop(bbox, self.height, self.width, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
-        return F.keypoint_center_crop(keypoint, self.height, self.width, **params)
+        return fcrops.keypoint_center_crop(keypoint, self.height, self.width, **params)
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("height", "width")
 
 
 class Crop(DualTransform):
     """Crop region from image.
@@ -184,21 +185,21 @@
         super().__init__(always_apply, p)
         self.x_min = x_min
         self.y_min = y_min
         self.x_max = x_max
         self.y_max = y_max
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        return F.crop(img, x_min=self.x_min, y_min=self.y_min, x_max=self.x_max, y_max=self.y_max)
+        return fcrops.crop(img, x_min=self.x_min, y_min=self.y_min, x_max=self.x_max, y_max=self.y_max)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_crop(bbox, x_min=self.x_min, y_min=self.y_min, x_max=self.x_max, y_max=self.y_max, **params)
+        return fcrops.bbox_crop(bbox, x_min=self.x_min, y_min=self.y_min, x_max=self.x_max, y_max=self.y_max, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
-        return F.crop_keypoint_by_coords(keypoint, crop_coords=(self.x_min, self.y_min, self.x_max, self.y_max))
+        return fcrops.crop_keypoint_by_coords(keypoint, crop_coords=(self.x_min, self.y_min, self.x_max, self.y_max))
 
     def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
         return ("x_min", "y_min", "x_max", "y_max")
 
 
 class CropNonEmptyMaskIfExists(DualTransform):
     """Crop area with mask if mask is non-empty, else make random crop.
@@ -250,26 +251,26 @@
         img: np.ndarray,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.crop(img, x_min, y_min, x_max, y_max)
+        return fcrops.crop(img, x_min, y_min, x_max, y_max)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> BoxInternalType:
-        return F.bbox_crop(
+        return fcrops.bbox_crop(
             bbox,
             x_min=x_min,
             x_max=x_max,
             y_min=y_min,
             y_max=y_max,
             rows=params["rows"],
             cols=params["cols"],
@@ -280,15 +281,15 @@
         keypoint: KeypointInternalType,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> KeypointInternalType:
-        return F.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
+        return fcrops.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
 
     def _preprocess_mask(self, mask: np.ndarray) -> np.ndarray:
         mask_height, mask_width = mask.shape[:2]
 
         if self.ignore_values is not None:
             ignore_values_np = np.array(self.ignore_values)
             mask = np.where(np.isin(mask, ignore_values_np), 0, mask)
@@ -376,45 +377,45 @@
         crop_height: int,
         crop_width: int,
         h_start: int,
         w_start: int,
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        crop = F.random_crop(img, crop_height, crop_width, h_start, w_start)
-        return FGeometric.resize(crop, self.size[0], self.size[1], interpolation)
+        crop = fcrops.random_crop(img, crop_height, crop_width, h_start, w_start)
+        return fgeometric.resize(crop, self.size[0], self.size[1], interpolation)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         crop_height: int,
         crop_width: int,
         h_start: int,
         w_start: int,
         rows: int,
         cols: int,
         **params: Any,
     ) -> BoxInternalType:
-        return F.bbox_random_crop(bbox, crop_height, crop_width, h_start, w_start, rows, cols)
+        return fcrops.bbox_random_crop(bbox, crop_height, crop_width, h_start, w_start, rows, cols)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         crop_height: int,
         crop_width: int,
         h_start: int,
         w_start: int,
         rows: int,
         cols: int,
         **params: Any,
     ) -> KeypointInternalType:
-        keypoint = F.keypoint_random_crop(keypoint, crop_height, crop_width, h_start, w_start, rows, cols)
+        keypoint = fcrops.keypoint_random_crop(keypoint, crop_height, crop_width, h_start, w_start, rows, cols)
         scale_y = self.size[0] / crop_height
         scale_x = self.size[1] / crop_width
-        return FGeometric.keypoint_scale(keypoint, scale_x, scale_y)
+        return fgeometric.keypoint_scale(keypoint, scale_x, scale_y)
 
 
 class RandomSizedCrop(_BaseRandomSizedCrop):
     """Crop a random portion of the input and rescale it to a specific size.
 
     Args:
         min_max_height ((int, int)): crop size limits.
@@ -521,21 +522,23 @@
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     class InitSchema(BaseTransformInitSchema):
-        scale: ZeroOneRangeType = (0.08, 1.0)
-        ratio: NonNegativeFloatRangeType = (0.75, 1.3333333333333333)
+        scale: Annotated[Tuple[float, float], AfterValidator(check_01)] = (0.08, 1.0)
+        ratio: Annotated[Tuple[float, float], AfterValidator(check_0plus)] = (0.75, 1.3333333333333333)
         width: Optional[int] = Field(
-            None, deprecated="Initializing with 'height' and 'width' is deprecated. Use size instead."
+            None,
+            deprecated="Initializing with 'height' and 'width' is deprecated. Use size instead.",
         )
         height: Optional[int] = Field(
-            None, deprecated="Initializing with 'height' and 'width' is deprecated. Use size instead."
+            None,
+            deprecated="Initializing with 'height' and 'width' is deprecated. Use size instead.",
         )
         size: Optional[ScaleIntType] = None
         p: ProbabilityType = 1
         interpolation: InterpolationType = cv2.INTER_LINEAR
 
         @model_validator(mode="after")
         def process(self) -> Self:
@@ -685,15 +688,15 @@
         img: np.ndarray,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.clamping_crop(img, x_min, y_min, x_max, y_max)
+        return fcrops.clamping_crop(img, x_min, y_min, x_max, y_max)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, int]:
         bbox = params[self.cropping_bbox_key]
         h_max_shift = round((bbox[3] - bbox[1]) * self.max_part_shift[0])
         w_max_shift = round((bbox[2] - bbox[0]) * self.max_part_shift[1])
 
         x_min = bbox[0] - random.randint(-w_max_shift, w_max_shift)
@@ -704,26 +707,26 @@
 
         x_min = max(0, x_min)
         y_min = max(0, y_min)
 
         return {"x_min": x_min, "x_max": x_max, "y_min": y_min, "y_max": y_max}
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_crop(bbox, **params)
+        return fcrops.bbox_crop(bbox, **params)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> KeypointInternalType:
-        return F.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
+        return fcrops.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
 
     @property
     def targets_as_params(self) -> List[str]:
         return [self.cropping_bbox_key]
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("max_part_shift", "cropping_bbox_key")
@@ -762,15 +765,15 @@
         img: np.ndarray,
         crop_height: int,
         crop_width: int,
         h_start: int,
         w_start: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.random_crop(img, crop_height, crop_width, h_start, w_start)
+        return fcrops.random_crop(img, crop_height, crop_width, h_start, w_start)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Union[int, float]]:
         img_h, img_w = params["image"].shape[:2]
         if len(params["bboxes"]) == 0:  # less likely, this class is for use with bboxes.
             erosive_h = int(img_h * (1.0 - self.erosion_rate))
             crop_height = img_h if erosive_h >= img_h else random.randint(erosive_h, img_h)
             return {
@@ -803,23 +806,32 @@
         crop_width: int,
         h_start: int,
         w_start: int,
         rows: int,
         cols: int,
         **params: Any,
     ) -> BoxInternalType:
-        return F.bbox_random_crop(bbox, crop_height, crop_width, h_start, w_start, rows, cols)
+        return fcrops.bbox_random_crop(bbox, crop_height, crop_width, h_start, w_start, rows, cols)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image", "bboxes"]
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("erosion_rate",)
 
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+            "bboxes": self.apply_to_bboxes,
+        }
+
 
 class RandomSizedBBoxSafeCrop(BBoxSafeRandomCrop):
     """Crop a random part of the input and rescale it to some size without loss of bboxes.
 
     Args:
         height: height after crop and resize.
         width: width after crop and resize.
@@ -865,123 +877,133 @@
         img: np.ndarray,
         crop_height: int,
         crop_width: int,
         h_start: int,
         w_start: int,
         **params: Any,
     ) -> np.ndarray:
-        crop = F.random_crop(img, crop_height, crop_width, h_start, w_start)
-        return FGeometric.resize(crop, self.height, self.width, self.interpolation)
+        crop = fcrops.random_crop(img, crop_height, crop_width, h_start, w_start)
+        return fgeometric.resize(crop, self.height, self.width, self.interpolation)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (*super().get_transform_init_args_names(), "height", "width", "interpolation")
 
 
 class CropAndPad(DualTransform):
     """Crop and pad images by pixel amounts or fractions of image sizes.
-    Cropping removes pixels at the sides (i.e. extracts a subimage from a given full image).
-    Padding adds pixels to the sides (e.g. black pixels).
-    This transformation will never crop images below a height or width of ``1``.
+    Cropping removes pixels at the sides (i.e., extracts a subimage from a given full image).
+    Padding adds pixels to the sides (e.g., black pixels).
+    This transformation will never crop images below a height or width of 1.
 
     Note:
         This transformation automatically resizes images back to their original size. To deactivate this, add the
-        parameter ``keep_size=False``.
+        parameter `keep_size=False`.
 
     Args:
-        px (int or tuple):
-            The number of pixels to crop (negative values) or pad (positive values)
-            on each side of the image. Either this or the parameter `percent` may
-            be set, not both at the same time.
-                * If ``None``, then pixel-based cropping/padding will not be used.
-                * If ``int``, then that exact number of pixels will always be cropped/padded.
-                * If a ``tuple`` of two ``int`` s with values ``a`` and ``b``,
-                  then each side will be cropped/padded by a random amount sampled
-                  uniformly per image and side from the interval ``[a, b]``. If
-                  however `sample_independently` is set to ``False``, only one
-                  value will be sampled per image and used for all sides.
-                * If a ``tuple`` of four entries, then the entries represent top,
-                  right, bottom, left. Each entry may be a single ``int`` (always
-                  crop/pad by exactly that value), a ``tuple`` of two ``int`` s
-                  ``a`` and ``b`` (crop/pad by an amount within ``[a, b]``), a
-                  ``list`` of ``int`` s (crop/pad by a random value that is
-                  contained in the ``list``).
-        percent (float or tuple):
-            The number of pixels to crop (negative values) or pad (positive values)
-            on each side of the image given as a *fraction* of the image
-            height/width. E.g. if this is set to ``-0.1``, the transformation will
-            always crop away ``10%`` of the image's height at both the top and the
-            bottom (both ``10%`` each), as well as ``10%`` of the width at the
-            right and left.
-            Expected value range is ``(-1.0, inf)``.
-            Either this or the parameter `px` may be set, not both
-            at the same time.
-                * If ``None``, then fraction-based cropping/padding will not be
-                  used.
-                * If ``float``, then that fraction will always be cropped/padded.
-                * If a ``tuple`` of two ``float`` s with values ``a`` and ``b``,
-                  then each side will be cropped/padded by a random fraction
-                  sampled uniformly per image and side from the interval
-                  ``[a, b]``. If however `sample_independently` is set to
-                  ``False``, only one value will be sampled per image and used for
-                  all sides.
-                * If a ``tuple`` of four entries, then the entries represent top,
-                  right, bottom, left. Each entry may be a single ``float``
-                  (always crop/pad by exactly that percent value), a ``tuple`` of
-                  two ``float`` s ``a`` and ``b`` (crop/pad by a fraction from
-                  ``[a, b]``), a ``list`` of ``float`` s (crop/pad by a random
-                  value that is contained in the list).
+        px (int,
+            Tuple[int, int],
+            Tuple[int, int, int, int],
+            Tuple[Union[int, Tuple[int, int], List[int]],
+                  Union[int, Tuple[int, int], List[int]],
+                  Union[int, Tuple[int, int], List[int]],
+                  Union[int, Tuple[int, int], List[int]]]):
+            The number of pixels to crop (negative values) or pad (positive values) on each side of the image.
+                Either this or the parameter `percent` may be set, not both at the same time.
+
+                * If `None`, then pixel-based cropping/padding will not be used.
+                * If `int`, then that exact number of pixels will always be cropped/padded.
+                * If a `tuple` of two `int`s with values `a` and `b`, then each side will be cropped/padded by a
+                    random amount sampled uniformly per image and side from the interval `[a, b]`.
+                    If `sample_independently` is set to `False`, only one value will be sampled per
+                        image and used for all sides.
+                * If a `tuple` of four entries, then the entries represent top, right, bottom, and left.
+                    Each entry may be:
+                    - A single `int` (always crop/pad by exactly that value).
+                    - A `tuple` of two `int`s `a` and `b` (crop/pad by an amount within `[a, b]`).
+                    - A `list` of `int`s (crop/pad by a random value that is contained in the `list`).
+
+        percent (float,
+                 Tuple[float, float],
+                 Tuple[float, float, float, float],
+                 Tuple[Union[float, Tuple[float, float], List[float]],
+                       Union[float, Tuple[float, float], List[float]],
+                       Union[float, Tuple[float, float], List[float]],
+                       Union[float, Tuple[float, float], List[float]]]):
+            The number of pixels to crop (negative values) or pad (positive values) on each side of the image given
+                as a *fraction* of the image height/width. E.g. if this is set to `-0.1`, the transformation will
+                always crop away `10%` of the image's height at both the top and the bottom (both `10%` each),
+                as well as `10%` of the width at the right and left. Expected value range is `(-1.0, inf)`.
+                Either this or the parameter `px` may be set, not both at the same time.
+
+                * If `None`, then fraction-based cropping/padding will not be used.
+                * If `float`, then that fraction will always be cropped/padded.
+                * If a `tuple` of two `float`s with values `a` and `b`, then each side will be cropped/padded by a
+                random fraction sampled uniformly per image and side from the interval `[a, b]`.
+                If `sample_independently` is set to `False`, only one value will be sampled per image and used
+                for all sides.
+                * If a `tuple` of four entries, then the entries represent top, right, bottom, and left.
+                    Each entry may be:
+                    - A single `float` (always crop/pad by exactly that percent value).
+                    - A `tuple` of two `float`s `a` and `b` (crop/pad by a fraction from `[a, b]`).
+                    - A `list` of `float`s (crop/pad by a random value that is contained in the `list`).
+
         pad_mode (int): OpenCV border mode.
-        pad_cval (number, Sequence[number]):
-            The constant value to use if the pad mode is ``BORDER_CONSTANT``.
-                * If ``number``, then that value will be used.
-                * If a ``tuple`` of two ``number`` s and at least one of them is
-                  a ``float``, then a random number will be uniformly sampled per
-                  image from the continuous interval ``[a, b]`` and used as the
-                  value. If both ``number`` s are ``int`` s, the interval is
-                  discrete.
-                * If a ``list`` of ``number``, then a random value will be chosen
-                  from the elements of the ``list`` and used as the value.
-        pad_cval_mask (number, Sequence[number]): Same as pad_cval but only for masks.
+        pad_cval (Union[int, float, Tuple[Union[int, float], Union[int, float]], List[Union[int, float]]]):
+            The constant value to use if the pad mode is `BORDER_CONSTANT`.
+                * If `number`, then that value will be used.
+                * If a `tuple` of two numbers and at least one of them is a `float`, then a random number
+                    will be uniformly sampled per image from the continuous interval `[a, b]` and used as the value.
+                    If both numbers are `int`s, the interval is discrete.
+                * If a `list` of numbers, then a random value will be chosen from the elements of the `list` and
+                    used as the value.
+
+        pad_cval_mask (Union[int, float, Tuple[Union[int, float], Union[int, float]], List[Union[int, float]]]):
+            Same as `pad_cval` but only for masks.
+
         keep_size (bool):
-            After cropping and padding, the result image will usually have a
-            different height/width compared to the original input image. If this
-            parameter is set to ``True``, then the cropped/padded image will be
-            resized to the input image's size, i.e. the output shape is always identical to the input shape.
+            After cropping and padding, the resulting image will usually have a different height/width compared to
+            the original input image. If this parameter is set to `True`, then the cropped/padded image will be
+            resized to the input image's size, i.e., the output shape is always identical to the input shape.
+
         sample_independently (bool):
-            If ``False`` *and* the values for `px`/`percent` result in exactly
-            *one* probability distribution for all image sides, only one single
-            value will be sampled from that probability distribution and used for
-            all sides. I.e. the crop/pad amount then is the same for all sides.
-            If ``True``, four values will be sampled independently, one per side.
-        interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
-            cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4.
-            Default: cv2.INTER_LINEAR.
+            If `False` and the values for `px`/`percent` result in exactly one probability distribution for all
+            image sides, only one single value will be sampled from that probability distribution and used for
+            all sides. I.e., the crop/pad amount then is the same for all sides. If `True`, four values
+            will be sampled independently, one per side.
+
+        interpolation (int):
+            OpenCV flag that is used to specify the interpolation algorithm for images. Should be one of:
+            `cv2.INTER_NEAREST`, `cv2.INTER_LINEAR`, `cv2.INTER_CUBIC`, `cv2.INTER_AREA`, `cv2.INTER_LANCZOS4`.
+            Default: `cv2.INTER_LINEAR`.
 
     Targets:
         image, mask, bboxes, keypoints
 
     Image types:
-        any
+        unit8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     class InitSchema(BaseTransformInitSchema):
-        px: Optional[Union[int, Tuple[int, int], Tuple[int, int, int, int]]] = Field(
+        px: Optional[PxType] = Field(
             default=None,
             description="Number of pixels to crop (negative) or pad (positive).",
         )
-        percent: Optional[Union[float, Tuple[float, float], Tuple[float, float, float, float]]] = Field(
+        percent: Optional[PercentType] = Field(
             default=None,
             description="Fraction of image size to crop (negative) or pad (positive).",
         )
         pad_mode: BorderModeType = cv2.BORDER_CONSTANT
-        pad_cval: ColorType = Field(default=0, description="Padding value if pad_mode is BORDER_CONSTANT.")
-        pad_cval_mask: ColorType = Field(
+        pad_cval: Union[ScalarType, Tuple[ScalarType, ScalarType], List[ScalarType]] = Field(
+            default=0,
+            description="Padding value if pad_mode is BORDER_CONSTANT.",
+        )
+        pad_cval_mask: Union[ScalarType, Tuple[ScalarType, ScalarType], List[ScalarType]] = Field(
             default=0,
             description="Padding value for masks if pad_mode is BORDER_CONSTANT.",
         )
         keep_size: bool = Field(
             default=True,
             description="Whether to resize the image back to the original size after cropping and padding.",
         )
@@ -991,28 +1013,28 @@
         )
         interpolation: InterpolationType = cv2.INTER_LINEAR
         p: ProbabilityType = 1
 
         @model_validator(mode="after")
         def check_px_percent(self) -> Self:
             if self.px is None and self.percent is None:
-                msg = "px and percent are empty!"
+                msg = "Both px and percent parameters cannot be None simultaneously."
                 raise ValueError(msg)
             if self.px is not None and self.percent is not None:
                 msg = "Only px or percent may be set!"
                 raise ValueError(msg)
             return self
 
     def __init__(
         self,
         px: Optional[Union[int, List[int]]] = None,
         percent: Optional[Union[float, List[float]]] = None,
         pad_mode: int = cv2.BORDER_CONSTANT,
-        pad_cval: ColorType = 0,
-        pad_cval_mask: ColorType = 0,
+        pad_cval: Union[ScalarType, Tuple[ScalarType, ScalarType], List[ScalarType]] = 0,
+        pad_cval_mask: Union[ScalarType, Tuple[ScalarType, ScalarType], List[ScalarType]] = 0,
         keep_size: bool = True,
         sample_independently: bool = True,
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 1.0,
     ):
         super().__init__(always_apply, p)
@@ -1036,15 +1058,15 @@
         pad_params: Sequence[int],
         pad_value: float,
         rows: int,
         cols: int,
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.crop_and_pad(
+        return fcrops.crop_and_pad(
             img,
             crop_params,
             pad_params,
             pad_value,
             rows,
             cols,
             interpolation,
@@ -1059,15 +1081,15 @@
         pad_params: Sequence[int],
         pad_value_mask: float,
         rows: int,
         cols: int,
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.crop_and_pad(
+        return fcrops.crop_and_pad(
             mask,
             crop_params,
             pad_params,
             pad_value_mask,
             rows,
             cols,
             interpolation,
@@ -1082,28 +1104,28 @@
         pad_params: Sequence[int],
         rows: int,
         cols: int,
         result_rows: int,
         result_cols: int,
         **params: Any,
     ) -> BoxInternalType:
-        return F.crop_and_pad_bbox(bbox, crop_params, pad_params, rows, cols, result_rows, result_cols)
+        return fcrops.crop_and_pad_bbox(bbox, crop_params, pad_params, rows, cols, result_rows, result_cols)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         crop_params: Sequence[int],
         pad_params: Sequence[int],
         rows: int,
         cols: int,
         result_rows: int,
         result_cols: int,
         **params: Any,
     ) -> KeypointInternalType:
-        return F.crop_and_pad_keypoint(
+        return fcrops.crop_and_pad_keypoint(
             keypoint,
             crop_params,
             pad_params,
             rows,
             cols,
             result_rows,
             result_cols,
@@ -1127,18 +1149,15 @@
             regain1 = val1
             regain2 += diff
         elif regain2 > val2:
             diff = regain2 - val2
             regain2 = val2
             regain1 += diff
 
-        val1 = val1 - regain1
-        val2 = val2 - regain2
-
-        return val1, val2
+        return val1 - regain1, val2 - regain2
 
     @staticmethod
     def _prevent_zero(crop_params: List[int], height: int, width: int) -> List[int]:
         top, right, bottom, left = crop_params
 
         remaining_height = height - (top + bottom)
         remaining_width = width - (left + right)
@@ -1195,53 +1214,59 @@
     def _get_px_params(self) -> List[int]:
         if self.px is None:
             msg = "px is not set"
             raise ValueError(msg)
 
         if isinstance(self.px, int):
             params = [self.px] * 4
-        elif len(self.px) == TWO:
+        elif len(self.px) == PAIR:
             if self.sample_independently:
                 params = [random.randrange(*self.px) for _ in range(4)]
             else:
                 px = random.randrange(*self.px)
                 params = [px] * 4
         elif isinstance(self.px[0], int):
             params = self.px
-        else:
+        elif len(self.px[0]) == PAIR:
             params = [random.randrange(*i) for i in self.px]
+        else:
+            params = [random.choice(i) for i in self.px]
 
         return params
 
     def _get_percent_params(self) -> List[float]:
         if self.percent is None:
             msg = "percent is not set"
             raise ValueError(msg)
 
         if isinstance(self.percent, float):
             params = [self.percent] * 4
-        elif len(self.percent) == TWO:
+        elif len(self.percent) == PAIR:
             if self.sample_independently:
                 params = [random.uniform(*self.percent) for _ in range(4)]
             else:
                 px = random.uniform(*self.percent)
                 params = [px] * 4
         elif isinstance(self.percent[0], (int, float)):
             params = self.percent
-        else:
+        elif len(self.percent[0]) == PAIR:
             params = [random.uniform(*i) for i in self.percent]
+        else:
+            params = [random.choice(i) for i in self.percent]
 
         return params  # params = [top, right, bottom, left]
 
     @staticmethod
-    def _get_pad_value(pad_value: Union[float, Sequence[float]]) -> Union[int, float]:
+    def _get_pad_value(
+        pad_value: Union[ScalarType, Tuple[ScalarType, ScalarType], List[ScalarType]],
+    ) -> ScalarType:
         if isinstance(pad_value, (int, float)):
             return pad_value
 
-        if len(pad_value) == TWO:
+        if len(pad_value) == PAIR:
             a, b = pad_value
             if isinstance(a, int) and isinstance(b, int):
                 return random.randint(a, b)
 
             return random.uniform(a, b)
 
         return random.choice(pad_value)
@@ -1351,49 +1376,49 @@
         img: np.ndarray,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.clamping_crop(img, x_min, y_min, x_max, y_max)
+        return fcrops.clamping_crop(img, x_min, y_min, x_max, y_max)
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.clamping_crop(mask, x_min, y_min, x_max, y_max)
+        return fcrops.clamping_crop(mask, x_min, y_min, x_max, y_max)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
-        return F.bbox_crop(bbox, x_min, y_min, x_max, y_max, rows, cols)
+        return fcrops.bbox_crop(bbox, x_min, y_min, x_max, y_max, rows, cols)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> KeypointInternalType:
-        return F.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
+        return fcrops.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return "crop_left", "crop_right", "crop_top", "crop_bottom"
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/domain_adaptation.py` & `albumentations-1.4.8/albumentations/augmentations/domain_adaptation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import random
 from typing import Any, Callable, Dict, List, Literal, Sequence, Tuple, cast
 
 import cv2
 import numpy as np
+from albucore.utils import is_grayscale_image, is_multispectral_image
 from pydantic import field_validator
 
 from albumentations.augmentations.domain_adaptation_functional import (
     adapt_pixel_distribution,
     apply_histogram,
     fourier_domain_adaptation,
 )
-from albumentations.augmentations.utils import (
-    is_grayscale_image,
-    is_multispectral_image,
-    read_rgb_image,
-)
+from albumentations.augmentations.utils import read_rgb_image
 from albumentations.core.pydantic import NonNegativeFloatRangeType, ZeroOneRangeType
 from albumentations.core.transforms_interface import BaseTransformInitSchema, ImageOnlyTransform
 from albumentations.core.types import ScaleFloatType
 
 __all__ = [
     "HistogramMatching",
     "FDA",
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/domain_adaptation_functional.py` & `albumentations-1.4.8/albumentations/augmentations/domain_adaptation_functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 import abc
 from copy import deepcopy
 from typing import Optional, Tuple
 
 import cv2
 import numpy as np
+from albucore.utils import clipped, get_num_channels, get_opencv_dtype_from_numpy, preserve_channel_dim
 from skimage.exposure import match_histograms
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import MinMaxScaler, StandardScaler
 from typing_extensions import Protocol
 
-from albumentations.augmentations.utils import (
-    clipped,
-    get_opencv_dtype_from_numpy,
-    preserve_channel_dim,
-)
-
-GRAYSCALE_IMAGE_SHAPE = 2
-NON_GRAY_IMAGE_SHAPE = 3
-RGB_NUM_CHANNELS = 3
+from albumentations.augmentations.functional import center
+from albumentations.core.types import MONO_CHANNEL_DIMENSIONS
 
 __all__ = [
     "fourier_domain_adaptation",
     "apply_histogram",
     "adapt_pixel_distribution",
 ]
 
@@ -103,30 +97,32 @@
     result = adapter(img).astype("float32")
     return (img.astype("float32") * (1 - weight) + result * weight).astype(initial_type)
 
 
 def low_freq_mutate(amp_src: np.ndarray, amp_trg: np.ndarray, beta: float) -> np.ndarray:
     height, width = amp_src.shape[:2]
     border = int(np.floor(min(height, width) * beta))
-    center_y, center_h = height // 2, width // 2
-    h1, h2 = max(0, center_y - border), min(center_y + border, height - 1)
-    w1, w2 = max(0, center_h - border), min(center_h + border, width - 1)
+
+    center_x, center_y = center(width, height)
+
+    h1, h2 = max(0, int(center_y - border)), min(int(center_y + border), height)
+    w1, w2 = max(0, int(center_x - border)), min(int(center_x + border), width)
     amp_src[h1:h2, w1:w2] = amp_trg[h1:h2, w1:w2]
     return amp_src
 
 
 @clipped
 @preserve_channel_dim
 def fourier_domain_adaptation(img: np.ndarray, target_img: np.ndarray, beta: float) -> np.ndarray:
     src_img = img.astype(np.float32)
     trg_img = target_img.astype(np.float32)
 
-    if len(src_img.shape) == GRAYSCALE_IMAGE_SHAPE:
+    if len(src_img.shape) == MONO_CHANNEL_DIMENSIONS:
         src_img = np.expand_dims(src_img, axis=-1)
-    if len(trg_img.shape) == GRAYSCALE_IMAGE_SHAPE:
+    if len(trg_img.shape) == MONO_CHANNEL_DIMENSIONS:
         trg_img = np.expand_dims(trg_img, axis=-1)
 
     num_channels = src_img.shape[-1]
 
     # Prepare container for the output image
     src_in_trg = np.zeros_like(src_img)
 
@@ -164,14 +160,14 @@
     # Resize reference image only if necessary
     if img.shape[:2] != reference_image.shape[:2]:
         reference_image = cv2.resize(reference_image, dsize=(img.shape[1], img.shape[0]))
 
     img, reference_image = np.squeeze(img), np.squeeze(reference_image)
 
     # Determine if the images are multi-channel based on a predefined condition or shape analysis
-    is_multichannel = img.ndim == NON_GRAY_IMAGE_SHAPE and img.shape[2] == RGB_NUM_CHANNELS
+    is_multichannel = get_num_channels(img) > 1
 
     # Match histograms between the images
     matched = match_histograms(img, reference_image, channel_axis=2 if is_multichannel else None)
 
     # Blend the original image and the matched image
     return cv2.addWeighted(matched, blend_ratio, img, 1 - blend_ratio, 0, dtype=get_opencv_dtype_from_numpy(img.dtype))
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/dropout/channel_dropout.py` & `albumentations-1.4.8/albumentations/augmentations/dropout/channel_dropout.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import random
 from typing import Any, Dict, List, Mapping, Tuple
 
 import numpy as np
+from albucore.utils import is_grayscale_image
 from pydantic import Field
 from typing_extensions import Annotated
 
 from albumentations import random_utils
-from albumentations.augmentations.utils import is_grayscale_image
 from albumentations.core.pydantic import OnePlusIntRangeType
 from albumentations.core.transforms_interface import BaseTransformInitSchema, ImageOnlyTransform
 from albumentations.core.types import ColorType
 
 from .functional import channel_dropout
 
 __all__ = ["ChannelDropout"]
 
-NUM_GRAYSCALE_LENGTH = 2
 MIN_DROPOUT_CHANNEL_LIST_LENGTH = 2
 
 
 class ChannelDropout(ImageOnlyTransform):
     """Randomly Drop Channels in the input Image.
 
     Args:
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/dropout/coarse_dropout.py` & `albumentations-1.4.8/albumentations/augmentations/dropout/coarse_dropout.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from pydantic import Field, model_validator
 from typing_extensions import Literal, Self
 
 from albumentations import random_utils
 from albumentations.core.pydantic import OnePlusIntNonDecreasingRangeType
@@ -243,7 +243,16 @@
         return (
             "num_holes_range",
             "hole_height_range",
             "hole_width_range",
             "fill_value",
             "mask_fill_value",
         )
+
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+            "keypoints": self.apply_to_keypoints,
+        }
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/dropout/functional.py` & `albumentations-1.4.8/albumentations/augmentations/dropout/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Iterable, Tuple, Union
 
 import numpy as np
+from albucore.utils import MAX_VALUES_BY_DTYPE, is_grayscale_image, preserve_channel_dim
 from typing_extensions import Literal
 
 from albumentations import random_utils
-from albumentations.augmentations.utils import MAX_VALUES_BY_DTYPE, is_grayscale_image, preserve_channel_dim
 from albumentations.core.types import MONO_CHANNEL_DIMENSIONS, ColorType, KeypointType
 
 __all__ = ["cutout", "channel_dropout", "keypoint_in_hole"]
 
 
 @preserve_channel_dim
 def channel_dropout(
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/dropout/grid_dropout.py` & `albumentations-1.4.8/albumentations/augmentations/dropout/grid_dropout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import random
-from typing import Any, Dict, Iterable, List, Optional, Tuple
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple
 
 import numpy as np
 from pydantic import Field
 
 from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
 from albumentations.core.types import ColorType, ScalarType, Targets
 
-from . import functional as F
+from . import functional as fdropout
 
 __all__ = ["GridDropout"]
 
 TWO = 2
 
 
 class GridDropout(DualTransform):
@@ -87,26 +87,26 @@
         self.shift_x = shift_x
         self.shift_y = shift_y
         self.random_offset = random_offset
         self.fill_value = fill_value
         self.mask_fill_value = mask_fill_value
 
     def apply(self, img: np.ndarray, holes: Iterable[Tuple[int, int, int, int]], **params: Any) -> np.ndarray:
-        return F.cutout(img, holes, self.fill_value)
+        return fdropout.cutout(img, holes, self.fill_value)
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
         holes: Iterable[Tuple[int, int, int, int]],
         **params: Any,
     ) -> np.ndarray:
         if self.mask_fill_value is None:
             return mask
 
-        return F.cutout(mask, holes, self.mask_fill_value)
+        return fdropout.cutout(mask, holes, self.mask_fill_value)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         img = params["image"]
         height, width = img.shape[:2]
         unit_width, unit_height = self._calculate_unit_dimensions(width, height)
         hole_width, hole_height = self._calculate_hole_dimensions(unit_width, unit_height)
         shift_x, shift_y = self._calculate_shifts(unit_width, unit_height, hole_width, hole_height)
@@ -209,7 +209,15 @@
             "holes_number_y",
             "shift_x",
             "shift_y",
             "random_offset",
             "fill_value",
             "mask_fill_value",
         )
+
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+        }
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/dropout/mask_dropout.py` & `albumentations-1.4.8/albumentations/augmentations/dropout/mask_dropout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import Any, Dict, List, Tuple, Union, cast
+from typing import Any, Callable, Dict, List, Tuple, Union, cast
 
 import cv2
 import numpy as np
 from pydantic import Field
 from skimage.measure import label
 from typing_extensions import Literal
 
@@ -113,7 +113,15 @@
 
         mask = mask.copy()
         mask[dropout_mask] = self.mask_fill_value
         return mask
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return "max_objects", "image_fill_value", "mask_fill_value"
+
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+        }
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/dropout/xy_masking.py` & `albumentations-1.4.8/albumentations/augmentations/dropout/xy_masking.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import Any, Dict, List, Optional, Sequence, Tuple, cast
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, cast
 
 import numpy as np
 from pydantic import Field, model_validator
 from typing_extensions import Self
 
 from albumentations import random_utils
 from albumentations.core.pydantic import NonNegativeIntRangeType
@@ -210,7 +210,16 @@
             "num_masks_x",
             "num_masks_y",
             "mask_x_length",
             "mask_y_length",
             "fill_value",
             "mask_fill_value",
         )
+
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+            "keypoints": self.apply_to_keypoints,
+        }
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/functional.py` & `albumentations-1.4.8/albumentations/augmentations/functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from collections import defaultdict
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 from warnings import warn
 
 import cv2
 import numpy as np
 import skimage
+from albucore.functions import clip, clipped, multiply, preserve_channel_dim
+from albucore.utils import MAX_VALUES_BY_DTYPE, contiguous, is_grayscale_image, is_rgb_image, maybe_process_in_chunks
 from typing_extensions import Literal
 
 from albumentations import random_utils
 from albumentations.augmentations.utils import (
-    MAX_VALUES_BY_DTYPE,
-    _maybe_process_in_chunks,
-    clip,
-    clipped,
-    ensure_contiguous,
-    is_grayscale_image,
-    is_rgb_image,
     non_rgb_warning,
-    preserve_channel_dim,
 )
 from albumentations.core.types import (
+    EIGHT,
+    FOUR,
+    MONO_CHANNEL_DIMENSIONS,
     ColorType,
     ImageMode,
+    NumericType,
     ScalarType,
     SpatterMode,
 )
 
 __all__ = [
     "add_fog",
     "add_rain",
@@ -49,15 +47,14 @@
     "gamma_transform",
     "gauss_noise",
     "image_compression",
     "invert",
     "iso_noise",
     "linear_transformation_rgb",
     "move_tone_curve",
-    "multiply",
     "noop",
     "normalize",
     "posterize",
     "shift_hsv",
     "shift_rgb",
     "solarize",
     "superpixels",
@@ -69,22 +66,14 @@
     "MAX_VALUES_BY_DTYPE",
     "split_uniform_grid",
     "chromatic_aberration",
     "erode",
     "dilate",
 ]
 
-TWO = 2
-THREE = 3
-NUM_RGB_CHANNELS = 3
-GRAYSCALE_SHAPE_LENGTH = 2
-FOUR = 4
-EIGHT = 8
-THREE_SIXTY = 360
-
 
 def normalize_cv2(img: np.ndarray, mean: np.ndarray, denominator: np.ndarray) -> np.ndarray:
     if mean.shape and len(mean) != FOUR and mean.shape != img.shape:
         mean = np.array(mean.tolist() + [0] * (4 - len(mean)), dtype=np.float64)
     if not denominator.shape:
         denominator = np.array([denominator.tolist()] * 4, dtype=np.float64)
     elif len(denominator) != FOUR and denominator.shape != img.shape:
@@ -100,27 +89,19 @@
     img = img.astype(np.float32)
     img -= mean
     img *= denominator
     return img
 
 
 @preserve_channel_dim
-def normalize(img: np.ndarray, mean: ColorType, std: ColorType, max_pixel_value: float = 255.0) -> np.ndarray:
-    mean_np = np.array(mean, dtype=np.float32)
-    mean_np *= max_pixel_value
-
-    std_np = np.array(std, dtype=np.float32)
-    std_np *= max_pixel_value
-
-    denominator = np.reciprocal(std_np, dtype=np.float32)
-
+def normalize(img: np.ndarray, mean: np.ndarray, denominator: np.ndarray) -> np.ndarray:
     if is_rgb_image(img):
-        return normalize_cv2(img, mean_np, denominator)
+        return normalize_cv2(img, mean, denominator)
 
-    return normalize_numpy(img, mean_np, denominator)
+    return normalize_numpy(img, mean, denominator)
 
 
 @preserve_channel_dim
 def normalize_per_image(
     img: np.ndarray,
     normalization: Literal["image", "image_per_channel", "min_max", "min_max_per_channel"],
 ) -> np.ndarray:
@@ -134,43 +115,44 @@
     Returns:
         np.ndarray: The normalized image.
 
     Reference:
         https://github.com/ChristofHenkel/kaggle-landmark-2021-1st-place/blob/main/data/ch_ds_1.py
     """
     img = img.astype(np.float32)
+    eps = 1e-4
 
-    if img.ndim == GRAYSCALE_SHAPE_LENGTH:
+    if img.ndim == MONO_CHANNEL_DIMENSIONS:
         img = np.expand_dims(img, axis=-1)  # Ensure the image is at least 3D
 
     if normalization == "image":
         # Normalize the whole image based on its global mean and std
         mean = img.mean()
-        std = img.std() + 1e-4  # Adding a small epsilon to avoid division by zero
+        std = img.std() + eps  # Adding a small epsilon to avoid division by zero
         normalized_img = (img - mean) / std
         normalized_img = normalized_img.clip(-20, 20)  # Clipping outliers
 
     elif normalization == "image_per_channel":
         # Normalize the image per channel based on each channel's mean and std
         pixel_mean = img.mean(axis=(0, 1))
-        pixel_std = img.std(axis=(0, 1)) + 1e-4
+        pixel_std = img.std(axis=(0, 1)) + eps
         normalized_img = (img - pixel_mean[None, None, :]) / pixel_std[None, None, :]
         normalized_img = normalized_img.clip(-20, 20)
 
     elif normalization == "min_max":
         # Apply min-max normalization to the whole image
         img_min = img.min()
         img_max = img.max()
-        normalized_img = (img - img_min) / (img_max - img_min)
+        normalized_img = (img - img_min) / (img_max - img_min + eps)
 
     elif normalization == "min_max_per_channel":
         # Apply min-max normalization per channel
         img_min = img.min(axis=(0, 1), keepdims=True)
         img_max = img.max(axis=(0, 1), keepdims=True)
-        normalized_img = (img - img_min) / (img_max - img_min)
+        normalized_img = (img - img_min) / (img_max - img_min + eps)
 
     else:
         raise ValueError(f"Unknown normalization method: {normalization}")
 
     return normalized_img
 
 
@@ -187,20 +169,20 @@
     if hue_shift != 0:
         lut_hue = np.arange(0, 256, dtype=np.int16)
         lut_hue = np.mod(lut_hue + hue_shift, 180).astype(dtype)
         hue = cv2.LUT(hue, lut_hue)
 
     if sat_shift != 0:
         lut_sat = np.arange(0, 256, dtype=np.int16)
-        lut_sat = np.clip(lut_sat + sat_shift, 0, 255).astype(dtype)
+        lut_sat = clip(lut_sat + sat_shift, img.dtype)
         sat = cv2.LUT(sat, lut_sat)
 
     if val_shift != 0:
         lut_val = np.arange(0, 256, dtype=np.int16)
-        lut_val = np.clip(lut_val + val_shift, 0, 255).astype(dtype)
+        lut_val = clip(lut_val + val_shift, img.dtype)
         val = cv2.LUT(val, lut_val)
 
     img = cv2.merge((hue, sat, val)).astype(dtype)
     return cv2.cvtColor(img, cv2.COLOR_HSV2RGB)
 
 
 def _shift_hsv_non_uint8(
@@ -214,18 +196,18 @@
     hue, sat, val = cv2.split(img)
 
     if hue_shift != 0:
         hue = cv2.add(hue, hue_shift)
         hue = np.mod(hue, 360)  # OpenCV fails with negative values
 
     if sat_shift != 0:
-        sat = clip(cv2.add(sat, sat_shift), dtype, 1.0)
+        sat = clip(cv2.add(sat, sat_shift), dtype)
 
     if val_shift != 0:
-        val = clip(cv2.add(val, val_shift), dtype, 1.0)
+        val = clip(cv2.add(val, val_shift), dtype)
 
     img = cv2.merge((hue, sat, val))
     return cv2.cvtColor(img, cv2.COLOR_HSV2RGB)
 
 
 @preserve_channel_dim
 def shift_hsv(img: np.ndarray, hue_shift: np.ndarray, sat_shift: np.ndarray, val_shift: np.ndarray) -> np.ndarray:
@@ -236,14 +218,15 @@
     if is_gray:
         if hue_shift != 0 or sat_shift != 0:
             hue_shift = 0
             sat_shift = 0
             warn(
                 "HueSaturationValue: hue_shift and sat_shift are not applicable to grayscale image. "
                 "Set them to 0 or use RGB image",
+                stacklevel=2,
             )
         img = cv2.cvtColor(img, cv2.COLOR_GRAY2RGB)
 
     if img.dtype == np.uint8:
         img = _shift_hsv_uint8(img, hue_shift, sat_shift, val_shift)
     else:
         img = _shift_hsv_non_uint8(img, hue_shift, sat_shift, val_shift)
@@ -264,15 +247,15 @@
     Returns:
         Solarized image.
 
     """
     dtype = img.dtype
     max_val = MAX_VALUES_BY_DTYPE[dtype]
 
-    if dtype == np.dtype("uint8"):
+    if dtype == np.uint8:
         lut = [(i if i < threshold else max_val - i) for i in range(int(max_val) + 1)]
 
         prev_shape = img.shape
         img = cv2.LUT(img, np.array(lut, dtype=dtype))
 
         if len(prev_shape) != len(img.shape):
             img = np.expand_dims(img, -1)
@@ -376,15 +359,15 @@
     scale = 255.0 / (total - histogram[i])
     _sum = 0
 
     lut = np.zeros(256, dtype=np.uint8)
 
     for idx in range(i + 1, len(histogram)):
         _sum += histogram[idx]
-        lut[idx] = clip(round(_sum * scale), np.dtype("uint8"), 255)
+        lut[idx] = clip(round(_sum * scale), np.uint8)
 
     return cv2.LUT(img, lut)
 
 
 def _check_preconditions(img: np.ndarray, mask: Optional[np.ndarray], by_channels: bool) -> None:
     if img.dtype != np.uint8:
         msg = "Image must have uint8 channel type"
@@ -469,15 +452,15 @@
     # Defines response of a four-point Bezier curve
     def evaluate_bez(t: np.ndarray) -> np.ndarray:
         return 3 * (1 - t) ** 2 * t * low_y + 3 * (1 - t) * t**2 * high_y + t**3
 
     evaluate_bez = np.vectorize(evaluate_bez)
     remapping = np.rint(evaluate_bez(t) * 255).astype(np.uint8)
 
-    lut_fn = _maybe_process_in_chunks(cv2.LUT, lut=remapping)
+    lut_fn = maybe_process_in_chunks(cv2.LUT, lut=remapping)
     return lut_fn(img)
 
 
 @clipped
 def _shift_rgb_non_uint8(img: np.ndarray, r_shift: float, g_shift: float, b_shift: float) -> np.ndarray:
     if r_shift == g_shift == b_shift:
         return img + r_shift
@@ -492,15 +475,15 @@
 
 def _shift_image_uint8(img: np.ndarray, value: np.ndarray) -> np.ndarray:
     max_value = MAX_VALUES_BY_DTYPE[img.dtype]
 
     lut = np.arange(0, max_value + 1).astype("float32")
     lut += value
 
-    lut = np.clip(lut, 0, max_value).astype(img.dtype)
+    lut = clip(lut, img.dtype)
     return cv2.LUT(img, lut)
 
 
 @preserve_channel_dim
 def _shift_rgb_uint8(img: np.ndarray, r_shift: ScalarType, g_shift: ScalarType, b_shift: ScalarType) -> np.ndarray:
     if r_shift == g_shift == b_shift:
         height, width, channels = img.shape
@@ -542,15 +525,15 @@
     img = cv2.cvtColor(img, cv2.COLOR_RGB2LAB)
     img[:, :, 0] = clahe_mat.apply(img[:, :, 0])
     return cv2.cvtColor(img, cv2.COLOR_LAB2RGB)
 
 
 @preserve_channel_dim
 def convolve(img: np.ndarray, kernel: np.ndarray) -> np.ndarray:
-    conv_fn = _maybe_process_in_chunks(cv2.filter2D, ddepth=-1, kernel=kernel)
+    conv_fn = maybe_process_in_chunks(cv2.filter2D, ddepth=-1, kernel=kernel)
     return conv_fn(img)
 
 
 @preserve_channel_dim
 def image_compression(img: np.ndarray, quality: int, image_type: Literal[".jpg", ".webp"]) -> np.ndarray:
     if image_type == ".jpg":
         quality_flag = cv2.IMWRITE_JPEG_QUALITY
@@ -564,14 +547,15 @@
 
     if input_dtype == np.float32:
         warn(
             "Image compression augmentation "
             "is most effective with uint8 inputs, "
             f"{input_dtype} is used as input.",
             UserWarning,
+            stacklevel=2,
         )
         img = from_float(img, dtype=np.dtype("uint8"))
         needs_float = True
     elif input_dtype not in (np.uint8, np.float32):
         raise ValueError(f"Unexpected dtype {input_dtype} for image augmentation")
 
     _, encoded_img = cv2.imencode(image_type, img, (int(quality_flag), quality))
@@ -580,47 +564,48 @@
     if needs_float:
         img = to_float(img, max_value=255)
     return img
 
 
 @preserve_channel_dim
 def add_snow(img: np.ndarray, snow_point: float, brightness_coeff: float) -> np.ndarray:
-    """Bleaches out pixels, imitation snow.
-
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+    """Bleaches out pixels, imitating snow.
 
     Args:
-        img: Image.
-        snow_point: Number of show points.
-        brightness_coeff: Brightness coefficient.
+        img (np.ndarray): Input image.
+        snow_point (float): A float in the range [0, 1], scaled and adjusted to determine
+            the threshold for pixel modification.
+        brightness_coeff (float): Coefficient applied to increase the brightness of pixels below the snow_point
+            threshold. Larger values lead to more pronounced snow effects.
 
     Returns:
-        Image.
+        np.ndarray: Image with simulated snow effect.
+
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
 
     """
     non_rgb_warning(img)
 
     input_dtype = img.dtype
     needs_float = False
 
     snow_point *= 127.5  # = 255 / 2
     snow_point += 85  # = 255 / 3
 
     if input_dtype == np.float32:
         img = from_float(img, dtype=np.dtype("uint8"))
         needs_float = True
-    elif input_dtype not in (np.uint8, np.float32):
-        raise ValueError(f"Unexpected dtype {input_dtype} for RandomSnow augmentation")
 
     image_hls = cv2.cvtColor(img, cv2.COLOR_RGB2HLS)
     image_hls = np.array(image_hls, dtype=np.float32)
 
     image_hls[:, :, 1][image_hls[:, :, 1] < snow_point] *= brightness_coeff
 
-    image_hls[:, :, 1] = clip(image_hls[:, :, 1], np.uint8, 255)
+    image_hls[:, :, 1] = clip(image_hls[:, :, 1], np.uint8)
 
     image_hls = np.array(image_hls, dtype=np.uint8)
 
     image_rgb = cv2.cvtColor(image_hls, cv2.COLOR_HLS2RGB)
 
     if needs_float:
         image_rgb = to_float(image_rgb, max_value=255)
@@ -635,40 +620,41 @@
     drop_length: int,
     drop_width: int,
     drop_color: Tuple[int, int, int],
     blur_value: int,
     brightness_coefficient: float,
     rain_drops: List[Tuple[int, int]],
 ) -> np.ndarray:
-    """From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+    """Adds rain drops to the image.
 
     Args:
-        img: Image.
-        slant:
-        drop_length:
-        drop_width:
-        drop_color:
-        blur_value: Rainy view are blurry.
-        brightness_coefficient: Rainy days are usually shady.
-        rain_drops:
+        img (np.ndarray): Input image.
+        slant (int): The angle of the rain drops.
+        drop_length (int): The length of each rain drop.
+        drop_width (int): The width of each rain drop.
+        drop_color (Tuple[int, int, int]): The color of the rain drops in RGB format.
+        blur_value (int): The size of the kernel used to blur the image. Rainy views are blurry.
+        brightness_coefficient (float): Coefficient to adjust the brightness of the image. Rainy days are usually shady.
+        rain_drops (List[Tuple[int, int]]): A list of tuples where each tuple represents the (x, y)
+            coordinates of the starting point of a rain drop.
 
     Returns:
-        Image
+        np.ndarray: Image with rain effect added.
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
     """
     non_rgb_warning(img)
 
     input_dtype = img.dtype
     needs_float = False
 
     if input_dtype == np.float32:
         img = from_float(img, dtype=np.dtype("uint8"))
         needs_float = True
-    elif input_dtype not in (np.uint8, np.float32):
-        raise ValueError(f"Unexpected dtype {input_dtype} for RandomRain augmentation")
 
     image = img.copy()
 
     for rain_drop_x0, rain_drop_y0 in rain_drops:
         rain_drop_x1 = rain_drop_x0 + slant
         rain_drop_y1 = rain_drop_y0 + drop_length
 
@@ -690,27 +676,31 @@
         return to_float(image_rgb, max_value=255)
 
     return image_rgb
 
 
 @preserve_channel_dim
 def add_fog(img: np.ndarray, fog_coef: float, alpha_coef: float, haze_list: List[Tuple[int, int]]) -> np.ndarray:
-    """Add fog to the image.
-
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+    """Add fog to an image using the provided coefficients and haze points.
 
     Args:
-        img: Image.
-        fog_coef: Fog coefficient.
-        alpha_coef: Alpha coefficient.
-        haze_list:
+        img (np.ndarray): The input image, expected to be a numpy array.
+        fog_coef (float): The fog coefficient, used to determine the intensity of the fog.
+        alpha_coef (float): The alpha coefficient, used to determine the transparency of the fog.
+        haze_list (List[Tuple[int, int]]): A list of tuples, where each tuple represents the x and y
+            coordinates of a haze point.
 
     Returns:
-        Image.
+        np.ndarray: The output image with added fog, as a numpy array.
+
+    Raises:
+        ValueError: If the input image's dtype is not uint8 or float32.
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
     """
     non_rgb_warning(img)
 
     input_dtype = img.dtype
     needs_float = False
 
     if input_dtype == np.float32:
@@ -748,40 +738,39 @@
     img: np.ndarray,
     flare_center_x: float,
     flare_center_y: float,
     src_radius: int,
     src_color: ColorType,
     circles: List[Any],
 ) -> np.ndarray:
-    """Add sun flare.
-
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+    """Add a sun flare effect to an image.
 
     Args:
-        img (numpy.ndarray):
-        flare_center_x (float):
-        flare_center_y (float):
-        src_radius:
-        src_color (int, int, int):
-        circles (list):
+        img (np.ndarray): The input image.
+        flare_center_x (float): The x-coordinate of the flare center.
+        flare_center_y (float): The y-coordinate of the flare center.
+        src_radius (int): The radius of the source of the flare.
+        src_color (ColorType): The color of the flare, represented as a tuple of RGB values.
+        circles (List[Any]): A list of tuples, each representing a circle that contributes to the flare effect.
+            Each tuple contains the alpha value, the center coordinates, the radius, and the color of the circle.
 
     Returns:
-        numpy.ndarray:
+        np.ndarray: The output image with the sun flare effect added.
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
     """
     non_rgb_warning(img)
 
     input_dtype = img.dtype
     needs_float = False
 
     if input_dtype == np.float32:
         img = from_float(img, dtype=np.dtype("uint8"))
         needs_float = True
-    elif input_dtype not in (np.uint8, np.float32):
-        raise ValueError(f"Unexpected dtype {input_dtype} for RandomSunFlareaugmentation")
 
     overlay = img.copy()
     output = img.copy()
 
     for alpha, (x, y), rad3, (r_color, g_color, b_color) in circles:
         cv2.circle(overlay, (x, y), rad3, (r_color, g_color, b_color), -1)
 
@@ -802,72 +791,70 @@
 
     if needs_float:
         image_rgb = to_float(image_rgb, max_value=255)
 
     return image_rgb
 
 
-@ensure_contiguous
+@contiguous
 @preserve_channel_dim
 def add_shadow(img: np.ndarray, vertices_list: List[np.ndarray]) -> np.ndarray:
-    """Add shadows to the image.
+    """Add shadows to the image by reducing the intensity of the RGB values in specified regions.
 
     Args:
-        img (numpy.ndarray):
-        vertices_list (list[numpy.ndarray]):
+        img (np.ndarray): Input image.
+        vertices_list (List[np.ndarray]): List of vertices for shadow polygons.
 
     Returns:
-        numpy.ndarray:
+        np.ndarray: Image with shadows added.
 
     Reference:
         https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
     """
     non_rgb_warning(img)
     input_dtype = img.dtype
     needs_float = False
 
+    max_value = MAX_VALUES_BY_DTYPE[np.uint8]
+
     if input_dtype == np.float32:
         img = from_float(img, dtype=np.dtype("uint8"))
         needs_float = True
-    elif input_dtype not in (np.uint8, np.float32):
-        raise ValueError(f"Unexpected dtype {input_dtype} for RandomShadow augmentation")
-
-    image_hls = cv2.cvtColor(img, cv2.COLOR_RGB2HLS)
-    mask = np.zeros_like(img)
 
-    # adding all shadow polygons on empty mask, single 255 denotes only red channel
-    cv2.fillPoly(mask, vertices_list, 255)
+    mask = np.zeros_like(img, dtype=np.uint8)
+    cv2.fillPoly(mask, vertices_list, (max_value, max_value, max_value))
 
-    # if red channel is hot, image's "Lightness" channel's brightness is lowered
-    red_max_value_ind = mask[:, :, 0] == MAX_VALUES_BY_DTYPE[np.dtype("uint8")]
-    image_hls[:, :, 1][red_max_value_ind] = image_hls[:, :, 1][red_max_value_ind] * 0.5
-
-    image_rgb = cv2.cvtColor(image_hls, cv2.COLOR_HLS2RGB)
+    # Apply shadow to the RGB channels directly
+    # It could be tempting to convert to HLS and apply the shadow to the L channel, but it creates artifacts
+    shadow_intensity = 0.5  # Adjust this value to control the shadow intensity
+    img_shadowed = img.copy()
+    shadowed_indices = mask[:, :, 0] == max_value
+    img_shadowed[shadowed_indices] = (img_shadowed[shadowed_indices] * shadow_intensity).astype(np.uint8)
 
     if needs_float:
-        return to_float(image_rgb, max_value=255)
+        return to_float(img_shadowed, max_value=max_value)
 
-    return image_rgb
+    return img_shadowed
 
 
-@ensure_contiguous
+@contiguous
 @preserve_channel_dim
 def add_gravel(img: np.ndarray, gravels: List[Any]) -> np.ndarray:
     """Add gravel to the image.
 
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
-
     Args:
         img (numpy.ndarray): image to add gravel to
         gravels (list): list of gravel parameters. (float, float, float, float):
             (top-left x, top-left y, bottom-right x, bottom right y)
 
     Returns:
         numpy.ndarray:
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
     """
     non_rgb_warning(img)
     input_dtype = img.dtype
     needs_float = False
 
     if input_dtype == np.float32:
         img = from_float(img, dtype=np.dtype("uint8"))
@@ -951,15 +938,15 @@
         lut *= alpha
     if beta != 0:
         if beta_by_max:
             lut += beta * max_value
         else:
             lut += (alpha * beta) * np.mean(img)
 
-    lut = np.clip(lut, 0, max_value).astype(dtype)
+    lut = clip(lut, img.dtype)
     return cv2.LUT(img, lut)
 
 
 def brightness_contrast_adjust(
     img: np.ndarray,
     alpha: float = 1,
     beta: float = 0,
@@ -975,27 +962,30 @@
 def iso_noise(
     image: np.ndarray,
     color_shift: float = 0.05,
     intensity: float = 0.5,
     random_state: Optional[int] = None,
     **kwargs: Any,
 ) -> np.ndarray:
-    """Apply poisson noise to image to simulate camera sensor noise.
+    """Apply poisson noise to an image to simulate camera sensor noise.
 
     Args:
-        image (numpy.ndarray): Input image, currently, only RGB, uint8 images are supported.
-        color_shift (float):
-        intensity (float): Multiplication factor for noise values. Values of ~0.5 are produce noticeable,
-                   yet acceptable level of noise.
-        random_state:
-        **kwargs:
+        image (np.ndarray): Input image. Currently, only RGB, uint8 images are supported.
+        color_shift (float): The amount of color shift to apply. Default is 0.05.
+        intensity (float): Multiplication factor for noise values. Values of ~0.5 produce a noticeable,
+                           yet acceptable level of noise. Default is 0.5.
+        random_state (Optional[int]): If specified, this will set the random seed for the noise generation,
+                                      ensuring consistent results for the same input and seed.
+        **kwargs: Additional keyword arguments.
 
     Returns:
-        numpy.ndarray: Noised image
+        np.ndarray: The noised image.
 
+    Raises:
+        TypeError: If the input image's dtype is not uint8 or if the image is not RGB.
     """
     if image.dtype != np.uint8:
         msg = "Image must have uint8 channel type"
         raise TypeError(msg)
     if not is_rgb_image(image):
         msg = "Image must be RGB"
         raise TypeError(msg)
@@ -1096,68 +1086,14 @@
         start_y_orig, start_x_orig, end_y_orig, end_x_orig = tiles[num]
         # Assign the corresponding tile from the original image to the new image
         new_image[start_y:end_y, start_x:end_x] = image[start_y_orig:end_y_orig, start_x_orig:end_x_orig]
 
     return new_image
 
 
-@clipped
-def _multiply_uint8(img: np.ndarray, multiplier: np.ndarray) -> np.ndarray:
-    img = img.astype(np.float32)
-    return np.multiply(img, multiplier)
-
-
-@preserve_channel_dim
-def _multiply_uint8_optimized(img: np.ndarray, multiplier: np.ndarray) -> np.ndarray:
-    if is_grayscale_image(img) or len(multiplier) == 1:
-        multiplier = multiplier[0]
-        lut = np.arange(0, 256, dtype=np.float32)
-        lut *= multiplier
-        lut = clip(lut, np.uint8, MAX_VALUES_BY_DTYPE[img.dtype])
-        func = _maybe_process_in_chunks(cv2.LUT, lut=lut)
-        return func(img)
-
-    channels = img.shape[-1]
-    lut = [np.arange(0, 256, dtype=np.float32)] * channels
-    lut = np.stack(lut, axis=-1)
-
-    lut *= multiplier
-    lut = clip(lut, np.uint8, MAX_VALUES_BY_DTYPE[img.dtype])
-
-    images = []
-    for i in range(channels):
-        func = _maybe_process_in_chunks(cv2.LUT, lut=lut[:, i])
-        images.append(func(img[:, :, i]))
-    return np.stack(images, axis=-1)
-
-
-@clipped
-def _multiply_non_uint8(img: np.ndarray, multiplier: np.ndarray) -> np.ndarray:
-    return img * multiplier
-
-
-def multiply(img: np.ndarray, multiplier: np.ndarray) -> np.ndarray:
-    """Args:
-
-        img: Image.
-        multiplier: Multiplier coefficient.
-
-    Returns:
-        Image multiplied by `multiplier` coefficient.
-
-    """
-    if img.dtype == np.uint8:
-        if len(multiplier.shape) == 1:
-            return _multiply_uint8_optimized(img, multiplier)
-
-        return _multiply_uint8(img, multiplier)
-
-    return _multiply_non_uint8(img, multiplier)
-
-
 def bbox_from_mask(mask: np.ndarray) -> Tuple[int, int, int, int]:
     """Create bounding box from binary mask (fast version)
 
     Args:
         mask (numpy.ndarray): binary mask.
 
     Returns:
@@ -1246,43 +1182,31 @@
 
     for idx in range(3):  # RGB
         orig_img[..., idx] += add_vect[idx] * 255
 
     # for image processing it was found that working with float 0.0 to 1.0
     # was easier than integers between 0-255
     # > orig_img /= 255.0
-    orig_img = np.clip(orig_img, 0.0, 255.0)
-
-    # > orig_img *= 255
-    return orig_img.astype(np.uint8)
-
-
-def _adjust_brightness_torchvision_uint8(img: np.ndarray, factor: float) -> np.ndarray:
-    lut = np.arange(0, 256) * factor
-    lut = np.clip(lut, 0, 255).astype(np.uint8)
-    return cv2.LUT(img, lut)
+    return clip(orig_img, np.uint8)
 
 
 @preserve_channel_dim
 def adjust_brightness_torchvision(img: np.ndarray, factor: np.ndarray) -> np:
     if factor == 0:
         return np.zeros_like(img)
     if factor == 1:
         return img
 
-    if img.dtype == np.uint8:
-        return _adjust_brightness_torchvision_uint8(img, factor)
-
-    return clip(img * factor, img.dtype, MAX_VALUES_BY_DTYPE[img.dtype])
+    return multiply(img, factor)
 
 
 def _adjust_contrast_torchvision_uint8(img: np.ndarray, factor: float, mean: np.ndarray) -> np.ndarray:
     lut = np.arange(0, 256) * factor
     lut = lut + mean * (1 - factor)
-    lut = clip(lut, img.dtype, 255)
+    lut = clip(lut, img.dtype)
 
     return cv2.LUT(img, lut)
 
 
 @preserve_channel_dim
 def adjust_contrast_torchvision(img: np.ndarray, factor: float) -> np.ndarray:
     if factor == 1:
@@ -1294,19 +1218,15 @@
         if img.dtype != np.float32:
             mean = int(mean + 0.5)
         return np.full_like(img, mean, dtype=img.dtype)
 
     if img.dtype == np.uint8:
         return _adjust_contrast_torchvision_uint8(img, factor, mean)
 
-    return clip(
-        img.astype(np.float32) * factor + mean * (1 - factor),
-        img.dtype,
-        MAX_VALUES_BY_DTYPE[img.dtype],
-    )
+    return clip(img.astype(np.float32) * factor + mean * (1 - factor), img.dtype)
 
 
 @preserve_channel_dim
 def adjust_saturation_torchvision(img: np.ndarray, factor: float, gamma: float = 0) -> np.ndarray:
     if factor == 1:
         return img
 
@@ -1320,15 +1240,15 @@
         return gray
 
     result = cv2.addWeighted(img, factor, gray, 1 - factor, gamma=gamma)
     if img.dtype == np.uint8:
         return result
 
     # OpenCV does not clip values for float dtype
-    return clip(result, img.dtype, MAX_VALUES_BY_DTYPE[img.dtype])
+    return clip(result, img.dtype)
 
 
 def _adjust_hue_torchvision_uint8(img: np.ndarray, factor: float) -> np.ndarray:
     img = cv2.cvtColor(img, cv2.COLOR_RGB2HSV)
 
     lut = np.arange(0, 256, dtype=np.int16)
     lut = np.mod(lut + 180 * factor, 180).astype(np.uint8)
@@ -1366,28 +1286,28 @@
     orig_shape = image.shape
     if max_size is not None:
         size = max(image.shape[:2])
         if size > max_size:
             scale = max_size / size
             height, width = image.shape[:2]
             new_height, new_width = int(height * scale), int(width * scale)
-            resize_fn = _maybe_process_in_chunks(cv2.resize, dsize=(new_width, new_height), interpolation=interpolation)
+            resize_fn = maybe_process_in_chunks(cv2.resize, dsize=(new_width, new_height), interpolation=interpolation)
             image = resize_fn(image)
 
     segments = skimage.segmentation.slic(
         image,
         n_segments=n_segments,
         compactness=10,
-        channel_axis=-1 if image.ndim > TWO else None,
+        channel_axis=-1 if image.ndim > MONO_CHANNEL_DIMENSIONS else None,
     )
 
     min_value = 0
     max_value = MAX_VALUES_BY_DTYPE[image.dtype]
     image = np.copy(image)
-    if image.ndim == TWO:
+    if image.ndim == MONO_CHANNEL_DIMENSIONS:
         image = image.reshape(*image.shape, 1)
     nb_channels = image.shape[2]
     for c in range(nb_channels):
         # segments+1 here because otherwise regionprops always misses the last label
         regions = skimage.measure.regionprops(segments + 1, intensity_image=image[..., c])
         for ridx, region in enumerate(regions):
             # with mod here, because slic can sometimes create more superpixel than requested.
@@ -1405,15 +1325,15 @@
                     value = min(max(value, min_value), max_value)
                 else:
                     value = mean_intensity
 
                 image_sp_c[segments == ridx] = value
 
     if orig_shape != image.shape:
-        resize_fn = _maybe_process_in_chunks(
+        resize_fn = maybe_process_in_chunks(
             cv2.resize,
             dsize=(orig_shape[1], orig_shape[0]),
             interpolation=interpolation,
         )
         return resize_fn(image)
 
     return image
@@ -1431,15 +1351,15 @@
 def unsharp_mask(
     image: np.ndarray,
     ksize: int,
     sigma: float = 0.0,
     alpha: float = 0.2,
     threshold: int = 10,
 ) -> np.ndarray:
-    blur_fn = _maybe_process_in_chunks(cv2.GaussianBlur, ksize=(ksize, ksize), sigmaX=sigma)
+    blur_fn = maybe_process_in_chunks(cv2.GaussianBlur, ksize=(ksize, ksize), sigmaX=sigma)
 
     input_dtype = image.dtype
     if input_dtype == np.uint8:
         image = to_float(image)
     elif input_dtype not in (np.uint8, np.float32):
         raise ValueError(f"Unexpected dtype {input_dtype} for UnsharpMask augmentation")
 
@@ -1554,17 +1474,23 @@
     random_state: Optional[np.random.RandomState] = None,
 ) -> np.ndarray:
     """Splits an image shape into a uniform grid specified by the grid dimensions.
 
     Args:
         image_shape (Tuple[int, int]): The shape of the image as (height, width).
         grid (Tuple[int, int]): The grid size as (rows, columns).
+        random_state (Optional[np.random.RandomState]): The random state to use for shuffling the splits.
+            If None, the splits are not shuffled.
 
     Returns:
         np.ndarray: An array containing the tiles' coordinates in the format (start_y, start_x, end_y, end_x).
+
+    Note:
+        The function uses `generate_shuffled_splits` to generate the splits for the height and width of the image.
+        The splits are then used to calculate the coordinates of the tiles.
     """
     n_rows, n_cols = grid
 
     height_splits = generate_shuffled_splits(image_shape[0], grid[0], random_state)
     width_splits = generate_shuffled_splits(image_shape[1], grid[1], random_state)
 
     # Calculate tiles coordinates
@@ -1696,7 +1622,20 @@
 def morphology(img: np.ndarray, kernel: np.ndarray, operation: str) -> np.ndarray:
     if operation == "dilation":
         return dilate(img, kernel)
     if operation == "erosion":
         return erode(img, kernel)
 
     raise ValueError(f"Unsupported operation: {operation}")
+
+
+def center(width: NumericType, height: NumericType) -> Tuple[float, float]:
+    """Calculate the center coordinates of a rectangle.
+
+    Args:
+        width (NumericType): The width of the rectangle.
+        height (NumericType): The height of the rectangle.
+
+    Returns:
+        Tuple[float, float]: The center coordinates of the rectangle.
+    """
+    return width / 2 - 0.5, height / 2 - 0.5
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/geometric/functional.py` & `albumentations-1.4.8/albumentations/augmentations/geometric/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import math
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
 
 import cv2
 import numpy as np
 import skimage.transform
+from albucore.utils import clipped, maybe_process_in_chunks, preserve_channel_dim
 from scipy.ndimage import gaussian_filter
 
 from albumentations import random_utils
-from albumentations.augmentations.utils import (
-    _maybe_process_in_chunks,
-    angle_2pi_range,
-    clipped,
-    preserve_channel_dim,
-)
+from albumentations.augmentations.functional import center
+from albumentations.augmentations.utils import angle_2pi_range
 from albumentations.core.bbox_utils import denormalize_bbox, normalize_bbox
 from albumentations.core.types import (
     NUM_MULTI_CHANNEL_DIMENSIONS,
     BoxInternalType,
     ColorType,
     D4Type,
     KeypointInternalType,
@@ -155,28 +152,28 @@
 def keypoint_rot90(
     keypoint: KeypointInternalType,
     factor: int,
     rows: int,
     cols: int,
     **params: Any,
 ) -> KeypointInternalType:
-    """Rotates a keypoint by 90 degrees CCW
+    """Rotate a keypoint by 90 degrees counter-clockwise (CCW) a specified number of times.
 
     Args:
-        keypoint: A keypoint `(x, y, angle, scale)`.
-        factor: Number of CCW rotations. Must be in range [0;3] See np.rot90.
-        rows: Image height.
-        cols: Image width.
+        keypoint (KeypointInternalType): A keypoint in the format `(x, y, angle, scale)`.
+        factor (int): The number of 90 degree CCW rotations to apply. Must be in the range [0, 3].
+        rows (int): The height of the image the keypoint belongs to.
+        cols (int): The width of the image the keypoint belongs to.
+        **params: Additional parameters.
 
     Returns:
-        tuple: A keypoint `(x, y, angle, scale)`.
+        KeypointInternalType: The rotated keypoint in the format `(x, y, angle, scale)`.
 
     Raises:
-        ValueError: if factor not in set {0, 1, 2, 3}
-
+        ValueError: If the factor is not in the set {0, 1, 2, 3}.
     """
     x, y, angle, scale = keypoint
 
     if factor not in {0, 1, 2, 3}:
         raise ValueError("Parameter factor must be in set {0, 1, 2, 3}")
 
     if factor == 1:
@@ -245,19 +242,19 @@
     img: np.ndarray,
     angle: float,
     interpolation: int,
     border_mode: int,
     value: Optional[ColorType] = None,
 ) -> np.ndarray:
     height, width = img.shape[:2]
-    # for images we use additional shifts of (0.5, 0.5) as otherwise
-    # we get an ugly black border for 90deg rotations
-    matrix = cv2.getRotationMatrix2D((width / 2 - 0.5, height / 2 - 0.5), angle, 1.0)
 
-    warp_fn = _maybe_process_in_chunks(
+    image_center = center(width, height)
+    matrix = cv2.getRotationMatrix2D(image_center, angle, 1.0)
+
+    warp_fn = maybe_process_in_chunks(
         cv2.warpAffine,
         M=matrix,
         dsize=(width, height),
         flags=interpolation,
         borderMode=border_mode,
         borderValue=value,
     )
@@ -310,28 +307,31 @@
 def keypoint_rotate(
     keypoint: KeypointInternalType,
     angle: float,
     rows: int,
     cols: int,
     **params: Any,
 ) -> KeypointInternalType:
-    """Rotate a keypoint by angle.
+    """Rotate a keypoint by a specified angle.
 
     Args:
-        keypoint: A keypoint `(x, y, angle, scale)`.
-        angle: Rotation angle.
-        rows: Image height.
-        cols: Image width.
+        keypoint (KeypointInternalType): A keypoint in the format `(x, y, angle, scale)`.
+        angle (float): The angle by which to rotate the keypoint, in degrees.
+        rows (int): The height of the image the keypoint belongs to.
+        cols (int): The width of the image the keypoint belongs to.
+        **params: Additional parameters.
 
     Returns:
-        A keypoint `(x, y, angle, scale)`.
+        KeypointInternalType: The rotated keypoint in the format `(x, y, angle, scale)`.
 
+    Note:
+        The rotation is performed around the center of the image.
     """
-    center = (cols - 1) * 0.5, (rows - 1) * 0.5
-    matrix = cv2.getRotationMatrix2D(center, angle, 1.0)
+    image_center = center(cols, rows)
+    matrix = cv2.getRotationMatrix2D(image_center, angle, 1.0)
     x, y, a, s = keypoint[:4]
     x, y = cv2.transform(np.array([[[x, y]]]), matrix).squeeze()
     return x, y, a + math.radians(angle), s
 
 
 @preserve_channel_dim
 def elastic_transform(
@@ -372,15 +372,15 @@
         dtype=np.float32,
     )
     pts2 = pts1 + random_utils.uniform(-alpha_affine, alpha_affine, size=pts1.shape, random_state=random_state).astype(
         np.float32,
     )
     matrix = cv2.getAffineTransform(pts1, pts2)
 
-    warp_fn = _maybe_process_in_chunks(
+    warp_fn = maybe_process_in_chunks(
         cv2.warpAffine,
         M=matrix,
         dsize=(width, height),
         flags=interpolation,
         borderMode=border_mode,
         borderValue=value,
     )
@@ -412,31 +412,30 @@
             )
 
     x, y = np.meshgrid(np.arange(width), np.arange(height))
 
     map_x = np.float32(x + dx)
     map_y = np.float32(y + dy)
 
-    remap_fn = _maybe_process_in_chunks(
+    remap_fn = maybe_process_in_chunks(
         cv2.remap,
         map1=map_x,
         map2=map_y,
         interpolation=interpolation,
         borderMode=border_mode,
         borderValue=value,
     )
     return remap_fn(img)
 
 
 @preserve_channel_dim
 def resize(img: np.ndarray, height: int, width: int, interpolation: int) -> np.ndarray:
-    img_height, img_width = img.shape[:2]
     if (height, width) == img.shape[:2]:
         return img
-    resize_fn = _maybe_process_in_chunks(cv2.resize, dsize=(width, height), interpolation=interpolation)
+    resize_fn = maybe_process_in_chunks(cv2.resize, dsize=(width, height), interpolation=interpolation)
     return resize_fn(img)
 
 
 @preserve_channel_dim
 def scale(img: np.ndarray, scale: float, interpolation: int) -> np.ndarray:
     height, width = img.shape[:2]
     new_height, new_width = int(height * scale), int(width * scale)
@@ -488,15 +487,15 @@
     max_height: int,
     border_val: Union[float, List[float], np.ndarray],
     border_mode: int,
     keep_size: bool,
     interpolation: int,
 ) -> np.ndarray:
     height, width = img.shape[:2]
-    perspective_func = _maybe_process_in_chunks(
+    perspective_func = maybe_process_in_chunks(
         cv2.warpPerspective,
         M=matrix,
         dsize=(max_width, max_height),
         borderMode=border_mode,
         borderValue=border_val,
         flags=interpolation,
     )
@@ -589,15 +588,15 @@
     mode: int,
     output_shape: Sequence[int],
 ) -> np.ndarray:
     if _is_identity_matrix(matrix):
         return image
 
     dsize = int(np.round(output_shape[1])), int(np.round(output_shape[0]))
-    warp_fn = _maybe_process_in_chunks(
+    warp_fn = maybe_process_in_chunks(
         cv2.warpAffine,
         M=matrix.params[:2],
         dsize=dsize,
         flags=interpolation,
         borderMode=mode,
         borderValue=cval,
     )
@@ -663,15 +662,15 @@
     img: np.ndarray,
     matrix: np.ndarray,
     interpolation: int,
     value: Optional[ColorType] = None,
     border_mode: int = cv2.BORDER_REFLECT_101,
 ) -> np.ndarray:
     height, width = img.shape[:2]
-    warp_fn = _maybe_process_in_chunks(
+    warp_fn = maybe_process_in_chunks(
         cv2.warpAffine,
         M=matrix,
         dsize=(width, height),
         flags=interpolation,
         borderMode=border_mode,
         borderValue=value,
     )
@@ -762,15 +761,15 @@
     The ``n``-th distance map contains at every location ``(y, x)`` the
     euclidean distance to the ``n``-th keypoint.
 
     This function can be used as a helper when augmenting keypoints with a
     method that only supports the augmentation of images.
 
     Args:
-        keypoint: keypoint coordinates
+        keypoints: keypoint coordinates
         height: image height
         width: image width
         inverted (bool): If ``True``, inverted distance maps are returned where each
             distance value d is replaced by ``d/(d+1)``, i.e. the distance
             maps have values in the range ``(0.0, 1.0]`` with ``1.0`` denoting
             exactly the position of the respective keypoint.
 
@@ -1208,15 +1207,15 @@
     h_pad_top: int,
     h_pad_bottom: int,
     w_pad_left: int,
     w_pad_right: int,
     border_mode: int,
     value: Optional[ColorType],
 ) -> np.ndarray:
-    pad_fn = _maybe_process_in_chunks(
+    pad_fn = maybe_process_in_chunks(
         cv2.copyMakeBorder,
         top=h_pad_top,
         bottom=h_pad_bottom,
         left=w_pad_left,
         right=w_pad_right,
         borderType=border_mode,
         value=value,
@@ -1301,15 +1300,15 @@
         yy[start:end] = np.linspace(prev, cur, end - start)
         prev = cur
 
     map_x, map_y = np.meshgrid(xx, yy)
     map_x = map_x.astype(np.float32)
     map_y = map_y.astype(np.float32)
 
-    remap_fn = _maybe_process_in_chunks(
+    remap_fn = maybe_process_in_chunks(
         cv2.remap,
         map1=map_x,
         map2=map_y,
         interpolation=interpolation,
         borderMode=border_mode,
         borderValue=value,
     )
@@ -1353,15 +1352,15 @@
         dtype=np.float32,
     )
     pts2 = pts1 + random_utils.uniform(-alpha_affine, alpha_affine, size=pts1.shape, random_state=random_state).astype(
         np.float32,
     )
     matrix = cv2.getAffineTransform(pts1, pts2)
 
-    warp_fn = _maybe_process_in_chunks(
+    warp_fn = maybe_process_in_chunks(
         cv2.warpAffine,
         M=matrix,
         dsize=(width, height),
         flags=interpolation,
         borderMode=border_mode,
         borderValue=value,
     )
@@ -1376,15 +1375,15 @@
     dy *= alpha
 
     x, y = np.meshgrid(np.arange(width), np.arange(height))
 
     map_x = np.float32(x + dx)
     map_y = np.float32(y + dy)
 
-    remap_fn = _maybe_process_in_chunks(
+    remap_fn = maybe_process_in_chunks(
         cv2.remap,
         map1=map_x,
         map2=map_y,
         interpolation=interpolation,
         borderMode=border_mode,
         borderValue=value,
     )
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/geometric/resize.py` & `albumentations-1.4.8/albumentations/augmentations/geometric/resize.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     BoxInternalType,
     KeypointInternalType,
     ScaleFloatType,
     Targets,
 )
 from albumentations.core.utils import to_tuple
 
-from . import functional as F
+from . import functional as fgeometric
 
 __all__ = ["RandomScale", "LongestMaxSize", "SmallestMaxSize", "Resize"]
 
 
 class RandomScale(DualTransform):
     """Randomly resize the input. Output image size is different from the input image size.
 
@@ -72,27 +72,27 @@
     def apply(
         self,
         img: np.ndarray,
         scale: float,
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.scale(img, scale, interpolation)
+        return fgeometric.scale(img, scale, interpolation)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         # Bounding box coordinates are scale invariant
         return bbox
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         scale: float,
         **params: Any,
     ) -> KeypointInternalType:
-        return F.keypoint_scale(keypoint, scale, scale)
+        return fgeometric.keypoint_scale(keypoint, scale, scale)
 
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {"interpolation": self.interpolation, "scale_limit": to_tuple(self.scale_limit, bias=-1.0)}
 
 
 class MaxSizeInitSchema(BaseTransformInitSchema):
     max_size: Union[int, List[int]] = Field(
@@ -149,15 +149,15 @@
     def apply(
         self,
         img: np.ndarray,
         max_size: int,
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.longest_max_size(img, max_size=max_size, interpolation=interpolation)
+        return fgeometric.longest_max_size(img, max_size=max_size, interpolation=interpolation)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         # Bounding box coordinates are scale invariant
         return bbox
 
     def apply_to_keypoint(
         self,
@@ -165,15 +165,15 @@
         max_size: int,
         **params: Any,
     ) -> KeypointInternalType:
         height = params["rows"]
         width = params["cols"]
 
         scale = max_size / max([height, width])
-        return F.keypoint_scale(keypoint, scale, scale)
+        return fgeometric.keypoint_scale(keypoint, scale, scale)
 
     def get_params(self) -> Dict[str, int]:
         return {"max_size": self.max_size if isinstance(self.max_size, int) else random.choice(self.max_size)}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("max_size", "interpolation")
 
@@ -214,30 +214,30 @@
     def apply(
         self,
         img: np.ndarray,
         max_size: int,
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.smallest_max_size(img, max_size=max_size, interpolation=interpolation)
+        return fgeometric.smallest_max_size(img, max_size=max_size, interpolation=interpolation)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         return bbox
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         max_size: int,
         **params: Any,
     ) -> KeypointInternalType:
         height = params["rows"]
         width = params["cols"]
 
         scale = max_size / min([height, width])
-        return F.keypoint_scale(keypoint, scale, scale)
+        return fgeometric.keypoint_scale(keypoint, scale, scale)
 
     def get_params(self) -> Dict[str, int]:
         return {"max_size": self.max_size if isinstance(self.max_size, int) else random.choice(self.max_size)}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("max_size", "interpolation")
 
@@ -279,22 +279,22 @@
     ):
         super().__init__(always_apply, p)
         self.height = height
         self.width = width
         self.interpolation = interpolation
 
     def apply(self, img: np.ndarray, interpolation: int, **params: Any) -> np.ndarray:
-        return F.resize(img, height=self.height, width=self.width, interpolation=interpolation)
+        return fgeometric.resize(img, height=self.height, width=self.width, interpolation=interpolation)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         # Bounding box coordinates are scale invariant
         return bbox
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
         height = params["rows"]
         width = params["cols"]
         scale_x = self.width / width
         scale_y = self.height / height
-        return F.keypoint_scale(keypoint, scale_x, scale_y)
+        return fgeometric.keypoint_scale(keypoint, scale_x, scale_y)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("height", "width", "interpolation")
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/geometric/rotate.py` & `albumentations-1.4.8/albumentations/augmentations/geometric/rotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from typing import Any, Dict, List, Optional, Tuple, cast
 
 import cv2
 import numpy as np
 from pydantic import Field
 from typing_extensions import Literal
 
-from albumentations.augmentations.crops import functional as FCrops
+from albumentations.augmentations.crops import functional as fcrops
+from albumentations.augmentations.functional import center
 from albumentations.core.pydantic import BorderModeType, InterpolationType, SymmetricRangeType
 from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
 from albumentations.core.types import (
     BoxInternalType,
     ColorType,
     KeypointInternalType,
     ScaleFloatType,
     Targets,
 )
 
-from . import functional as F
+from . import functional as fgeometric
 
 __all__ = ["Rotate", "RandomRotate90", "SafeRotate"]
 
 SMALL_NUMBER = 1e-10
 
 
 class RandomRotate90(DualTransform):
@@ -49,18 +50,18 @@
         return np.ascontiguousarray(np.rot90(img, factor))
 
     def get_params(self) -> Dict[str, int]:
         # Random int in the range [0, 3]
         return {"factor": random.randint(0, 3)}
 
     def apply_to_bbox(self, bbox: BoxInternalType, factor: int, **params: Any) -> BoxInternalType:
-        return F.bbox_rot90(bbox, factor, **params)
+        return fgeometric.bbox_rot90(bbox, factor, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, factor: int, **params: Any) -> BoxInternalType:
-        return F.keypoint_rot90(keypoint, factor, **params)
+        return fgeometric.keypoint_rot90(keypoint, factor, **params)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class RotateInitSchema(BaseTransformInitSchema):
     limit: SymmetricRangeType = (-90, 90)
@@ -141,66 +142,66 @@
         interpolation: int,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> np.ndarray:
-        img_out = F.rotate(img, angle, interpolation, self.border_mode, self.value)
+        img_out = fgeometric.rotate(img, angle, interpolation, self.border_mode, self.value)
         if self.crop_border:
-            return FCrops.crop(img_out, x_min, y_min, x_max, y_max)
+            return fcrops.crop(img_out, x_min, y_min, x_max, y_max)
         return img_out
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
         angle: float,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         **params: Any,
     ) -> np.ndarray:
-        img_out = F.rotate(mask, angle, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
+        img_out = fgeometric.rotate(mask, angle, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
         if self.crop_border:
-            return FCrops.crop(img_out, x_min, y_min, x_max, y_max)
+            return fcrops.crop(img_out, x_min, y_min, x_max, y_max)
         return img_out
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         angle: float,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         cols: int,
         rows: int,
         **params: Any,
     ) -> np.ndarray:
-        bbox_out = F.bbox_rotate(bbox, angle, self.rotate_method, rows, cols)
+        bbox_out = fgeometric.bbox_rotate(bbox, angle, self.rotate_method, rows, cols)
         if self.crop_border:
-            return FCrops.bbox_crop(bbox_out, x_min, y_min, x_max, y_max, rows, cols)
+            return fcrops.bbox_crop(bbox_out, x_min, y_min, x_max, y_max, rows, cols)
         return bbox_out
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         angle: float,
         x_min: int,
         x_max: int,
         y_min: int,
         y_max: int,
         cols: int,
         rows: int,
         **params: Any,
     ) -> KeypointInternalType:
-        keypoint_out = F.keypoint_rotate(keypoint, angle, rows, cols, **params)
+        keypoint_out = fgeometric.keypoint_rotate(keypoint, angle, rows, cols, **params)
         if self.crop_border:
-            return FCrops.crop_keypoint_by_coords(keypoint_out, (x_min, y_min, x_max, y_max))
+            return fcrops.crop_keypoint_by_coords(keypoint_out, (x_min, y_min, x_max, y_max))
         return keypoint_out
 
     @staticmethod
     def _rotated_rect_with_max_area(height: int, width: int, angle: float) -> Dict[str, int]:
         """Given a rectangle of size wxh that has been rotated by 'angle' (in
         degrees), computes the width and height of the largest possible
         axis-aligned rectangle (maximal area) within the rotated rectangle.
@@ -299,46 +300,46 @@
         self.limit = cast(Tuple[float, float], limit)
         self.interpolation = interpolation
         self.border_mode = border_mode
         self.value = value
         self.mask_value = mask_value
 
     def apply(self, img: np.ndarray, matrix: np.ndarray, **params: Any) -> np.ndarray:
-        return F.safe_rotate(img, matrix, self.interpolation, self.value, self.border_mode)
+        return fgeometric.safe_rotate(img, matrix, self.interpolation, self.value, self.border_mode)
 
     def apply_to_mask(self, mask: np.ndarray, matrix: np.ndarray, **params: Any) -> np.ndarray:
-        return F.safe_rotate(mask, matrix, cv2.INTER_NEAREST, self.mask_value, self.border_mode)
+        return fgeometric.safe_rotate(mask, matrix, cv2.INTER_NEAREST, self.mask_value, self.border_mode)
 
     def apply_to_bbox(self, bbox: BoxInternalType, cols: int, rows: int, **params: Any) -> BoxInternalType:
-        return F.bbox_safe_rotate(bbox, params["matrix"], cols, rows)
+        return fgeometric.bbox_safe_rotate(bbox, params["matrix"], cols, rows)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         angle: float,
         scale_x: float,
         scale_y: float,
         cols: int,
         rows: int,
         **params: Any,
     ) -> KeypointInternalType:
-        return F.keypoint_safe_rotate(keypoint, params["matrix"], angle, scale_x, scale_y, cols, rows)
+        return fgeometric.keypoint_safe_rotate(keypoint, params["matrix"], angle, scale_x, scale_y, cols, rows)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         angle = random.uniform(self.limit[0], self.limit[1])
 
         image = params["image"]
         height, width = image.shape[:2]
 
         # https://stackoverflow.com/questions/43892506/opencv-python-rotate-image-without-cropping-sides
-        image_center = (width / 2, height / 2)
+        image_center = center(width, height)
 
         # Rotation Matrix
         rotation_mat = cv2.getRotationMatrix2D(image_center, angle, 1.0)
 
         # rotation calculates the cos and sin, taking absolutes of those.
         abs_cos = abs(rotation_mat[0, 0])
         abs_sin = abs(rotation_mat[0, 1])
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/geometric/transforms.py` & `albumentations-1.4.8/albumentations/augmentations/geometric/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import math
 import random
 from enum import Enum
-from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union, cast
+from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, Tuple, Union, cast
 from warnings import warn
 
 import cv2
 import numpy as np
 import skimage.transform
+from albucore.utils import get_num_channels
 from pydantic import Field, ValidationInfo, field_validator, model_validator
 from typing_extensions import Annotated, Self
 
 from albumentations import random_utils
-from albumentations.augmentations.functional import bbox_from_mask
-from albumentations.augmentations.utils import BIG_INTEGER, check_range, get_num_channels
+from albumentations.augmentations.functional import bbox_from_mask, center
+from albumentations.augmentations.utils import check_range
 from albumentations.core.bbox_utils import denormalize_bbox, normalize_bbox
 from albumentations.core.pydantic import (
     BorderModeType,
     InterpolationType,
     NonNegativeFloatRangeType,
     ProbabilityType,
     SymmetricRangeType,
 )
 from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
 from albumentations.core.types import (
+    BIG_INTEGER,
     NUM_MULTI_CHANNEL_DIMENSIONS,
+    TWO,
     BoxInternalType,
     ColorType,
     D4Type,
     KeypointInternalType,
     ScaleFloatType,
     ScaleIntType,
     SizeType,
     Targets,
     d4_group_elements,
 )
 from albumentations.core.utils import to_tuple
 
-from . import functional as F
+from . import functional as fgeometric
 
 __all__ = [
     "ShiftScaleRotate",
     "ElasticTransform",
     "Perspective",
     "Affine",
     "PiecewiseAffine",
@@ -50,16 +53,14 @@
     "Transpose",
     "OpticalDistortion",
     "GridDistortion",
     "PadIfNeeded",
     "D4",
 ]
 
-TWO = 2
-
 
 class ElasticTransform(DualTransform):
     """Elastic deformation of images as described in [Simard2003]_ (with modifications).
 
     .. [Simard2003] Simard, Steinkraus and Platt, "Best Practices for
          Convolutional Neural Networks applied to Visual Document Analysis", in
          Proc. of the International Conference on Document Analysis and
@@ -142,29 +143,29 @@
     def apply(
         self,
         img: np.ndarray,
         random_seed: int,
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.elastic_transform(
+        return fgeometric.elastic_transform(
             img,
             self.alpha,
             self.sigma,
             self.alpha_affine,
             interpolation,
             self.border_mode,
             self.value,
             np.random.RandomState(random_seed),
             self.approximate,
             self.same_dxdy,
         )
 
     def apply_to_mask(self, mask: np.ndarray, random_seed: int, **params: Any) -> np.ndarray:
-        return F.elastic_transform(
+        return fgeometric.elastic_transform(
             mask,
             self.alpha,
             self.sigma,
             self.alpha_affine,
             cv2.INTER_NEAREST,
             self.border_mode,
             self.mask_value,
@@ -177,31 +178,31 @@
         self,
         bbox: BoxInternalType,
         random_seed: int,
         **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
-        bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
+        bbox_denorm = fgeometric.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
         mask[y_min:y_max, x_min:x_max] = 1
-        mask = F.elastic_transform(
+        mask = fgeometric.elastic_transform(
             mask,
             self.alpha,
             self.sigma,
             self.alpha_affine,
             cv2.INTER_NEAREST,
             self.border_mode,
             self.mask_value,
             np.random.RandomState(random_seed),
             self.approximate,
         )
         bbox_returned = bbox_from_mask(mask)
-        return cast(BoxInternalType, F.normalize_bbox(bbox_returned, rows, cols))
+        return cast(BoxInternalType, fgeometric.normalize_bbox(bbox_returned, rows, cols))
 
     def get_params(self) -> Dict[str, int]:
         return {"random_seed": random_utils.get_random_seed()}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (
             "alpha",
@@ -211,14 +212,23 @@
             "border_mode",
             "value",
             "mask_value",
             "approximate",
             "same_dxdy",
         )
 
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+            "bboxes": self.apply_to_bboxes,
+        }
+
 
 class Perspective(DualTransform):
     """Perform a random four point perspective transform of the input.
 
     Args:
         scale: standard deviation of the normal distributions. These are used to sample
             the random distances of the subimage's corners from the full image's corners.
@@ -288,15 +298,15 @@
         self,
         img: np.ndarray,
         matrix: np.ndarray,
         max_height: int,
         max_width: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.perspective(
+        return fgeometric.perspective(
             img,
             matrix,
             max_width,
             max_height,
             self.pad_val,
             self.pad_mode,
             self.keep_size,
@@ -307,25 +317,33 @@
         self,
         bbox: BoxInternalType,
         matrix: np.ndarray,
         max_height: int,
         max_width: int,
         **params: Any,
     ) -> BoxInternalType:
-        return F.perspective_bbox(bbox, params["rows"], params["cols"], matrix, max_width, max_height, self.keep_size)
+        return fgeometric.perspective_bbox(
+            bbox,
+            params["rows"],
+            params["cols"],
+            matrix,
+            max_width,
+            max_height,
+            self.keep_size,
+        )
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         matrix: np.ndarray,
         max_height: int,
         max_width: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.perspective_keypoint(
+        return fgeometric.perspective_keypoint(
             keypoint,
             params["rows"],
             params["cols"],
             matrix,
             max_width,
             max_height,
             self.keep_size,
@@ -682,15 +700,15 @@
     def apply(
         self,
         img: np.ndarray,
         matrix: skimage.transform.ProjectiveTransform,
         output_shape: Sequence[int],
         **params: Any,
     ) -> np.ndarray:
-        return F.warp_affine(
+        return fgeometric.warp_affine(
             img,
             matrix,
             interpolation=self.interpolation,
             cval=self.cval,
             mode=self.mode,
             output_shape=output_shape,
         )
@@ -698,15 +716,15 @@
     def apply_to_mask(
         self,
         mask: np.ndarray,
         matrix: skimage.transform.ProjectiveTransform,
         output_shape: Sequence[int],
         **params: Any,
     ) -> np.ndarray:
-        return F.warp_affine(
+        return fgeometric.warp_affine(
             mask,
             matrix,
             interpolation=self.mask_interpolation,
             cval=self.cval_mask,
             mode=self.mode,
             output_shape=output_shape,
         )
@@ -716,15 +734,15 @@
         bbox: BoxInternalType,
         matrix: skimage.transform.ProjectiveTransform,
         rows: int,
         cols: int,
         output_shape: Sequence[int],
         **params: Any,
     ) -> BoxInternalType:
-        return F.bbox_affine(bbox, matrix, self.rotate_method, rows, cols, output_shape)
+        return fgeometric.bbox_affine(bbox, matrix, self.rotate_method, rows, cols, output_shape)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         matrix: skimage.transform.ProjectiveTransform,
         scale: Dict[str, Any],
         **params: Any,
@@ -732,15 +750,15 @@
         if scale is None:
             msg = "Expected scale to be provided, but got None."
             raise ValueError(msg)
         if matrix is None:
             msg = "Expected matrix to be provided, but got None."
             raise ValueError(msg)
 
-        return F.keypoint_affine(keypoint, matrix=matrix, scale=scale)
+        return fgeometric.keypoint_affine(keypoint, matrix=matrix, scale=scale)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         height, width = params["image"].shape[:2]
@@ -760,18 +778,15 @@
         scale = {key: random.uniform(*value) for key, value in self.scale.items()}
         if self.keep_ratio:
             scale["y"] = scale["x"]
 
         # Look to issue https://github.com/albumentations-team/albumentations/issues/1079
         rotate = -random.uniform(*self.rotate)
 
-        # for images we use additional shifts of (0.5, 0.5) as otherwise
-        # we get an ugly black border for 90deg rotations
-        shift_x = width / 2 - 0.5
-        shift_y = height / 2 - 0.5
+        shift_x, shift_y = center(width, height)
 
         matrix_to_topleft = skimage.transform.SimilarityTransform(translation=[-shift_x, -shift_y])
         matrix_shear_y_rot = skimage.transform.AffineTransform(rotation=-np.pi / 2)
         matrix_shear_y = skimage.transform.AffineTransform(shear=np.deg2rad(shear["y"]))
         matrix_shear_y_rot_inv = skimage.transform.AffineTransform(rotation=np.pi / 2)
         matrix_transforms = skimage.transform.AffineTransform(
             scale=(scale["x"], scale["y"]),
@@ -1064,15 +1079,18 @@
         absolute_scale: bool = False,
         always_apply: bool = False,
         keypoints_threshold: float = 0.01,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
 
-        warn("This augmenter is very slow. Try to use ``ElasticTransformation`` instead, which is at least 10x faster.")
+        warn(
+            "This augmenter is very slow. Try to use ``ElasticTransformation`` instead, which is at least 10x faster.",
+            stacklevel=2,
+        )
 
         self.scale = cast(Tuple[float, float], scale)
         self.nb_rows = cast(Tuple[int, int], nb_rows)
         self.nb_cols = cast(Tuple[int, int], nb_cols)
         self.interpolation = interpolation
         self.mask_interpolation = mask_interpolation
         self.cval = cval
@@ -1152,43 +1170,43 @@
 
     def apply(
         self,
         img: np.ndarray,
         matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> np.ndarray:
-        return F.piecewise_affine(img, matrix, self.interpolation, self.mode, self.cval)
+        return fgeometric.piecewise_affine(img, matrix, self.interpolation, self.mode, self.cval)
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
         matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> np.ndarray:
-        return F.piecewise_affine(mask, matrix, self.mask_interpolation, self.mode, self.cval_mask)
+        return fgeometric.piecewise_affine(mask, matrix, self.mask_interpolation, self.mode, self.cval_mask)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         rows: int,
         cols: int,
         matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> BoxInternalType:
-        return F.bbox_piecewise_affine(bbox, matrix, rows, cols, self.keypoints_threshold)
+        return fgeometric.bbox_piecewise_affine(bbox, matrix, rows, cols, self.keypoints_threshold)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         rows: int,
         cols: int,
         matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> KeypointInternalType:
-        return F.keypoint_piecewise_affine(keypoint, matrix, rows, cols, self.keypoints_threshold)
+        return fgeometric.keypoint_piecewise_affine(keypoint, matrix, rows, cols, self.keypoints_threshold)
 
 
 class PadIfNeeded(DualTransform):
     """Pads the sides of an image if the image dimensions are less than the specified minimum dimensions.
     If the `pad_height_divisor` or `pad_width_divisor` is specified, the function additionally ensures
     that the image dimensions are divisible by these values.
 
@@ -1361,15 +1379,15 @@
         img: np.ndarray,
         pad_top: int,
         pad_bottom: int,
         pad_left: int,
         pad_right: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.pad_with_params(
+        return fgeometric.pad_with_params(
             img,
             pad_top,
             pad_bottom,
             pad_left,
             pad_right,
             border_mode=self.border_mode,
             value=self.value,
@@ -1380,15 +1398,15 @@
         mask: np.ndarray,
         pad_top: int,
         pad_bottom: int,
         pad_left: int,
         pad_right: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.pad_with_params(
+        return fgeometric.pad_with_params(
             mask,
             pad_top,
             pad_bottom,
             pad_left,
             pad_right,
             border_mode=self.border_mode,
             value=self.mask_value,
@@ -1488,21 +1506,21 @@
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        return F.vflip(img)
+        return fgeometric.vflip(img)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_vflip(bbox, **params)
+        return fgeometric.bbox_vflip(bbox, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
-        return F.keypoint_vflip(keypoint, **params)
+        return fgeometric.keypoint_vflip(keypoint, **params)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class HorizontalFlip(DualTransform):
     """Flip the input horizontally around the y-axis.
@@ -1520,23 +1538,23 @@
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         if get_num_channels(img) > 1 and img.dtype == np.uint8:
             # Opencv is faster than numpy only in case of
             # non-gray scale 8bits images
-            return F.hflip_cv2(img)
+            return fgeometric.hflip_cv2(img)
 
-        return F.hflip(img)
+        return fgeometric.hflip(img)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_hflip(bbox, **params)
+        return fgeometric.bbox_hflip(bbox, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
-        return F.keypoint_hflip(keypoint, **params)
+        return fgeometric.keypoint_hflip(keypoint, **params)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class Flip(DualTransform):
     """Flip the input either horizontally, vertically or both horizontally and vertically.
@@ -1556,25 +1574,25 @@
 
     def apply(self, img: np.ndarray, d: int, **params: Any) -> np.ndarray:
         """Args:
         d (int): code that specifies how to flip the input. 0 for vertical flipping, 1 for horizontal flipping,
                 -1 for both vertical and horizontal flipping (which is also could be seen as rotating the input by
                 180 degrees).
         """
-        return F.random_flip(img, d)
+        return fgeometric.random_flip(img, d)
 
     def get_params(self) -> Dict[str, int]:
         # Random int in the range [-1, 1]
         return {"d": random.randint(-1, 1)}
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_flip(bbox, **params)
+        return fgeometric.bbox_flip(bbox, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
-        return F.keypoint_flip(keypoint, **params)
+        return fgeometric.keypoint_flip(keypoint, **params)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class Transpose(DualTransform):
     """Transpose the input by swapping rows and columns.
@@ -1589,21 +1607,21 @@
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        return F.transpose(img)
+        return fgeometric.transpose(img)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_transpose(bbox, **params)
+        return fgeometric.bbox_transpose(bbox, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
-        return F.keypoint_transpose(keypoint, **params)
+        return fgeometric.keypoint_transpose(keypoint, **params)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class OpticalDistortion(DualTransform):
     """Args:
@@ -1670,36 +1688,36 @@
         img: np.ndarray,
         k: int,
         dx: int,
         dy: int,
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.optical_distortion(img, k, dx, dy, interpolation, self.border_mode, self.value)
+        return fgeometric.optical_distortion(img, k, dx, dy, interpolation, self.border_mode, self.value)
 
     def apply_to_mask(self, mask: np.ndarray, k: int, dx: int, dy: int, **params: Any) -> np.ndarray:
-        return F.optical_distortion(mask, k, dx, dy, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
+        return fgeometric.optical_distortion(mask, k, dx, dy, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         k: int,
         dx: int,
         dy: int,
         **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
-        bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
+        bbox_denorm = fgeometric.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
         mask[y_min:y_max, x_min:x_max] = 1
-        mask = F.optical_distortion(mask, k, dx, dy, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
+        mask = fgeometric.optical_distortion(mask, k, dx, dy, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
         bbox_returned = bbox_from_mask(mask)
-        return cast(BoxInternalType, F.normalize_bbox(bbox_returned, rows, cols))
+        return cast(BoxInternalType, fgeometric.normalize_bbox(bbox_returned, rows, cols))
 
     def get_params(self) -> Dict[str, Any]:
         return {
             "k": random.uniform(self.distort_limit[0], self.distort_limit[1]),
             "dx": round(random.uniform(self.shift_limit[0], self.shift_limit[1])),
             "dy": round(random.uniform(self.shift_limit[0], self.shift_limit[1])),
         }
@@ -1710,14 +1728,23 @@
             "shift_limit",
             "interpolation",
             "border_mode",
             "value",
             "mask_value",
         )
 
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+            "bboxes": self.apply_to_bboxes,
+        }
+
 
 class GridDistortion(DualTransform):
     """Applies grid distortion augmentation to images, masks, and bounding boxes. This technique involves dividing
     the image into a grid of cells and randomly displacing the intersection points of the grid,
     resulting in localized distortions.
 
     Args:
@@ -1803,24 +1830,32 @@
         self,
         img: np.ndarray,
         stepsx: Tuple[()],
         stepsy: Tuple[()],
         interpolation: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.grid_distortion(img, self.num_steps, stepsx, stepsy, interpolation, self.border_mode, self.value)
+        return fgeometric.grid_distortion(
+            img,
+            self.num_steps,
+            stepsx,
+            stepsy,
+            interpolation,
+            self.border_mode,
+            self.value,
+        )
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
         stepsx: Tuple[()],
         stepsy: Tuple[()],
         **params: Any,
     ) -> np.ndarray:
-        return F.grid_distortion(
+        return fgeometric.grid_distortion(
             mask,
             self.num_steps,
             stepsx,
             stepsy,
             cv2.INTER_NEAREST,
             self.border_mode,
             self.mask_value,
@@ -1831,29 +1866,29 @@
         bbox: BoxInternalType,
         stepsx: Tuple[()],
         stepsy: Tuple[()],
         **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
-        bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
+        bbox_denorm = fgeometric.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
         mask[y_min:y_max, x_min:x_max] = 1
-        mask = F.grid_distortion(
+        mask = fgeometric.grid_distortion(
             mask,
             self.num_steps,
             stepsx,
             stepsy,
             cv2.INTER_NEAREST,
             self.border_mode,
             self.mask_value,
         )
         bbox_returned = bbox_from_mask(mask)
-        return cast(BoxInternalType, F.normalize_bbox(bbox_returned, rows, cols))
+        return cast(BoxInternalType, fgeometric.normalize_bbox(bbox_returned, rows, cols))
 
     def _normalize(self, h: int, w: int, xsteps: List[float], ysteps: List[float]) -> Dict[str, Any]:
         # compensate for smaller last steps in source image.
         x_step = w // self.num_steps
         last_x_step = min(w, ((self.num_steps + 1) * x_step)) - (self.num_steps * x_step)
         xsteps[-1] *= last_x_step / x_step
 
@@ -1887,14 +1922,23 @@
             return self._normalize(height, width, stepsx, stepsy)
 
         return {"stepsx": stepsx, "stepsy": stepsy}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return "num_steps", "distort_limit", "interpolation", "border_mode", "value", "mask_value", "normalized"
 
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+            "bboxes": self.apply_to_bboxes,
+        }
+
 
 class D4(DualTransform):
     """Applies one of the eight possible D4 dihedral group transformations to a square-shaped input,
         maintaining the square shape. These transformations correspond to the symmetries of a square,
         including rotations and reflections.
 
     The D4 group transformations include:
@@ -1936,26 +1980,26 @@
         self,
         always_apply: bool = False,
         p: float = 1,
     ):
         super().__init__(always_apply, p)
 
     def apply(self, img: np.ndarray, group_element: D4Type, **params: Any) -> np.ndarray:
-        return F.d4(img, group_element)
+        return fgeometric.d4(img, group_element)
 
     def apply_to_bbox(self, bbox: BoxInternalType, group_element: D4Type, **params: Any) -> BoxInternalType:
-        return F.bbox_d4(bbox, group_element, **params)
+        return fgeometric.bbox_d4(bbox, group_element, **params)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         group_element: D4Type,
         **params: Any,
     ) -> KeypointInternalType:
-        return F.keypoint_d4(keypoint, group_element, **params)
+        return fgeometric.keypoint_d4(keypoint, group_element, **params)
 
     def get_params(self) -> Dict[str, D4Type]:
         return {
             "group_element": random_utils.choice(d4_group_elements),
         }
 
     def get_transform_init_args_names(self) -> Tuple[()]:
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/mixing/transforms.py` & `albumentations-1.4.8/albumentations/augmentations/mixing/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import random
 import types
 from typing import Any, Callable, Dict, Generator, Iterable, Iterator, List, Optional, Sequence, Tuple, Union
 from warnings import warn
 
 import numpy as np
+from albucore.utils import is_grayscale_image
 from pydantic import Field
 from typing_extensions import Annotated
 
 from albumentations.augmentations.functional import add_weighted
-from albumentations.augmentations.utils import is_grayscale_image
 from albumentations.core.transforms_interface import BaseTransformInitSchema, ReferenceBasedTransform
 from albumentations.core.types import BoxType, KeypointType, ReferenceImage, Targets
 from albumentations.random_utils import beta
 
 __all__ = ["MixUp"]
 
 
@@ -126,15 +126,15 @@
         super().__init__(always_apply, p)
         self.mix_coef_return_name = mix_coef_return_name
 
         self.read_fn = read_fn
         self.alpha = alpha
 
         if reference_data is None:
-            warn("No reference data provided for MixUp. This transform will act as a no-op.")
+            warn("No reference data provided for MixUp. This transform will act as a no-op.", stacklevel=2)
             # Create an empty generator
             self.reference_data: List[Any] = []
         elif (
             isinstance(reference_data, types.GeneratorType)
             or isinstance(reference_data, Iterable)
             and not isinstance(reference_data, str)
         ):
@@ -199,14 +199,15 @@
             try:
                 mix_data = next(self.reference_data)  # Attempt to get the next item
             except StopIteration:
                 warn(
                     "Reference data iterator/generator has been exhausted. "
                     "Further mixing augmentations will not be applied.",
                     RuntimeWarning,
+                    stacklevel=2,
                 )
                 return {"mix_data": {}, "mix_coef": 1}
 
         # If mix_data is None or empty after the above checks, return default values
         if mix_data is None:
             return {"mix_data": {}, "mix_coef": 1}
```

### Comparing `albumentations-1.4.7/albumentations/augmentations/transforms.py` & `albumentations-1.4.8/albumentations/augmentations/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,48 +4,48 @@
 import warnings
 from types import LambdaType
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
 from warnings import warn
 
 import cv2
 import numpy as np
+from albucore.functions import multiply
+from albucore.utils import get_num_channels, is_grayscale_image, is_rgb_image
 from pydantic import AfterValidator, BaseModel, Field, ValidationInfo, field_validator, model_validator
 from scipy import special
 from scipy.ndimage import gaussian_filter
 from typing_extensions import Annotated, Literal, Self, TypedDict
 
 from albumentations import random_utils
 from albumentations.augmentations.blur.functional import blur
 from albumentations.augmentations.blur.transforms import BlurInitSchema, process_blur_limit
-from albumentations.augmentations.utils import (
-    check_range,
-    get_num_channels,
-    is_grayscale_image,
-    is_rgb_image,
-)
+from albumentations.augmentations.utils import check_range
 from albumentations.core.pydantic import (
     InterpolationType,
     NonNegativeFloatRangeType,
     OnePlusFloatRangeType,
     OnePlusIntNonDecreasingRangeType,
     OnePlusIntRangeType,
     ProbabilityType,
     SymmetricRangeType,
     ZeroOneRangeType,
-    check_01_range,
-    check_nondecreasing_range,
+    check_0plus,
+    check_01,
+    check_1plus,
+    nondecreasing,
 )
 from albumentations.core.transforms_interface import (
     BaseTransformInitSchema,
     DualTransform,
     ImageOnlyTransform,
     Interpolation,
     NoOp,
 )
 from albumentations.core.types import (
+    MAX_RAIN_ANGLE,
     MONO_CHANNEL_DIMENSIONS,
     NUM_RGB_CHANNELS,
     BoxInternalType,
     ChromaticAberrationMode,
     ColorType,
     ImageCompressionType,
     ImageMode,
@@ -56,15 +56,15 @@
     ScaleIntType,
     ScaleType,
     SpatterMode,
     Targets,
 )
 from albumentations.core.utils import format_args, to_tuple
 
-from . import functional as F
+from . import functional as fmain
 
 __all__ = [
     "Normalize",
     "RandomGamma",
     "RandomGridShuffle",
     "HueSaturationValue",
     "RGBShift",
@@ -153,18 +153,18 @@
     _targets = (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS)
 
     def __init__(self, grid: Tuple[int, int] = (3, 3), always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply=always_apply, p=p)
         self.grid = grid
 
     def apply(self, img: np.ndarray, tiles: np.ndarray, mapping: List[int], **params: Any) -> np.ndarray:
-        return F.swap_tiles_on_image(img, tiles, mapping)
+        return fmain.swap_tiles_on_image(img, tiles, mapping)
 
     def apply_to_mask(self, mask: np.ndarray, tiles: np.ndarray, mapping: List[int], **params: Any) -> np.ndarray:
-        return F.swap_tiles_on_image(mask, tiles, mapping)
+        return fmain.swap_tiles_on_image(mask, tiles, mapping)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         tiles: np.ndarray,
         mapping: List[int],
         **params: Any,
@@ -185,37 +185,47 @@
 
                 return (new_x, new_y, *keypoint[2:])
 
         # If the keypoint wasn't in any tile (shouldn't happen), log a warning for debugging purposes
         warn(
             "Keypoint not in any tile, returning it unchanged. This is unexpected and should be investigated.",
             RuntimeWarning,
+            stacklevel=2,
         )
         return keypoint
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
         height, width = params["image"].shape[:2]
         random_state = random_utils.get_random_state()
-        original_tiles = F.split_uniform_grid(
+        original_tiles = fmain.split_uniform_grid(
             (height, width),
             self.grid,
             random_state=random_state,
         )
-        shape_groups = F.create_shape_groups(original_tiles)
-        mapping = F.shuffle_tiles_within_shape_groups(shape_groups, random_state=random_state)
+        shape_groups = fmain.create_shape_groups(original_tiles)
+        mapping = fmain.shuffle_tiles_within_shape_groups(shape_groups, random_state=random_state)
 
         return {"tiles": original_tiles, "mapping": mapping}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("grid",)
 
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+            "keypoints": self.apply_to_keypoints,
+        }
+
 
 class Normalize(ImageOnlyTransform):
     """Applies various normalization techniques to an image. The specific normalization technique can be selected
         with the `normalization` parameter.
 
     Standard normalization is applied using the formula:
         `img = (img - mean * max_pixel_value) / (std * max_pixel_value)`.
@@ -292,29 +302,32 @@
         max_pixel_value: Optional[float] = 255.0,
         normalization: Literal["standard", "image", "image_per_channel", "min_max", "min_max_per_channel"] = "standard",
         always_apply: bool = False,
         p: float = 1.0,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.mean = mean
+        self.mean_np = np.array(mean, dtype=np.float32) * max_pixel_value
         self.std = std
+        self.denominator = np.reciprocal(np.array(std, dtype=np.float32) * max_pixel_value)
         self.max_pixel_value = max_pixel_value
+        if normalization not in {"standard", "image", "image_per_channel", "min_max", "min_max_per_channel"}:
+            raise ValueError(
+                f"Error during Normalize initialization. Unknown normalization type: {normalization}",
+            )
         self.normalization = normalization
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         if self.normalization == "standard":
-            return F.normalize(
+            return fmain.normalize(
                 img,
-                cast(ColorType, self.mean),
-                cast(ColorType, self.std),
-                cast(float, self.max_pixel_value),
+                self.mean_np,
+                self.denominator,
             )
-        if self.normalization in {"image", "image_per_channel", "min_max", "min_max_per_channel"}:
-            return F.normalize_per_image(img, self.normalization)
-        raise ValueError(f"Unknown normalization type: {self.normalization}")
+        return fmain.normalize_per_image(img, self.normalization)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("mean", "std", "max_pixel_value", "normalization")
 
 
 class ImageCompression(ImageOnlyTransform):
     """Decreases image quality by Jpeg, WebP compression of an image.
@@ -389,15 +402,15 @@
         self.quality_range = quality_range
         self.compression_type = compression_type
 
     def apply(self, img: np.ndarray, quality: int, image_type: Literal[".jpg", ".webp"], **params: Any) -> np.ndarray:
         if img.ndim != MONO_CHANNEL_DIMENSIONS and img.shape[-1] not in (1, 3, 4):
             msg = "ImageCompression transformation expects 1, 3 or 4 channel images."
             raise TypeError(msg)
-        return F.image_compression(img, quality, image_type)
+        return fmain.image_compression(img, quality, image_type)
 
     def get_params(self) -> Dict[str, Any]:
         if self.compression_type == ImageCompressionType.JPEG:
             image_type = ".jpg"
         elif self.compression_type == ImageCompressionType.WEBP:
             image_type = ".webp"
         else:
@@ -412,65 +425,97 @@
         return {
             "quality_range": self.quality_range,
             "compression_type": self.compression_type.value,
         }
 
 
 class RandomSnow(ImageOnlyTransform):
-    """Bleach out some pixel values simulating snow.
-
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+    """Bleach out some pixel values imitating snow.
 
     Args:
-        snow_point_lower: lower_bond of the amount of snow. Should be in [0, 1] range
-        snow_point_upper: upper_bond of the amount of snow. Should be in [0, 1] range
-        brightness_coeff: larger number will lead to a more snow on the image. Should be >= 0
+        snow_point_range (tuple): Tuple of bounds on the amount of snow i.e. (snow_point_lower, snow_point_upper).
+            Both values should be in the (0, 1) range. Default: (0.1, 0.3).
+        brightness_coeff (float): Coefficient applied to increase the brightness of pixels
+            below the snow_point threshold. Larger values lead to more pronounced snow effects.
+            Should be > 0. Default: 2.5.
+        p (float): Probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+
     """
 
     class InitSchema(BaseTransformInitSchema):
-        snow_point_lower: float = Field(default=0.1, description="Lower bound of the amount of snow", ge=0, le=1)
-        snow_point_upper: float = Field(default=0.3, description="Upper bound of the amount of snow", ge=0, le=1)
-        brightness_coeff: float = Field(default=2.5, description="Brightness coefficient, must be >= 0", ge=0)
+        snow_point_range: Annotated[Tuple[float, float], AfterValidator(check_01), AfterValidator(nondecreasing)] = (
+            Field(
+                default=(0.1, 0.3),
+                description="lower and upper bound on the amount of snow as tuple (snow_point_lower, snow_point_upper)",
+            )
+        )
+        snow_point_lower: Optional[float] = Field(
+            default=None,
+            description="Lower bound of the amount of snow",
+            gt=0,
+            lt=1,
+            deprecated="`snow_point_lower` deprecated."
+            "Use `snow_point_range` as tuple (snow_point_lower, snow_point_upper) instead.",
+        )
+        snow_point_upper: Optional[float] = Field(
+            default=None,
+            description="Upper bound of the amount of snow",
+            gt=0,
+            lt=1,
+            deprecated="`snow_point_upper` deprecated."
+            "Use `snow_point_range` as tuple (snow_point_lower, snow_point_upper) instead.",
+        )
+        brightness_coeff: float = Field(default=2.5, description="Brightness coefficient, must be > 0", gt=0)
 
         @model_validator(mode="after")
-        def validate_snow_points(self) -> Self:
-            if self.snow_point_lower > self.snow_point_upper:
-                msg = "snow_point_lower must be less than or equal to snow_point_upper."
-                raise ValueError(msg)
+        def validate_ranges(self) -> Self:
+            if self.snow_point_lower is not None or self.snow_point_upper is not None:
+                lower = self.snow_point_lower if self.snow_point_lower is not None else self.snow_point_range[0]
+                upper = self.snow_point_upper if self.snow_point_upper is not None else self.snow_point_range[1]
+                self.snow_point_range = (lower, upper)
+                self.snow_point_lower = None
+                self.snow_point_upper = None
+
+            # Validate the snow_point_range
+            if not (0 < self.snow_point_range[0] <= self.snow_point_range[1] < 1):
+                raise ValueError("snow_point_range values should be increasing within (0, 1) range.")
+
             return self
 
     def __init__(
         self,
-        snow_point_lower: float = 0.1,
-        snow_point_upper: float = 0.3,
+        snow_point_lower: Optional[float] = None,
+        snow_point_upper: Optional[float] = None,
         brightness_coeff: float = 2.5,
+        snow_point_range: Tuple[float, float] = (0.1, 0.3),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
 
-        self.snow_point_lower = snow_point_lower
-        self.snow_point_upper = snow_point_upper
+        self.snow_point_range = snow_point_range
         self.brightness_coeff = brightness_coeff
 
     def apply(self, img: np.ndarray, snow_point: float, **params: Any) -> np.ndarray:
-        return F.add_snow(img, snow_point, self.brightness_coeff)
+        return fmain.add_snow(img, snow_point, self.brightness_coeff)
 
     def get_params(self) -> Dict[str, np.ndarray]:
-        return {"snow_point": random.uniform(self.snow_point_lower, self.snow_point_upper)}
+        return {"snow_point": random_utils.uniform(*self.snow_point_range)}
 
-    def get_transform_init_args_names(self) -> Tuple[str, ...]:
-        return ("snow_point_lower", "snow_point_upper", "brightness_coeff")
+    def get_transform_init_args_names(self) -> Tuple[str, str]:
+        return "snow_point_range", "brightness_coeff"
 
 
 class RandomGravel(ImageOnlyTransform):
     """Add gravels.
 
     Args:
         gravel_roi: (top-left x, top-left y,
@@ -521,15 +566,15 @@
         gravels[:, 0] = random_utils.randint(x1, x2, count)
         gravels[:, 1] = random_utils.randint(y1, y2, count)
         return gravels
 
     def apply(self, img: np.ndarray, gravels_infos: List[Any], **params: Any) -> np.ndarray:
         if gravels_infos is None:
             gravels_infos = []
-        return F.add_gravel(img, gravels_infos)
+        return fmain.add_gravel(img, gravels_infos)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
         img = params["image"]
@@ -586,75 +631,98 @@
         }
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return "gravel_roi", "number_of_patches"
 
 
 class RandomRain(ImageOnlyTransform):
-    """Adds rain effects.
+    """Adds rain effects to an image.
 
     Args:
-        slant_lower: should be in range [-20, 20].
-        slant_upper: should be in range [-20, 20].
-        drop_length: should be in range [0, 100].
-        drop_width: should be in range [1, 5].
-        drop_color (list of (r, g, b)): rain lines color.
-        blur_value (int): rainy view are blurry
-        brightness_coefficient (float): rainy days are usually shady. Should be in range [0, 1].
-        rain_type: One of [None, "drizzle", "heavy", "torrential"]
+        slant_range (Tuple[int, int]): Tuple of type (slant_lower, slant_upper) representing the range for
+            rain slant angle.
+        drop_length (int): Length of the raindrops.
+        drop_width (int): Width of the raindrops.
+        drop_color (Tuple[int, int, int]): Color of the rain drops in RGB format.
+        blur_value (int): Blur value for simulating rain effect. Rainy views are blurry.
+        brightness_coefficient (float): Coefficient to adjust the brightness of the image.
+            Rainy days are usually shady. Should be in the range (0, 1].
+        rain_type (Optional[str]): Type of rain to simulate. One of [None, "drizzle", "heavy", "torrential"].
+
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
     Reference:
         https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
 
     """
 
     class InitSchema(BaseTransformInitSchema):
-        slant_lower: int = Field(default=-10, description="Lower bound for rain slant angle", ge=-20, le=20)
-        slant_upper: int = Field(default=10, description="Upper bound for rain slant angle", ge=-20, le=20)
-        drop_length: int = Field(default=20, description="Length of raindrops", ge=0, le=100)
-        drop_width: int = Field(default=1, description="Width of raindrops", ge=1, le=5)
+        slant_lower: Optional[int] = Field(
+            default=None,
+            description="Lower bound for rain slant angle",
+            deprecated="`slant_lower` is deprecated.Use `slant_range` as tuple (slant_lower, slant_upper) instead.",
+        )
+        slant_upper: Optional[int] = Field(
+            default=None,
+            description="Upper bound for rain slant angle",
+            deprecated="`slant_upper` is deprecated.Use `slant_range` as tuple (slant_lower, slant_upper) instead.",
+        )
+        slant_range: Annotated[Tuple[float, float], AfterValidator(nondecreasing)] = Field(
+            default=(-10, 10),
+            description="Tuple like (slant_lower, slant_upper) for rain slant angle",
+        )
+        drop_length: int = Field(default=20, description="Length of raindrops", ge=1)
+        drop_width: int = Field(default=1, description="Width of raindrops", ge=1)
         drop_color: Tuple[int, int, int] = Field(default=(200, 200, 200), description="Color of raindrops")
-        blur_value: int = Field(default=7, description="Blur value for simulating rain effect", ge=0)
+        blur_value: int = Field(default=7, description="Blur value for simulating rain effect", ge=1)
         brightness_coefficient: float = Field(
             default=0.7,
             description="Brightness coefficient for rainy effect",
-            ge=0,
+            gt=0,
             le=1,
         )
         rain_type: Optional[RainMode] = Field(default=None, description="Type of rain to simulate")
 
         @model_validator(mode="after")
-        def validate_slant_range_and_rain_type(self) -> Self:
-            if self.slant_lower >= self.slant_upper:
-                msg = "slant_upper must be greater than or equal to slant_lower."
-                raise ValueError(msg)
+        def validate_ranges(self) -> Self:
+            if self.slant_lower is not None or self.slant_upper is not None:
+                lower = self.slant_lower if self.slant_lower is not None else self.slant_range[0]
+                upper = self.slant_upper if self.slant_upper is not None else self.slant_range[1]
+                self.slant_range = (lower, upper)
+                self.slant_lower = None
+                self.slant_upper = None
+
+            # Validate the slant_range
+            if not (-MAX_RAIN_ANGLE <= self.slant_range[0] <= self.slant_range[1] <= MAX_RAIN_ANGLE):
+                raise ValueError(
+                    f"slant_range values should be increasing within [-{MAX_RAIN_ANGLE}, {MAX_RAIN_ANGLE}] range.",
+                )
             return self
 
     def __init__(
         self,
-        slant_lower: int = -10,
-        slant_upper: int = 10,
+        slant_lower: Optional[int] = None,
+        slant_upper: Optional[int] = None,
+        slant_range: Tuple[int, int] = (-10, 10),
         drop_length: int = 20,
         drop_width: int = 1,
         drop_color: Tuple[int, int, int] = (200, 200, 200),
         blur_value: int = 7,
         brightness_coefficient: float = 0.7,
         rain_type: Optional[RainMode] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
-        self.slant_lower = slant_lower
-        self.slant_upper = slant_upper
+        self.slant_range = slant_range
         self.drop_length = drop_length
         self.drop_width = drop_width
         self.drop_color = drop_color
         self.blur_value = blur_value
         self.brightness_coefficient = brightness_coefficient
         self.rain_type = rain_type
 
@@ -662,15 +730,15 @@
         self,
         img: np.ndarray,
         slant: int,
         drop_length: int,
         rain_drops: List[Tuple[int, int]],
         **params: Any,
     ) -> np.ndarray:
-        return F.add_rain(
+        return fmain.add_rain(
             img,
             slant,
             drop_length,
             self.drop_width,
             self.drop_color,
             self.blur_value,
             self.brightness_coefficient,
@@ -679,15 +747,15 @@
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         img = params["image"]
-        slant = int(random.uniform(self.slant_lower, self.slant_upper))
+        slant = int(random_utils.uniform(*self.slant_range))
 
         height, width = img.shape[:2]
         area = height * width
 
         if self.rain_type == "drizzle":
             num_drops = area // 770
             drop_length = 10
@@ -710,16 +778,15 @@
 
             rain_drops.append((x, y))
 
         return {"drop_length": drop_length, "slant": slant, "rain_drops": rain_drops}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (
-            "slant_lower",
-            "slant_upper",
+            "slant_range",
             "drop_length",
             "drop_width",
             "drop_color",
             "blur_value",
             "brightness_coefficient",
             "rain_type",
         )
@@ -772,15 +839,15 @@
     def apply(
         self,
         img: np.ndarray,
         fog_coef: np.ndarray,
         haze_list: List[Tuple[int, int]],
         **params: Any,
     ) -> np.ndarray:
-        return F.add_fog(img, fog_coef, self.alpha_coef, haze_list)
+        return fmain.add_fog(img, fog_coef, self.alpha_coef, haze_list)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         img = params["image"]
@@ -898,15 +965,15 @@
         flare_center_x: float,
         flare_center_y: float,
         circles: List[Any],
         **params: Any,
     ) -> np.ndarray:
         if circles is None:
             circles = []
-        return F.add_sun_flare(
+        return fmain.add_sun_flare(
             img,
             flare_center_x,
             flare_center_y,
             self.src_radius,
             self.src_color,
             circles,
         )
@@ -1000,31 +1067,41 @@
     """
 
     class InitSchema(BaseTransformInitSchema):
         shadow_roi: Tuple[float, float, float, float] = Field(
             default=(0, 0.5, 1, 1),
             description="Region of the image where shadows will appear",
         )
-        num_shadows_limit: OnePlusIntNonDecreasingRangeType = (1, 2)
+        num_shadows_limit: Annotated[Tuple[int, int], AfterValidator(check_1plus), AfterValidator(nondecreasing)] = (
+            1,
+            2,
+        )
         num_shadows_lower: Optional[int] = Field(
             default=None,
             description="Lower limit for the possible number of shadows",
-            deprecated="num_shadows_lower is deprecated. Use num_shadows_limit instead.",
+            deprecated="`num_shadows_lower` is deprecated. Use `num_shadows_limit` instead.",
         )
         num_shadows_upper: Optional[int] = Field(
             default=None,
             description="Upper limit for the possible number of shadows",
-            deprecated="num_shadows_upper is deprecated. Use num_shadows_limit instead.",
+            deprecated="`num_shadows_upper` is deprecated. Use `num_shadows_limit` instead.",
         )
-        shadow_dimension: int = Field(default=5, description="Number of edges in the shadow polygons", gt=0)
+        shadow_dimension: int = Field(default=5, description="Number of edges in the shadow polygons", ge=1)
 
         @model_validator(mode="after")
         def validate_shadows(self) -> Self:
             if self.num_shadows_lower is not None or self.num_shadows_upper is not None:
-                self.num_shadows_limit = cast(Tuple[int, int], (self.num_shadows_lower, self.num_shadows_upper))
+                num_shadows_lower = (
+                    self.num_shadows_lower if self.num_shadows_lower is not None else self.num_shadows_limit[0]
+                )
+                num_shadows_upper = (
+                    self.num_shadows_upper if self.num_shadows_upper is not None else self.num_shadows_limit[1]
+                )
+
+                self.num_shadows_limit = (num_shadows_lower, num_shadows_upper)
                 self.num_shadows_lower = None
                 self.num_shadows_upper = None
 
             shadow_lower_x, shadow_lower_y, shadow_upper_x, shadow_upper_y = self.shadow_roi
 
             if not 0 <= shadow_lower_x <= shadow_upper_x <= 1 or not 0 <= shadow_lower_y <= shadow_upper_y <= 1:
                 raise ValueError(f"Invalid shadow_roi. Got: {self.shadow_roi}")
@@ -1044,15 +1121,15 @@
         super().__init__(always_apply=always_apply, p=p)
 
         self.shadow_roi = shadow_roi
         self.shadow_dimension = shadow_dimension
         self.num_shadows_limit = num_shadows_limit
 
     def apply(self, img: np.ndarray, vertices_list: List[np.ndarray], **params: Any) -> np.ndarray:
-        return F.add_shadow(img, vertices_list)
+        return fmain.add_shadow(img, vertices_list)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, List[np.ndarray]]:
         img = params["image"]
@@ -1118,15 +1195,15 @@
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.scale = scale
 
     def apply(self, img: np.ndarray, low_y: float, high_y: float, **params: Any) -> np.ndarray:
-        return F.move_tone_curve(img, low_y, high_y)
+        return fmain.move_tone_curve(img, low_y, high_y)
 
     def get_params(self) -> Dict[str, float]:
         return {
             "low_y": np.clip(random_utils.normal(loc=0.25, scale=self.scale), 0, 1),
             "high_y": np.clip(random_utils.normal(loc=0.75, scale=self.scale), 0, 1),
         }
 
@@ -1179,15 +1256,15 @@
         sat_shift: int,
         val_shift: int,
         **params: Any,
     ) -> np.ndarray:
         if not is_rgb_image(img) and not is_grayscale_image(img):
             msg = "HueSaturationValue transformation expects 1-channel or 3-channel images."
             raise TypeError(msg)
-        return F.shift_hsv(img, hue_shift, sat_shift, val_shift)
+        return fmain.shift_hsv(img, hue_shift, sat_shift, val_shift)
 
     def get_params(self) -> Dict[str, float]:
         return {
             "hue_shift": random.uniform(self.hue_shift_limit[0], self.hue_shift_limit[1]),
             "sat_shift": random.uniform(self.sat_shift_limit[0], self.sat_shift_limit[1]),
             "val_shift": random.uniform(self.val_shift_limit[0], self.val_shift_limit[1]),
         }
@@ -1204,30 +1281,30 @@
             If threshold is a single value, the range will be [1, threshold]. Default: 128.
         p: probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     Image types:
-        any
+        uint8, float32
 
     """
 
     class InitSchema(BaseTransformInitSchema):
         threshold: OnePlusFloatRangeType = (128, 128)
 
     def __init__(self, threshold: ScaleType = (128, 128), always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply=always_apply, p=p)
         self.threshold = cast(Tuple[float, float], threshold)
 
     def apply(self, img: np.ndarray, threshold: int, **params: Any) -> np.ndarray:
-        return F.solarize(img, threshold)
+        return fmain.solarize(img, threshold)
 
     def get_params(self) -> Dict[str, float]:
-        return {"threshold": random.uniform(self.threshold[0], self.threshold[1])}
+        return {"threshold": random_utils.uniform(self.threshold[0], self.threshold[1])}
 
     def get_transform_init_args_names(self) -> Tuple[str]:
         return ("threshold",)
 
 
 class Posterize(ImageOnlyTransform):
     """Reduce the number of bits for each color channel.
@@ -1269,15 +1346,15 @@
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.num_bits = cast(Union[Tuple[int, ...], List[Tuple[int, ...]]], num_bits)
 
     def apply(self, img: np.ndarray, num_bits: int, **params: Any) -> np.ndarray:
-        return F.posterize(img, num_bits)
+        return fmain.posterize(img, num_bits)
 
     def get_params(self) -> Dict[str, Any]:
         if len(self.num_bits) == NUM_BITS_ARRAY_LENGTH:
             return {"num_bits": [random.randint(int(i[0]), int(i[1])) for i in self.num_bits]}  # type: ignore[index]
         num_bits = self.num_bits
         return {"num_bits": random.randint(int(num_bits[0]), int(num_bits[1]))}  # type: ignore[arg-type]
 
@@ -1327,15 +1404,15 @@
 
         self.mode = mode
         self.by_channels = by_channels
         self.mask = mask
         self.mask_params = mask_params
 
     def apply(self, img: np.ndarray, mask: np.ndarray, **params: Any) -> np.ndarray:
-        return F.equalize(img, mode=self.mode, by_channels=self.by_channels, mask=mask)
+        return fmain.equalize(img, mode=self.mode, by_channels=self.by_channels, mask=mask)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         if not callable(self.mask):
             return {"mask": self.mask}
 
         return {"mask": self.mask(**params)}
 
@@ -1385,15 +1462,15 @@
         self.g_shift_limit = cast(Tuple[float, float], g_shift_limit)
         self.b_shift_limit = cast(Tuple[float, float], b_shift_limit)
 
     def apply(self, img: np.ndarray, r_shift: int, g_shift: int, b_shift: int, **params: Any) -> np.ndarray:
         if not is_rgb_image(img):
             msg = "RGBShift transformation expects 3-channel images."
             raise TypeError(msg)
-        return F.shift_rgb(img, r_shift, g_shift, b_shift)
+        return fmain.shift_rgb(img, r_shift, g_shift, b_shift)
 
     def get_params(self) -> Dict[str, Any]:
         return {
             "r_shift": random_utils.uniform(self.r_shift_limit[0], self.r_shift_limit[1]),
             "g_shift": random_utils.uniform(self.g_shift_limit[0], self.g_shift_limit[1]),
             "b_shift": random_utils.uniform(self.b_shift_limit[0], self.b_shift_limit[1]),
         }
@@ -1437,15 +1514,15 @@
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.brightness_limit = cast(Tuple[float, float], brightness_limit)
         self.contrast_limit = cast(Tuple[float, float], contrast_limit)
         self.brightness_by_max = brightness_by_max
 
     def apply(self, img: np.ndarray, alpha: float, beta: float, **params: Any) -> np.ndarray:
-        return F.brightness_contrast_adjust(img, alpha, beta, self.brightness_by_max)
+        return fmain.brightness_contrast_adjust(img, alpha, beta, self.brightness_by_max)
 
     def get_params(self) -> Dict[str, float]:
         return {
             "alpha": 1.0 + random.uniform(self.contrast_limit[0], self.contrast_limit[1]),
             "beta": 0.0 + random.uniform(self.brightness_limit[0], self.brightness_limit[1]),
         }
 
@@ -1487,15 +1564,15 @@
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.var_limit = cast(Tuple[float, float], var_limit)
         self.mean = mean
         self.per_channel = per_channel
 
     def apply(self, img: np.ndarray, gauss: float, **params: Any) -> np.ndarray:
-        return F.gauss_noise(img, gauss=gauss)
+        return fmain.gauss_noise(img, gauss=gauss)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, float]:
         image = params["image"]
         var = random.uniform(self.var_limit[0], self.var_limit[1])
         sigma = var**0.5
 
         if self.per_channel:
@@ -1560,15 +1637,15 @@
         self,
         img: np.ndarray,
         color_shift: float,
         intensity: float,
         random_seed: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.iso_noise(img, color_shift, intensity, np.random.RandomState(random_seed))
+        return fmain.iso_noise(img, color_shift, intensity, np.random.RandomState(random_seed))
 
     def get_params(self) -> Dict[str, Any]:
         return {
             "color_shift": random_utils.uniform(self.color_shift[0], self.color_shift[1]),
             "intensity": random_utils.uniform(self.intensity[0], self.intensity[1]),
             "random_seed": random_utils.get_random_seed(),
         }
@@ -1610,15 +1687,15 @@
         self.tile_grid_size = tile_grid_size
 
     def apply(self, img: np.ndarray, clip_limit: float, **params: Any) -> np.ndarray:
         if not is_rgb_image(img) and not is_grayscale_image(img):
             msg = "CLAHE transformation expects 1-channel or 3-channel images."
             raise TypeError(msg)
 
-        return F.clahe(img, clip_limit, self.tile_grid_size)
+        return fmain.clahe(img, clip_limit, self.tile_grid_size)
 
     def get_params(self) -> Dict[str, float]:
         return {"clip_limit": random.uniform(self.clip_limit[0], self.clip_limit[1])}
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("clip_limit", "tile_grid_size")
 
@@ -1638,15 +1715,15 @@
     """
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def apply(self, img: np.ndarray, channels_shuffled: Tuple[int, ...], **params: Any) -> np.ndarray:
-        return F.channel_shuffle(img, channels_shuffled)
+        return fmain.channel_shuffle(img, channels_shuffled)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         img = params["image"]
         ch_arr = list(range(img.shape[2]))
         ch_arr = random_utils.shuffle(ch_arr)
         return {"channels_shuffled": ch_arr}
 
@@ -1666,15 +1743,15 @@
 
     Image types:
         uint8, float32
 
     """
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        return F.invert(img)
+        return fmain.invert(img)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class RandomGamma(ImageOnlyTransform):
     """Applies random gamma correction to an image as a form of data augmentation.
@@ -1711,15 +1788,15 @@
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.gamma_limit = cast(Tuple[float, float], gamma_limit)
 
     def apply(self, img: np.ndarray, gamma: float, **params: Any) -> np.ndarray:
-        return F.gamma_transform(img, gamma=gamma)
+        return fmain.gamma_transform(img, gamma=gamma)
 
     def get_params(self) -> Dict[str, float]:
         return {"gamma": random.uniform(self.gamma_limit[0], self.gamma_limit[1]) / 100.0}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("gamma_limit",)
 
@@ -1743,21 +1820,21 @@
 
     Raises:
         TypeError: If the input image is not a 3-channel RGB image.
     """
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         if is_grayscale_image(img):
-            warnings.warn("The image is already gray.")
+            warnings.warn("The image is already gray.", stacklevel=2)
             return img
         if not is_rgb_image(img):
             msg = "ToGray transformation expects 3-channel images."
             raise TypeError(msg)
 
-        return F.to_gray(img)
+        return fmain.to_gray(img)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class ToRGB(ImageOnlyTransform):
     """Convert the input grayscale image to RGB.
@@ -1774,21 +1851,21 @@
     """
 
     def __init__(self, always_apply: bool = True, p: float = 1.0):
         super().__init__(always_apply=always_apply, p=p)
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         if is_rgb_image(img):
-            warnings.warn("The image is already an RGB.")
+            warnings.warn("The image is already an RGB.", stacklevel=2)
             return img
         if not is_grayscale_image(img):
             msg = "ToRGB transformation expects 2-dim images or 3-dim with the last dimension equal to 1."
             raise TypeError(msg)
 
-        return F.gray_to_rgb(img)
+        return fmain.gray_to_rgb(img)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class ToSepia(ImageOnlyTransform):
     """Applies sepia filter to the input RGB image
@@ -1810,15 +1887,15 @@
             [[0.393, 0.769, 0.189], [0.349, 0.686, 0.168], [0.272, 0.534, 0.131]],
         )
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         if not is_rgb_image(img):
             msg = "ToSepia transformation expects 3-channel images."
             raise TypeError(msg)
-        return F.linear_transformation_rgb(img, self.sepia_transformation_matrix)
+        return fmain.linear_transformation_rgb(img, self.sepia_transformation_matrix)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class ToFloat(ImageOnlyTransform):
     """Divide pixel values by `max_value` to get a float32 output array where all values lie in the range [0, 1.0].
@@ -1845,15 +1922,15 @@
         p: ProbabilityType = 1
 
     def __init__(self, max_value: Optional[float] = None, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.max_value = max_value
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        return F.to_float(img, self.max_value)
+        return fmain.to_float(img, self.max_value)
 
     def get_transform_init_args_names(self) -> Tuple[str]:
         return ("max_value",)
 
 
 class FromFloat(ImageOnlyTransform):
     """Take an input array where all values should lie in the range [0, 1.0], multiply them by `max_value` and then
@@ -1892,15 +1969,15 @@
         p: float = 1.0,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.dtype = np.dtype(dtype)
         self.max_value = max_value
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        return F.from_float(img, self.dtype, self.max_value)
+        return fmain.from_float(img, self.dtype, self.max_value)
 
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {"dtype": self.dtype.name, "max_value": self.max_value}
 
 
 class InterpolationDict(TypedDict):
     upscale: int
@@ -1959,58 +2036,61 @@
 
         interpolation: Optional[Union[int, Interpolation, InterpolationDict]] = Field(
             default_factory=lambda: Interpolation(downscale=cv2.INTER_NEAREST, upscale=cv2.INTER_NEAREST),
             deprecated="Use interpolation_pair instead.",
         )
         interpolation_pair: InterpolationPydantic
 
-        scale_range: Annotated[
-            Tuple[float, float], AfterValidator(check_01_range), AfterValidator(check_nondecreasing_range)
-        ] = (0.25, 0.25)
+        scale_range: Annotated[Tuple[float, float], AfterValidator(check_01), AfterValidator(nondecreasing)] = (
+            0.25,
+            0.25,
+        )
 
         @model_validator(mode="after")
         def validate_params(self) -> Self:
             if self.scale_min is not None and self.scale_max is not None:
                 self.scale_range = (self.scale_min, self.scale_max)
                 self.scale_min = None
                 self.scale_max = None
 
             if self.interpolation is not None:
                 if isinstance(self.interpolation, dict):
                     self.interpolation_pair = InterpolationPydantic(**self.interpolation)
                 elif isinstance(self.interpolation, int):
                     self.interpolation_pair = InterpolationPydantic(
-                        upscale=self.interpolation, downscale=self.interpolation
+                        upscale=self.interpolation,
+                        downscale=self.interpolation,
                     )
                 elif isinstance(self.interpolation, Interpolation):
                     self.interpolation_pair = InterpolationPydantic(
-                        upscale=self.interpolation.upscale, downscale=self.interpolation.downscale
+                        upscale=self.interpolation.upscale,
+                        downscale=self.interpolation.downscale,
                     )
                 self.interpolation = None
 
             return self
 
     def __init__(
         self,
         scale_min: Optional[float] = None,
         scale_max: Optional[float] = None,
         interpolation: Optional[Union[int, Interpolation, InterpolationDict]] = None,
         scale_range: Tuple[float, float] = (0.25, 0.25),
         interpolation_pair: InterpolationDict = InterpolationDict(
-            {"upscale": cv2.INTER_NEAREST, "downscale": cv2.INTER_NEAREST}
+            {"upscale": cv2.INTER_NEAREST, "downscale": cv2.INTER_NEAREST},
         ),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.scale_range = scale_range
         self.interpolation_pair = interpolation_pair
 
     def apply(self, img: np.ndarray, scale: float, **params: Any) -> np.ndarray:
-        return F.downscale(
+        return fmain.downscale(
             img,
             scale=scale,
             down_interpolation=self.interpolation_pair["downscale"],
             up_interpolation=self.interpolation_pair["upscale"],
         )
 
     def get_params(self) -> Dict[str, Any]:
@@ -2052,28 +2132,29 @@
         always_apply: bool = False,
         p: float = 1.0,
     ):
         super().__init__(always_apply, p)
 
         self.name = name
         self.custom_apply_fns = {
-            target_name: F.noop for target_name in ("image", "mask", "keypoint", "bbox", "global_label")
+            target_name: fmain.noop for target_name in ("image", "mask", "keypoint", "bbox", "global_label")
         }
         for target_name, custom_apply_fn in {
             "image": image,
             "mask": mask,
             "keypoint": keypoint,
             "bbox": bbox,
             "global_label": global_label,
         }.items():
             if custom_apply_fn is not None:
                 if isinstance(custom_apply_fn, LambdaType) and custom_apply_fn.__name__ == "<lambda>":
                     warnings.warn(
                         "Using lambda is incompatible with multiprocessing. "
                         "Consider using regular functions or partial().",
+                        stacklevel=2,
                     )
 
                 self.custom_apply_fns[target_name] = custom_apply_fn
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         fn = self.custom_apply_fns["image"]
         return fn(img, **params)
@@ -2111,77 +2192,84 @@
         state = {"name": self.name}
         state.update(self.custom_apply_fns.items())  # type: ignore[arg-type]
         state.update(self.get_base_init_args())
         return f"{self.__class__.__name__}({format_args(state)})"
 
 
 class MultiplicativeNoise(ImageOnlyTransform):
-    """Multiply image to random number or array of numbers.
+    """Multiply image by a random number or array of numbers.
 
     Args:
-        multiplier: If single float image will be multiplied to this number.
-            If tuple of float multiplier will be in range `[multiplier[0], multiplier[1])`. Default: (0.9, 1.1).
-        per_channel: If `False`, same values for all channels will be used.
-            If `True` use sample values for each channels. Default False.
-        elementwise: If `False` multiply multiply all pixels in an image with a random value sampled once.
-            If `True` Multiply image pixels with values that are pixelwise randomly sampled. Default: False.
+        multiplier: If a single float, the image will be multiplied by this number.
+            If a tuple of floats, the multiplier will be a random number in the range `[multiplier[0], multiplier[1])`.
+            Default: (0.9, 1.1).
+        elementwise: If `False`, multiply all pixels in the image by a single random value sampled once.
+            If `True`, multiply image pixels by values that are pixelwise randomly sampled. Default: False.
+        p: Probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     Image types:
-        Any
+        uint8, np.float32
 
     """
 
     class InitSchema(BaseTransformInitSchema):
-        multiplier: NonNegativeFloatRangeType = (0.9, 1.1)
-        per_channel: bool = Field(default=False, description="Apply multiplier per channel.")
+        multiplier: Annotated[Tuple[float, float], AfterValidator(check_0plus), AfterValidator(nondecreasing)] = (
+            0.9,
+            1.1,
+        )
+        per_channel: Optional[bool] = Field(
+            default=False,
+            description="Apply multiplier per channel.",
+            deprecated="Does not have any effect. Will be removed in future releases.",
+        )
         elementwise: bool = Field(default=False, description="Apply multiplier element-wise to pixels.")
 
     def __init__(
         self,
         multiplier: ScaleFloatType = (0.9, 1.1),
-        per_channel: bool = False,
+        per_channel: Optional[bool] = None,
         elementwise: bool = False,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.multiplier = cast(Tuple[float, float], multiplier)
-        self.per_channel = per_channel
         self.elementwise = elementwise
 
-    def apply(self, img: np.ndarray, multiplier: float, **kwargs: Any) -> np.ndarray:
-        return F.multiply(img, multiplier)
+    def apply(
+        self,
+        img: np.ndarray,
+        multiplier: Union[float, np.ndarray, Sequence[float]],
+        **kwargs: Any,
+    ) -> np.ndarray:
+        return multiply(img, multiplier)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         if self.multiplier[0] == self.multiplier[1]:
-            return {"multiplier": np.array([self.multiplier[0]])}
+            return {"multiplier": self.multiplier[0]}
 
         img = params["image"]
 
-        height, width = img.shape[:2]
-
-        num_channels = (1 if is_grayscale_image(img) else img.shape[-1]) if self.per_channel else 1
+        num_channels = get_num_channels(img)
 
-        shape = [height, width, num_channels] if self.elementwise else [num_channels]
+        shape = img.shape if self.elementwise else [num_channels]
 
-        multiplier = random_utils.uniform(self.multiplier[0], self.multiplier[1], tuple(shape))
-        if img.ndim == MONO_CHANNEL_DIMENSIONS:
-            multiplier = np.squeeze(multiplier)
+        multiplier = random_utils.uniform(self.multiplier[0], self.multiplier[1], shape).astype(np.float32)
 
         return {"multiplier": multiplier}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
-        return "multiplier", "per_channel", "elementwise"
+        return "multiplier", "elementwise"
 
 
 class FancyPCA(ImageOnlyTransform):
     """Augment RGB image using FancyPCA from Krizhevsky's paper
     "ImageNet Classification with Deep Convolutional Neural Networks"
 
     Args:
@@ -2205,15 +2293,15 @@
         alpha: float = Field(default=0.1, description="Scale for perturbing the eigen vectors and values", ge=0)
 
     def __init__(self, alpha: float = 0.1, always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply=always_apply, p=p)
         self.alpha = alpha
 
     def apply(self, img: np.ndarray, alpha: float, **params: Any) -> np.ndarray:
-        return F.fancy_pca(img, alpha)
+        return fmain.fancy_pca(img, alpha)
 
     def get_params(self) -> Dict[str, float]:
         return {"alpha": random.gauss(0, self.alpha)}
 
     def get_transform_init_args_names(self) -> Tuple[str]:
         return ("alpha",)
 
@@ -2286,18 +2374,18 @@
 
         self.brightness = cast(Tuple[float, float], brightness)
         self.contrast = cast(Tuple[float, float], contrast)
         self.saturation = cast(Tuple[float, float], saturation)
         self.hue = cast(Tuple[float, float], hue)
 
         self.transforms = [
-            F.adjust_brightness_torchvision,
-            F.adjust_contrast_torchvision,
-            F.adjust_saturation_torchvision,
-            F.adjust_hue_torchvision,
+            fmain.adjust_brightness_torchvision,
+            fmain.adjust_contrast_torchvision,
+            fmain.adjust_saturation_torchvision,
+            fmain.adjust_hue_torchvision,
         ]
 
     def get_params(self) -> Dict[str, Any]:
         brightness = random.uniform(self.brightness[0], self.brightness[1])
         contrast = random.uniform(self.contrast[0], self.contrast[1])
         saturation = random.uniform(self.saturation[0], self.saturation[1])
         hue = random.uniform(self.hue[0], self.hue[1])
@@ -2326,15 +2414,15 @@
         if order is None:
             order = [0, 1, 2, 3]
         if not is_rgb_image(img) and not is_grayscale_image(img):
             msg = "ColorJitter transformation expects 1-channel or 3-channel images."
             raise TypeError(msg)
         color_transforms = [brightness, contrast, saturation, hue]
         for i in order:
-            img = self.transforms[i](img, color_transforms[i])  # type: ignore[operator]
+            img = self.transforms[i](img, color_transforms[i])
         return img
 
     def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
         return ("brightness", "contrast", "saturation", "hue")
 
 
 class Sharpen(ImageOnlyTransform):
@@ -2379,15 +2467,15 @@
     def get_params(self) -> Dict[str, np.ndarray]:
         alpha = random.uniform(*self.alpha)
         lightness = random.uniform(*self.lightness)
         sharpening_matrix = self.__generate_sharpening_matrix(alpha_sample=alpha, lightness_sample=lightness)
         return {"sharpening_matrix": sharpening_matrix}
 
     def apply(self, img: np.ndarray, sharpening_matrix: np.ndarray, **params: Any) -> np.ndarray:
-        return F.convolve(img, sharpening_matrix)
+        return fmain.convolve(img, sharpening_matrix)
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("alpha", "lightness")
 
 
 class Emboss(ImageOnlyTransform):
     """Emboss the input image and overlays the result with the original image.
@@ -2434,15 +2522,15 @@
     def get_params(self) -> Dict[str, np.ndarray]:
         alpha = random.uniform(*self.alpha)
         strength = random.uniform(*self.strength)
         emboss_matrix = self.__generate_emboss_matrix(alpha_sample=alpha, strength_sample=strength)
         return {"emboss_matrix": emboss_matrix}
 
     def apply(self, img: np.ndarray, emboss_matrix: np.ndarray, **params: Any) -> np.ndarray:
-        return F.convolve(img, emboss_matrix)
+        return fmain.convolve(img, emboss_matrix)
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("alpha", "strength")
 
 
 class Superpixels(ImageOnlyTransform):
     """Transform images partially/completely to their superpixel representation.
@@ -2520,15 +2608,15 @@
     def apply(
         self,
         img: np.ndarray,
         replace_samples: Sequence[bool],
         n_segments: int,
         **kwargs: Any,
     ) -> np.ndarray:
-        return F.superpixels(img, n_segments, replace_samples, self.max_size, self.interpolation)
+        return fmain.superpixels(img, n_segments, replace_samples, self.max_size, self.interpolation)
 
 
 class TemplateTransform(ImageOnlyTransform):
     """Apply blending of input image with specified templates
     Args:
         templates (numpy array or list of numpy arrays): Images as template for transform.
         img_weight: If single float weight will be sampled from (0, img_weight).
@@ -2593,15 +2681,15 @@
         self,
         img: np.ndarray,
         template: np.ndarray,
         img_weight: float,
         template_weight: float,
         **params: Any,
     ) -> np.ndarray:
-        return F.add_weighted(img, img_weight, template, template_weight)
+        return fmain.add_weighted(img, img_weight, template, template_weight)
 
     def get_params(self) -> Dict[str, float]:
         return {
             "img_weight": random.uniform(self.img_weight[0], self.img_weight[1]),
             "template_weight": random.uniform(self.template_weight[0], self.template_weight[1]),
         }
 
@@ -2715,15 +2803,15 @@
 
         # Normalize kernel
         kernel = kernel.astype(np.float32) / np.sum(kernel)
 
         return {"kernel": kernel}
 
     def apply(self, img: np.ndarray, kernel: int, **params: Any) -> np.ndarray:
-        return F.convolve(img, kernel)
+        return fmain.convolve(img, kernel)
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("blur_limit", "cutoff")
 
 
 class UnsharpMask(ImageOnlyTransform):
     """Sharpen the input image using Unsharp Masking processing and overlays the result with the original image.
@@ -2787,15 +2875,15 @@
         return {
             "ksize": random.randrange(self.blur_limit[0], self.blur_limit[1] + 1, 2),
             "sigma": random.uniform(*self.sigma_limit),
             "alpha": random.uniform(*self.alpha),
         }
 
     def apply(self, img: np.ndarray, ksize: int, sigma: int, alpha: float, **params: Any) -> np.ndarray:
-        return F.unsharp_mask(img, ksize, sigma=sigma, alpha=alpha, threshold=self.threshold)
+        return fmain.unsharp_mask(img, ksize, sigma=sigma, alpha=alpha, threshold=self.threshold)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return "blur_limit", "sigma_limit", "alpha", "threshold"
 
 
 class PixelDropout(DualTransform):
     """Set pixels to 0 with some probability.
@@ -2861,24 +2949,24 @@
     def apply(
         self,
         img: np.ndarray,
         drop_mask: np.ndarray,
         drop_value: Union[float, Sequence[float]],
         **params: Any,
     ) -> np.ndarray:
-        return F.pixel_dropout(img, drop_mask, drop_value)
+        return fmain.pixel_dropout(img, drop_mask, drop_value)
 
     def apply_to_mask(self, mask: np.ndarray, drop_mask: np.ndarray, **params: Any) -> np.ndarray:
         if self.mask_drop_value is None:
             return mask
 
         if mask.ndim == MONO_CHANNEL_DIMENSIONS:
             drop_mask = np.squeeze(drop_mask)
 
-        return F.pixel_dropout(mask, drop_mask, self.mask_drop_value)
+        return fmain.pixel_dropout(mask, drop_mask, self.mask_drop_value)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         return bbox
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
         return keypoint
 
@@ -2893,15 +2981,15 @@
         drop_value: Union[float, Sequence[float], np.ndarray]
         if drop_mask.ndim != img.ndim:
             drop_mask = np.expand_dims(drop_mask, -1)
         if self.drop_value is None:
             drop_shape = 1 if is_grayscale_image(img) else int(img.shape[-1])
 
             if img.dtype in (np.uint8, np.uint16, np.uint32):
-                drop_value = rnd.randint(0, int(F.MAX_VALUES_BY_DTYPE[img.dtype]), drop_shape, img.dtype)
+                drop_value = rnd.randint(0, int(fmain.MAX_VALUES_BY_DTYPE[img.dtype]), drop_shape, img.dtype)
             elif img.dtype in [np.float32, np.double]:
                 drop_value = rnd.uniform(0, 1, drop_shape).astype(img.dtype)
             else:
                 raise ValueError(f"Unsupported dtype: {img.dtype}")
         else:
             drop_value = self.drop_value
 
@@ -3033,15 +3121,15 @@
         img: np.ndarray,
         non_mud: np.ndarray,
         mud: np.ndarray,
         drops: np.ndarray,
         mode: SpatterMode,
         **params: Dict[str, Any],
     ) -> np.ndarray:
-        return F.spatter(img, non_mud, mud, drops, mode)
+        return fmain.spatter(img, non_mud, mud, drops, mode)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         height, width = params["image"].shape[:2]
@@ -3060,18 +3148,18 @@
 
         if mode == "rain":
             liquid_layer = (liquid_layer * 255).astype(np.uint8)
             dist = 255 - cv2.Canny(liquid_layer, 50, 150)
             dist = cv2.distanceTransform(dist, cv2.DIST_L2, 5)
             _, dist = cv2.threshold(dist, 20, 20, cv2.THRESH_TRUNC)
             dist = blur(dist, 3).astype(np.uint8)
-            dist = F.equalize(dist)
+            dist = fmain.equalize(dist)
 
             ker = np.array([[-2, -1, 0], [-1, 1, 1], [0, 1, 2]])
-            dist = F.convolve(dist, ker)
+            dist = fmain.convolve(dist, ker)
             dist = blur(dist, 3).astype(np.float32)
 
             m = liquid_layer * dist
             m *= 1 / np.max(m, axis=(0, 1))
 
             drops = m[:, :, None] * color * intensity
             mud = None
@@ -3157,15 +3245,15 @@
         img: np.ndarray,
         primary_distortion_red: float,
         secondary_distortion_red: float,
         primary_distortion_blue: float,
         secondary_distortion_blue: float,
         **params: Any,
     ) -> np.ndarray:
-        return F.chromatic_aberration(
+        return fmain.chromatic_aberration(
             img,
             primary_distortion_red,
             secondary_distortion_red,
             primary_distortion_blue,
             secondary_distortion_blue,
             self.interpolation,
         )
@@ -3266,19 +3354,27 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.scale = cast(Tuple[int, int], scale)
         self.operation = operation
 
     def apply(self, img: np.ndarray, kernel: Tuple[int, int], **params: Any) -> np.ndarray:
-        return F.morphology(img, kernel, self.operation)
+        return fmain.morphology(img, kernel, self.operation)
 
     def apply_to_mask(self, mask: np.ndarray, kernel: Tuple[int, int], **params: Any) -> np.ndarray:
-        return F.morphology(mask, kernel, self.operation)
+        return fmain.morphology(mask, kernel, self.operation)
 
     def get_params(self) -> Dict[str, float]:
         return {
             "kernel": cv2.getStructuringElement(cv2.MORPH_ELLIPSE, self.scale),
         }
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("scale", "operation")
+
+    @property
+    def targets(self) -> Dict[str, Callable[..., Any]]:
+        return {
+            "image": self.apply,
+            "mask": self.apply_to_mask,
+            "masks": self.apply_to_masks,
+        }
```

### Comparing `albumentations-1.4.7/albumentations/core/bbox_utils.py` & `albumentations-1.4.8/albumentations/core/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/albumentations/core/composition.py` & `albumentations-1.4.8/albumentations/core/composition.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 NUM_ONEOF_TRANSFORMS = 2
 REPR_INDENT_STEP = 2
 
 TransformType = Union[BasicTransform, "BaseCompose"]
 TransformsSeqType = List[TransformType]
 
+AVAILABLE_KEYS = ("image", "mask", "masks", "bboxes", "keypoints", "global_label")
+
 
 def get_always_apply(transforms: Union["BaseCompose", TransformsSeqType]) -> TransformsSeqType:
     new_transforms: TransformsSeqType = []
     for transform in transforms:
         if isinstance(transform, BaseCompose):
             new_transforms.extend(get_always_apply(transform))
         elif transform.always_apply:
@@ -52,14 +54,15 @@
 
 
 class BaseCompose(Serializable):
     def __init__(self, transforms: TransformsSeqType, p: float):
         if isinstance(transforms, (BaseCompose, BasicTransform)):
             warnings.warn(
                 "transforms is single transform, but a sequence is expected! Transform will be wrapped into list.",
+                stacklevel=2,
             )
             transforms = [transforms]
 
         self.transforms = transforms
         self.p = p
 
         self.replay_mode = False
@@ -144,15 +147,18 @@
         """Set _available_keys"""
         for t in self.transforms:
             self._available_keys.update(t.available_keys)
         if self.processors:
             self._available_keys.update(["labels"])
             for proc in self.processors.values():
                 if proc.default_data_name not in self._available_keys:  # if no transform to process this data
-                    warnings.warn(f"Got processor for {proc.default_data_name}, but no transform to process it.")
+                    warnings.warn(
+                        f"Got processor for {proc.default_data_name}, but no transform to process it.",
+                        stacklevel=2,
+                    )
                 self._available_keys.update(proc.data_fields)
                 if proc.params.label_fields:
                     self._available_keys.update(proc.params.label_fields)
 
     def set_deterministic(self, flag: bool, save_key: str = "replay") -> None:
         for t in self.transforms:
             t.set_deterministic(flag, save_key)
@@ -203,14 +209,16 @@
                 raise ValueError(msg)
             self.processors["keypoints"] = KeypointsProcessor(k_params)
 
         for proc in self.processors.values():
             proc.ensure_transforms_valid(self.transforms)
 
         self.add_targets(additional_targets)
+        if not self.transforms:  # if no transforms -> do nothing, all keys will be available
+            self._available_keys.update(AVAILABLE_KEYS)
 
         self.is_check_args = True
         self._disable_check_args_for_transforms(self.transforms)
 
         self.is_check_shapes = is_check_shapes
         self._always_apply = get_always_apply(self.transforms)  # transforms list that always apply
         self._check_each_transform = tuple(  # processors that checks after each transform
@@ -432,15 +440,15 @@
         if transforms is None:
             if first is None or second is None:
                 msg = "You must set both first and second or set transforms argument."
                 raise ValueError(msg)
             transforms = [first, second]
         super().__init__(transforms, p)
         if len(self.transforms) != NUM_ONEOF_TRANSFORMS:
-            warnings.warn("Length of transforms is not equal to 2.")
+            warnings.warn("Length of transforms is not equal to 2.", stacklevel=2)
 
     def __call__(self, *args: Any, force_apply: bool = False, **data: Any) -> Dict[str, Any]:
         if self.replay_mode:
             for t in self.transforms:
                 data = t(**data)
             return data
```

### Comparing `albumentations-1.4.7/albumentations/core/keypoints_utils.py` & `albumentations-1.4.8/albumentations/core/keypoints_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/albumentations/core/pydantic.py` & `albumentations-1.4.8/albumentations/core/pydantic.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,46 +71,52 @@
 SymmetricRangeType = Annotated[ScaleType, AfterValidator(create_symmetric_range)]
 
 
 def convert_to_1plus_range(value: ScaleType) -> Tuple[float, float]:
     return to_tuple(value, low=1)
 
 
-def check_1plus_range(value: Tuple[ScalarType, ScalarType]) -> Tuple[ScalarType, ScalarType]:
+def check_1plus(value: Tuple[ScalarType, ScalarType]) -> Tuple[ScalarType, ScalarType]:
     if any(x < 1 for x in value):
         raise ValueError(f"All values should be >= 1, got {value} instead")
     return value
 
 
-def check_nondecreasing_range(value: Tuple[ScalarType, ScalarType]) -> Tuple[ScalarType, ScalarType]:
+def check_0plus(value: Tuple[ScalarType, ScalarType]) -> Tuple[ScalarType, ScalarType]:
+    if any(x < 0 for x in value):
+        raise ValueError(f"All values should be >= 0, got {value} instead")
+    return value
+
+
+def nondecreasing(value: Tuple[ScalarType, ScalarType]) -> Tuple[ScalarType, ScalarType]:
     if not value[0] <= value[1]:
         raise ValueError(f"First value should be less than the second value, got {value} instead")
     return value
 
 
-OnePlusFloatRangeType = Annotated[ScaleType, AfterValidator(convert_to_1plus_range), AfterValidator(check_1plus_range)]
+OnePlusFloatRangeType = Annotated[ScaleType, AfterValidator(convert_to_1plus_range), AfterValidator(check_1plus)]
 OnePlusIntRangeType = Annotated[
     ScaleType,
     AfterValidator(convert_to_1plus_range),
-    AfterValidator(check_1plus_range),
+    AfterValidator(check_1plus),
     AfterValidator(float2int),
 ]
 
 OnePlusIntNonDecreasingRangeType = Annotated[
     Tuple[ScalarType, ScalarType],
-    AfterValidator(check_1plus_range),
-    AfterValidator(check_nondecreasing_range),
+    AfterValidator(check_1plus),
+    AfterValidator(nondecreasing),
     AfterValidator(float2int),
 ]
 
 
 def convert_to_0plus_range(value: ScaleType) -> Tuple[float, float]:
     return to_tuple(value, low=0)
 
 
-def check_01_range(value: Tuple[float, float]) -> Tuple[float, float]:
+def check_01(value: Tuple[float, float]) -> Tuple[float, float]:
     if not all(0 <= x <= 1 for x in value):
         raise ValueError(f"All values should be in [0, 1], got {value} instead")
     return value
 
 
-ZeroOneRangeType = Annotated[ScaleType, AfterValidator(convert_to_0plus_range), AfterValidator(check_01_range)]
+ZeroOneRangeType = Annotated[ScaleType, AfterValidator(convert_to_0plus_range), AfterValidator(check_01)]
```

### Comparing `albumentations-1.4.7/albumentations/core/serialization.py` & `albumentations-1.4.8/albumentations/core/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 
             transform_dict = {}
             warnings.warn(
                 f"Got NotImplementedError while trying to serialize {self}. Object arguments are not preserved. "
                 f"Implement either '{self.__class__.__name__}.get_transform_init_args_names' "
                 f"or '{self.__class__.__name__}.get_transform_init_args' "
                 "method to make the transform serializable",
+                stacklevel=2,
             )
         return {"__version__": __version__, "transform": transform_dict}
 
 
 def to_dict(transform: Serializable, on_not_implemented_error: str = "raise") -> Dict[str, Any]:
     """Take a transform pipeline and convert it to a serializable representation that uses only standard
     python data types: dictionaries, lists, strings, integers, and floats.
```

### Comparing `albumentations-1.4.7/albumentations/core/transforms_interface.py` & `albumentations-1.4.8/albumentations/core/transforms_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,15 @@
             raise KeyError(msg)
 
         self.deterministic = flag
         if self.deterministic and self.targets_as_params:
             warn(
                 self.get_class_fullname() + " could work incorrectly in ReplayMode for other input data"
                 " because its' params depend on targets.",
+                stacklevel=2,
             )
         self.save_key = save_key
         return self
 
     def __repr__(self) -> str:
         state = self.get_base_init_args()
         state.update(self.get_transform_init_args())
```

### Comparing `albumentations-1.4.7/albumentations/core/types.py` & `albumentations-1.4.8/albumentations/core/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from enum import Enum, IntEnum
-from typing import Any, Literal, Sequence, Tuple, Union
+from typing import Any, List, Literal, Sequence, Tuple, TypeVar, Union
 
 import numpy as np
+from albucore.utils import MAX_VALUES_BY_DTYPE
 from typing_extensions import NotRequired, TypedDict
 
 ScalarType = Union[int, float]
 ColorType = Union[float, Sequence[float]]
 SizeType = Sequence[int]
 
 BoxInternalType = Tuple[float, float, float, float]
@@ -14,15 +15,17 @@
 KeypointType = Union[KeypointInternalType, Tuple[float, float, float, float, Any]]
 
 BoxOrKeypointType = Union[BoxType, KeypointType]
 
 ScaleFloatType = Union[float, Tuple[float, float]]
 ScaleIntType = Union[int, Tuple[int, int]]
 
-ScaleType = Union[ScaleFloatType, ScaleIntType]
+NumericType = TypeVar("NumericType", float, int)
+
+ScaleType = Union[ScaleIntType, ScaleFloatType]
 
 NumType = Union[int, float, np.ndarray]
 
 IntNumType = Union[np.integer, np.ndarray]
 FloatNumType = Union[np.floating, np.ndarray]
 
 ImageMode = Literal["cv", "pil"]
@@ -66,7 +69,43 @@
     JPEG = 0
     WEBP = 1
 
 
 NUM_MULTI_CHANNEL_DIMENSIONS = 3
 MONO_CHANNEL_DIMENSIONS = 2
 NUM_RGB_CHANNELS = 3
+
+PAIR = 2
+TWO = 2
+THREE = 3
+FOUR = 4
+EIGHT = 8
+THREE_SIXTY = 360
+
+BIG_INTEGER = MAX_VALUES_BY_DTYPE[np.uint32]
+MAX_RAIN_ANGLE = 45  # Maximum angle for rain augmentation in degrees
+
+
+PercentType = Union[
+    float,
+    Tuple[float, float],
+    Tuple[float, float, float, float],
+    Tuple[
+        Union[float, Tuple[float, float], List[float]],
+        Union[float, Tuple[float, float], List[float]],
+        Union[float, Tuple[float, float], List[float]],
+        Union[float, Tuple[float, float], List[float]],
+    ],
+]
+
+
+PxType = Union[
+    int,
+    Tuple[int, int],
+    Tuple[int, int, int, int],
+    Tuple[
+        Union[int, Tuple[int, int], List[int]],
+        Union[int, Tuple[int, int], List[int]],
+        Union[int, Tuple[int, int], List[int]],
+        Union[int, Tuple[int, int], List[int]],
+    ],
+]
```

### Comparing `albumentations-1.4.7/albumentations/core/utils.py` & `albumentations-1.4.8/albumentations/core/utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/albumentations/core/validation.py` & `albumentations-1.4.8/albumentations/core/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                 config = dct["InitSchema"](**full_kwargs)
 
                 validated_kwargs = config.model_dump()
                 for name_arg in kwargs:
                     if name_arg not in validated_kwargs:
                         warn(
                             f"Argument '{name_arg}' is not valid and will be ignored.",
+                            stacklevel=2,
                         )
 
                 original_init(self, **validated_kwargs)
 
             # Preserve the original signature and docstring
             custom_init.__signature__ = original_sig  # type: ignore[attr-defined]
             custom_init.__doc__ = original_init.__doc__
```

### Comparing `albumentations-1.4.7/albumentations/pytorch/transforms.py` & `albumentations-1.4.8/albumentations/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/albumentations/random_utils.py` & `albumentations-1.4.8/albumentations/random_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/albumentations.egg-info/PKG-INFO` & `albumentations-1.4.8/albumentations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.7
+Version: 1.4.8
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,16 @@
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: PyYAML
 Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: pydantic>=2.7.0
-Requires-Dist: opencv-python-headless>=4.9.0
+Requires-Dist: albucore>=0.0.4
+Requires-Dist: opencv-python-headless>=4.9.0.80
 
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/albumentations.svg?label=PyPI%20downloads)](
 https://pypi.org/project/albumentations/)
```

### Comparing `albumentations-1.4.7/albumentations.egg-info/SOURCES.txt` & `albumentations-1.4.8/albumentations.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 albumentations/core/utils.py
 albumentations/core/validation.py
 albumentations/pytorch/__init__.py
 albumentations/pytorch/transforms.py
 tests/test_augmentations.py
 tests/test_bbox.py
 tests/test_blur.py
+tests/test_check_version.py
 tests/test_core.py
 tests/test_functional.py
 tests/test_functional_cutout.py
 tests/test_functional_mixing.py
 tests/test_keypoint.py
 tests/test_mixing.py
 tests/test_pydantic.py
```

### Comparing `albumentations-1.4.7/pyproject.toml` & `albumentations-1.4.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,187 +1,177 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
-
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools",
   "wheel",
 ]
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".git-rewrite",
-    ".hg",
-    ".ipynb_checkpoints",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pyenv",
-    ".pytest_cache",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    ".vscode",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "site-packages",
-    "venv",
-    "tests",
-    "setup.py",
-    "tools",
-    "benchmark",
-    "site",
-]
+target-version = "py38"
 
 line-length = 120
 indent-width = 4
 
 # Assume Python 3.8
-target-version = "py38"
-
-[tool.ruff.lint]
-explicit-preview-rules = true
+exclude = [
+  ".bzr",
+  ".direnv",
+  ".eggs",
+  ".git",
+  ".git-rewrite",
+  ".hg",
+  ".ipynb_checkpoints",
+  ".mypy_cache",
+  ".nox",
+  ".pants.d",
+  ".pyenv",
+  ".pytest_cache",
+  ".pytype",
+  ".ruff_cache",
+  ".svn",
+  ".tox",
+  ".venv",
+  ".vscode",
+  "__pypackages__",
+  "_build",
+  "benchmark",
+  "buck-out",
+  "build",
+  "dist",
+  "node_modules",
+  "setup.py",
+  "site",
+  "site-packages",
+  "tests",
+  "tools",
+  "venv",
+]
 
-select = [
-    "F",
-    "E",
-    "W",
-    "C90",
-    "I",
-    "N",
-    "D",
-    "UP",
-    "YTT",
-    "ANN",
-    "ASYNC",
-    "TRIO",
-    "S",
-    "BLE",
-    "FBT",
-    "B",
-    "A",
-    "COM",
-    "CPY",
-    "C4",
-    "DTZ",
-    "T10",
-    "DJ",
-    "EM",
-    "EXE",
-    "ISC",
-    "ICN",
-    "G",
-    "INP",
-    "PIE",
-    "T20",
-    "PYI",
-    "PT",
-    "Q",
-    "RSE",
-    "RET",
-    "SLF",
-    "SLOT",
-    "SIM",
-    "TID",
-    "TCH",
-    "INT",
-    "ARG",
-    "PTH",
-    "TD",
-    "FIX",
-    "ERA",
-    "PD",
-    "PGH",
-    "PL",
-    "TRY",
-    "FLY",
-    "NPY",
-    "PERF",
-    "FURB",
-    "LOG",
-    "RUF",
-]
-ignore = [
-    "ANN101",
-    "D107",
-    "ANN401",
-    "ANN204",
-    "ARG002",
-    "S311",
-    "F403",
-    "PLR0913",
-    "FBT001",
-    "FBT002",
-    "ANN102",
-    "EM102",
-    "TRY003",
-    "A002",
-    "PTH123",
-    "ARG001",
-    "ARG005",
-    "B028",
-    "N812",
-    "FBT003",
-    "B027",
-    "D104",
-    "D100",
-    "D103",
-    "D102",
-    "D415",
-    "D101",
-    "D205",
-    "D105",
-    "D417",
-    "D106",
-    "EM101",
-    "COM812",
-    "B008",
-    "G004",
+format.indent-style = "space"
+# Like Black, respect magic trailing commas.
+format.quote-style = "double"
+# Like Black, indent with spaces, rather than tabs.
+format.line-ending = "auto"
+format.skip-magic-trailing-comma = false
+# Like Black, automatically detect the appropriate line ending.
+lint.select = [
+  "A",
+  "ANN",
+  "ARG",
+  "ASYNC",
+  "B",
+  "BLE",
+  "C4",
+  "C90",
+  "COM",
+  "CPY",
+  "D",
+  "DJ",
+  "DTZ",
+  "E",
+  "EM",
+  "ERA",
+  "EXE",
+  "F",
+  "FBT",
+  "FIX",
+  "FLY",
+  "FURB",
+  "G",
+  "I",
+  "ICN",
+  "INP",
+  "INT",
+  "ISC",
+  "LOG",
+  "N",
+  "NPY",
+  "PD",
+  "PERF",
+  "PGH",
+  "PIE",
+  "PL",
+  "PT",
+  "PTH",
+  "PYI",
+  "Q",
+  "RET",
+  "RSE",
+  "RUF",
+  "S",
+  "SIM",
+  "SLF",
+  "SLOT",
+  "T10",
+  "T20",
+  "TCH",
+  "TD",
+  "TID",
+  "TRIO",
+  "TRY",
+  "UP",
+  "W",
+  "YTT",
+]
+lint.ignore = [
+  "A002",
+  "ANN101",
+  "ANN102",
+  "ANN204",
+  "ANN401",
+  "ARG001",
+  "ARG002",
+  "B008",
+  "B027",
+  "D100",
+  "D101",
+  "D102",
+  "D103",
+  "D104",
+  "D105",
+  "D106",
+  "D107",
+  "D205",
+  "D415",
+  "EM101",
+  "EM102",
+  "F403",
+  "FBT001",
+  "FBT002",
+  "FBT003",
+  "G004",
+  "PLR0913",
+  "PTH123",
+  "S311",
+  "TRY003",
 ]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
-fixable = ["ALL"]
-unfixable = []
 
+lint.explicit-preview-rules = true
+lint.fixable = [
+  "ALL",
+]
+lint.unfixable = [
+]
 # Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-
-[tool.ruff.format]
+lint.dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 # Like Black, use double quotes for strings.
-quote-style = "double"
-
-# Like Black, indent with spaces, rather than tabs.
-indent-style = "space"
-
-# Like Black, respect magic trailing commas.
-skip-magic-trailing-comma = false
-
-# Like Black, automatically detect the appropriate line ending.
-line-ending = "auto"
-
-[tool.ruff.lint.pydocstyle]
-convention = "google"
+lint.pydocstyle.convention = "google"
 
 [tool.mypy]
-plugins = ["pydantic.mypy"]
+plugins = [
+  "pydantic.mypy",
+]
 
 python_version = "3.8"
 ignore_missing_imports = true
 follow_imports = "silent"
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
```

### Comparing `albumentations-1.4.7/setup.py` & `albumentations-1.4.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 from pkg_resources import DistributionNotFound, get_distribution
 from setuptools import find_packages, setup
 
 INSTALL_REQUIRES = [
     "numpy>=1.24.4", "scipy>=1.10.0", "scikit-image>=0.21.0",
     "PyYAML", "typing-extensions>=4.9.0", "scikit-learn>=1.3.2",
-    "pydantic>=2.7.0"
+    "pydantic>=2.7.0",
+    "albucore>=0.0.4"
 ]
 
+MIN_OPENCV_VERSION = "4.9.0.80"
+
 CHOOSE_INSTALL_REQUIRES = [
     (
-        ("opencv-python>=4.9.0", "opencv-contrib-python>=4.9.0", "opencv-contrib-python-headless>=4.9.0"),
-        "opencv-python-headless>=4.9.0",
+        (f"opencv-python>={MIN_OPENCV_VERSION}", f"opencv-contrib-python>={MIN_OPENCV_VERSION}", f"opencv-contrib-python-headless>={MIN_OPENCV_VERSION}"),
+        f"opencv-python-headless>={MIN_OPENCV_VERSION}",
     ),
 ]
 
 def get_version() -> str:
     current_dir = Path(__file__).parent
     version_file = current_dir / "albumentations" / "__init__.py"
     with open(version_file, encoding="utf-8") as f:
```

### Comparing `albumentations-1.4.7/tests/test_augmentations.py` & `albumentations-1.4.8/tests/test_augmentations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Tuple, Type
 
 import cv2
 import numpy as np
 import pytest
 
 import albumentations as A
-from tests.conftest import FLOAT32_IMAGES, IMAGES, SQUARE_FLOAT_IMAGE, SQUARE_IMAGES, SQUARE_UINT8_IMAGE, UINT8_IMAGES
+from tests.conftest import IMAGES, SQUARE_FLOAT_IMAGE, SQUARE_UINT8_IMAGE
 
 from .utils import get_dual_transforms, get_image_only_transforms, get_transforms, set_seed
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_image_only_transforms(
@@ -1064,9 +1064,7 @@
             assert not image.flags["C_CONTIGUOUS"]
         elif augmentation_cls == A.MaskDropout:
             # requires single channel mask
             mask = mask[:, :, 0]
 
         aug = augmentation_cls(p=1, **params)
         aug(image=image, mask=mask)
-
-    # OK, if no exception is raised
```

### Comparing `albumentations-1.4.7/tests/test_bbox.py` & `albumentations-1.4.8/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_blur.py` & `albumentations-1.4.8/tests/test_blur.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_core.py` & `albumentations-1.4.8/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,16 @@
             A.MedianBlur(p=1),
             A.ToGray(p=1),
             A.CLAHE(p=1),
             A.RandomBrightnessContrast(p=1),
             A.RandomGamma(p=1),
             A.ImageCompression(quality_range=(75, 100), p=1),
             A.Crop(x_max=50, y_max=50),
-        ]
+        ],
+        [],  # empty
     ]
 )
 @pytest.mark.parametrize(
     ["compose_args", "args"],
     [
         [
             {},
```

### Comparing `albumentations-1.4.7/tests/test_functional.py` & `albumentations-1.4.8/tests/test_functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 from numpy.testing import assert_array_almost_equal_nulp, assert_almost_equal
 import skimage
 
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
-from albumentations.augmentations.utils import get_opencv_dtype_from_numpy, is_multispectral_image, MAX_VALUES_BY_DTYPE
+from albucore.utils import is_multispectral_image, MAX_VALUES_BY_DTYPE
 
 from albumentations.core.types import d4_group_elements
 from tests.conftest import IMAGES, RECTANGULAR_IMAGES
 from tests.utils import convert_2d_to_target_format, set_seed
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
@@ -101,20 +101,27 @@
     img = np.array([[0.0, 0.0, 0.4], [0.0, 0.0, 0.4], [0.0, 0.0, 0.4]], dtype=np.float32)
     expected = np.array([[0.4, 0.4, 0.4], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]], dtype=np.float32)
     img, expected = convert_2d_to_target_format([img, expected], target=target)
     rotated = FGeometric.rot90(img, factor=1)
     assert_array_almost_equal_nulp(rotated, expected)
 
 
-def test_normalize():
-    img = np.ones((100, 100, 3), dtype=np.uint8) * 127
-    normalized = F.normalize(img, mean=50, std=3)
+@pytest.mark.parametrize("dtype", [
+    np.uint8,
+    np.float32,
+])
+def test_normalize(dtype: np.dtype) -> None:
+    img = np.ones((100, 100, 3), dtype=dtype) * 127
+    mean = np.array(50, dtype=np.float32) * 255
+    denominator = np.reciprocal(np.array(3, dtype=np.float32) * 255)
+    normalized = F.normalize(img, mean=mean, denominator=denominator)
     expected = (np.ones((100, 100, 3), dtype=np.float32) * 127 / 255 - 50) / 3
     assert_array_almost_equal_nulp(normalized, expected)
 
+
 # Parameterize tests for all combinations
 @pytest.mark.parametrize("shape", [
     (100, 100),  # height, width
     (100, 100, 1),  # height, width, 1 channel
     (100, 100, 3),  # height, width, 3 channels
     (100, 100, 7),  # height, width, 7 channels
 ])
@@ -160,17 +167,35 @@
                 for c in range(shape[2]):
                     channel_mean = normalized_img[:, :, c].mean()
                     channel_std = normalized_img[:, :, c].std()
                     assert np.isclose(channel_mean, 0, atol=1e-3), f"Mean for channel {c} should be close to 0"
                     assert np.isclose(channel_std, 1, atol=1e-3), f"STD for channel {c} should be close to 1"
 
 
-def test_normalize_float():
-    img = np.ones((100, 100, 3), dtype=np.float32) * 0.4
-    normalized = F.normalize(img, mean=50, std=3, max_pixel_value=1.0)
+
+@pytest.mark.parametrize("normalization", ("min_max", "min_max_per_channel"))
+@pytest.mark.parametrize("dtype", [
+    np.uint8,
+    np.float32,
+])
+def test_zero_image(normalization: str, dtype: np.dtype) -> None:
+    img = np.zeros((100, 100, 3), dtype=dtype)
+    normalized = F.normalize_per_image(img, normalization)
+    assert np.all(normalized == 0), "All values should be zero after normalization"
+
+
+@pytest.mark.parametrize("dtype", [
+    np.uint8,
+    np.float32,
+])
+def test_normalize_float(dtype: np.dtype) -> None:
+    img = np.ones((100, 100, 3), dtype=dtype) * 0.4
+    mean = np.array(50, dtype=np.float32)
+    denominator = np.array(1 / 3, dtype=np.float32)
+    normalized = F.normalize(img, mean=mean, denominator=denominator)
     expected = (np.ones((100, 100, 3), dtype=np.float32) * 0.4 - 50) / 3
     assert_array_almost_equal_nulp(normalized, expected)
 
 
 def generate_rotation_matrix(image: np.ndarray, angle: float) -> np.ndarray:
     """
     Generates a rotation matrix for the given angle with rotation around the center of the image.
@@ -266,28 +291,14 @@
     expected2 = expected1 + 2
     cropped_img1 = A.random_crop(img, crop_height=2, crop_width=2, h_start=0.0, w_start=0.0)
     cropped_img2 = A.random_crop(img, crop_height=2, crop_width=2, h_start=0.9999, w_start=0.9999)
     assert np.array_equal(cropped_img1, expected1)
     assert np.array_equal(cropped_img2, expected2)
 
 
-def test_clip():
-    img = np.array([[-300, 0], [100, 400]], dtype=np.float32)
-    expected = np.array([[0, 0], [100, 255]], dtype=np.float32)
-    clipped = F.clip(img, dtype=np.uint8, maxval=255)
-    assert np.array_equal(clipped, expected)
-
-
-def test_clip_float():
-    img = np.array([[-0.02, 0], [0.5, 2.2]], dtype=np.float32)
-    expected = np.array([[0, 0], [0.5, 1.0]], dtype=np.float32)
-    clipped = F.clip(img, dtype=np.float32, maxval=1.0)
-    assert_array_almost_equal_nulp(clipped, expected)
-
-
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_pad(target):
     img = np.array([[1, 2], [3, 4]], dtype=np.uint8)
     expected = np.array([[4, 3, 4, 3], [2, 1, 2, 1], [4, 3, 4, 3], [2, 1, 2, 1]], dtype=np.uint8)
     img, expected = convert_2d_to_target_format([img, expected], target=target)
     padded = FGeometric.pad(img, min_height=4, min_width=4, border_mode=cv2.BORDER_REFLECT_101, value=None)
     assert np.array_equal(padded, expected)
@@ -418,26 +429,26 @@
         expected = (img.astype(np.float32) / max_value).astype(np.float32)
 
     actual = F.to_float(img, max_value=max_value)
     assert_almost_equal(actual, expected, decimal=6)
     assert actual.dtype == np.float32, "Resulting dtype is not float32."
 
 
-@pytest.mark.parametrize("dtype", [np.float64, np.int64])
+@pytest.mark.parametrize("dtype", [np.int64])
 def test_to_float_raises_for_unsupported_dtype_without_max_value(dtype):
     img = np.ones((100, 100, 3), dtype=dtype)
     with pytest.raises(RuntimeError) as exc_info:
         F.to_float(img)
     assert "Unsupported dtype" in str(exc_info.value)
 
 
-@pytest.mark.parametrize("dtype", [np.float64, np.int64])
+@pytest.mark.parametrize("dtype", [np.int64])
 def test_to_float_with_max_value_for_unsupported_dtypes(dtype):
     img = np.ones((100, 100, 3), dtype=dtype)
-    max_value = 1.0 if dtype == np.float64 else np.iinfo(dtype).max
+    max_value = np.iinfo(dtype).max
     expected = (img.astype(np.float32) / max_value).astype(np.float32)
     actual = F.to_float(img, max_value=max_value)
     assert_almost_equal(actual, expected, decimal=6)
     assert actual.dtype == np.float32, "Resulting dtype is not float32."
 
 
 @pytest.mark.parametrize(
@@ -453,15 +464,15 @@
     img = np.random.rand(100, 100, 3).astype(np.float32)  # Use random data for more robust testing
     expected_multiplier = multiplier if max_value is None else max_value
     expected = (img * expected_multiplier).astype(dtype)
     actual = F.from_float(img, dtype=np.dtype(dtype), max_value=max_value)
     assert_array_almost_equal_nulp(actual, expected)
 
 
-@pytest.mark.parametrize("dtype", [np.int64, np.float64])
+@pytest.mark.parametrize("dtype", [np.int64])
 def test_from_float_unsupported_dtype_without_max_value(dtype):
     img = np.random.rand(100, 100, 3).astype(np.float32)
     with pytest.raises(RuntimeError) as exc_info:
         F.from_float(img, dtype=dtype)
     expected_part_of_message = "Can't infer the maximum value for dtype"
     assert expected_part_of_message in str(exc_info.value), "Expected error message not found."
 
@@ -745,37 +756,15 @@
 
     assert np.array_equal(F.brightness_contrast_adjust(image_uint8), F._brightness_contrast_adjust_uint(image_uint8))
 
     assert np.array_equal(
         F._brightness_contrast_adjust_non_uint(image_uint8), F._brightness_contrast_adjust_uint(image_uint8)
     )
 
-    dtype = np.uint16
-    min_value = np.iinfo(dtype).min
-    max_value = np.iinfo(dtype).max
-
-    image_uint16 = np.random.randint(min_value, max_value, size=(5, 5, 3), dtype=dtype)
-
-    assert np.array_equal(
-        F.brightness_contrast_adjust(image_uint16), F._brightness_contrast_adjust_non_uint(image_uint16)
-    )
-
-    F.brightness_contrast_adjust(image_uint16)
-
-    dtype = np.uint32
-    min_value = np.iinfo(dtype).min
-    max_value = np.iinfo(dtype).max
-
-    image_uint32 = np.random.randint(min_value, max_value, size=(5, 5, 3), dtype=dtype)
-
-    assert np.array_equal(
-        F.brightness_contrast_adjust(image_uint32), F._brightness_contrast_adjust_non_uint(image_uint32)
-    )
-
-    image_float = np.random.random((5, 5, 3))
+    image_float = np.random.random((5, 5, 3)).astype(np.float32)
 
     assert np.array_equal(
         F.brightness_contrast_adjust(image_float), F._brightness_contrast_adjust_non_uint(image_float)
     )
 
 
 @pytest.mark.parametrize(
@@ -816,28 +805,24 @@
         # Test with splitting tiles vertically
         (
             np.array([[1, 2], [3, 4]], dtype=np.uint8),
             np.array([[0, 0, 1, 2], [1, 0, 2, 2]]),
             [1, 0],
             np.array([[3, 4], [1, 2]], dtype=np.uint8)  # Corrected expectation
         ),
-
-        # Test with splitting tiles diag
-
-        # Other tests remain the same if they correctly represent what your function does
     ]
 )
 def test_swap_tiles_on_image(img, tiles, mapping, expected):
     result_img = F.swap_tiles_on_image(img, tiles, mapping)
     assert np.array_equal(result_img, expected)
 
 
-@pytest.mark.parametrize("dtype", list(F.MAX_VALUES_BY_DTYPE.keys()))
+@pytest.mark.parametrize("dtype", [np.uint8, np.float32])
 def test_solarize(dtype):
-    max_value = F.MAX_VALUES_BY_DTYPE[dtype]
+    max_value = MAX_VALUES_BY_DTYPE[dtype]
 
     if dtype == np.dtype("float32"):
         img = np.arange(2**10, dtype=np.float32) / (2**10)
         img = img.reshape([2**5, 2**5])
     else:
         max_count = 1024
         count = min(max_value + 1, 1024)
@@ -972,55 +957,21 @@
 
     for i in range(1, image.shape[-1] + 1):
         before = image[:, :, :i]
         after = FGeometric.rotate(before, angle=1, interpolation=cv2.INTER_LINEAR, border_mode=cv2.BORDER_REFLECT_101)
         assert before.shape == after.shape
 
 
-def test_multiply_uint8_optimized():
-    image = np.random.randint(0, 256, [256, 320], np.uint8)
-    m = 1.5
-
-    result = F._multiply_uint8_optimized(image, [m])
-    tmp = F.clip(image * m, image.dtype, F.MAX_VALUES_BY_DTYPE[image.dtype])
-    assert np.all(tmp == result)
-
-    image = np.random.randint(0, 256, [256, 320, 3], np.uint8)
-    result = F._multiply_uint8_optimized(image, [m])
-    tmp = F.clip(image * m, image.dtype, F.MAX_VALUES_BY_DTYPE[image.dtype])
-    assert np.all(tmp == result)
-
-    m = np.array([1.5, 0.75, 1.1])
-    image = np.random.randint(0, 256, [256, 320, 3], np.uint8)
-    result = F._multiply_uint8_optimized(image, m)
-    tmp = F.clip(image * m, image.dtype, F.MAX_VALUES_BY_DTYPE[image.dtype])
-    assert np.all(tmp == result)
-
-
 @pytest.mark.parametrize(
     "img", [np.random.randint(0, 256, [100, 100], dtype=np.uint8), np.random.random([100, 100]).astype(np.float32)]
 )
 def test_shift_hsv_gray(img):
     F.shift_hsv(img, 0.5, 0.5, 0.5)
 
 
-def test_cv_dtype_from_np():
-    assert get_opencv_dtype_from_numpy(np.uint8) == cv2.CV_8U
-    assert get_opencv_dtype_from_numpy(np.uint16) == cv2.CV_16U
-    assert get_opencv_dtype_from_numpy(np.float32) == cv2.CV_32F
-    assert get_opencv_dtype_from_numpy(np.float64) == cv2.CV_64F
-    assert get_opencv_dtype_from_numpy(np.int32) == cv2.CV_32S
-
-    assert get_opencv_dtype_from_numpy(np.dtype("uint8")) == cv2.CV_8U
-    assert get_opencv_dtype_from_numpy(np.dtype("uint16")) == cv2.CV_16U
-    assert get_opencv_dtype_from_numpy(np.dtype("float32")) == cv2.CV_32F
-    assert get_opencv_dtype_from_numpy(np.dtype("float64")) == cv2.CV_64F
-    assert get_opencv_dtype_from_numpy(np.dtype("int32")) == cv2.CV_32S
-
-
 @pytest.mark.parametrize(
     ["image", "mean", "std"],
     [
         [np.random.randint(0, 256, [101, 99, 3], dtype=np.uint8), [0.485, 0.456, 0.406], [0.229, 0.224, 0.225]],
         [np.random.randint(0, 256, [101, 99, 3], dtype=np.uint8), 0.5, 0.5],
         [np.random.randint(0, 256, [101, 99], dtype=np.uint8), 0.5, 0.5],
     ],
```

### Comparing `albumentations-1.4.7/tests/test_functional_cutout.py` & `albumentations-1.4.8/tests/test_functional_cutout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 
 from albumentations.augmentations.dropout.functional import cutout
-from albumentations.augmentations.utils import MAX_VALUES_BY_DTYPE
+from albucore.utils import MAX_VALUES_BY_DTYPE
 from tests.utils import set_seed
 
 
 @pytest.mark.parametrize(
     "img, fill_value",
     [
         # Single-channel image, fill_value is a number
```

### Comparing `albumentations-1.4.7/tests/test_functional_mixing.py` & `albumentations-1.4.8/tests/test_functional_mixing.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_keypoint.py` & `albumentations-1.4.8/tests/test_keypoint.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_mixing.py` & `albumentations-1.4.8/tests/test_mixing.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_pydantic.py` & `albumentations-1.4.8/tests/test_pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     ProbabilityType,
     SymmetricRangeType,
     ZeroOneRangeType,
     check_valid_interpolation,
     check_valid_border_modes,
     process_non_negative_range,
     create_symmetric_range,
-    check_1plus_range,
-    check_01_range,
+    check_1plus,
+    check_01,
     valid_interpolations,
     valid_border_modes
 )
 from albumentations.core.validation import ValidatedTransformMeta
 
 # Interpolation Tests
 @pytest.mark.parametrize("interpolation, exception", [
@@ -102,36 +102,36 @@
 
 @pytest.mark.parametrize("value", [
     (0, 0.9),  # Invalid input
     (0, 1.1),  # Invalid input
 ])
 def test_check_1plus_range_with_invalid_input(value):
     with pytest.raises(ValueError):
-        check_1plus_range(value)
+        check_1plus(value)
 
 @pytest.mark.parametrize("value,expected", [
     ((1, 2), (1.0, 2.0)),
 ])
 def test_check_1plus_range_with_valid_input(value, expected):
-    assert check_1plus_range(value) == expected
+    assert check_1plus(value) == expected
 
 @pytest.mark.parametrize("value", [
     (0, -0.1),
     (2, 1.2),
 ])
 def test_check_01_range_with_invalid_input(value):
     with pytest.raises(ValueError):
-        check_01_range(value)
+        check_01(value)
 
 @pytest.mark.parametrize("value,expected", [
     ((0, 1), (0.0, 1.0)),
     ((0, 0.3), (0.0, 0.3)),
 ])
 def test_check_01_range_with_valid_input(value, expected):
-    assert check_01_range(value) == expected
+    assert check_01(value) == expected
 
 class ValidationModel(BaseModel):
     interpolation: Optional[InterpolationType] = None
     border_mode: Optional[BorderModeType] = None
     probability: Optional[ProbabilityType] = None
     non_negative_range_float: Optional[NonNegativeFloatRangeType] = None
     non_negative_range_int: Optional[NonNegativeIntRangeType] = None
```

### Comparing `albumentations-1.4.7/tests/test_pytorch.py` & `albumentations-1.4.8/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_random.py` & `albumentations-1.4.8/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_serialization.py` & `albumentations-1.4.8/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_targets.py` & `albumentations-1.4.8/tests/test_targets.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.7/tests/test_transforms.py` & `albumentations-1.4.8/tests/test_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 import cv2
 import numpy as np
 
 import pytest
 import warnings
 from torchvision import transforms as torch_transforms
 
+from albumentations.core.pydantic import valid_interpolations, valid_border_modes
+
+from albucore.utils import clip
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
-from albumentations.augmentations.transforms import ImageCompression
+from albumentations.augmentations.transforms import ImageCompression, RandomRain
 from albumentations.core.types import ImageCompressionType
 from albumentations.random_utils import get_random_seed
+from albumentations.augmentations.transforms import RandomSnow
 from tests.conftest import IMAGES, SQUARE_MULTI_UINT8_IMAGE, SQUARE_UINT8_IMAGE
 
 from .utils import get_dual_transforms, get_image_only_transforms, get_transforms, set_seed
 
 
 
 def test_transpose_both_image_and_mask():
@@ -397,15 +401,15 @@
 
     mask = np.random.randint(0, 2, 256 * 256, np.uint8).reshape((256, 256))
     aug = A.Equalize(mask=mask, p=1)
     a = aug(image=img)["image"]
     b = F.equalize(img, mask=mask)
     assert np.all(a == b)
 
-    def mask_func(image, test):  # skipcq: PYL-W0613
+    def mask_func(image, test):
         return mask
 
     aug = A.Equalize(mask=mask_func, mask_params=["test"], p=1)
     assert np.all(aug(image=img, test=mask)["image"] == F.equalize(img, mask=mask))
 
 
 def test_crop_non_empty_mask():
@@ -544,65 +548,49 @@
         np.random.random([256, 320]).astype(np.float32),
         np.random.randint(0, 256, [256, 320, 1], np.uint8),
         np.random.random([256, 320, 1]).astype(np.float32),
     ],
 )
 def test_multiplicative_noise_grayscale(image):
     m = 0.5
-    aug = A.MultiplicativeNoise((m, m), p=1)
-    result = aug(image=image)["image"]
-    image = F.clip(image * m, image.dtype, F.MAX_VALUES_BY_DTYPE[image.dtype])
-    assert np.allclose(image, result)
+    aug = A.MultiplicativeNoise((m, m), elementwise=False, p=1)
+    params = aug.get_params_dependent_on_targets({"image": image})
+    assert m == params["multiplier"]
+    result_e = aug(image=image)["image"]
+    assert np.allclose(clip(image * m, image.dtype), result_e)
 
-    aug = A.MultiplicativeNoise(elementwise=True, p=1)
+    aug = A.MultiplicativeNoise((m, m), elementwise=True, p=1)
     params = aug.get_params_dependent_on_targets({"image": image})
-    mul = params["multiplier"]
-    assert mul.shape == image.shape
-    result = aug.apply(image, mul)
-    dtype = image.dtype
-    image = image.astype(np.float32) * mul
-    image = F.clip(image, dtype, F.MAX_VALUES_BY_DTYPE[dtype])
-    assert np.allclose(image, result)
+    result_ne = aug.apply(image, params["multiplier"])
 
+    assert np.allclose(clip(image * params["multiplier"], image.dtype), result_ne)
 
 @pytest.mark.parametrize(
-    "image", [np.random.randint(0, 256, [256, 320, 3], np.uint8), np.random.random([256, 320, 3]).astype(np.float32)]
+    "image", [
+        np.random.randint(0, 256, [256, 320, 3], np.uint8),
+        np.random.random([256, 320, 3]).astype(np.float32)
+    ]
 )
-def test_multiplicative_noise_rgb(image):
+@pytest.mark.parametrize(
+    "elementwise", ( True, False )
+)
+def test_multiplicative_noise_rgb(image, elementwise):
     dtype = image.dtype
 
-    m = 0.5
-    aug = A.MultiplicativeNoise((m, m), p=1)
-    result = aug(image=image)["image"]
-    image = F.clip(image * m, dtype, F.MAX_VALUES_BY_DTYPE[dtype])
-    assert np.allclose(image, result)
-
-    aug = A.MultiplicativeNoise(elementwise=True, p=1)
+    aug = A.MultiplicativeNoise(multiplier=(0.9, 1.1), elementwise=elementwise, p=1)
     params = aug.get_params_dependent_on_targets({"image": image})
     mul = params["multiplier"]
-    assert mul.shape == image.shape[:2] + (1,)
-    result = aug.apply(image, mul)
-    image = F.clip(image.astype(np.float32) * mul, dtype, F.MAX_VALUES_BY_DTYPE[dtype])
-    assert np.allclose(image, result)
 
-    aug = A.MultiplicativeNoise(per_channel=True, p=1)
-    params = aug.get_params_dependent_on_targets({"image": image})
-    mul = params["multiplier"]
-    assert mul.shape == (3,)
-    result = aug.apply(image, mul)
-    image = F.clip(image.astype(np.float32) * mul, dtype, F.MAX_VALUES_BY_DTYPE[dtype])
-    assert np.allclose(image, result)
+    if elementwise:
+        assert mul.shape == image.shape
+    else:
+        assert mul.shape == (image.shape[-1],)
 
-    aug = A.MultiplicativeNoise(elementwise=True, per_channel=True, p=1)
-    params = aug.get_params_dependent_on_targets({"image": image})
-    mul = params["multiplier"]
-    assert mul.shape == image.shape
     result = aug.apply(image, mul)
-    image = F.clip(image.astype(np.float32) * mul, image.dtype, F.MAX_VALUES_BY_DTYPE[image.dtype])
-    assert np.allclose(image, result)
+    assert np.allclose(clip(image.astype(np.float32) * mul.astype(np.float32), dtype), result)
 
 
 def test_mask_dropout():
     # In this case we have mask with all ones, so MaskDropout wipe entire mask and image
     img = np.random.randint(0, 256, [50, 10], np.uint8)
     mask = np.ones([50, 10], dtype=np.int64)
 
@@ -1001,24 +989,18 @@
                     [199, 0, 10, 10],
                     [199, 99, 20, 20],
                     [0, 99, 30, 30],
                 ],
             },
             {
                 "bboxes": [
-                    [15.65896994771262, 0.2946228229078849, 21.047137067150473, 4.617219579173327, 0],
-                    [194.29851584295034, 25.564320319214918, 199.68668296238818, 29.88691707548036, 0],
-                    [178.9528629328495, 95.38278042082668, 184.34103005228735, 99.70537717709212, 0],
-                    [0.47485022613917677, 70.11308292451965, 5.701484157049652, 73.70074852182076, 0],
+                    [(16.036253471129026, 0.7268824985344293, 21.42442059056688, 5.049479254799872, 0), (194.61183288056216, 25.996579994841458, 200.0, 30.319176751106898, 0), (179.33014645626594, 95.67740324373456, 184.71831357570377, 100.0, 0), (0.8521337495555823, 70.54534260014618, 6.078767680466058, 74.1330081974473, 0)]
                 ],
                 "keypoints": [
-                    [16.466635890349504, 0.2946228229078849, 147.04220486917677, 0.0],
-                    [198.770582727028, 26.08267308836993, 157.04220486917674, 9.30232558139535],
-                    [182.77879706281766, 98.84085782583904, 167.04220486917674, 18.6046511627907],
-                    [0.4748502261391767, 73.05280756037699, 177.04220486917674, 27.90697674418604],
+                    [(16.84391941376591, 0.7268824985344293, 147.04220486917677, 0.0), (199.0, 26.514932763996473, 157.04220486917674, 9.30232558139535), (183.15608058623408, 99.0, 167.04220486917674, 18.6046511627907), (0.8521337495555823, 73.48506723600353, 177.04220486917674, 27.906976744186046)]
                 ],
             },
         ],
         [
             10,
             {
                 "bboxes": [
@@ -1032,24 +1014,18 @@
                     [199, 0, 10, 10],
                     [199, 99, 20, 20],
                     [0, 99, 30, 30],
                 ],
             },
             {
                 "bboxes": [
-                    [0.3133170376117963, 25.564320319214918, 5.701484157049649, 29.88691707548036, 0],
-                    [178.9528629328495, 0.2946228229078862, 184.34103005228735, 4.617219579173327, 0],
-                    [194.29851584295034, 70.11308292451965, 199.68668296238818, 74.43567968078509, 0],
-                    [15.658969947712617, 95.38278042082668, 20.88560387862309, 98.97044601812779, 0],
+                    [(0.8521337495555819, 25.866991802552704, 6.240300868993435, 30.18958855881814, 0), (179.4916796447933, 0.5972943062456757, 184.87984676423113, 4.919891062511116, 0), (194.61183288056216, 70.41575440785743, 200.0, 74.73835116412288, 0), (16.1977866596564, 95.68545190416447, 21.424420590566875, 99.27311750146558, 0)]
                 ],
                 "keypoints": [
-                    [0.3133170376117963, 26.212261280658684, 212.95779513082323, 0.0],
-                    [182.6172638742903, 0.42421101519664006, 222.95779513082323, 9.30232558139535],
-                    [198.60904953850064, 73.18239575266574, 232.9577951308232, 18.6046511627907],
-                    [16.305102701822126, 98.97044601812779, 242.9577951308232, 27.906976744186046],
+                    [(0.852133749555582, 26.514932763996473, 212.95779513082323, 0.0), (183.15608058623408, 0.7268824985344295, 222.95779513082323, 9.30232558139535), (199.0, 73.48506723600353, 232.9577951308232, 18.6046511627907), (16.84391941376591, 99.0, 242.9577951308232, 27.906976744186046)]
                 ],
             },
         ],
     ],
 )
 def test_safe_rotate(angle: float, targets: dict, expected: dict):
     image = np.empty([100, 200, 3], dtype=np.uint8)
@@ -1266,15 +1242,15 @@
     res = aug(image=image, mask=mask)
     assert res["image"].shape == image.shape
     assert res["mask"].shape == mask.shape
 
     assert not np.array_equal(res["image"], image)
     assert not np.array_equal(res["mask"], mask)
 
-    np.testing.assert_allclose(res["image"].sum(axis=(0, 1)), image.sum(axis=(0, 1)), atol=0.03)
+    np.testing.assert_allclose(res["image"].sum(axis=(0, 1)), image.sum(axis=(0, 1)), atol=0.04)
     np.testing.assert_allclose(res["mask"].sum(axis=(0, 1)), mask.sum(axis=(0, 1)), atol=0.03)
 
 @pytest.mark.parametrize("image", IMAGES)
 @pytest.mark.parametrize("crop_left, crop_right, crop_top, crop_bottom", [
     (0, 0, 0, 0),
     (0, 1, 0, 1),
     (1, 0, 1, 0),
@@ -1520,7 +1496,220 @@
     aug = A.PadIfNeeded(**params, p=1)
     # Get the initialization arguments to check against expected
     aug_dict = {key: getattr(aug, key) for key in expected.keys()}
 
     # Assert each expected key/value pair
     for key, value in expected.items():
         assert aug_dict[key] == value, f"Failed on {key} with value {value}"
+
+@pytest.mark.parametrize("params, expected", [
+    # Test default initialization values
+    ({}, {"slant_range": (-10, 10)}),
+    ({"slant_range": (-7, 4)},
+     {"slant_range": (-7, 4)}),
+    ({"slant_lower": 2}, {"slant_range": (2, 10)}),
+    ({"slant_upper": 2}, {"slant_range": (-10, 2)}),
+])
+def test_random_rain_initialization(params, expected):
+    img_rain = RandomRain(**params)
+    for key, value in expected.items():
+        assert getattr(img_rain, key) == value, f"Failed on {key} with value {value}"
+
+@pytest.mark.parametrize("params", [
+    ({"slant_range": (12, 8)}),  # Invalid slant range -> decreasing
+    ({"slant_range": (-8, 62)}),  # invalid slant range -> 62 out of upper bound
+])
+def test_random_rain_invalid_input(params):
+    with pytest.raises(Exception):
+        RandomRain(**params)
+
+@pytest.mark.parametrize("params, expected", [
+    # Test default initialization values
+    ({}, {"snow_point_range": (0.1, 0.3)}),
+    # Test snow point range
+    ({"snow_point_range": (0.2, 0.6)},
+     {"snow_point_range": (0.2, 0.6)}),
+    # Deprecated quality values handling
+    ({"snow_point_lower": 0.15}, {"snow_point_range": (0.15, 0.3)}),
+    ({"snow_point_upper": 0.4}, {"snow_point_range": (0.1, 0.4)}),
+])
+def test_random_snow_initialization(params, expected):
+    img_comp = RandomSnow(**params)
+    for key, value in expected.items():
+        assert getattr(img_comp, key) == value, f"Failed on {key} with value {value}"
+
+@pytest.mark.parametrize("params", [
+    ({"snow_point_range": (1.2, 1.5)}),  # Invalid quality range -> upper bound
+    ({"snow_point_range": (0.9, 0.7)}),  # Invalid range  -> decreasing
+])
+def test_random_snow_invalid_input(params):
+    with pytest.raises(Exception):
+        a = RandomSnow(**params)
+        print(a.snow_point_range)
+
+
+@pytest.mark.parametrize(
+    ["augmentation_cls", "params"],
+    get_transforms(
+        custom_arguments={
+            A.Crop: {"y_min": 0, "y_max": 10, "x_min": 0, "x_max": 10},
+            A.CenterCrop: {"height": 10, "width": 10},
+            A.CropNonEmptyMaskIfExists: {"height": 10, "width": 10},
+            A.RandomCrop: {"height": 10, "width": 10},
+            A.RandomResizedCrop: {"height": 10, "width": 10},
+            A.RandomSizedCrop: {"min_max_height": (4, 8), "height": 10, "width": 10},
+            A.CropAndPad: {"px": 10},
+            A.Resize: {"height": 10, "width": 10},
+            A.TemplateTransform: {
+                "templates": np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8),
+            },
+            A.XYMasking: {
+                "num_masks_x": (1, 3),
+                "num_masks_y": (1, 3),
+                "mask_x_length": 10,
+                "mask_y_length": 10,
+                "mask_fill_value": 1,
+                "fill_value": 0,
+            },
+        },
+        except_augmentations={
+        #     A.RandomCropNearBBox,
+            A.RandomSizedBBoxSafeCrop,
+            A.BBoxSafeRandomCrop,
+            A.CropNonEmptyMaskIfExists,
+            A.FDA,
+            A.HistogramMatching,
+            A.PixelDistributionAdaptation,
+            A.MaskDropout,
+            A.MixUp
+        },
+    ),
+)
+def test_dual_transforms_methods(augmentation_cls, params):
+    """Checks whether transformations based on DualTransform dont has abstract methods."""
+    aug = augmentation_cls(p=1, **params)
+    image = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
+    mask = np.random.randint(low=0, high=4, size=(100, 100), dtype=np.uint8) * 64
+
+    arg = {
+        "masks": mask,
+        "masks": [mask],
+        "bboxes": [[0, 0, 0.1, 0.1, 1]],
+        "keypoints": [(0, 0, 0, 0), (1, 1, 0, 0)],
+    }
+
+    for target in aug.targets:
+        if target in arg:
+            kwarg = {target: arg[target]}
+            try:
+                _res = aug(image=image, **kwarg)
+            except Exception as e:
+                if isinstance(e, NotImplementedError):
+                    raise NotImplementedError(f"{target} error at: {augmentation_cls},  {e}")
+                raise e
+
+
+@pytest.mark.parametrize("px", [
+    10,
+    (10, 20),
+    (-10, 20, -30, 40),
+    ((10, 20), (20, 30), (30, 40), (40, 50)),
+    ([1, 2, 3, 4],  [1, 2, 3, 4], [1, 2, 3, 4], [1, 2, 3, 4]),
+    None
+])
+@pytest.mark.parametrize("percent", [
+    0.1,
+    (0.1, 0.2),
+    (0.1, 0.2, 0.3, 0.4),
+    ((-0.1, -0.2), (-0.2, -0.3), (0.3, 0.4), (0.4, 0.5)),
+    ([0.1, 0.2, 0.3, 0.4],  [0.1, 0.2, 0.3, 0.4], [0.1, 0.2, 0.3, 0.4], [0.1, 0.2, 0.3, 0.4]),
+    None
+])
+@pytest.mark.parametrize("pad_cval", [
+    0,
+    (0, 255),
+    [0, 255]
+])
+@pytest.mark.parametrize("keep_size", [
+    True,
+    False
+])
+@pytest.mark.parametrize("sample_independently", [
+    True,
+    False
+])
+@pytest.mark.parametrize("image", IMAGES)
+def test_crop_and_pad(px, percent, pad_cval, keep_size, sample_independently, image):
+    pad_cval_mask = 255 if isinstance(pad_cval, list) else pad_cval
+    interpolation = cv2.INTER_LINEAR
+    pad_mode = cv2.BORDER_CONSTANT
+    if (px is None) ==  (percent is None):
+        # Skip the test case where both px and percent are None or both are not None
+        return
+
+    transform = A.Compose([A.CropAndPad(
+        px=px,
+        percent=percent,
+        pad_mode=pad_mode,
+        pad_cval=pad_cval,
+        pad_cval_mask=pad_cval_mask,
+        keep_size=keep_size,
+        sample_independently=sample_independently,
+        interpolation=interpolation,
+        p=1
+    )])
+
+    transformed_image = transform(image=image)["image"]
+
+    if keep_size:
+        assert transformed_image.shape == image.shape
+
+    assert transformed_image is not None
+    assert transformed_image.shape[0] > 0
+    assert transformed_image.shape[1] > 0
+    assert transformed_image.shape[2] == image.shape[2]
+
+
+@pytest.mark.parametrize("percent, expected_shape", [
+    (0.1, (12, 12, 3)),  # Padding 10% of image size on each side
+    (-0.1, (8, 8, 3)),  # Cropping 10% of image size from each side
+    ((0.1, 0.2, 0.3, 0.4), (14, 16, 3)),  # Padding: top=10%, right=20%, bottom=30%, left=40%
+    ((-0.1, -0.2, -0.3, -0.4), (6, 4, 3)),  # Cropping: top=10%, right=20%, bottom=30%, left=40%
+])
+def test_crop_and_pad_percent(percent, expected_shape):
+    transform = A.Compose([A.CropAndPad(px=None, percent=percent, pad_mode=cv2.BORDER_CONSTANT, pad_cval=0, keep_size=False)])
+
+    image = np.ones((10, 10, 3), dtype=np.uint8)
+
+    transformed_image = transform(image=image)["image"]
+
+    assert transformed_image.shape == expected_shape
+    if percent is not None and all(p >= 0 for p in np.array(percent).flatten()):
+        assert transformed_image.sum() == image.sum()
+
+@pytest.mark.parametrize("px, expected_shape", [
+    (2, (14, 14, 3)),  # Padding 2 pixels on each side
+    (-2, (6, 6, 3)),  # Cropping 2 pixels from each side
+    ((1, 2, 3, 4), (14, 16, 3)),  # Padding: top=1, right=2, bottom=3, left=4
+    ((-1, -2, -3, -4), (6, 4, 3)),  # Cropping: top=1, right=2, bottom=3, left=4
+])
+def test_crop_and_pad_px_pixel_values(px, expected_shape):
+    transform = A.Compose([A.CropAndPad(px=px, percent=None, pad_mode=cv2.BORDER_CONSTANT, pad_cval=0, keep_size=False)])
+
+    image = np.ones((10, 10, 3), dtype=np.uint8) * 255
+
+    transformed_image = transform(image=image)["image"]
+
+    if isinstance(px, int):
+        px = [px] * 4  # Convert to list of 4 elements
+    if isinstance(px, tuple) and len(px) == 2:
+        px = [px[0], px[1], px[0], px[1]]  # Convert to 4 elements for padding
+
+    if px is not None:
+        if all(p >= 0 for p in px):  # Padding
+            pad_top, pad_right, pad_bottom, pad_left = px
+            central_region = transformed_image[pad_top:pad_top + image.shape[0], pad_left:pad_left + image.shape[1], :]
+            assert np.all(central_region == 255)
+        elif all(p <= 0 for p in px):  # Cropping
+            crop_top, crop_right, crop_bottom, crop_left = [-p for p in px]
+            cropped_region = image[crop_top:image.shape[0] - crop_bottom, crop_left:image.shape[1] - crop_right, :]
+            assert np.all(transformed_image == cropped_region)
```

