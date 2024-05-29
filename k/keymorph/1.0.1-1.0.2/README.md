# Comparing `tmp/keymorph-1.0.1.tar.gz` & `tmp/keymorph-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keymorph-1.0.1.tar", last modified: Thu May 23 14:14:45 2024, max compression
+gzip compressed data, was "keymorph-1.0.2.tar", last modified: Wed May 29 20:38:05 2024, max compression
```

## Comparing `keymorph-1.0.1.tar` & `keymorph-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.769303 keymorph-1.0.1/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1068 2023-10-17 18:20:30.000000 keymorph-1.0.1/LICENSE
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    15759 2024-05-23 14:14:45.769303 keymorph-1.0.1/PKG-INFO
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    15145 2024-05-21 13:58:38.000000 keymorph-1.0.1/README.md
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.741303 keymorph-1.0.1/keymorph/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       50 2024-05-23 14:13:37.000000 keymorph-1.0.1/keymorph/__init__.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    10299 2024-05-10 14:19:13.000000 keymorph-1.0.1/keymorph/augmentation.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    20976 2024-04-20 17:29:13.000000 keymorph-1.0.1/keymorph/keypoint_aligners.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     5327 2024-04-18 18:04:36.000000 keymorph-1.0.1/keymorph/layers.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    17717 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/loss_ops.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    19960 2024-05-15 02:30:56.000000 keymorph-1.0.1/keymorph/model.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1345 2024-05-10 14:17:23.000000 keymorph-1.0.1/keymorph/net.py
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.765303 keymorph-1.0.1/keymorph/unet3d/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        0 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/__init__.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    20881 2024-04-20 17:23:30.000000 keymorph-1.0.1/keymorph/unet3d/buildingblocks.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      885 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/config.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13344 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/losses.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16873 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/metrics.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    14982 2024-04-19 20:00:16.000000 keymorph-1.0.1/keymorph/unet3d/model.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    11935 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/predictor.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     3992 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/se.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     3890 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/seg_metrics.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16068 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/trainer.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     9784 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/utils.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    11303 2024-05-23 14:09:35.000000 keymorph-1.0.1/keymorph/utils.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    12970 2024-05-23 13:53:56.000000 keymorph-1.0.1/keymorph/viz_tools.py
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.749303 keymorph-1.0.1/keymorph.egg-info/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    15759 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/PKG-INFO
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      689 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/SOURCES.txt
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        1 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/dependency_links.txt
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      161 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/requires.txt
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        9 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/top_level.txt
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       38 2024-05-23 14:14:45.769303 keymorph-1.0.1/setup.cfg
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1413 2024-05-23 14:13:09.000000 keymorph-1.0.1/setup.py
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.769303 keymorph-1.0.1/tests/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13696 2024-04-17 14:01:56.000000 keymorph-1.0.1/tests/test.py
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-29 20:38:05.132146 keymorph-1.0.2/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1068 2023-10-17 18:20:30.000000 keymorph-1.0.2/LICENSE
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16643 2024-05-29 20:38:05.132146 keymorph-1.0.2/PKG-INFO
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16029 2024-05-27 15:50:33.000000 keymorph-1.0.2/README.md
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-29 20:38:05.104146 keymorph-1.0.2/keymorph/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       50 2024-05-29 20:36:42.000000 keymorph-1.0.2/keymorph/__init__.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    10299 2024-05-10 14:19:13.000000 keymorph-1.0.2/keymorph/augmentation.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    21199 2024-05-29 20:22:14.000000 keymorph-1.0.2/keymorph/keypoint_aligners.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     5633 2024-05-29 18:19:46.000000 keymorph-1.0.2/keymorph/layers.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    17717 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/loss_ops.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    20143 2024-05-29 20:31:55.000000 keymorph-1.0.2/keymorph/model.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1345 2024-05-10 14:17:23.000000 keymorph-1.0.2/keymorph/net.py
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-29 20:38:05.128146 keymorph-1.0.2/keymorph/unet3d/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        0 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/__init__.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    20881 2024-04-20 17:23:30.000000 keymorph-1.0.2/keymorph/unet3d/buildingblocks.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      885 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/config.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13344 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/losses.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16873 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/metrics.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    14982 2024-04-19 20:00:16.000000 keymorph-1.0.2/keymorph/unet3d/model.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    11935 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/predictor.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     3992 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/se.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     3890 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/seg_metrics.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16068 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/trainer.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     9784 2024-04-17 14:01:55.000000 keymorph-1.0.2/keymorph/unet3d/utils.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    12198 2024-05-29 17:27:48.000000 keymorph-1.0.2/keymorph/utils.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13059 2024-05-23 15:28:34.000000 keymorph-1.0.2/keymorph/viz_tools.py
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-29 20:38:05.108146 keymorph-1.0.2/keymorph.egg-info/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16643 2024-05-29 20:38:04.000000 keymorph-1.0.2/keymorph.egg-info/PKG-INFO
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      705 2024-05-29 20:38:05.000000 keymorph-1.0.2/keymorph.egg-info/SOURCES.txt
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        1 2024-05-29 20:38:04.000000 keymorph-1.0.2/keymorph.egg-info/dependency_links.txt
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      161 2024-05-29 20:38:04.000000 keymorph-1.0.2/keymorph.egg-info/requires.txt
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       14 2024-05-29 20:38:04.000000 keymorph-1.0.2/keymorph.egg-info/top_level.txt
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       38 2024-05-29 20:38:05.132146 keymorph-1.0.2/setup.cfg
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1413 2024-05-29 20:36:33.000000 keymorph-1.0.2/setup.py
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-29 20:38:05.128146 keymorph-1.0.2/test/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-29 17:58:38.000000 keymorph-1.0.2/test/__init__.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    12930 2024-05-29 18:16:13.000000 keymorph-1.0.2/test/test.py
```

### Comparing `keymorph-1.0.1/LICENSE` & `keymorph-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/PKG-INFO` & `keymorph-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,21 @@
-Metadata-Version: 2.1
-Name: keymorph
-Version: 1.0.1
-Summary: KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints.
-Home-page: https://github.com/alanqrwang/keymorph
-Author: Alan Q. Wang
-Author-email: alanqrwang@gmail.com
-License: MIT
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # KeyMorph: Robust and Flexible Multi-modal Registration via Keypoint Detection
 
 KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints. 
 It supports unimodal/multimodal pairwise and groupwise registration using rigid, affine, or nonlinear transformations.
 
 This repository contains the code for KeyMorph, as well as example scripts for training your own KeyMorph model.
 As an example, it uses data from the [IXI dataset](https://brain-development.org/ixi-dataset/) to train and evaluate the model.
 
 [BrainMorph](https://github.com/alanqrwang/brainmorph) is a foundation model based on the KeyMorph framework, trained on over 100,000 brain MR images at full resolution (256x256x256).
 The model is robust to normal and diseased brains, a variety of MRI modalities, and skullstripped and non-skullstripped images.
 Check out the dedicated repository for the latest updates and models!
 
 ## Updates
+- [May 2024] Added option to use CSV file to train KeyMorph on your own data. See "Training KeyMorph on your own data" below.
 - [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) has been moved to its own dedicated repository. See the repository for the latest updates and models.
 - [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) is released, a foundational keypoint model based on KeyMorph for robust and flexible brain MRI registration!
 - [Dec 2023] [Journal paper](https://arxiv.org/abs/2304.09941) extension of MIDL paper published in Medical Image Analysis. Instructions under "IXI-trained, half-resolution models".
 - [Feb 2022] [Conference paper](https://openreview.net/forum?id=OrNzjERFybh) published in MIDL 2021.
 
 ## Installation
 
@@ -63,17 +48,115 @@
 Running `pip install keymorph` or `pip install -e .` will automatically check for and install all of these requirements.
 
 ## Downloading Trained Weights
 You can find all full-resolution, BrainMorph trained weights [here](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i).
 Half-resolution trained weights are under [Releases](https://github.com/alanqrwang/keymorph/releases).
 Download your preferred model(s) and put them in the folder specified by `--weights_dir` in the commands below.
 
+
+## TLDR in code
+The crux of the code is in the `forward()` function in `keymorph/model.py`, which performs one forward pass through the entire KeyMorph pipeline.
+
+Here's a pseudo-code version of the function:
+```python
+def forward(img_f, img_m, seg_f, seg_m, network, optimizer, kp_aligner):
+    '''Forward pass for one mini-batch step. 
+    Variables with (_f, _m, _a) denotes (fixed, moving, aligned).
+    
+    Args:
+        img_f, img_m: Fixed and moving intensity image (bs, 1, l, w, h)
+        seg_f, seg_m: Fixed and moving one-hot segmentation map (bs, num_classes, l, w, h)
+        network: Keypoint extractor network
+        kp_aligner: Rigid, affine or TPS keypoint alignment module
+    '''
+    optimizer.zero_grad()
+
+    # Extract keypoints
+    points_f = network(img_f)
+    points_m = network(img_m)
+
+    # Align via keypoints
+    grid = kp_aligner.grid_from_points(points_m, points_f, img_f.shape, lmbda=lmbda)
+    img_a, seg_a = utils.align_moving_img(grid, img_m, seg_m)
+
+    # Compute losses
+    mse = MSELoss()(img_f, img_a)
+    soft_dice = DiceLoss()(seg_a, seg_f)
+
+    if unsupervised:
+        loss = mse
+    else:
+        loss = soft_dice
+
+    # Backward pass
+    loss.backward()
+    optimizer.step()
+```
+The `network` variable is a CNN with center-of-mass layer which extracts keypoints from the input images.
+The `kp_aligner` variable is a keypoint alignment module. It has a function `grid_from_points()` which returns a flow-field grid encoding the transformation to perform on the moving image. The transformation can either be rigid, affine, or nonlinear (TPS).
+
+## Training KeyMorph on your own data
+`scripts/run.py` with `--run_mode train` allows you to easily train KeyMorph on your own data.
+
+### Create a CSV file
+The CSV file should contain the following columns: `img_path`, `seg_path`, `mask_path`, `modality`, `train`.
++ `img_path` is the path to the intensity image.
++ `seg_path` is the (optional )path to the corresponding segmentation map. Set to "None" if not available.
++ `mask_path` is the (optional) path to the mask. Set to "None" if not available.
++ `modality` is the modality of the image.
++ `train` is a boolean indicating whether the image is in the train or test set.
+
+Then, simply pass the path to the CSV file as `--data_csv_path`.
+
+### Editing pre-processing/augmentations
+You probably need to set the `TRANSFORM` variable in `scripts/hyperparameters.py` to correspond to the pre-processing/augmentations that you want to apply to your own data.
+The code uses `torchio` for pre-processing and augmentations. You can find the list of available transforms [here](https://torchio.readthedocs.io/transforms/augmentation.html).
+You can also use your own custom transforms by wrapping them in the [Lambda](https://torchio.readthedocs.io/transforms/others.html#torchio.transforms.Lambda) transform.
+
+Note, affine augmentations are applied separately and is determined by the `--max_random_affine_augment_params` flag in `scripts/run.py`. By default, it is set to `(0.0, 0.0, 0.0, 0.0)`. For example, `(0.2, 0.2, 3.1416, 0.1)` denotes:
++ Scaling by [1-0.2, 1+0.2]
++ Translation by [-0.2, 0.2], as a fraction of the image size
++ Rotation by [-3.1416, 3.1416] radians
++ Shearing by [-0.1, 0.1]
+
+### Run the training script
+We use the weights from the pretraining step to initialize our model.
+Our pretraining weights are provided in [Releases](https://github.com/evanmy/keymorph/releases/tag/weights).
+
+
+```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --loss_fn mse \
+    --transform_type affine \
+    --train_dataset csv \
+    --data_path /path/to/data_csv
+```
+
+
+Description of all flags:
++ `--num_keypoints <num_key>` flag specifies the number of keypoints to extract per image as `<num_key>`.
++ `--loss_fn <loss>` specifies the loss function to train. Options are `mse` (unsupervised training) and `dice` (supervised training). Unsupervised only requires intensity images and minimizes MSE loss, while supervised assumes availability of corresponding segmentation maps for each image and minimizes soft Dice loss.
++ `--transform_type <ttype>`. 
+Transform to use for registration. Options are `rigid`, `affine`, `tps_<lambda>`.
+TPS uses a (non-linear) thin-plate-spline interpolant to align the corresponding keypoints. A hyperparameter lambda controls the degree of non-linearity for TPS. A value of 0 corresponds to exact keypoint alignment (resulting in a maximally nonlinear transformation while still minimizing bending energy), while higher values result in the transformation becoming more and more affine-like. In practice, we find a value of 10 is very similar to an affine transformation.
+The code also supports sampling lambda according to some distribution (`tps_uniform`, `tps_lognormal`, `tps_loguniform`).
++ `--train_dataset csv` specifies that we are training on a csv dataset specified by...
++ `--data_path <path>` specifies the path to the CSV file containing the dataset.
+
+Other optional flags:
++  `--mix_modalities` flag, if set, mixes modalities between sampled pairs during training. You should probably set this when `--loss_fn dice` (supervised training), and not when `--loss_fn mse` (unsupervised training).
++ `--visualize` flag to visualize results with matplotlib
++ `--debug_mode` flag to print some debugging information
++ `--use_wandb` flag to log results to Weights & Biases
+
 ## Registering brain volumes 
 ### BrainMorph
-Warning: Please see the [BrainMorph repository](https://github.com/alanqrwang/brainmorph) for the latest updates and models! This is a legacy version of the code and is not guaranteed to be maintained.
+WARNING: Please see the [BrainMorph repository](https://github.com/alanqrwang/brainmorph) for the latest updates and models! This is a legacy version of the code and is not guaranteed to be maintained.
 
 BrainMorph is trained on over 100,000 brain MR images at full resolution (256x256x256). 
 The script will automatically min-max normalize the images and resample to 1mm isotropic resolution.
 
 `--num_keypoints` and `num_levels_for_unet` will determine which model will be used to perform the registration.
 Make sure the corresponding weights are present in `--weights_dir`.
 `--num_keypoints` can be set to `128, 256, 512` and `--num_levels_for_unet` can be set to `4, 5, 6, 7`, respectively (corresponding to 'S', 'M', 'L', 'H' in the paper).
@@ -155,192 +238,76 @@
     --fixed_seg ./example_data_half/seg_m/IXI_002_128x128x128.nii.gz \
     --list_of_aligns affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
-## TLDR in code
-The crux of the code is in the `forward()` function in `keymorph/model.py`, which performs one forward pass through the entire KeyMorph pipeline.
-
-Here's a pseudo-code version of the function:
-```python
-def forward(img_f, img_m, seg_f, seg_m, network, optimizer, kp_aligner):
-    '''Forward pass for one mini-batch step. 
-    Variables with (_f, _m, _a) denotes (fixed, moving, aligned).
-    
-    Args:
-        img_f, img_m: Fixed and moving intensity image (bs, 1, l, w, h)
-        seg_f, seg_m: Fixed and moving one-hot segmentation map (bs, num_classes, l, w, h)
-        network: Keypoint extractor network
-        kp_aligner: Rigid, affine or TPS keypoint alignment module
-    '''
-    optimizer.zero_grad()
-
-    # Extract keypoints
-    points_f = network(img_f)
-    points_m = network(img_m)
-
-    # Align via keypoints
-    grid = kp_aligner.grid_from_points(points_m, points_f, img_f.shape, lmbda=lmbda)
-    img_a, seg_a = utils.align_moving_img(grid, img_m, seg_m)
-
-    # Compute losses
-    mse = MSELoss()(img_f, img_a)
-    soft_dice = DiceLoss()(seg_a, seg_f)
-
-    if unsupervised:
-        loss = mse
-    else:
-        loss = soft_dice
-
-    # Backward pass
-    loss.backward()
-    optimizer.step()
-```
-The `network` variable is a CNN with center-of-mass layer which extracts keypoints from the input images.
-The `kp_aligner` variable is a keypoint alignment module. It has a function `grid_from_points()` which returns a flow-field grid encoding the transformation to perform on the moving image. The transformation can either be rigid, affine, or nonlinear (TPS).
-
-## Training KeyMorph
-Use `scripts/run.py` with `--run_mode train` to train KeyMorph.
-
-We use the weights from the pretraining step to initialize our model.
-Our pretraining weights are provided in [Releases](https://github.com/evanmy/keymorph/releases/tag/weights).
-
-The `--num_keypoints <num_key>` flag specifies the number of keypoints to extract per image as `<num_key>`.
-For all commands, optionally add the `--use_wandb` flag to log results to Weights & Biases.
-
-This repository supports several variants of training KeyMorph.
-Here's a overview of the variants:
-
-### Supervised vs. unsupervised
-Unsupervised only requires intensity images and minimizes MSE loss, while supervised assumes availability of corresponding segmentation maps for each image and minimizes soft Dice loss.
-
-To specify unsupervised, set `--loss_fn mse`.
-To specify supervised, set `--loss_fn dice`.
-
+## Step-by-step guide for reproducing our results
 
-### Affine vs. TPS
-Affine uses an affine transformation to align the corresponding keypoints.
+### Dataset 
+[A] Scripts in `./notebooks/[A] Download Data` will download the IXI data and perform some basic preprocessing
 
-TPS uses a (non-linear) thin-plate-spline interpolant to align the corresponding keypoints. A hyperparameter `--tps_lmbda` controls the degree of non-linearity for TPS. A value of 0 corresponds to exact keypoint alignment (resulting in a maximally nonlinear transformation while still minimizing bending energy), while higher values result in the transformation becoming more and more affine-like. In practice, we find a value of 10 is very similar to an affine transformation.
+[B] Once the data is downloaded `./notebooks/[B] Brain extraction` can be used to extract remove non-brain tissue. 
 
-To specify affine, set `--kp_align_method affine`.
-To specify tps, set `--kp_align_method tps` and the lmbda value `--tps_lmbda 0`.
+[C] Once the brain has been extracted, we center the brain using `./notebooks/[C] Centering`. During training, we randomly introduce affine augmentation to the dataset. This ensure that the brain stays within the volume given the affine augmentation we introduce. It also helps during the pretraining step of our algorithm.
 
-### Example commands
-**Affine, Unsupervised**
+### Pretraining KeyMorph
 
-To train unsupervised KeyMorph with affine transformation and 128 keypoints, use `mse` as the loss function:
+This step helps with the convergence of our model. We pick 1 subject and random points within the brain of that subject. We then introduce affine transformation to the subject brain and same transformation to the keypoints. In other words, this is a self-supervised task in where the network learns to predict the keypoints on a brain under random affine transformation. We found that initializing our model with these weights helps with the training.
 
+To pretrain, run:
+ 
 ```bash
 python scripts/run.py \
-    --run_mode train \
+    --run_mode pretrain \
     --num_keypoints 128 \
     --loss_fn mse \
-    --transform_type affine \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
+    --transform_type tps_0 \
+    --max_random_affine_augment_params (0.2, 0.2, 3.1416, 0.1) \
+    --affine_slope 1000 \
+    --data_dir ./centered_IXI 
 ```
 
-<!-- For unsupervised KeyMorph, optionally add `--kpconsistency_coeff` to optimize keypoint consistency across modalities for same subject: -->
+`--affine_slope` linearly ramps up the ``max_random_affine_augment_params` such that it starts at 0 for all parameters and reaches their maximum values at epoch 1000. This helps the model to learn the keypoints under increasing affine transformations.
 
-<!-- ```bash
-python scripts/run.py \
-    --run_mode train \
-    --num_keypoints 128 \
-    --kp_align_method affine \
-    --loss_fn mse \
-    --kpconsistency_coeff 10 \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
-``` -->
-
-**Affine, Supervised**
-
-To train supervised KeyMorph, use `dice` as the loss function:
+### Training KeyMorph
+Follow instructions for "Training KeyMorph" above, for more options.
 
 ```bash
 python scripts/run.py \
     --run_mode train \
     --num_keypoints 128 \
-    --kp_align_method affine \
-    --loss_fn dice \
-    --mix_modalities \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
-```
-
-Note that the `--mix_modalities` flag allows fixed and moving images to be of different modalities during training. This should not be set for unsupervised training, which uses MSE as the loss function.
-
-**Nonlinear thin-plate-spline (TPS)**
-
-To train the TPS variant of KeyMorph which allows for nonlinear registrations, specify `tps` as the keypoint alignment method and specify the tps lambda value: 
-
-```
-python scripts/run.py \
-    --run_mode train \
-    --num_keypoints 128 \
-    --kp_align_method tps \
-    --tps_lmbda 0 \
-    --loss_fn dice \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
+    --loss_fn mse \
+    --transform_type affine \
+    --train_dataset ixi \
+    --data_path ./centered_IXI \
+    --max_random_affine_augment_params (0.2, 0.2, 3.1416, 0.1) \
+    --load_path ./weights/numkey128_pretrain.2500.h5 
 ```
 
-The code also supports sampling lambda according to some distribution (`uniform`, `lognormal`, `loguniform`). For example, to sample from the `loguniform` distribution during training:
+`--load_path <path>` specifies the path to the pretraining weights.
 
-```
+### Evaluating KeyMorph
+```bash
 python scripts/run.py \
+    --run_mode eval \
     --num_keypoints 128 \
-    --kp_align_method tps \
-    --tps_lmbda loguniform \
     --loss_fn dice \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
+    --transform_type tps_0 \
+    --data_dir ./centered_IXI \
+    --load_path ./weights/best_trained_model.h5 \
+    --save_eval_to_disk
 ```
 
-Note that supervised/unsupervised variants can be run similarly to affine, as described above. 
-
-## Step-by-step guide for reproducing our results
-
-### Dataset 
-[A] Scripts in `./notebooks/[A] Download Data` will download the IXI data and perform some basic preprocessing
-
-[B] Once the data is downloaded `./notebooks/[B] Brain extraction` can be used to extract remove non-brain tissue. 
-
-[C] Once the brain has been extracted, we center the brain using `./notebooks/[C] Centering`. During training, we randomly introduce affine augmentation to the dataset. This ensure that the brain stays within the volume given the affine augmentation we introduce. It also helps during the pretraining step of our algorithm.
-
-### Pretraining KeyMorph
-
-This step helps with the convergence of our model. We pick 1 subject and random points within the brain of that subject. We then introduce affine transformation to the subject brain and same transformation to the keypoints. In other words, this is a self-supervised task in where the network learns to predict the keypoints on a brain under random affine transformation. We found that initializing our model with these weights helps with the training.
-
-To pretrain, run:
- 
-```
-python scripts/run.py --run_mode pretrain --num_keypoints 128 --data_dir ./data/centered_IXI/ 
-```
-
-### Training KeyMorph
-Follow instructions for "Training KeyMorph" above, depending on the variant you want.
-
-### Evaluating KeyMorph
-To evaluate on the test set, simply add the `--eval` flag to any of the above commands. For example, for affine, unsupervised KeyMorph evaluation:
-
-```
-python run.py --kp_align_method affine --num_keypoints 128 --loss_fn mse --eval \
-                --load_path ./weights/best_trained_model.h5
-```
-
-Evaluation proceeds by looping through all test augmentations in `list_of_test_augs`, all test modality pairs in `list_of_test_mods`, and all pairs of volumes in the test set.
-Set `--save_preds` flag to save all outputs to disk.
-
-**Automatic Delineation/Segmentation of the Brain**
-
-For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. 
+## Related Projects
++ For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. 
++ [BrainMorph](https://github.com/alanqrwang/brainmorph) is a foundation model based on the KeyMorph framework, trained on over 100,000 brain MR images at full resolution (256x256x256).
+The model is robust to normal and diseased brains, a variety of MRI modalities, and skullstripped and non-skullstripped images.
+Check out the dedicated repository for the latest updates and models!
 
 ## Issues
 This repository is being actively maintained. Feel free to open an issue for any problems or questions.
 
 ## Legacy code
 For a legacy version of the code, see our [legacy branch](https://github.com/alanqrwang/keymorph/tree/legacy).
```

### Comparing `keymorph-1.0.1/keymorph/augmentation.py` & `keymorph-1.0.2/keymorph/augmentation.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/keypoint_aligners.py` & `keymorph-1.0.2/keymorph/keypoint_aligners.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils import checkpoint
 
 
 class MatrixKeypointAligner(nn.Module):
+    """Keypoint aligner for transformations that can be represented as a matrix."""
+
     def __init__(self, dim):
         super().__init__()
         self.dim = dim
 
     def get_matrix(self, p1, p2, w=None):
+        """Get matrix given point sets p1 and p2.
+        For transformation y = A x + b, returns [A, b] concatenated matrix.
+        """
         pass
 
     def forward(self, *args, **kwargs):
         return self.grid_from_points(*args, **kwargs)
 
     def grid_from_points(
         self,
```

### Comparing `keymorph-1.0.1/keymorph/layers.py` & `keymorph-1.0.2/keymorph/layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,30 +56,41 @@
         cy = (arangey * my).sum(dim=-1, keepdim=True) / My
 
         # center of mass, shape [n_batch, chs, 2]
         return torch.cat([cx, cy], dim=-1) * 2 - 1
 
 
 class CenterOfMass3d(nn.Module):
-    def forward(self, vol):
+    def forward(self, vol, grid_lims=((-1, 1), (-1, 1), (-1, 1))):
         """
-        x: tensor of shape [n_batch, chs, dimz, dimy, dimx]
-        returns: center of mass in normalized coordinates [-1,1]x[-1,1]x[-1,1], shape [n_batch, chs, 2]
+        vol: tensor of shape [n_batch, chs, dimz, dimy, dimx]
+        grid_lims: tuple of 3 tuples, each specifying the limits of the grid in the corresponding dimension
+        returns: center of mass w.r.t. specified grid, shape [n_batch, chs, 2]
         """
         vol = F.relu(vol)
         n_batch, chs, dimz, dimy, dimx = vol.shape
         eps = 1e-8
+        xlim, ylim, zlim = grid_lims
         arangex = (
-            torch.linspace(0, 1, dimx).float().view(1, 1, -1).repeat(n_batch, chs, 1)
+            torch.linspace(xlim[0], xlim[1], dimx)
+            .float()
+            .view(1, 1, -1)
+            .repeat(n_batch, chs, 1)
         )
         arangey = (
-            torch.linspace(0, 1, dimy).float().view(1, 1, -1).repeat(n_batch, chs, 1)
+            torch.linspace(ylim[0], ylim[1], dimy)
+            .float()
+            .view(1, 1, -1)
+            .repeat(n_batch, chs, 1)
         )
         arangez = (
-            torch.linspace(0, 1, dimz).float().view(1, 1, -1).repeat(n_batch, chs, 1)
+            torch.linspace(zlim[0], zlim[1], dimz)
+            .float()
+            .view(1, 1, -1)
+            .repeat(n_batch, chs, 1)
         )
 
         arangex, arangey, arangez = (
             arangex.to(vol.device),
             arangey.to(vol.device),
             arangez.to(vol.device),
         )
@@ -95,15 +106,15 @@
 
         # center of mass along dimN, shape [n_batch, chs, 1]
         cx = (arangex * mx).sum(dim=-1, keepdim=True) / Mx
         cy = (arangey * my).sum(dim=-1, keepdim=True) / My
         cz = (arangez * mz).sum(dim=-1, keepdim=True) / Mz
 
         # center of mass, shape [n_batch, chs, 3]
-        return torch.cat([cx, cy, cz], dim=-1) * 2 - 1
+        return torch.cat([cx, cy, cz], dim=-1)
 
 
 class ConvBlock(nn.Module):
     def __init__(
         self, in_channels, out_channels, stride, norm_type, down_sample=True, dim=2
     ):
         super(ConvBlock, self).__init__()
```

### Comparing `keymorph-1.0.1/keymorph/loss_ops.py` & `keymorph-1.0.2/keymorph/loss_ops.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/model.py` & `keymorph-1.0.2/keymorph/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             return True
         return False
 
     def forward(self, img_f, img_m, transform_type="affine", **kwargs):
         """Forward pass for one mini-batch step.
 
         :param img_f, img_m: Fixed and moving images
-        :param align_type: str or tuple of str of keypoint alignment types. Used for finding registrations
+        :param transform_type: str or tuple of str of keypoint alignment types. Used for finding registrations
             for multiple alignment types in one forward pass, without having to extract keypoints
             every time.
 
         :return res: Dictionary of results
         """
         start_time = time.time()
         return_aligned_points = kwargs["return_aligned_points"]
@@ -242,14 +242,18 @@
                 "points_m": points_m,
                 "points_weights": weights,
                 "tps_lmbda": tps_lmbda,
                 "time_keypoint_extract": keypoint_extract_time,
                 "time_align": align_time,
                 "time": keypoint_extract_time + align_time,
             }
+            if align_type in ["rigid", "affine"]:
+                res["matrix"] = keypoint_aligner.get_matrix(
+                    points_m, points_f, w=weights
+                )
             if return_aligned_points:
                 points_a = keypoint_aligner.points_from_points(
                     points_m, points_f, points_m, lmbda=tps_lmbda, weights=weights
                 )
                 res["points_a"] = points_a
             result_dict[align_type_str] = res
         return result_dict
```

### Comparing `keymorph-1.0.1/keymorph/net.py` & `keymorph-1.0.2/keymorph/net.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/buildingblocks.py` & `keymorph-1.0.2/keymorph/unet3d/buildingblocks.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/config.py` & `keymorph-1.0.2/keymorph/unet3d/config.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/losses.py` & `keymorph-1.0.2/keymorph/unet3d/losses.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/metrics.py` & `keymorph-1.0.2/keymorph/unet3d/metrics.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/model.py` & `keymorph-1.0.2/keymorph/unet3d/model.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/predictor.py` & `keymorph-1.0.2/keymorph/unet3d/predictor.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/se.py` & `keymorph-1.0.2/keymorph/unet3d/se.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/seg_metrics.py` & `keymorph-1.0.2/keymorph/unet3d/seg_metrics.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/trainer.py` & `keymorph-1.0.2/keymorph/unet3d/trainer.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/unet3d/utils.py` & `keymorph-1.0.2/keymorph/unet3d/utils.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.1/keymorph/utils.py` & `keymorph-1.0.2/keymorph/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,21 @@
 #     x = itk.image_view_from_array(x)
 #     transform_parameters.SetParameter("FinalBSplineInterpolationOrder", "0")
 #     result_image = itk.transformix_filter(x, transform_parameters)
 #     res = torch.tensor(itk.array_view_from_image(result_image))
 #     return res
 
 
-def displacement2flow(displacement_field):
-    """displacement_field: (N, D, H, W, 3).
-    Assumes original space is physical space (voxel units), 256x256x256."""
+def displacement2pytorchflow(displacement_field):
+    """Converts displacement field in index coordinates into a flow-field usable by F.grid_sample.
+    Assumes original space is in index (voxel) units, 256x256x256.
+    Output will be in the [-1, 1] space.
+
+    :param: displacement_field: (N, D, H, W, 3).
+    """
     W, H, D = displacement_field.shape[1:-1]
 
     # Step 1: Create the original grid for 3D
     coords_x, coords_y, coords_z = torch.meshgrid(
         torch.linspace(-1, 1, W),
         torch.linspace(-1, 1, H),
         torch.linspace(-1, 1, D),
@@ -59,14 +63,36 @@
         # Normalize such that the displacement of 1 full dimension length corresponds to a move from -1 to 1
         displacement_field[..., i] = 2 * displacement_field[..., i] / (dim_size - 1)
 
     # Step 3: Add the displacement field to the original grid to get the transformed coordinates
     return coords + displacement_field
 
 
+def pytorchflow2displacement(flow):
+    """Converts pytorch flow-field in [-1, 1] to a displacement field in index (voxel) units
+
+    :param: flow: (N, D, H, W, 3).
+    """
+    flow = flow.permute(0, 4, 1, 2, 3)  # Bring channels to second dimension
+    shape = flow.shape[2:]
+
+    # Scale normalized flow to pixel indices
+    for i in range(3):
+        flow[:, i, ...] = (flow[:, i, ...] + 1) / 2 * (shape[i] - 1)
+
+    # Create an image grid for the target size
+    vectors = [torch.arange(0, s) for s in shape]
+    grids = torch.meshgrid(vectors, indexing="ij")
+    grid = torch.stack(grids, dim=0).unsqueeze(0).to(flow.device, dtype=torch.float32)
+
+    # Calculate displacements from the image grid
+    disp = flow - grid
+    return disp
+
+
 def rescale_intensity(array, out_range=(0, 1), percentiles=(0, 100)):
     if isinstance(array, torch.Tensor):
         array = array.float()
 
     if percentiles != (0, 100):
         cutoff = np.percentile(array, percentiles)
         np.clip(array, *cutoff, out=array)  # type: ignore[call-overload]
```

### Comparing `keymorph-1.0.1/keymorph/viz_tools.py` & `keymorph-1.0.2/keymorph/viz_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,32 +138,34 @@
 
 
 def imshow_img_and_points_3d(
     img=None,
     all_points=None,
     all_weights=None,
     projection=False,
-    center_slices=(128, 128, 128),
     slab_thickness=10,
     axes=None,
     rotate_90_deg=0,
-    img_dims=(256, 256, 256),
     markers=(".", "x"),
 ):
     """
     Plots 3 orthogonal slices of a 3D image and overlays points on them.
 
     img: (H, W, D) image
     all_points: (N, 3) or (1, N, 3) or (2, N, 3) array of points.
         Points can be defined on:
          1. the Pytorch grid, i.e. in [-1, 1]
          2. the image grid, e.g. in [0, 256]
         The code converts Pytorch grids to image grids by internally checking if
     all_weights: (N,) or (1, N) or (2, N) array of weights
     """
+    print(img.shape)
+    print(all_points.shape)
+    img_dims = img.shape[-3:]
+    center_slices = (img_dims[0] // 2, img_dims[1] // 2, img_dims[2] // 2)
 
     def normalize(data):
         return (data - np.min(data)) / (np.max(data) - np.min(data))
 
     plot_img = True if img is not None else None
     plot_points = True if all_points is not None else None
```

### Comparing `keymorph-1.0.1/keymorph.egg-info/PKG-INFO` & `keymorph-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keymorph
-Version: 1.0.1
+Version: 1.0.2
 Summary: KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints.
 Home-page: https://github.com/alanqrwang/keymorph
 Author: Alan Q. Wang
 Author-email: alanqrwang@gmail.com
 License: MIT
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
@@ -23,14 +23,15 @@
 As an example, it uses data from the [IXI dataset](https://brain-development.org/ixi-dataset/) to train and evaluate the model.
 
 [BrainMorph](https://github.com/alanqrwang/brainmorph) is a foundation model based on the KeyMorph framework, trained on over 100,000 brain MR images at full resolution (256x256x256).
 The model is robust to normal and diseased brains, a variety of MRI modalities, and skullstripped and non-skullstripped images.
 Check out the dedicated repository for the latest updates and models!
 
 ## Updates
+- [May 2024] Added option to use CSV file to train KeyMorph on your own data. See "Training KeyMorph on your own data" below.
 - [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) has been moved to its own dedicated repository. See the repository for the latest updates and models.
 - [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) is released, a foundational keypoint model based on KeyMorph for robust and flexible brain MRI registration!
 - [Dec 2023] [Journal paper](https://arxiv.org/abs/2304.09941) extension of MIDL paper published in Medical Image Analysis. Instructions under "IXI-trained, half-resolution models".
 - [Feb 2022] [Conference paper](https://openreview.net/forum?id=OrNzjERFybh) published in MIDL 2021.
 
 ## Installation
 
@@ -63,17 +64,115 @@
 Running `pip install keymorph` or `pip install -e .` will automatically check for and install all of these requirements.
 
 ## Downloading Trained Weights
 You can find all full-resolution, BrainMorph trained weights [here](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i).
 Half-resolution trained weights are under [Releases](https://github.com/alanqrwang/keymorph/releases).
 Download your preferred model(s) and put them in the folder specified by `--weights_dir` in the commands below.
 
+
+## TLDR in code
+The crux of the code is in the `forward()` function in `keymorph/model.py`, which performs one forward pass through the entire KeyMorph pipeline.
+
+Here's a pseudo-code version of the function:
+```python
+def forward(img_f, img_m, seg_f, seg_m, network, optimizer, kp_aligner):
+    '''Forward pass for one mini-batch step. 
+    Variables with (_f, _m, _a) denotes (fixed, moving, aligned).
+    
+    Args:
+        img_f, img_m: Fixed and moving intensity image (bs, 1, l, w, h)
+        seg_f, seg_m: Fixed and moving one-hot segmentation map (bs, num_classes, l, w, h)
+        network: Keypoint extractor network
+        kp_aligner: Rigid, affine or TPS keypoint alignment module
+    '''
+    optimizer.zero_grad()
+
+    # Extract keypoints
+    points_f = network(img_f)
+    points_m = network(img_m)
+
+    # Align via keypoints
+    grid = kp_aligner.grid_from_points(points_m, points_f, img_f.shape, lmbda=lmbda)
+    img_a, seg_a = utils.align_moving_img(grid, img_m, seg_m)
+
+    # Compute losses
+    mse = MSELoss()(img_f, img_a)
+    soft_dice = DiceLoss()(seg_a, seg_f)
+
+    if unsupervised:
+        loss = mse
+    else:
+        loss = soft_dice
+
+    # Backward pass
+    loss.backward()
+    optimizer.step()
+```
+The `network` variable is a CNN with center-of-mass layer which extracts keypoints from the input images.
+The `kp_aligner` variable is a keypoint alignment module. It has a function `grid_from_points()` which returns a flow-field grid encoding the transformation to perform on the moving image. The transformation can either be rigid, affine, or nonlinear (TPS).
+
+## Training KeyMorph on your own data
+`scripts/run.py` with `--run_mode train` allows you to easily train KeyMorph on your own data.
+
+### Create a CSV file
+The CSV file should contain the following columns: `img_path`, `seg_path`, `mask_path`, `modality`, `train`.
++ `img_path` is the path to the intensity image.
++ `seg_path` is the (optional )path to the corresponding segmentation map. Set to "None" if not available.
++ `mask_path` is the (optional) path to the mask. Set to "None" if not available.
++ `modality` is the modality of the image.
++ `train` is a boolean indicating whether the image is in the train or test set.
+
+Then, simply pass the path to the CSV file as `--data_csv_path`.
+
+### Editing pre-processing/augmentations
+You probably need to set the `TRANSFORM` variable in `scripts/hyperparameters.py` to correspond to the pre-processing/augmentations that you want to apply to your own data.
+The code uses `torchio` for pre-processing and augmentations. You can find the list of available transforms [here](https://torchio.readthedocs.io/transforms/augmentation.html).
+You can also use your own custom transforms by wrapping them in the [Lambda](https://torchio.readthedocs.io/transforms/others.html#torchio.transforms.Lambda) transform.
+
+Note, affine augmentations are applied separately and is determined by the `--max_random_affine_augment_params` flag in `scripts/run.py`. By default, it is set to `(0.0, 0.0, 0.0, 0.0)`. For example, `(0.2, 0.2, 3.1416, 0.1)` denotes:
++ Scaling by [1-0.2, 1+0.2]
++ Translation by [-0.2, 0.2], as a fraction of the image size
++ Rotation by [-3.1416, 3.1416] radians
++ Shearing by [-0.1, 0.1]
+
+### Run the training script
+We use the weights from the pretraining step to initialize our model.
+Our pretraining weights are provided in [Releases](https://github.com/evanmy/keymorph/releases/tag/weights).
+
+
+```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --loss_fn mse \
+    --transform_type affine \
+    --train_dataset csv \
+    --data_path /path/to/data_csv
+```
+
+
+Description of all flags:
++ `--num_keypoints <num_key>` flag specifies the number of keypoints to extract per image as `<num_key>`.
++ `--loss_fn <loss>` specifies the loss function to train. Options are `mse` (unsupervised training) and `dice` (supervised training). Unsupervised only requires intensity images and minimizes MSE loss, while supervised assumes availability of corresponding segmentation maps for each image and minimizes soft Dice loss.
++ `--transform_type <ttype>`. 
+Transform to use for registration. Options are `rigid`, `affine`, `tps_<lambda>`.
+TPS uses a (non-linear) thin-plate-spline interpolant to align the corresponding keypoints. A hyperparameter lambda controls the degree of non-linearity for TPS. A value of 0 corresponds to exact keypoint alignment (resulting in a maximally nonlinear transformation while still minimizing bending energy), while higher values result in the transformation becoming more and more affine-like. In practice, we find a value of 10 is very similar to an affine transformation.
+The code also supports sampling lambda according to some distribution (`tps_uniform`, `tps_lognormal`, `tps_loguniform`).
++ `--train_dataset csv` specifies that we are training on a csv dataset specified by...
++ `--data_path <path>` specifies the path to the CSV file containing the dataset.
+
+Other optional flags:
++  `--mix_modalities` flag, if set, mixes modalities between sampled pairs during training. You should probably set this when `--loss_fn dice` (supervised training), and not when `--loss_fn mse` (unsupervised training).
++ `--visualize` flag to visualize results with matplotlib
++ `--debug_mode` flag to print some debugging information
++ `--use_wandb` flag to log results to Weights & Biases
+
 ## Registering brain volumes 
 ### BrainMorph
-Warning: Please see the [BrainMorph repository](https://github.com/alanqrwang/brainmorph) for the latest updates and models! This is a legacy version of the code and is not guaranteed to be maintained.
+WARNING: Please see the [BrainMorph repository](https://github.com/alanqrwang/brainmorph) for the latest updates and models! This is a legacy version of the code and is not guaranteed to be maintained.
 
 BrainMorph is trained on over 100,000 brain MR images at full resolution (256x256x256). 
 The script will automatically min-max normalize the images and resample to 1mm isotropic resolution.
 
 `--num_keypoints` and `num_levels_for_unet` will determine which model will be used to perform the registration.
 Make sure the corresponding weights are present in `--weights_dir`.
 `--num_keypoints` can be set to `128, 256, 512` and `--num_levels_for_unet` can be set to `4, 5, 6, 7`, respectively (corresponding to 'S', 'M', 'L', 'H' in the paper).
@@ -155,192 +254,76 @@
     --fixed_seg ./example_data_half/seg_m/IXI_002_128x128x128.nii.gz \
     --list_of_aligns affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
-## TLDR in code
-The crux of the code is in the `forward()` function in `keymorph/model.py`, which performs one forward pass through the entire KeyMorph pipeline.
-
-Here's a pseudo-code version of the function:
-```python
-def forward(img_f, img_m, seg_f, seg_m, network, optimizer, kp_aligner):
-    '''Forward pass for one mini-batch step. 
-    Variables with (_f, _m, _a) denotes (fixed, moving, aligned).
-    
-    Args:
-        img_f, img_m: Fixed and moving intensity image (bs, 1, l, w, h)
-        seg_f, seg_m: Fixed and moving one-hot segmentation map (bs, num_classes, l, w, h)
-        network: Keypoint extractor network
-        kp_aligner: Rigid, affine or TPS keypoint alignment module
-    '''
-    optimizer.zero_grad()
-
-    # Extract keypoints
-    points_f = network(img_f)
-    points_m = network(img_m)
-
-    # Align via keypoints
-    grid = kp_aligner.grid_from_points(points_m, points_f, img_f.shape, lmbda=lmbda)
-    img_a, seg_a = utils.align_moving_img(grid, img_m, seg_m)
-
-    # Compute losses
-    mse = MSELoss()(img_f, img_a)
-    soft_dice = DiceLoss()(seg_a, seg_f)
-
-    if unsupervised:
-        loss = mse
-    else:
-        loss = soft_dice
-
-    # Backward pass
-    loss.backward()
-    optimizer.step()
-```
-The `network` variable is a CNN with center-of-mass layer which extracts keypoints from the input images.
-The `kp_aligner` variable is a keypoint alignment module. It has a function `grid_from_points()` which returns a flow-field grid encoding the transformation to perform on the moving image. The transformation can either be rigid, affine, or nonlinear (TPS).
-
-## Training KeyMorph
-Use `scripts/run.py` with `--run_mode train` to train KeyMorph.
-
-We use the weights from the pretraining step to initialize our model.
-Our pretraining weights are provided in [Releases](https://github.com/evanmy/keymorph/releases/tag/weights).
-
-The `--num_keypoints <num_key>` flag specifies the number of keypoints to extract per image as `<num_key>`.
-For all commands, optionally add the `--use_wandb` flag to log results to Weights & Biases.
-
-This repository supports several variants of training KeyMorph.
-Here's a overview of the variants:
-
-### Supervised vs. unsupervised
-Unsupervised only requires intensity images and minimizes MSE loss, while supervised assumes availability of corresponding segmentation maps for each image and minimizes soft Dice loss.
-
-To specify unsupervised, set `--loss_fn mse`.
-To specify supervised, set `--loss_fn dice`.
-
+## Step-by-step guide for reproducing our results
 
-### Affine vs. TPS
-Affine uses an affine transformation to align the corresponding keypoints.
+### Dataset 
+[A] Scripts in `./notebooks/[A] Download Data` will download the IXI data and perform some basic preprocessing
 
-TPS uses a (non-linear) thin-plate-spline interpolant to align the corresponding keypoints. A hyperparameter `--tps_lmbda` controls the degree of non-linearity for TPS. A value of 0 corresponds to exact keypoint alignment (resulting in a maximally nonlinear transformation while still minimizing bending energy), while higher values result in the transformation becoming more and more affine-like. In practice, we find a value of 10 is very similar to an affine transformation.
+[B] Once the data is downloaded `./notebooks/[B] Brain extraction` can be used to extract remove non-brain tissue. 
 
-To specify affine, set `--kp_align_method affine`.
-To specify tps, set `--kp_align_method tps` and the lmbda value `--tps_lmbda 0`.
+[C] Once the brain has been extracted, we center the brain using `./notebooks/[C] Centering`. During training, we randomly introduce affine augmentation to the dataset. This ensure that the brain stays within the volume given the affine augmentation we introduce. It also helps during the pretraining step of our algorithm.
 
-### Example commands
-**Affine, Unsupervised**
+### Pretraining KeyMorph
 
-To train unsupervised KeyMorph with affine transformation and 128 keypoints, use `mse` as the loss function:
+This step helps with the convergence of our model. We pick 1 subject and random points within the brain of that subject. We then introduce affine transformation to the subject brain and same transformation to the keypoints. In other words, this is a self-supervised task in where the network learns to predict the keypoints on a brain under random affine transformation. We found that initializing our model with these weights helps with the training.
 
+To pretrain, run:
+ 
 ```bash
 python scripts/run.py \
-    --run_mode train \
+    --run_mode pretrain \
     --num_keypoints 128 \
     --loss_fn mse \
-    --transform_type affine \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
+    --transform_type tps_0 \
+    --max_random_affine_augment_params (0.2, 0.2, 3.1416, 0.1) \
+    --affine_slope 1000 \
+    --data_dir ./centered_IXI 
 ```
 
-<!-- For unsupervised KeyMorph, optionally add `--kpconsistency_coeff` to optimize keypoint consistency across modalities for same subject: -->
+`--affine_slope` linearly ramps up the ``max_random_affine_augment_params` such that it starts at 0 for all parameters and reaches their maximum values at epoch 1000. This helps the model to learn the keypoints under increasing affine transformations.
 
-<!-- ```bash
-python scripts/run.py \
-    --run_mode train \
-    --num_keypoints 128 \
-    --kp_align_method affine \
-    --loss_fn mse \
-    --kpconsistency_coeff 10 \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
-``` -->
-
-**Affine, Supervised**
-
-To train supervised KeyMorph, use `dice` as the loss function:
+### Training KeyMorph
+Follow instructions for "Training KeyMorph" above, for more options.
 
 ```bash
 python scripts/run.py \
     --run_mode train \
     --num_keypoints 128 \
-    --kp_align_method affine \
-    --loss_fn dice \
-    --mix_modalities \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
-```
-
-Note that the `--mix_modalities` flag allows fixed and moving images to be of different modalities during training. This should not be set for unsupervised training, which uses MSE as the loss function.
-
-**Nonlinear thin-plate-spline (TPS)**
-
-To train the TPS variant of KeyMorph which allows for nonlinear registrations, specify `tps` as the keypoint alignment method and specify the tps lambda value: 
-
-```
-python scripts/run.py \
-    --run_mode train \
-    --num_keypoints 128 \
-    --kp_align_method tps \
-    --tps_lmbda 0 \
-    --loss_fn dice \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
+    --loss_fn mse \
+    --transform_type affine \
+    --train_dataset ixi \
+    --data_path ./centered_IXI \
+    --max_random_affine_augment_params (0.2, 0.2, 3.1416, 0.1) \
+    --load_path ./weights/numkey128_pretrain.2500.h5 
 ```
 
-The code also supports sampling lambda according to some distribution (`uniform`, `lognormal`, `loguniform`). For example, to sample from the `loguniform` distribution during training:
+`--load_path <path>` specifies the path to the pretraining weights.
 
-```
+### Evaluating KeyMorph
+```bash
 python scripts/run.py \
+    --run_mode eval \
     --num_keypoints 128 \
-    --kp_align_method tps \
-    --tps_lmbda loguniform \
     --loss_fn dice \
-    --data_dir ./data/centered_IXI/ \
-    --load_path ./weights/numkey128_pretrain.2500.h5
-```
-
-Note that supervised/unsupervised variants can be run similarly to affine, as described above. 
-
-## Step-by-step guide for reproducing our results
-
-### Dataset 
-[A] Scripts in `./notebooks/[A] Download Data` will download the IXI data and perform some basic preprocessing
-
-[B] Once the data is downloaded `./notebooks/[B] Brain extraction` can be used to extract remove non-brain tissue. 
-
-[C] Once the brain has been extracted, we center the brain using `./notebooks/[C] Centering`. During training, we randomly introduce affine augmentation to the dataset. This ensure that the brain stays within the volume given the affine augmentation we introduce. It also helps during the pretraining step of our algorithm.
-
-### Pretraining KeyMorph
-
-This step helps with the convergence of our model. We pick 1 subject and random points within the brain of that subject. We then introduce affine transformation to the subject brain and same transformation to the keypoints. In other words, this is a self-supervised task in where the network learns to predict the keypoints on a brain under random affine transformation. We found that initializing our model with these weights helps with the training.
-
-To pretrain, run:
- 
-```
-python scripts/run.py --run_mode pretrain --num_keypoints 128 --data_dir ./data/centered_IXI/ 
+    --transform_type tps_0 \
+    --data_dir ./centered_IXI \
+    --load_path ./weights/best_trained_model.h5 \
+    --save_eval_to_disk
 ```
 
-### Training KeyMorph
-Follow instructions for "Training KeyMorph" above, depending on the variant you want.
-
-### Evaluating KeyMorph
-To evaluate on the test set, simply add the `--eval` flag to any of the above commands. For example, for affine, unsupervised KeyMorph evaluation:
-
-```
-python run.py --kp_align_method affine --num_keypoints 128 --loss_fn mse --eval \
-                --load_path ./weights/best_trained_model.h5
-```
-
-Evaluation proceeds by looping through all test augmentations in `list_of_test_augs`, all test modality pairs in `list_of_test_mods`, and all pairs of volumes in the test set.
-Set `--save_preds` flag to save all outputs to disk.
-
-**Automatic Delineation/Segmentation of the Brain**
-
-For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. 
+## Related Projects
++ For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. 
++ [BrainMorph](https://github.com/alanqrwang/brainmorph) is a foundation model based on the KeyMorph framework, trained on over 100,000 brain MR images at full resolution (256x256x256).
+The model is robust to normal and diseased brains, a variety of MRI modalities, and skullstripped and non-skullstripped images.
+Check out the dedicated repository for the latest updates and models!
 
 ## Issues
 This repository is being actively maintained. Feel free to open an issue for any problems or questions.
 
 ## Legacy code
 For a legacy version of the code, see our [legacy branch](https://github.com/alanqrwang/keymorph/tree/legacy).
```

### Comparing `keymorph-1.0.1/keymorph.egg-info/SOURCES.txt` & `keymorph-1.0.2/keymorph.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 keymorph/unet3d/metrics.py
 keymorph/unet3d/model.py
 keymorph/unet3d/predictor.py
 keymorph/unet3d/se.py
 keymorph/unet3d/seg_metrics.py
 keymorph/unet3d/trainer.py
 keymorph/unet3d/utils.py
-tests/test.py
+test/__init__.py
+test/test.py
```

### Comparing `keymorph-1.0.1/setup.py` & `keymorph-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 sys.path.insert(0, os.path.join(here, "keymorph"))
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="keymorph",
-    version="1.0.1",
+    version="1.0.2",
     author="Alan Q. Wang",
     author_email="alanqrwang@gmail.com",
     url="https://github.com/alanqrwang/keymorph",
     description="KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `keymorph-1.0.1/tests/test.py` & `keymorph-1.0.2/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,35 +318,14 @@
             [[np.cos(r), -np.sin(r), 0, 0], [np.sin(r), np.cos(r), 0, 0], [0, 0, 1, 0]]
         ).float()
         true = true.view(1, 3, 4)
         weights = torch.tensor([1, 1, 1, 1]).float().view(1, -1)
         result = rigid_aligner.get_matrix(input1, input2, w=weights)
         assert_close(result, true)
 
-    def test_rigid_5(self):
-        """Test 2d rotation around z-axis plus scaling for 3d points, with weights. Should ignore scaling."""
-        rigid_aligner = RigidKeypointAligner(dim=2)
-
-        input1 = torch.tensor([[1, 0, 0], [0, -1, 0], [-1, 0, 0], [0, 1, 0]]).float()
-        input2 = torch.tensor([[0, -1, 0], [-1, 0, 0], [0, 1, 0], [1, 0, 0]]).float()
-        # Scaling
-        input2 *= 2
-        input1 = input1.view(1, 4, 3)
-        input2 = input2.view(1, 4, 3)
-
-        r = -np.pi / 2
-        true = torch.tensor(
-            [[np.cos(r), -np.sin(r), 0, 0], [np.sin(r), np.cos(r), 0, 0], [0, 0, 1, 0]]
-        ).float()
-        true = true.view(1, 3, 4)
-
-        weights = torch.tensor([0, 0, 0, 1]).float().view(1, -1)
-        result = rigid_aligner.get_matrix(input1, input2, w=weights)
-        assert_close(result, true)
-
 
 class TestAffineAligner(unittest.TestCase):
     def test_affine_0(self):
         """Test 2d rotation around z-axis for 2d points."""
         affine_aligner = AffineKeypointAligner(dim=2)
 
         input1 = torch.tensor([[1, 0], [0, -1], [-1, 0], [0, 1]]).float()
@@ -363,27 +342,28 @@
         assert_close(result, true)
 
     def test_affine_1(self):
         """Test 2d rotation around z-axis for 2d points plus scaling."""
         affine_aligner = AffineKeypointAligner(dim=2)
 
         input1 = torch.tensor([[1, 0], [0, -1], [-1, 0], [0, 1]]).float()
-        input2 = torch.tensor([[0, -1], [-1, 0], [0, 1], [1, 0]]).float()
+        input2 = torch.tensor([[0, -2], [-2, 0], [0, 2], [2, 0]]).float()
         input1 = input1.view(1, 4, 2)
         input2 = input2.view(1, 4, 2)
 
         r = -np.pi / 2
         rot_mat = torch.tensor(
             [[np.cos(r), -np.sin(r)], [np.sin(r), np.cos(r)]]
         ).float()
-        sca_mat = torch.tensor([[0.5, 0], [0, 0.5]]).float()
+        sca_mat = torch.tensor([[2, 0], [0, 2]]).float()
+        # input2 is rotated, and then scaled by 2
 
+        # Output should be [A, b] concatenated matrix
         true = torch.zeros(2, 3)
         true[:2, :2] = rot_mat @ sca_mat
-        true[-1, -1] = 1
         true = true.view(1, 2, 3)
         result = affine_aligner.get_matrix(input1, input2)
         assert_close(result, true)
 
 
 if __name__ == "__main__":
     unittest.main()
```

