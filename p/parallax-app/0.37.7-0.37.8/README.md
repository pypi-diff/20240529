# Comparing `tmp/parallax_app-0.37.7.tar.gz` & `tmp/parallax_app-0.37.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallax_app-0.37.7.tar", last modified: Wed May 22 22:21:46 2024, max compression
+gzip compressed data, was "parallax_app-0.37.8.tar", last modified: Tue May 28 22:58:48 2024, max compression
```

## Comparing `parallax_app-0.37.7.tar` & `parallax_app-0.37.8.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.794746 parallax_app-0.37.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.778746 parallax_app-0.37.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.778746 parallax_app-0.37.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 22:21:06.000000 parallax_app-0.37.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-22 22:21:06.000000 parallax_app-0.37.7/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 22:21:06.000000 parallax_app-0.37.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 22:21:06.000000 parallax_app-0.37.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 22:21:06.000000 parallax_app-0.37.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-22 22:21:46.794746 parallax_app-0.37.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-22 22:21:06.000000 parallax_app-0.37.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.782746 parallax_app-0.37.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/ReadMe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/parallax.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.782746 parallax_app-0.37.7/img/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/recordingButton.png
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/sextant.png
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/snapshotButton_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/stop-sign.png
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/target.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.786746 parallax_app-0.37.7/parallax/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/axis_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/calibration_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27905 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/curr_bg_cmp_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/curr_prev_cmp_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    32369 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/main_window_wip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/mask_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6058 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/no_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15573 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/probe_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/probe_detect_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/probe_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/probe_fine_tip_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/recording_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/reticle_detect_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/reticle_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/reticle_detection_coords_interests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13577 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/screen_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/stage_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/stage_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    39667 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/user_setting_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.790746 parallax_app-0.37.7/parallax_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 22:21:06.000000 parallax_app-0.37.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:21:46.794746 parallax_app-0.37.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-22 22:21:06.000000 parallax_app-0.37.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.786746 parallax_app-0.37.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-22 22:21:06.000000 parallax_app-0.37.7/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-22 22:21:06.000000 parallax_app-0.37.7/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-22 22:21:06.000000 parallax_app-0.37.7/tests/test_screen_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.790746 parallax_app-0.37.7/ui/
--rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/ParallaxReadME.JPG
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.790746 parallax_app-0.37.7/ui/font/
--rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/font/FiraCode-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/mainWindow.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/probe_calib.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.790746 parallax_app-0.37.7/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/check.png
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/recordingButton.png
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/recordingButton_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/sextant.png
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/snapshotButton_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/snapshotButton_green.png
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/snapshotButton_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/stop-sign.png
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/target.png
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/x.png
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/reticle_calib.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/settingPopUpMenu.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/stage_info.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.394233 parallax_app-0.37.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.378233 parallax_app-0.37.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.378233 parallax_app-0.37.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-28 22:58:11.000000 parallax_app-0.37.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-28 22:58:11.000000 parallax_app-0.37.8/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 22:58:11.000000 parallax_app-0.37.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 22:58:11.000000 parallax_app-0.37.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-28 22:58:11.000000 parallax_app-0.37.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-28 22:58:48.394233 parallax_app-0.37.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-28 22:58:11.000000 parallax_app-0.37.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.382233 parallax_app-0.37.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/ReadMe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/parallax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.382233 parallax_app-0.37.8/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/target.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.386233 parallax_app-0.37.8/parallax/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/axis_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/calibration_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27905 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/coords_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/curr_bg_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/curr_prev_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32369 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/main_window_wip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/mask_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6058 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/no_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16261 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/probe_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/probe_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/probe_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/probe_fine_tip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/recording_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/reticle_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/reticle_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/reticle_detection_coords_interests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13577 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/screen_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/stage_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/stage_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39642 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/stage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/user_setting_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/parallax_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-28 22:58:11.000000 parallax_app-0.37.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 22:58:48.394233 parallax_app-0.37.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 22:58:11.000000 parallax_app-0.37.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 22:58:11.000000 parallax_app-0.37.8/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 22:58:11.000000 parallax_app-0.37.8/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-28 22:58:11.000000 parallax_app-0.37.8/tests/test_screen_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/ParallaxReadME.JPG
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/ui/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/font/FiraCode-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/mainWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/probe_calib.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/check.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/recordingButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/snapshotButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/snapshotButton_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/target.png
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/reticle_calib.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/settingPopUpMenu.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/stage_info.ui
```

### Comparing `parallax_app-0.37.7/.github/workflows/ci.yml` & `parallax_app-0.37.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/.github/workflows/tag_and_publish.yml` & `parallax_app-0.37.8/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/LICENSE` & `parallax_app-0.37.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/PKG-INFO` & `parallax_app-0.37.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.7
+Version: 0.37.8
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: MIT
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parallax_app-0.37.7/README.md` & `parallax_app-0.37.8/README.md`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/docs/Makefile` & `parallax_app-0.37.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/docs/ReadMe.rst` & `parallax_app-0.37.8/docs/ReadMe.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/docs/conf.py` & `parallax_app-0.37.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/docs/make.bat` & `parallax_app-0.37.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/docs/parallax.rst` & `parallax_app-0.37.8/docs/parallax.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/img/arrow-right.png` & `parallax_app-0.37.8/img/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/img/gear.png` & `parallax_app-0.37.8/img/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/img/recordingButton.png` & `parallax_app-0.37.8/img/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/img/sextant.png` & `parallax_app-0.37.8/img/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/img/snapshotButton_white.png` & `parallax_app-0.37.8/img/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/img/stop-sign.png` & `parallax_app-0.37.8/img/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/img/target.png` & `parallax_app-0.37.8/img/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/__main__.py` & `parallax_app-0.37.8/parallax/__main__.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/axis_filter.py` & `parallax_app-0.37.8/parallax/axis_filter.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/calibration_camera.py` & `parallax_app-0.37.8/parallax/calibration_camera.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/camera.py` & `parallax_app-0.37.8/parallax/camera.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/curr_bg_cmp_processor.py` & `parallax_app-0.37.8/parallax/curr_bg_cmp_processor.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/curr_prev_cmp_processor.py` & `parallax_app-0.37.8/parallax/curr_prev_cmp_processor.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/main_window_wip.py` & `parallax_app-0.37.8/parallax/main_window_wip.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/mask_generator.py` & `parallax_app-0.37.8/parallax/mask_generator.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/model.py` & `parallax_app-0.37.8/parallax/model.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/no_filter.py` & `parallax_app-0.37.8/parallax/no_filter.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/probe_calibration.py` & `parallax_app-0.37.8/parallax/probe_calibration.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import os
 
 import numpy as np
 import pandas as pd
 from PyQt5.QtCore import QObject, pyqtSignal
 from sklearn.linear_model import LinearRegression
-from sklearn.linear_model import Ridge
+from coords_transformation import RotationTransformation
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
@@ -44,14 +44,15 @@
     """Class for probe calibration."""
 
     def __init__(self, stage_listener):
         """
         Initializes the ProbeCalibration object with a given stage listener.
         """
         super().__init__()
+        self.transformer = RotationTransformation()
         self.stage_listener = stage_listener
         self.stage_listener.probeCalibRequest.connect(self.update)
         self.stages = {}
         self.df = None
         self.inliers = []
         self.stage = None
         self.threshold_min_max = 2500 
@@ -145,15 +146,15 @@
         """
         self.df = pd.read_csv(self.csv_file)
         # Filter the DataFrame based on self.stage.sn
         filtered_df = self.df[self.df["sn"] == self.stage.sn]
         # Extract local and global points
         local_points = filtered_df[["local_x", "local_y", "local_z"]].values
         global_points = filtered_df[["global_x", "global_y", "global_z"]].values
-        
+
         return local_points, global_points
 
     def _get_transM_LR(self, local_points, global_points):
         """
         Computes the transformation matrix from local to global coordinates.
 
         Args:
@@ -179,19 +180,39 @@
 
         # Combine weights and bias to form the transformation matrix
         transformation_matrix = np.hstack([weights, bias.reshape(-1, 1)])
         # Adding the extra row to complete the affine transformation matrix
         transformation_matrix = np.vstack([transformation_matrix, [0, 0, 0, 1]])
 
         return model, transformation_matrix
+    
+    def _get_transM_LR_orthogonal(self, local_points, global_points):
+        """
+        Computes the transformation matrix from local to global coordinates using orthogonal distance regression.
+        Args:
+            local_points (np.array): Array of local points.
+            global_points (np.array): Array of global points.
+        Returns:
+            tuple: Linear regression model and transformation matrix.
+        """
+
+        origin, R = self.transformer.fit_params(local_points, global_points)
+        transformation_matrix = np.hstack([R, origin.reshape(-1, 1)])
+        transformation_matrix = np.vstack([transformation_matrix, [0, 0, 0, 1]])
+
+        return transformation_matrix
 
     def _update_local_global_point(self, debug_info=None):
         """
         Updates the CSV file with a new set of local and global points from the current stage position.
         """
+        # Check if stage_z_global is under 10 microns
+        if self.stage.stage_z_global < 10:
+            return  # Do not update if condition is met (to avoid noise)
+        
         with open(self.csv_file, "a", newline='') as file:
             writer = csv.writer(file)
             row_data = [
                 self.stage.sn,
                 self.stage.stage_x,
                 self.stage.stage_y,
                 self.stage.stage_z,
@@ -344,25 +365,14 @@
                     logger.debug("Enough points gathered.")
                     return True
 
         self.transM_LR_prev = self.transM_LR
         return False
 
     def _update_info_ui(self):
-        """
-        x_diff = self.max_x - self.min_x
-        y_diff = self.max_y - self.min_y
-        z_diff = self.max_z - self.min_z
-        self.transM_info.emit(
-            self.stage.sn,
-            self.transM_LR,
-            self.LR_err_L2_current,
-            np.array([x_diff, y_diff, z_diff]),
-        )
-        """
         sn = self.stage.sn
         if sn is not None and sn in self.stages:
             stage_data = self.stages[sn]
             
             x_diff = stage_data['max_x'] - stage_data['min_x']
             y_diff = stage_data['max_y'] - stage_data['min_y']
             z_diff = stage_data['max_z'] - stage_data['min_z']
@@ -382,17 +392,19 @@
             stage (Stage): The current stage object with new position data.
         """
         # update points in the file
         self.stage = stage
         self._update_local_global_point(debug_info)
         # get whole list of local and global points in pd format
         local_points, global_points = self._get_local_global_points()
-        self.model_LR, self.transM_LR = self._get_transM_LR(
-            local_points, global_points
-        )
+        
+        if len(local_points) < 3 or len(global_points) < 3:
+            return
+        self.transM_LR = self._get_transM_LR_orthogonal(local_points, global_points)
+        
         self.LR_err_L2_current = self._l2_error_current_point()
         self._update_min_max_x_y_z()  # update min max x,y,z
 
         # update transformation matrix and overall LR in UI
         self._update_info_ui()
 
         # if ret, send the signal
```

### Comparing `parallax_app-0.37.7/parallax/probe_detect_manager.py` & `parallax_app-0.37.8/parallax/probe_detect_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/probe_detector.py` & `parallax_app-0.37.8/parallax/probe_detector.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/probe_fine_tip_detector.py` & `parallax_app-0.37.8/parallax/probe_fine_tip_detector.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/recording_manager.py` & `parallax_app-0.37.8/parallax/recording_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/reticle_detect_manager.py` & `parallax_app-0.37.8/parallax/reticle_detect_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/reticle_detection.py` & `parallax_app-0.37.8/parallax/reticle_detection.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/reticle_detection_coords_interests.py` & `parallax_app-0.37.8/parallax/reticle_detection_coords_interests.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/screen_widget.py` & `parallax_app-0.37.8/parallax/screen_widget.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/stage_listener.py` & `parallax_app-0.37.8/parallax/stage_listener.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/stage_ui.py` & `parallax_app-0.37.8/parallax/stage_ui.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/stage_widget.py` & `parallax_app-0.37.8/parallax/stage_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,18 +682,19 @@
                     screen.probe_coords_detected.disconnect(
                         self.probe_detect_two_screens
                     )
                     screen.run_no_filter()
  
             self.filter = "no_filter"
             logger.debug(f"filter: {self.filter}")
-            self.probeCalibration.clear(self.selected_stage_id)
 
+        # Reset the probe calibration status
+        self.probeCalibration.clear(self.selected_stage_id)
         # update global coords. Set  to '-' on UI
-        self.stageListener.requestClearGlobalDataTransformM(sn = sn)  # TODO
+        self.stageListener.requestClearGlobalDataTransformM(sn = sn)
 
     def probe_detect_default_status(self, sn = None):
         """
         Resets the probe detection status to its default state and updates the UI to reflect this change.
         This method is called after completing or aborting the probe detection process.
         """
         self.probe_detection_status = "default"
@@ -937,15 +938,14 @@
     def update_stages(self, prev_stage_id, curr_stage_id):
         logger.debug(f"update_stages, prev:{prev_stage_id}, curr:{curr_stage_id}")
         self.selected_stage_id = curr_stage_id
         if prev_stage_id is None or curr_stage_id is None:
             return
 
         # Save the previous stage's calibration info
-        #if self.moving_stage_id == prev_stage_id: # TODO
         info = self.get_stage_info()
         self.model.add_stage_calib_info(prev_stage_id, info)
         logger.debug(f"Saved stage {prev_stage_id} info: {info}")
 
         # Load the current stage's calibration info
         info = self.model.get_stage_calib_info(curr_stage_id)
         logger.debug(f"Loaded stage {curr_stage_id} info: {info}")
```

### Comparing `parallax_app-0.37.7/parallax/user_setting_manager.py` & `parallax_app-0.37.8/parallax/user_setting_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax/utils.py` & `parallax_app-0.37.8/parallax/utils.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/parallax_app.egg-info/PKG-INFO` & `parallax_app-0.37.8/parallax_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.7
+Version: 0.37.8
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: MIT
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parallax_app-0.37.7/parallax_app.egg-info/SOURCES.txt` & `parallax_app-0.37.8/parallax_app.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 img/stop-sign.png
 img/target.png
 parallax/__init__.py
 parallax/__main__.py
 parallax/axis_filter.py
 parallax/calibration_camera.py
 parallax/camera.py
+parallax/coords_transformation.py
 parallax/curr_bg_cmp_processor.py
 parallax/curr_prev_cmp_processor.py
 parallax/main_window_wip.py
 parallax/mask_generator.py
 parallax/model.py
 parallax/no_filter.py
 parallax/probe_calibration.py
```

### Comparing `parallax_app-0.37.7/pyproject.toml` & `parallax_app-0.37.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/tests/test_screen_widget.py` & `parallax_app-0.37.8/tests/test_screen_widget.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/ParallaxReadME.JPG` & `parallax_app-0.37.8/ui/ParallaxReadME.JPG`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/font/FiraCode-VariableFont_wght.ttf` & `parallax_app-0.37.8/ui/font/FiraCode-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/mainWindow.ui` & `parallax_app-0.37.8/ui/mainWindow.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/probe_calib.ui` & `parallax_app-0.37.8/ui/probe_calib.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/arrow-right.png` & `parallax_app-0.37.8/ui/resources/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/check.png` & `parallax_app-0.37.8/ui/resources/check.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/gear.png` & `parallax_app-0.37.8/ui/resources/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/recordingButton.png` & `parallax_app-0.37.8/ui/resources/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/recordingButton_disabled.png` & `parallax_app-0.37.8/ui/resources/recordingButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/sextant.png` & `parallax_app-0.37.8/ui/resources/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/snapshotButton_disabled.png` & `parallax_app-0.37.8/ui/resources/snapshotButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/snapshotButton_green.png` & `parallax_app-0.37.8/ui/resources/snapshotButton_green.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/snapshotButton_white.png` & `parallax_app-0.37.8/ui/resources/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/stop-sign.png` & `parallax_app-0.37.8/ui/resources/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/resources/target.png` & `parallax_app-0.37.8/ui/resources/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/reticle_calib.ui` & `parallax_app-0.37.8/ui/reticle_calib.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/settingPopUpMenu.ui` & `parallax_app-0.37.8/ui/settingPopUpMenu.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.7/ui/stage_info.ui` & `parallax_app-0.37.8/ui/stage_info.ui`

 * *Files identical despite different names*

