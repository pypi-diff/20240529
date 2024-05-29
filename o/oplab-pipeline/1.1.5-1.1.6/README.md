# Comparing `tmp/oplab_pipeline-1.1.5.tar.gz` & `tmp/oplab_pipeline-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oplab_pipeline-1.1.5.tar", last modified: Tue Nov 21 13:21:09 2023, max compression
+gzip compressed data, was "oplab_pipeline-1.1.6.tar", last modified: Wed May 29 16:24:47 2024, max compression
```

## Comparing `oplab_pipeline-1.1.5.tar` & `oplab_pipeline-1.1.6.tar`

### file list

```diff
@@ -1,232 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.553957 oplab_pipeline-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    20848 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2023-11-21 13:21:09.553957 oplab_pipeline-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 13:21:09.553957 oplab_pipeline-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.521957 oplab_pipeline-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.525957 oplab_pipeline-1.1.5/src/auv_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/auv_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25715 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    57996 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/camera_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/cone_fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.525957 oplab_pipeline-1.1.5/src/auv_cal/default_yaml/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/default_yaml/default_calibration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/euler_angles_from_rotation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    41020 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/laser_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/plane_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/plot_points_and_planes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_cal/ransac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.525957 oplab_pipeline-1.1.5/src/auv_nav/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/auv_nav.py
--rw-r--r--   0 runner    (1001) docker     (127)    14819 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.525957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.517957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ae2000/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.525957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ae2000/YK17-23C/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.517957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/dy152/
--rwxr-xr-x   0 runner    (1001) docker     (127)      444 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/dy152/camera.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1468 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/dy152/mission.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1736 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/insite/
--rwxr-xr-x   0 runner    (1001) docker     (127)      444 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/insite/camera.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1757 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/insite/mission.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1962 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/insite/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/jc220/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/jc220/camera.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.517957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/as6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/as6/DY109/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/as6/DY109/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/as6/DY109/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/auv_nav.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/hybis/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/hybis/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/hybis/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/hybis/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_rov/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_rov/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.517957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_stereo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_stereo/tautra21/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_stereo/tautra21/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.517957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/rosbag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/rosbag/grassmap/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/rosbag/grassmap/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.517957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.529957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/stereo_gopro/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.533957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/voyis/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/voyis/camera.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.517957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.533957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts1/SSK17-01/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts1/SSK17-01/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.517957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.533957 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts2/SSK16-01/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.533957 oplab_pipeline-1.1.5/src/auv_nav/localisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/localisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/localisation/dead_reckoning.py
--rw-r--r--   0 runner    (1001) docker     (127)    44420 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/localisation/ekf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/localisation/particle.py
--rw-r--r--   0 runner    (1001) docker     (127)    31172 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/localisation/particle_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19387 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/localisation/pf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/localisation/usbl_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/localisation/usbl_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)    28770 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.541957 oplab_pipeline-1.1.5/src/auv_nav/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/acfr_combined_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/acfr_stereo_pose.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/acfr_vehicle_pose.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/generic_csv_payload_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8477 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/hybis.py
--rw-r--r--   0 runner    (1001) docker     (127)    38972 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/koyo20rov.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/load_matlab_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_NOC_nmea.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_NOC_polpred.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_acfr_images.py
--rw-r--r--   0 runner    (1001) docker     (127)    17452 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_ae2000.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_alr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_autosub.py
--rw-r--r--   0 runner    (1001) docker     (127)    13309 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_biocam_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_eiva_navipac.py
--rw-r--r--   0 runner    (1001) docker     (127)    21687 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_gaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_interlacer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_koyo21rov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_ntnu_dvl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_ntnu_stereo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_phins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_rdi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_rosbag.py
--rw-r--r--   0 runner    (1001) docker     (127)    15385 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_seaxerocks_images.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_sonardyne_mrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_stereo_gopro.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_tide_CTI.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_usbl_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_voyis.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/parsers/parser_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.541957 oplab_pipeline-1.1.5/src/auv_nav/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/plot/plot_parse_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    60072 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/plot/plot_process_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    81746 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    74474 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.541957 oplab_pipeline-1.1.5/src/auv_nav/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/body_to_inertial.py
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/csv_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/displayable_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/dvl_level_arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/inertial_to_body.py
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/latlon_wgs84.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/time_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    58260 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/auv_nav/tools/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.541957 oplab_pipeline-1.1.5/src/correct_images/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20852 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/correct_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/corrections/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrections/attenuation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrections/debayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrections/gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrections/manual_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrections/pixel_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrections/rescale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrections/undistort.py
--rw-r--r--   0 runner    (1001) docker     (127)    56607 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/corrector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.521957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/acfr/
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/acfr/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/biocam/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/biocam/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/biocam4000_15c/
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/hybis/
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/hybis/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/ntnu_stereo/
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/rosbag/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/rosbag/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/stereo_gopro/
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/sx3/
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/sx3/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/default_yaml/voyis/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/default_yaml/voyis/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.545957 oplab_pipeline-1.1.5/src/correct_images/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/loaders/default.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/loaders/depth_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/loaders/rosbag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/loaders/xviii.py
--rw-r--r--   0 runner    (1001) docker     (127)    13667 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.549957 oplab_pipeline-1.1.5/src/correct_images/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/tools/curve_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/tools/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/tools/joblib_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/tools/memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/correct_images/tools/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.549957 oplab_pipeline-1.1.5/src/oplab/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/camera_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11572 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/camera_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.521957 oplab_pipeline-1.1.5/src/oplab/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.521957 oplab_pipeline-1.1.5/src/oplab/default_yaml/ae2000/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.549957 oplab_pipeline-1.1.5/src/oplab/default_yaml/ae2000/YK17-23C/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.521957 oplab_pipeline-1.1.5/src/oplab/default_yaml/as6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.549957 oplab_pipeline-1.1.5/src/oplab/default_yaml/as6/DY109/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/as6/DY109/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/as6/DY109/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/as6/DY109/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.521957 oplab_pipeline-1.1.5/src/oplab/default_yaml/smarty200/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.549957 oplab_pipeline-1.1.5/src/oplab/default_yaml/smarty200/rk23-01/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/smarty200/rk23-01/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/smarty200/rk23-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/smarty200/rk23-01/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.521957 oplab_pipeline-1.1.5/src/oplab/default_yaml/ts1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.549957 oplab_pipeline-1.1.5/src/oplab/default_yaml/ts1/SSK17-01/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/ts1/SSK17-01/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.521957 oplab_pipeline-1.1.5/src/oplab/default_yaml/ts2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.549957 oplab_pipeline-1.1.5/src/oplab/default_yaml/ts2/SSK16-01/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/filename_to_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/folder_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    19757 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/mission.py
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/oplab/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.553957 oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2023-11-21 13:21:09.000000 oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2023-11-21 13:21:09.000000 oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 13:21:09.000000 oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-21 13:21:09.000000 oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-11-21 13:21:09.000000 oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-21 13:21:09.000000 oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 13:21:09.553957 oplab_pipeline-1.1.5/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/scripts/auv_cd.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/scripts/debayer_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/scripts/extract_rosbag_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/scripts/merge_dataset_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2023-11-21 13:20:46.000000 oplab_pipeline-1.1.5/src/scripts/pixel_stats_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.949086 oplab_pipeline-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-29 16:24:47.949086 oplab_pipeline-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:24:47.949086 oplab_pipeline-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.917086 oplab_pipeline-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.917086 oplab_pipeline-1.1.6/src/auv_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/auv_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25715 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57996 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/camera_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/cone_fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.917086 oplab_pipeline-1.1.6/src/auv_cal/default_yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/default_yaml/default_calibration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/euler_angles_from_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41020 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/laser_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/plane_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/plot_points_and_planes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_cal/ransac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.921086 oplab_pipeline-1.1.6/src/auv_nav/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/auv_nav.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.921086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.909086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ae2000/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.921086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ae2000/YK17-23C/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.909086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.921086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/dy152/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      444 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/dy152/camera.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1468 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/dy152/mission.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1736 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.921086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/insite/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      444 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/insite/camera.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1757 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/insite/mission.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1962 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/insite/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.921086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/jc220/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/jc220/camera.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.909086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/as6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.921086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/as6/DY109/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/as6/DY109/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/as6/DY109/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/auv_nav.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.925086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/hybis/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/hybis/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/hybis/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/hybis/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.925086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_rov/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_rov/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.909086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_stereo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.925086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_stereo/tautra21/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_stereo/tautra21/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.909086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/rosbag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.925086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/rosbag/grassmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/rosbag/grassmap/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.909086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.925086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/stereo_gopro/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.925086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/voyis/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/voyis/camera.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/voyis/mission.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      907 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/voyis/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.909086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.925086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts1/SSK17-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts1/SSK17-01/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.913086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.925086 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts2/SSK16-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.929086 oplab_pipeline-1.1.6/src/auv_nav/localisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/localisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/localisation/dead_reckoning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44762 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/localisation/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/localisation/particle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31172 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/localisation/particle_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19387 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/localisation/pf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/localisation/usbl_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/localisation/usbl_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29134 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.933086 oplab_pipeline-1.1.6/src/auv_nav/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/acfr_combined_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/acfr_stereo_pose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/acfr_vehicle_pose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/generic_csv_payload_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/hybis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38972 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/koyo20rov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/load_matlab_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_NOC_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_NOC_polpred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_acfr_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17452 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_ae2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_alr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_autosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_biocam_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_eiva_navipac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_gaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_interlacer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_koyo21rov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_ntnu_dvl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_ntnu_stereo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_phins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_rdi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_seaxerocks_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20214 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_sonardyne_mrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_stereo_gopro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_tide_CTI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_usbl_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_voyis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/parsers/parser_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.937086 oplab_pipeline-1.1.6/src/auv_nav/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/plot/plot_parse_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60309 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/plot/plot_process_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81937 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74716 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.937086 oplab_pipeline-1.1.6/src/auv_nav/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/body_to_inertial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/csv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/displayable_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/dvl_level_arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/inertial_to_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/latlon_wgs84.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/time_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58260 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/auv_nav/tools/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.937086 oplab_pipeline-1.1.6/src/correct_images/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21564 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/correct_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/corrections/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrections/attenuation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrections/debayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrections/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrections/manual_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrections/pixel_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrections/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrections/undistort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57955 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/corrector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.913086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/acfr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/acfr/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/biocam/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/biocam/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/biocam4000_15c/
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/hybis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/hybis/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/ntnu_stereo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/rosbag/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/stereo_gopro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/sx3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/sx3/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/default_yaml/voyis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/default_yaml/voyis/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.941086 oplab_pipeline-1.1.6/src/correct_images/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/loaders/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/loaders/depth_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/loaders/rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/loaders/xviii.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.945086 oplab_pipeline-1.1.6/src/correct_images/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/tools/curve_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/tools/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/tools/joblib_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/tools/memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/correct_images/tools/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.945086 oplab_pipeline-1.1.6/src/oplab/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/camera_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11572 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/camera_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.913086 oplab_pipeline-1.1.6/src/oplab/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.913086 oplab_pipeline-1.1.6/src/oplab/default_yaml/ae2000/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.945086 oplab_pipeline-1.1.6/src/oplab/default_yaml/ae2000/YK17-23C/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.913086 oplab_pipeline-1.1.6/src/oplab/default_yaml/as6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.945086 oplab_pipeline-1.1.6/src/oplab/default_yaml/as6/DY109/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/as6/DY109/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/as6/DY109/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/as6/DY109/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.913086 oplab_pipeline-1.1.6/src/oplab/default_yaml/smarty200/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.945086 oplab_pipeline-1.1.6/src/oplab/default_yaml/smarty200/rk23-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/smarty200/rk23-01/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/smarty200/rk23-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/smarty200/rk23-01/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.913086 oplab_pipeline-1.1.6/src/oplab/default_yaml/ts1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.945086 oplab_pipeline-1.1.6/src/oplab/default_yaml/ts1/SSK17-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/ts1/SSK17-01/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.913086 oplab_pipeline-1.1.6/src/oplab/default_yaml/ts2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.945086 oplab_pipeline-1.1.6/src/oplab/default_yaml/ts2/SSK16-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/filename_to_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/folder_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20318 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/mission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/oplab/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.949086 oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-29 16:24:47.000000 oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-29 16:24:47.000000 oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:24:47.000000 oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 16:24:47.000000 oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-29 16:24:47.000000 oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 16:24:47.000000 oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:24:47.949086 oplab_pipeline-1.1.6/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/scripts/auv_cd.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/scripts/debayer_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/scripts/extract_rosbag_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/scripts/merge_dataset_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-05-29 16:24:28.000000 oplab_pipeline-1.1.6/src/scripts/pixel_stats_folder.py
```

### Comparing `oplab_pipeline-1.1.5/LICENSE` & `oplab_pipeline-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/PKG-INFO` & `oplab_pipeline-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oplab_pipeline
-Version: 1.1.5
+Version: 1.1.6
 Summary: Toolchain for AUV dive processing, camera calibration and image correction
 Home-page: https://github.com/ocean-perception/oplab_pipeline
 Author: Ocean Perception - University of Southampton
 Author-email: miquel.massot-campos@soton.ac.uk
 License: BSD
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -72,14 +72,18 @@
 This will make the commands `auv_nav`, `auv_cal` and `correct_images` available in the terminal. For more details refer to the documentation.
 
 For __development__, clone the repository, navigate to the oplab-pipeline folder and run 
 ```bash
 pip install -U --user -e .
 ```
 
+Notes:
+
+To import rosbag, using `pip install baypy`. (see the docs: https://jmscslgroup.github.io/bagpy/)
+
 ## Documentation
 The documentation is hosted in [read the docs](https://oplab-pipeline.readthedocs.io).
 
 
 ## Citation
 If you use this software, please cite the following article:
```

### Comparing `oplab_pipeline-1.1.5/README.md` & `oplab_pipeline-1.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 This will make the commands `auv_nav`, `auv_cal` and `correct_images` available in the terminal. For more details refer to the documentation.
 
 For __development__, clone the repository, navigate to the oplab-pipeline folder and run 
 ```bash
 pip install -U --user -e .
 ```
 
+Notes:
+
+To import rosbag, using `pip install baypy`. (see the docs: https://jmscslgroup.github.io/bagpy/)
+
 ## Documentation
 The documentation is hosted in [read the docs](https://oplab-pipeline.readthedocs.io).
 
 
 ## Citation
 If you use this software, please cite the following article:
 
@@ -49,8 +53,8 @@
 If you are using VSCode, there is a useful extension that helps named [Python Docstring Generator](https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring). Once installed, make sure you select Numpy documentation in the settings.
 
 Run `pre-commit install` to install [pre-commit](https://pre-commit.com/) into your git hooks. pre-commit will now run on every commit. If you don't have `pre-commit` installed, run `pip install pre-commit`.
 
 
 [cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
 [cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
-[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
+[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
```

### Comparing `oplab_pipeline-1.1.5/setup.py` & `oplab_pipeline-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
         subprocess.call(["git", "--version"], stdout=subprocess.PIPE)
     except OSError:
         print("The command git --version was not successful. Is git installed?")
         return None
     version_full = git_command(["describe", "--tags", "--dirty=.dirty"])
     version_tag = git_command(["describe", "--tags", "--abbrev=0"])
     version_tail = version_full[len(version_tag) :]  # noqa
+    if version_tail == ".dirty":
+        version_tail = "+dirty"
     return version_tag + version_tail.replace("-", ".dev", 1).replace("-", "+", 1)
 
 
 def run_setup():
     """Get version from git, then install."""
     # load long description from README.md
     readme_file = "README.md"
```

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/auv_cal.py` & `oplab_pipeline-1.1.6/src/auv_cal/auv_cal.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/calibration.py` & `oplab_pipeline-1.1.6/src/auv_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/camera_calibrator.py` & `oplab_pipeline-1.1.6/src/auv_cal/camera_calibrator.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/cone_fitting.py` & `oplab_pipeline-1.1.6/src/auv_cal/cone_fitting.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/default_yaml/default_calibration.yaml` & `oplab_pipeline-1.1.6/src/auv_cal/default_yaml/default_calibration.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/euler_angles_from_rotation_matrix.py` & `oplab_pipeline-1.1.6/src/auv_cal/euler_angles_from_rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/laser_calibrator.py` & `oplab_pipeline-1.1.6/src/auv_cal/laser_calibrator.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/plane_fitting.py` & `oplab_pipeline-1.1.6/src/auv_cal/plane_fitting.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/plot_points_and_planes.py` & `oplab_pipeline-1.1.6/src/auv_cal/plot_points_and_planes.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_cal/ransac.py` & `oplab_pipeline-1.1.6/src/auv_cal/ransac.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/auv_nav.py` & `oplab_pipeline-1.1.6/src/auv_nav/auv_nav.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 See LICENSE.md file in the project root for full license information.
 """
 
 import argparse
 import os
 import sys
 import time
-
 import argcomplete
-
+sys.path.insert(0, '/home/cl24n22/git/oplab_pipeline/src/')
 from auv_nav.convert import (
     acfr_to_oplab,
     hybis_to_oplab,
     koyo20rov_to_oplab,
     oplab_to_acfr,
 )
 from auv_nav.parse import parse
@@ -162,22 +161,18 @@
 
     # ACFR to OPLAB CSV
     subparser_oplab_to_acfr = subsubparsers.add_parser(
         "oplab_to_acfr",
         help="Converts an already processed dive to ACFR format",
     )
     subparser_oplab_to_acfr.add_argument(
-        "-d",
-        "--dive-folder",
         dest="dive_folder",
         help="Input dive path.",
     )
     subparser_oplab_to_acfr.add_argument(
-        "-o",
-        "--output-folder",
         dest="output_folder",
         help="Path where results will be written.",
     )
     subparser_oplab_to_acfr.add_argument(
         "-F",
         "--Force",
         dest="force",
@@ -332,8 +327,9 @@
         args.relative_pose_uncertainty,
         args.start_image_identifier,
         args.end_image_identifier,
     )
 
 
 if __name__ == "__main__":
-    main()
+    # sys.argv = ["auv_nav", "process", "/media/hdd20/cable_data/processed/ss24-01/20240417_120721_smarty200_denseA","-F"]
+    main()
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/convert.py` & `oplab_pipeline-1.1.6/src/auv_nav/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from auv_nav.tools.csv_tools import write_csv
 from auv_nav.tools.interpolate import interpolate_camera
 from auv_nav.tools.time_conversions import (
     epoch_from_json,
     epoch_to_datetime,
     string_to_epoch,
 )
-from oplab import Console, Mission, Vehicle, get_processed_folder
+from oplab import Console, Mission, Vehicle, get_raw_folder, get_processed_folder
 
 # fmt: on
 
 
 def koyo20rov_to_oplab(args):
     if args.dive_path is None:
         Console.error("Please provide a dive path using --dive-path (-i)")
@@ -217,24 +217,25 @@
     vf = output_folder / "vehicle_pose_est.data"
     sf = output_folder / "stereo_pose_est.data"
     if (vf.exists() or sf.exists()) and not args.force:
         Console.error("Output folder already exists. Use -F to overwrite. Exiting...")
         Console.quit("Default behaviour: not to overwrite results")
 
     Console.info("Loading mission.yaml")
-    path_processed = get_processed_folder(args.dive_folder)
-    mission_file = path_processed / "mission.yaml"
+    path_raw = get_raw_folder(args.dive_folder)
+    mission_file = path_raw / "mission.yaml"
     mission = Mission(mission_file)
 
-    vehicle_file = path_processed / "vehicle.yaml"
+    vehicle_file = path_raw / "vehicle.yaml"
     vehicle = Vehicle(vehicle_file)
 
     origin_lat = mission.origin.latitude
     origin_lon = mission.origin.longitude
 
+    path_processed = get_processed_folder(args.dive_folder)
     json_list = list(path_processed.glob("json_*"))
     if len(json_list) == 0:
         Console.quit(
             "No navigation solution could be found. Please run ",
             "auv_nav parse and process first",
         )
     navigation_path = path_processed / json_list[0]
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/dy152/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/dy152/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/insite/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/insite/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/insite/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/insite/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/alr/jc220/camera.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/alr/jc220/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/as6/DY109/camera.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/as6/DY109/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/as6/DY109/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/as6/DY109/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/auv_nav.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/auv_nav.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_rov/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_rov/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/smarty200/voyis/camera.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/smarty200/voyis/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml` & `oplab_pipeline-1.1.6/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/localisation/dead_reckoning.py` & `oplab_pipeline-1.1.6/src/auv_nav/localisation/dead_reckoning.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/localisation/ekf.py` & `oplab_pipeline-1.1.6/src/auv_nav/localisation/ekf.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 All rights reserved.
 Licensed under the BSD 3-Clause License.
 See LICENSE.md file in the project root for full license information.
 """
 
 import copy
 import math
+from datetime import datetime, timezone
 from typing import List, Optional
 
 import numpy as np
 
 from auv_nav.sensors import Camera, Depth, SyncedOrientationBodyVelocity, Usbl
 from auv_nav.tools.body_to_inertial import body_to_inertial
 from auv_nav.tools.interpolate import interpolate
@@ -1140,15 +1141,21 @@
         ekf_ts = ekf_list[ekf_idx].epoch_timestamp
 
         if cam_ts < ekf_ts:
             if not camera_list[c_idx].updated:
                 Console.error(
                     "There is a camera entry with index",
                     c_idx,
-                    "that is not updated to EKF...",
+                    "at epoch time",
+                    camera_list[c_idx].epoch_timestamp,
+                    "(UTC:",
+                    datetime.fromtimestamp(
+                        camera_list[c_idx].epoch_timestamp, tz=timezone.utc
+                    ).strftime("%Y/%m/%d %H:%M:%S.%f")[:-3],
+                    ") that is not updated to EKF",
                 )
             c_idx += 1
         elif cam_ts > ekf_ts:
             ekf_idx += 1
         elif cam_ts == ekf_ts:
             c = Camera()
             c.fromSyncedBodyVelocity(
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/localisation/particle.py` & `oplab_pipeline-1.1.6/src/auv_nav/localisation/particle.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/localisation/particle_filter.py` & `oplab_pipeline-1.1.6/src/auv_nav/localisation/particle_filter.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/localisation/pf.py` & `oplab_pipeline-1.1.6/src/auv_nav/localisation/pf.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/localisation/usbl_filter.py` & `oplab_pipeline-1.1.6/src/auv_nav/localisation/usbl_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         + ((usbl2.northings_std) ** 2 + (usbl2.eastings_std) ** 2) ** 0.5
     ) + time_difference * max_auv_speed
 
     distance_envelope = sigma_factor * lateral_distance_uncertainty_envelope
     return lateral_distance <= distance_envelope
 
 
-def usbl_filter(usbl_list, depth_list, sigma_factor, max_auv_speed):
+def usbl_filter(usbl_list, depth_list, sigma_factor, max_auv_speed,
+                apply_north_east_filter=True,
+                apply_depth_filter=True):
     """Filter USBL data based on time, depth and distance between points
 
     Returns
     -------
     list of Usbl
         USBL measurements filtered based on time and depth
     list of Usbl
@@ -95,90 +97,97 @@
                 Console.info("Discarding USBL measurements after DR...")
                 printed2 = True
             continue
         else:
             usbl_filtered_list.append(usbl_list[i])
     Console.info("Total USBL measurements removed pre DR: ", pre)
     Console.info("Total USBL measurements removed post DR: ", post)
-    usbl_list = usbl_filtered_list
-    usbl_filtered_list = []
-    Console.info(
-        "{} remain of {} USBL measurements after timestamp based filtering "
-        "(eliminating all USBL for which no depth data exists).".format(
-            len(usbl_list), original_size
+
+    if apply_depth_filter:
+        usbl_list = usbl_filtered_list
+        usbl_filtered_list = []
+        Console.info(
+            "{} remain of {} USBL measurements after timestamp based filtering "
+            "(eliminating all USBL for which no depth data exists).".format(
+                len(usbl_list), original_size
+            )
         )
-    )
 
-    # Depth-based filtering
-    depth_interpolated = []
-    depth_std_interpolated = []
-    # Interpolate depth meter data for USBL timestamps
-    for i in range(len(usbl_list)):
-        # Find depth measurement following USBL measurement
-        while (
-            j < len(depth_list) - 1
-            and depth_list[j].epoch_timestamp < usbl_list[i].epoch_timestamp
-        ):
-            j = j + 1
-        if j >= 1:
-            depth_interpolated.append(
-                interpolate(
-                    usbl_list[i].epoch_timestamp,
-                    depth_list[j - 1].epoch_timestamp,
-                    depth_list[j].epoch_timestamp,
-                    depth_list[j - 1].depth,
-                    depth_list[j].depth,
+        # Depth-based filtering
+        depth_interpolated = []
+        depth_std_interpolated = []
+        # Interpolate depth meter data for USBL timestamps
+        for i in range(len(usbl_list)):
+            # Find depth measurement following USBL measurement
+            while (
+                j < len(depth_list) - 1
+                and depth_list[j].epoch_timestamp < usbl_list[i].epoch_timestamp
+            ):
+                j = j + 1
+            if j >= 1:
+                depth_interpolated.append(
+                    interpolate(
+                        usbl_list[i].epoch_timestamp,
+                        depth_list[j - 1].epoch_timestamp,
+                        depth_list[j].epoch_timestamp,
+                        depth_list[j - 1].depth,
+                        depth_list[j].depth,
+                    )
                 )
-            )
-            depth_std_interpolated.append(
-                interpolate(
-                    usbl_list[i].epoch_timestamp,
-                    depth_list[j - 1].epoch_timestamp,
-                    depth_list[j].epoch_timestamp,
-                    depth_list[j - 1].depth_std,
-                    depth_list[j].depth_std,
+                depth_std_interpolated.append(
+                    interpolate(
+                        usbl_list[i].epoch_timestamp,
+                        depth_list[j - 1].epoch_timestamp,
+                        depth_list[j].epoch_timestamp,
+                        depth_list[j - 1].depth_std,
+                        depth_list[j].depth_std,
+                    )
                 )
-            )
 
-    for i in range(len(depth_interpolated)):
-        if depth_filter(
-            usbl_list[i],
-            depth_interpolated[i],
-            depth_std_interpolated[i],
-            sigma_factor,
-        ):
-            usbl_filtered_list.append(usbl_list[i])
-        i += 1
-    Console.info(
-        "{} remain of {} USBL measurements after depth filtering".format(
-            len(usbl_filtered_list), original_size
+        for i in range(len(depth_interpolated)):
+            if depth_filter(
+                usbl_list[i],
+                depth_interpolated[i],
+                depth_std_interpolated[i],
+                sigma_factor,
+            ):
+                usbl_filtered_list.append(usbl_list[i])
+            i += 1
+        Console.info(
+            "{} remain of {} USBL measurements after depth filtering".format(
+                len(usbl_filtered_list), original_size
+            )
         )
-    )
-    usbl_list = usbl_filtered_list
-    usbl_filtered_list = []
-
-    # Distance-based filtering
-    continuity_condition = 2
-    # want to check continuity over several readings to get rid of just
-    # outliers and not good data around them. Current approach has a lot of
-    # redundancy and can be improved when someone has the bandwidth
-    i = continuity_condition
-    n = -continuity_condition
-    while i < len(usbl_list) - continuity_condition:
-        if distance_filter(usbl_list[i], usbl_list[i + n], sigma_factor, max_auv_speed):
-            n += 1
-            if n == 0:
+    else:
+        Console.warn("The depth filter for usbl is ignored as required by misson.yaml")
+    if apply_north_east_filter:
+        usbl_list = usbl_filtered_list
+        usbl_filtered_list = []
+
+        # Distance-based filtering
+        continuity_condition = 2
+        # want to check continuity over several readings to get rid of just
+        # outliers and not good data around them. Current approach has a lot of
+        # redundancy and can be improved when someone has the bandwidth
+        i = continuity_condition
+        n = -continuity_condition
+        while i < len(usbl_list) - continuity_condition:
+            if distance_filter(usbl_list[i], usbl_list[i + n], sigma_factor, max_auv_speed):
                 n += 1
-            if n > continuity_condition:
-                usbl_filtered_list.append(usbl_list[i])
+                if n == 0:
+                    n += 1
+                if n > continuity_condition:
+                    usbl_filtered_list.append(usbl_list[i])
+                    n = -continuity_condition
+                    i += 1
+            else:
                 n = -continuity_condition
                 i += 1
-        else:
-            n = -continuity_condition
-            i += 1
 
-    Console.info(
-        "{} remain of {} USBL measurements after distance filter".format(
-            len(usbl_filtered_list), original_size
+        Console.info(
+            "{} remain of {} USBL measurements after distance filter".format(
+                len(usbl_filtered_list), original_size
+            )
         )
-    )
+    else:
+        Console.warn("The distance filter for usbl is ignored as required by misson.yaml")
     return usbl_list, usbl_filtered_list
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/localisation/usbl_offset.py` & `oplab_pipeline-1.1.6/src/auv_nav/localisation/usbl_offset.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parse.py` & `oplab_pipeline-1.1.6/src/auv_nav/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from auv_nav.parsers.parse_NOC_polpred import parse_NOC_polpred
 from auv_nav.parsers.parse_ntnu_dvl import parse_ntnu_dvl
 from auv_nav.parsers.parse_ntnu_stereo import parse_ntnu_stereo_images
 from auv_nav.parsers.parse_phins import parse_phins
 from auv_nav.parsers.parse_rdi import parse_rdi
 from auv_nav.parsers.parse_rosbag import parse_rosbag, parse_rosbag_extracted_images
 from auv_nav.parsers.parse_seaxerocks_images import parse_seaxerocks_images
-from auv_nav.parsers.parse_sonardyne_mrt import parse_sonardyne_mrt
+from auv_nav.parsers.parse_sonardyne_mrt import parse_sonardyne_mrt, parse_sonardyne_gga
 from auv_nav.parsers.parse_stereo_gopro import parse_stereo_gopro_images
 from auv_nav.parsers.parse_tide_CTI import parse_tide_CTI
 from auv_nav.parsers.parse_usbl_dump import parse_usbl_dump
 from auv_nav.parsers.parse_voyis import parse_voyis_images
 
 # from lib_sensors.parse_chemical import parse_chemical
 from auv_nav.plot.plot_parse_data import plot_parse_data
@@ -96,14 +96,15 @@
 
     return data_list
 
 
 def parse(filepath, force_overwrite, merge):
     # Filepath is a list. Get the first element by default
     for p in filepath:
+        Console.info(f"...Parsing {p}")
         parse_single(p, force_overwrite)
 
     if merge and len(filepath) > 1:
         Console.info("Merging the dives...")
 
         # Generate a merged output
         dates = []
@@ -361,14 +362,21 @@
         elif mission.usbl.format == "sonardyne_mrt":
             pool_list.append(
                 pool.apply_async(
                     parse_sonardyne_mrt,
                     [mission, vehicle, "usbl", ftype, outpath],
                 )
             )
+        elif mission.usbl.format == "sonardyne_gga":
+            pool_list.append(
+                pool.apply_async(
+                    parse_sonardyne_gga,
+                    [mission, vehicle, "usbl", ftype, outpath],
+                )
+            )
         else:
             Console.quit("Mission usbl format", mission.usbl.format, "not supported.")
 
     if not mission.velocity.empty():
         if mission.velocity.format == "phins":
             pool_list.append(
                 pool.apply_async(
@@ -742,15 +750,15 @@
     del data_list_temp
     del data_list
 
     # interlace the data based on timestamps
     Console.info("Interlacing data...")
     parse_interlacer(outpath, filename)
     Console.info("...done interlacing data. Output saved to", outpath / filename)
-    plot_parse_data(outpath, ftype)
+    plot_parse_data(outpath, ftype) # it makes the program stuck with unknown reasons
     Console.info("Complete parse data")
 
 
 def check_output_files_exist(processed_dataset_folder):
     """Check if any of the files exist, which `auv_nav parse` writes to disk"""
     mission_file = processed_dataset_folder / "mission.yaml"
     vehicle_file = processed_dataset_folder / "vehicle.yaml"
@@ -766,8 +774,8 @@
     if nav_file.exists():
         existing_files += str(nav_file) + "\n"
     if data_plot_file.exists():
         existing_files += str(data_plot_file) + "\n"
     if history_plot_file.exists():
         existing_files += str(history_plot_file) + "\n"
 
-    return existing_files
+    return existing_files
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/acfr_combined_raw.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/acfr_combined_raw.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/acfr_stereo_pose.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/acfr_stereo_pose.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/acfr_vehicle_pose.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/acfr_vehicle_pose.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/generic_csv_payload_parser.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/generic_csv_payload_parser.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/hybis.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/hybis.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/koyo20rov.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/koyo20rov.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/load_matlab_file.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/load_matlab_file.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_NOC_nmea.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_NOC_nmea.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_NOC_polpred.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_NOC_polpred.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_acfr_images.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_acfr_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_ae2000.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_ae2000.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_alr.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_alr.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_autosub.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_autosub.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_biocam_images.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_biocam_images.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,23 +131,27 @@
     # convert to seconds from utc
     # timeoffset = -timezone_offset*60*60 + timeoffset
 
     Console.info("Parsing " + sensor_string + " images...")
 
     # determine file paths
     base_path = get_raw_folder(outpath / ".." / filepath)
-    filepath1 = base_path / str(camera1_label + "_strobe/*.*")
-    filepath1b = base_path / str(camera1_label + "_laser/**/*.*")
-    filepath2 = base_path / str(camera2_label + "_strobe/*.*")
-    filepath2b = base_path / str(camera2_label + "_laser/**/*.*")
+    filepath1a = base_path / str(camera1_label + "_strobe/*.tif")
+    filepath1b = base_path / str(camera1_label + "_laser/**/*.jpg")
+    filepath1c = base_path / str(camera1_label + "_laser/*.tif")  # laser calibration
+    filepath2a = base_path / str(camera2_label + "_strobe/*.tif")
+    filepath2b = base_path / str(camera2_label + "_laser/**/*.jpg")
+    filepath2c = base_path / str(camera2_label + "_laser/*.tif")  # laser calibration
 
-    camera1_list = glob.glob(str(filepath1))
+    camera1_list = glob.glob(str(filepath1a))
     camera1_list.extend(glob.glob(str(filepath1b), recursive=True))
-    camera2_list = glob.glob(str(filepath2))
+    camera1_list.extend(glob.glob(str(filepath1c), recursive=True))
+    camera2_list = glob.glob(str(filepath2a))
     camera2_list.extend(glob.glob(str(filepath2b), recursive=True))
+    camera2_list.extend(glob.glob(str(filepath2c), recursive=True))
 
     camera1_filename = [
         line for line in camera1_list if ".txt" not in line and "._" not in line
     ]
     camera2_filename = [
         line for line in camera2_list if ".txt" not in line and ".jpg" not in line
     ]
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_eiva_navipac.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_eiva_navipac.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_gaps.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_gaps.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_interlacer.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_interlacer.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_koyo21rov.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_koyo21rov.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_ntnu_dvl.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_ntnu_dvl.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_ntnu_stereo.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_ntnu_stereo.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_phins.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_phins.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_rdi.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_rdi.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_rosbag.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_rosbag.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,26 +58,29 @@
     -------
     list
         Processed data list
     """
     if wanted_topic is None:
         Console.quit("data_method for bagfile is not specified for topic", wanted_topic)
     for bagfile in bagfile_list:
-        bag = rosbag.Bag(bagfile, "r")
-        for topic, msg, _ in bag.read_messages(topics=[wanted_topic]):
-            if topic == wanted_topic:
-                func = getattr(data_object, "from_ros")
-                type_str = str(type(msg))
-                # rosbag library does not store a clean message type,
-                # so we need to make it ourselves from a dirty string
-                msg_type = type_str.split(".")[1][1:-2].replace("__", "/")
-                func(msg, msg_type, output_dir)
-                if data_object.valid():
-                    data = data_object.export(output_format)
-                    data_list.append(data)
+        try:
+            bag = rosbag.Bag(bagfile, "r")
+            for topic, msg, _ in bag.read_messages(topics=[wanted_topic]):
+                if topic == wanted_topic:
+                    func = getattr(data_object, "from_ros")
+                    type_str = str(type(msg))
+                    # rosbag library does not store a clean message type,
+                    # so we need to make it ourselves from a dirty string
+                    msg_type = type_str.split(".")[1][1:-2].replace("__", "/")
+                    func(msg, msg_type, output_dir)
+                    if data_object.valid():
+                        data = data_object.export(output_format)
+                        data_list.append(data)
+        except:
+            Console.error(f"{bagfile} is unable to read!")
     return data_list
 
 
 def parse_rosbag(mission, vehicle, category, output_format, outpath):
     """Parse rosbag files
 
     Parameters
@@ -139,73 +142,73 @@
 
     body_velocity.sensor_string = "rosbag"
     orientation.sensor_string = "rosbag"
     depth.sensor_string = "rosbag"
     altitude.sensor_string = "rosbag"
     usbl.sensor_string = "rosbag"
 
-    # Adjust timezone offsets
+    # Adjust timezone offsets,
     body_velocity.tz_offset_s = (
-        read_timezone(mission.velocity.timezone) * 60 + mission.velocity.offset_s
+        read_timezone(mission.velocity.timezone) *60 + mission.velocity.offset_s
     )
     orientation.tz_offset_s = (
-        read_timezone(mission.orientation.timezone) * 60 + mission.orientation.offset_s
+        read_timezone(mission.orientation.timezone) *60 + mission.orientation.offset_s
     )
     depth.tz_offset_s = (
-        read_timezone(mission.depth.timezone) * 60 + mission.depth.offset_s
+        read_timezone(mission.depth.timezone) *60 + mission.depth.offset_s
     )
     altitude.tz_offset_s = (
-        read_timezone(mission.altitude.timezone) * 60 + mission.altitude.offset_s
+        read_timezone(mission.altitude.timezone) *60 + mission.altitude.offset_s
     )
-    usbl.tz_offset_s = read_timezone(mission.usbl.timezone) * 60 + mission.usbl.offset_s
+    usbl.tz_offset_s = read_timezone(mission.usbl.timezone) *60+ mission.usbl.offset_s
 
     if len(mission.image.cameras) > 0:
         camera = Camera()
         camera.sensor_string = mission.image.cameras[0].name
         camera.tz_offset_s = (
-            read_timezone(mission.image.timezone) * 60 + mission.image.offset_s
+            read_timezone(mission.image.timezone) *60 + mission.image.offset_s
         )
 
     data_list = []
 
     bagfile = None
     wanted_topic = None
     data_object = None
     filepath = None
 
     raw_path = get_raw_folder(outpath.parent)
 
     if category == Category.ORIENTATION:
         Console.info("... parsing orientation")
         filepath = raw_path / mission.orientation.filepath
-        bagfile = mission.orientation.filename
+        bagfile = "*.bag"
         wanted_topic = mission.orientation.topic
         data_object = orientation
     elif category == Category.VELOCITY:
         Console.info("... parsing velocity")
         filepath = raw_path / mission.velocity.filepath
-        bagfile = mission.velocity.filename
+        bagfile = "*.bag"
         wanted_topic = mission.velocity.topic
         data_object = body_velocity
     elif category == Category.DEPTH:
         Console.info("... parsing depth")
         filepath = raw_path / mission.depth.filepath
-        bagfile = mission.depth.filename
+        bagfile = "*.bag"
         wanted_topic = mission.depth.topic
         data_object = depth
     elif category == Category.ALTITUDE:
         Console.info("... parsing altitude")
         filepath = raw_path / mission.altitude.filepath
-        bagfile = mission.altitude.filename
+        bagfile = "*.bag"
         wanted_topic = mission.altitude.topic
         data_object = altitude
     elif category == Category.USBL:
         Console.info("... parsing position")
         filepath = raw_path / mission.usbl.filepath
-        bagfile = mission.usbl.filename
+        bagfile = "*.bag"
         wanted_topic = mission.usbl.topic
         data_object = usbl
     elif category == Category.IMAGES:
         Console.info("... parsing images")
         filepath = raw_path / mission.image.cameras[0].path
         bagfile = "*.bag"
         wanted_topic = mission.image.cameras[0].topic
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_seaxerocks_images.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_seaxerocks_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_sonardyne_mrt.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_sonardyne_mrt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import datetime
 import math
 from dataclasses import dataclass, field
 from pathlib import Path
-
+import pandas as pd
+import re
 from auv_nav.sensors import Category
 from auv_nav.tools.latlon_wgs84 import latlon_to_metres, metres_to_latlon
 from auv_nav.tools.time_conversions import read_timezone
 from oplab import Console, get_raw_folder
 
 
 @dataclass
@@ -234,14 +235,68 @@
     estimate_uid: str
     filter_uid2: str
     weight: str
     predicted: str
     mde: str
     w_test: str
 
+def parse_gga_txt(filename, field_id:int):
+    """
+    for gga txt, there are only lot, long and time_stamp that are useful.
+    """
+    observations = []
+    with open(filename, "r") as file:
+        try:
+            data_list = file.readlines()
+        except:
+            Console.error("file_errors: ", str(filename))
+            return []
+
+    data_list = [re.split(",| |\*", data_list[i]) for i in range(len(data_list))]
+    for idx, data in enumerate(data_list):
+        try:
+            if int(data[9]) != field_id:
+                continue
+            lat_sign = 1
+            long_sign = 1
+            if data[6] == "S":
+                lat_sign = -1
+            if data[8] == "W":
+                long_sign = -1
+            lat = float(data[5][:2]) + float(data[5][2:]) / 60
+            long = float(data[7][:3]) + float(data[7][3:]) / 60
+            lat *= lat_sign
+            long *= long_sign
+            time_stamp = filename.stem[0:4] + "-" + filename.stem[4:6] + "-" + filename.stem[6:8] + " " + data[1]
+
+            obs = USBLVectorObs(
+                obs_uid = "",
+                source_uid = "",
+                source_name = "",
+                parent_uid = "",
+                parent_name =  "",
+                assoc_uid = "",
+                time_stamp = time_stamp,
+                filter_uid = "",
+                fix_number = "",
+                jx = long,
+                jy = lat,
+                jz = 0.0,
+                valid_jx = False,
+                valid_jy = False,
+                valid_jz = False,
+                frequency = 0,
+                qj_sum = 0,
+                n_good_samples = 0,
+                direction_sd = 0.0, )
+            observations.append(obs)
+        except:
+            Console.warn(f"errors exist in {idx} row, already ignore it")
+    return observations
+
 
 def parse_mrt_csv(filename):
     filename = Path(filename)
     with filename.open("r") as f:
         observations = []
         # Loop through each line
         for i, line in enumerate(f):
@@ -504,7 +559,129 @@
                     "depth_std": float(distance_std),
                 },
                 {"distance_to_ship": float(distance)},
             ],
         }
         data_list.append(data)
     return data_list
+
+def parse_sonardyne_gga(mission, vehicle, category, ftype, outpath):
+    """
+    copied from def parse_sonardyne_mrt so there are a lot of variables we don't need.
+    you are free to delete or modify.
+    """
+    Console.info("... parsing Sonardyne GGA")
+
+    # parser meta data
+    class_string = "measurement"
+    sensor_string = "sonardyne_gga"
+    frame_string = "inertial"
+
+    timezone = mission.usbl.timezone
+    timeoffset = mission.usbl.timeoffset_s
+
+    timezone_offset_h = read_timezone(timezone)
+    timeoffset_s = -timezone_offset_h * 60 * 60 - timeoffset
+
+    filepath = mission.usbl.filepath
+    filename = mission.usbl.filename
+    # usbl_id = mission.usbl.label
+    latitude_reference = mission.origin.latitude
+    longitude_reference = mission.origin.longitude
+
+    distance_std_factor = mission.usbl.std_factor
+    distance_std_offset = mission.usbl.std_offset
+    field_id = int(mission.usbl.field_id)
+
+    # parse data
+    Console.info(f"Filename {filename}")
+    print(filename)
+    Console.info(f"Filepath {filepath}")
+    print(filepath)
+    filename = get_raw_folder(outpath / ".." / filepath / filename)
+    Console.info(f"Filename_full {filename}")
+    print(filename)
+    # Find all files with the same filename ending in "_1, _2, _3, etc"
+    filename = Path(filename)
+    if not filename.exists():
+        Console.error(f"File {filename} does not exist")
+        return None
+    base_name = filename.stem
+    files = filename.glob("*GGAlsq*.txt")
+    files = sorted(files)
+    date_prefix = []
+    all_observations = []
+    for filename in files:
+        observations = parse_gga_txt(filename,field_id)
+        all_observations.extend(observations)
+
+    """
+    for the gga data, we could only get the lat, long and timestamp so couldn't calcute 
+    the closest_observation like mrc_csv"""
+
+    # auv_observations = find_closest_observations(all_observations)
+    auv_observations = all_observations
+    data_list = []
+
+    # Calculate the distance between the two
+    for auv_obs in auv_observations:
+        latitude = float(auv_obs.jy)
+        longitude = float(auv_obs.jx)
+        depth = -float(auv_obs.jz)
+
+        lateral_distance_ship, bearing_ship = latlon_to_metres(
+            latitude,
+            longitude,
+            latitude_reference,
+            longitude_reference,
+        )
+        eastings_target = (
+                math.sin(bearing_ship * math.pi / 180.0) * lateral_distance_ship
+        )
+        northings_target = (
+                math.cos(bearing_ship * math.pi / 180.0) * lateral_distance_ship
+        )
+
+        data = {
+            "epoch_timestamp": datetime.datetime.strptime(auv_obs.time_stamp, "%Y-%m-%d %H:%M:%S.%f"
+        ).timestamp() + timeoffset_s,
+            "class": class_string,
+            "sensor": sensor_string,
+            "frame": frame_string,
+            "category": Category.USBL,
+            "data_ship": [
+                {
+                    "latitude": 0,
+                    "longitude": 0,
+                },
+                {
+                    "northings": 0,
+                    "eastings": 0,
+                },
+                {"heading": 0},
+            ],
+            "data_target": [
+                {
+                    "latitude": float(latitude),
+                    "latitude_std": 0.0001,
+                },
+                {
+                    "longitude": float(longitude),
+                    "longitude_std": 0.0001,
+                },
+                {
+                    "northings": northings_target,
+                    "northings_std": 5.0,
+                },
+                {
+                    "eastings": eastings_target,
+                    "eastings_std": 5.0,
+                },
+                {
+                    "depth": float(depth),
+                    "depth_std": 0.0,
+                },
+                {"distance_to_ship": ""},
+            ],
+        }
+        data_list.append(data)
+    return data_list
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_stereo_gopro.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_stereo_gopro.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_tide_CTI.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_tide_CTI.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_usbl_dump.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_usbl_dump.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parse_voyis.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parse_voyis.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 See LICENSE.md file in the project root for full license information.
 """
 
 import glob
 from pathlib import Path
 
 from oplab import Console, FilenameToDate, get_raw_folder
-
+from auv_nav.tools.time_conversions import read_timezone
 
 def pathlist_relativeto(input_pathlist, base_path):                   
     out_list = []                                                       
     for x in input_pathlist:                                                   
         p = Path(x)                                      
         pr = p.relative_to(base_path)                                       
         out_list.append(str(pr))                                            
@@ -28,59 +28,78 @@
     sensor_string = "voyis"
 
     dive_folder = get_raw_folder(outpath.parent)
 
     stills_filepath = dive_folder / Path(mission.image.cameras[0].path)
     laser_filepath = dive_folder / Path(mission.image.cameras[1].path)
 
-    stills_format = "xxxxxxxxxxxxxxxxxxxYYYYxMMxDDxhhmmssxfffuuuxx.xxx"
-    laser_format = "xxxxxxxxxxxxxxxxxxxxYYYYxMMxDDxhhmmssxfffuuuxx.xxx"
+    stills_format_PPS = "xxxxxxxxxxxxxxxNNNxYYYYxMMxDDxhhmmssxfffuuuxx.xxx"                            
+    stills_format_SYS = "xxxxxxxxxxxxxxxNNNNNNxYYYYxMMxDDxhhmmssxfffuuuxx.xxx"                     
+
+    laser_format_PPS  = "xxxxxxxxxxxxxxxxNNNxYYYYxMMxDDxhhmmssxfffuuuxx.xxx"
+    laser_format_SYS  = "xxxxxxxxxxxxxxxxNNNNNNxYYYYxMMxDDxhhmmssxfffuuuxx.xxx"
+
+
 
-    stills_filename_to_date = FilenameToDate(stills_format)
-    laser_filename_to_date = FilenameToDate(laser_format)
+    stills_filename_to_date_PPS = FilenameToDate(stills_format_PPS)
+    laser_filename_to_date_PPS = FilenameToDate(laser_format_PPS)
+
+    stills_filename_to_date_SYS = FilenameToDate(stills_format_SYS)
+    laser_filename_to_date_SYS = FilenameToDate(laser_format_SYS)
 
     Console.info("... parsing " + sensor_string + " images")
 
     # Find all *.tif images in stills_filepath and subfolders
     stills_image_list = glob.glob(str(stills_filepath) + "/**/*.tif", recursive=True)
     laser_image_list = glob.glob(str(laser_filepath) + "/**/*.tif", recursive=True)
 
     stills_image_list_rel = pathlist_relativeto(stills_image_list, dive_folder)
     laser_image_list_rel = pathlist_relativeto(laser_image_list, dive_folder)
 
     Console.info(f" .. found {len(stills_image_list)} stills images in {stills_filepath}")
     Console.info(f" .. found {len(laser_image_list)} laser images in {laser_filepath}")
 
     data_list = []
+    timezone = mission.image.timezone
+    timeoffset = mission.image.timeoffset_s
+
+    timezone_offset_h = read_timezone(timezone)
+    timeoffset_s = -timezone_offset_h * 60 * 60 - timeoffset
     for i, img in enumerate(stills_image_list):
-        epoch = stills_filename_to_date(str(Path(img).name))
+        if str(Path(img).name)[15:18]=='PPS':
+            epoch = stills_filename_to_date_PPS(str(Path(img).name))
+        elif str(Path(img).name)[15:18]=='SYSTEM':
+            epoch = stills_filename_to_date_SYS(str(Path(img).name))
         data = {
-            "epoch_timestamp": float(epoch),
+            "epoch_timestamp": float(epoch)+timeoffset_s,
             "class": class_string,
             "sensor": sensor_string,
             "frame": frame_string,
             "category": "image",
             "camera1": [
                 {
-                    "epoch_timestamp": float(epoch),
+                    "epoch_timestamp": float(epoch)+timeoffset_s,
                     "filename": str(stills_image_list_rel[i]),
                 }
             ],
         }
         data_list.append(data)
     for img in laser_image_list:
-        epoch = laser_filename_to_date(str(Path(img).name))
+        if str(Path(img).name[16:19])=='PPS':
+            epoch = laser_filename_to_date_PPS(str(Path(img).name))
+        elif str(Path(img).name[16:19])=='SYSTEM':
+            epoch = laser_filename_to_date_SYS(str(Path(img).name))        
         data = {
-            "epoch_timestamp": float(epoch),
+            "epoch_timestamp": float(epoch)+timeoffset_s,
             "class": class_string,
             "sensor": sensor_string,
             "frame": frame_string,
             "category": "laser",
             "camera1": [
                 {
-                    "epoch_timestamp": float(epoch),
+                    "epoch_timestamp": float(epoch)+timeoffset_s,
                     "filename": str(laser_image_list_rel[i]),
                 }
             ],
-        }
+        }        
         data_list.append(data)
     return data_list
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/parsers/parser_template.py` & `oplab_pipeline-1.1.6/src/auv_nav/parsers/parser_template.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/plot/plot_parse_data.py` & `oplab_pipeline-1.1.6/src/auv_nav/plot/plot_parse_data.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/plot/plot_process_data.py` & `oplab_pipeline-1.1.6/src/auv_nav/plot/plot_process_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,20 +209,20 @@
         if velocity_inertial_list[0].down_velocity is not None:
             fig.append_trace(tr_inertial_down, 3, 1)
     fig.append_trace(tr_dr_east, 2, 1)
     fig.append_trace(tr_dr_down, 3, 1)
     fig.append_trace(tr_dr_x, 1, 2)
     fig.append_trace(tr_dr_y, 2, 2)
     fig.append_trace(tr_dr_z, 3, 2)
-    fig["layout"]["xaxis1"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis2"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis3"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis4"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis5"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis6"].update(title="Epoch time, s", tickformat=".3f")
+    fig["layout"]["xaxis1"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis2"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis3"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis4"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis5"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis6"].update(title="Epoch time, s", tickformat=".f")
 
     fig["layout"]["yaxis1"].update(title="Velocity, m/s")
     fig["layout"]["yaxis2"].update(title="Velocity, m/s")
     fig["layout"]["yaxis3"].update(title="Velocity, m/s")
     fig["layout"]["yaxis4"].update(title="Velocity, m/s")
     fig["layout"]["yaxis5"].update(title="Velocity, m/s")
     fig["layout"]["yaxis6"].update(title="Velocity, m/s")
@@ -346,18 +346,18 @@
             inertial_eastings,
             "Easting {}".format(velocity_inertial_sensor_name),
             "green",
         )
         fig.append_trace(tr_vi_northings, 1, 1)
         fig.append_trace(tr_vi_eastings, 1, 2)
 
-    fig["layout"]["xaxis1"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis2"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis3"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis4"].update(title="Epoch time, s", tickformat=".3f")
+    fig["layout"]["xaxis1"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis2"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis3"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis4"].update(title="Epoch time, s", tickformat=".f")
     fig["layout"]["yaxis1"].update(title="Northing, m")
     fig["layout"]["yaxis2"].update(title="Easting, m")
     fig["layout"]["yaxis3"].update(title="Depth, m", autorange="reversed")
     fig["layout"]["yaxis4"].update(title="Altitude, m")
     fig["layout"].update(
         title="Deadreckoning vs Time", dragmode="pan", hovermode="closest"
     )
@@ -390,15 +390,15 @@
     tr_pf_eastings_std = create_trace(
         pf_time, pf_eastings_std, "eastings_std (m)", "blue"
     )
     tr_pf_yaw_std = create_trace(pf_time, pf_yaw_std, "yaw_std (deg)", "green")
     layout = go.Layout(
         title="Particle Filter Uncertainty Plot",
         hovermode="closest",
-        xaxis=dict(title="Epoch time, s", tickformat=".3f"),
+        xaxis=dict(title="Epoch time, s", tickformat=".f"),
         yaxis=dict(title="Degrees or Metres"),
         dragmode="pan",
     )
     config = {"scrollZoom": True}
     fig = go.Figure(
         data=[tr_pf_northings_std, tr_pf_eastings_std, tr_pf_yaw_std],
         layout=layout,
@@ -1267,20 +1267,20 @@
             fig.append_trace(tr_iv_e, 2, 2)
         if iv_d_vel_std[0] is not None:
             fig.append_trace(tr_iv_d, 2, 2)
 
     fig.append_trace(tr_n, 2, 3)
     fig.append_trace(tr_e, 2, 3)
 
-    fig["layout"]["xaxis1"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis2"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis3"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis4"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis5"].update(title="Epoch time, s", tickformat=".3f")
-    fig["layout"]["xaxis6"].update(title="Epoch time, s", tickformat=".3f")
+    fig["layout"]["xaxis1"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis2"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis3"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis4"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis5"].update(title="Epoch time, s", tickformat=".f")
+    fig["layout"]["xaxis6"].update(title="Epoch time, s", tickformat=".f")
     fig["layout"]["yaxis1"].update(title="Angle, degrees")
     fig["layout"]["yaxis2"].update(title="Velocity, m/s")
     fig["layout"]["yaxis3"].update(title="LatLong, degrees")
     fig["layout"]["yaxis4"].update(title="Depth, m")
     fig["layout"]["yaxis5"].update(title="Velocity, m/s")
     fig["layout"]["yaxis6"].update(title="NorthEast, m")
     fig["layout"].update(title="Uncertainty Plots", dragmode="pan", hovermode="closest")
@@ -1353,28 +1353,35 @@
         try:
             make_data(
                 figure,
                 i[0],
                 [float(j.eastings) for j in i[1]],
                 [float(j.northings) for j in i[1]],
                 visibility=i[2],
+                hoverinfo="x+y+text",
+                hovertext=[
+                    time.strftime(
+                        "%Y/%m/%d %H:%M:%S.%f", time.gmtime(j.epoch_timestamp)
+                    )[:-3]
+                    for j in i[1]
+                ],
             )
         except TypeError:
             Console.error("TypeError in plotting ", i[0])
 
     if len(pf_fusion_centre_list) > 1:
         make_data(
             figure,
             "pf_camera1",
             [float(i.eastings) for i in camera1_pf_list],
             [float(i.northings) for i in camera1_pf_list],
             visibility="legendonly",
             hoverinfo="x+y+text",
             hovertext=[
-                time.strftime("%H:%M:%S", time.localtime(i.epoch_timestamp))
+                time.strftime("%H:%M:%S", time.gmtime(i.epoch_timestamp))
                 for i in camera1_pf_list
             ],
         )
         make_data(
             figure,
             "pf_centre",
             [float(i.eastings) for i in pf_fusion_centre_list],
@@ -1385,15 +1392,15 @@
             figure,
             "pf_dvl",
             [float(i.eastings) for i in pf_fusion_dvl_list],
             [float(i.northings) for i in pf_fusion_dvl_list],
             visibility=True,
             hoverinfo="x+y+text",
             hovertext=[
-                time.strftime("%H:%M:%S", time.localtime(i.epoch_timestamp))
+                time.strftime("%H:%M:%S", time.gmtime(i.epoch_timestamp))
                 for i in pf_fusion_dvl_list
             ],
         )
         pf_timestamps_interval = []
         pf_eastings_interval = []
         pf_northings_interval = []
         if particles_time_interval is not False:
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/process.py` & `oplab_pipeline-1.1.6/src/auv_nav/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,15 +494,15 @@
                 if len(mission.image.cameras) > 1 and "camera2" in parsed_json_data[i]:
                     camera2 = Camera()
                     camera2.from_json(parsed_json_data[i], "camera2")
                     camera2_list.append(camera2)
 
             if "laser" in parsed_json_data[i]["category"]:
                 camera3 = Camera()
-                camera3.from_json(parsed_json_data[i], "camera3")
+                camera3.from_json(parsed_json_data[i], "camera1")
                 camera3_list.append(camera3)
 
     camera1_dr_list = copy.deepcopy(camera1_list)
     camera2_dr_list = copy.deepcopy(camera2_list)
     camera3_dr_list = copy.deepcopy(camera3_list)
 
     payload_offset = {}
@@ -747,15 +747,17 @@
             len(velocity_body_list),
             "elements)",
         )
 
     # perform usbl_filter
     if usbl_filter_activate:
         usbl_list_no_dist_filter, usbl_list = usbl_filter(
-            usbl_list, depth_list, sigma_factor, max_auv_speed
+            usbl_list, depth_list, sigma_factor, max_auv_speed,
+            apply_depth_filter=mission.usbl.apply_depth_filter,
+            apply_north_east_filter = mission.usbl.apply_north_east_filter
         )
         if len(usbl_list) == 0:
             Console.warn("Filtering USBL measurements lead to an empty list. ")
             Console.warn(" * Is USBL reliable?")
             Console.warn(" * Can you change filter parameters?")
 
     """
@@ -1231,15 +1233,15 @@
             camera2_dr_list,
             mission.image.cameras[1].name,
             camera2_offsets,
             origin_offsets,
             latlon_reference,
             dead_reckoning_centre_list,
         )
-    if len(camera3_dr_list) > 1:
+    if len(camera3_dr_list) > 1 and camera3_dr_list[0].epoch_timestamp is not None:
         if len(mission.image.cameras) > 2:
             interpolate_sensor_list(
                 camera3_dr_list,
                 mission.image.cameras[2].name + "_laser",
                 camera3_offsets,
                 origin_offsets,
                 latlon_reference,
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/sensors.py` & `oplab_pipeline-1.1.6/src/auv_nav/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1294,14 +1294,22 @@
     def from_alr(self, time, lat, lon, depth):
         self.epoch_timestamp = time
         self.latitude = lat
         self.longitude = lon
         self.depth = depth
         self.fill_from_lat_lon_depth()
 
+    def from_gga(self, time, lat, lon, depth):
+        self.sensor_string = "gga"
+        self.epoch_timestamp = time
+        self.latitude = lat
+        self.longitude = lon
+        self.depth = depth
+        self.fill_from_lat_lon_depth()
+
     def fill_from_lat_lon_depth(self):
         # calculate in meters from reference
         lateral_distance, bearing = latlon_to_metres(
             self.latitude,
             self.longitude,
             self.latitude_reference,
             self.longitude_reference,
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/body_to_inertial.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/body_to_inertial.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/csv_tools.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/csv_tools.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/displayable_path.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/displayable_path.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/dvl_level_arm.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/dvl_level_arm.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/graph.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/graph.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/inertial_to_body.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/inertial_to_body.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/interpolate.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/interpolate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 """
-Copyright (c) 2020, University of Southampton
+Copyright (c) 2024, University of Southampton
 All rights reserved.
 Licensed under the BSD 3-Clause License.
 See LICENSE.md file in the project root for full license information.
 """
 
+import time
+
 import numpy as np
 
 from auv_nav.sensors import Camera, SyncedOrientationBodyVelocity, Usbl
 from auv_nav.tools.body_to_inertial import body_to_inertial
 from auv_nav.tools.latlon_wgs84 import metres_to_latlon
 from oplab import Console
 
@@ -335,30 +337,38 @@
                     Console.warn(
                         "Deleted",
                         i,
                         "out of",
                         len(sensor_list),
                         "entries from sensor",
                         sensor_name,
-                        ". Reason: data before start of mission",
+                        ". Reason: data before start of mission (epoch:",
+                        start_time,
+                        "; UTC:",
+                        time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(start_time)),
+                        ")",
                     )
                     del sensor_list[:i]
                 break
         for i in range(len(sensor_list)):
             if j >= len(_centre_list) - 1:
                 ii = len(sensor_list) - i
                 if ii > 0:
                     Console.warn(
                         "Deleted",
                         ii,
                         "out of",
                         len(sensor_list),
                         "entries from sensor",
                         sensor_name,
-                        ". Reason: data after end of mission",
+                        ". Reason: data after end of mission (epoch:",
+                        end_time,
+                        "; UTC:",
+                        time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(end_time)),
+                        ")",
                     )
                     del sensor_list[i:]
                 sensor_overlap_flag = 1
                 break
             while _centre_list[j].epoch_timestamp < sensor_list[i].epoch_timestamp:
                 if (
                     j + 1 > len(_centre_list) - 1
```

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/latlon_wgs84.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/latlon_wgs84.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/time_conversions.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/time_conversions.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/auv_nav/tools/transformations.py` & `oplab_pipeline-1.1.6/src/auv_nav/tools/transformations.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/correct_images.py` & `oplab_pipeline-1.1.6/src/correct_images/correct_images.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,14 +85,27 @@
     )
     subparser_parse.add_argument(
         "--suffix",
         dest="suffix",
         default="",
         help="Expected suffix for correct_images configuration and output folders.",
     )
+    subparser_parse.add_argument(
+        "--memmap-location",
+        dest="memmap_location",
+        default=".",
+        help="Location for memmap files. Defaults to current directory.",
+    )
+    subparser_parse.add_argument(
+        "--memmap-size-gb",
+        dest="memmap_size_gb",
+        default=50,
+        type=int,
+        help="Size of individual memmap files in GB. Defaults to 50.",
+    )
     subparser_parse.set_defaults(func=call_parse)
 
     # subparser process
     subparser_process = subparsers.add_parser(
         "process", help="Process image correction"
     )
     subparser_process.add_argument("path", help="Path to raw directory till dive.")
@@ -240,15 +253,20 @@
             Console.info("Parsing for camera", camera.name)
             # Create a Corrector object for each camera with empty configuration
             # The configuration and the paths will be populated later on a per-dive basis
             corrector = Corrector(
                 "parse", args.force, args.suffix, camera, correct_config=None
             )
             # call new list-compatible implementation of parse()
-            corrector.parse(path_list, correct_config_list)
+            corrector.parse(
+                path_list,
+                correct_config_list,
+                args.memmap_location,
+                args.memmap_size_gb,
+            )
             corrector.cleanup()
 
     Console.info(
         "Parse completed for all cameras. Please run process to develop",
         "corrected images",
     )
 
@@ -365,94 +383,96 @@
     # resolve path to camera.yaml file
     camera_yaml_raw_path = path_raw_folder / "camera.yaml"
     camera_yaml_config_path = path_config_folder / "camera.yaml"
 
     camera_yaml_path = None
     default_file_path_correct_config = None
 
+    acfr_std_correct_config_file = (
+        "correct_images/default_yaml/acfr/correct_images.yaml"
+    )
+    sx3_std_correct_config_file = "correct_images/default_yaml/sx3/correct_images.yaml"
+    biocam_std_correct_config_file = (
+        "correct_images/default_yaml/biocam/correct_images.yaml"
+    )
+    biocam4000_15c_std_correct_config_file = (
+        "correct_images/default_yaml/biocam4000_15c/correct_images.yaml"
+    )
+    hybis_std_correct_config_file = (
+        "correct_images/default_yaml/hybis/correct_images.yaml"
+    )
+    ntnu_std_correct_config_file = (
+        "correct_images/default_yaml/ntnu_stereo/correct_images.yaml"
+    )
+    stereo_gopro_std_correct_config_file = (
+        "correct_images/default_yaml/stereo_gopro/correct_images.yaml"
+    )
+    voyis_std_correct_config_file = (
+        "correct_images/default_yaml/voyis/correct_images.yaml"
+    )
+    rosbag_std_correct_config_file = (
+        "correct_images/default_yaml/rosbag/correct_images.yaml"
+    )
+    root = Path(__file__).resolve().parents[1]
+    if mission.image.format == "acfr_standard":
+        default_file_path_correct_config = root / acfr_std_correct_config_file
+    elif mission.image.format == "seaxerocks_3":
+        default_file_path_correct_config = root / sx3_std_correct_config_file
+    elif mission.image.format == "biocam":
+        default_file_path_correct_config = root / biocam_std_correct_config_file
+    elif mission.image.format == "biocam4000_15c":
+        default_file_path_correct_config = root / biocam4000_15c_std_correct_config_file
+    elif mission.image.format == "hybis":
+        default_file_path_correct_config = root / hybis_std_correct_config_file
+    elif mission.image.format == "ntnu_stereo":
+        default_file_path_correct_config = root / ntnu_std_correct_config_file
+    elif mission.image.format == "stereo_gopro":
+        default_file_path_correct_config = root / stereo_gopro_std_correct_config_file
+    elif mission.image.format == "voyis":
+        default_file_path_correct_config = root / voyis_std_correct_config_file
+    elif mission.image.format == "rosbag":
+        default_file_path_correct_config = root / rosbag_std_correct_config_file
+
     if not camera_yaml_raw_path.exists() and not camera_yaml_config_path.exists():
         Console.info(
             "camera.yaml file not found neither in /raw nor in /config folder.",
             "Using default camera.yaml file for image format",
             mission.image.format,
         )
         # find out default yaml paths
-        root = Path(__file__).resolve().parents[1]
-
         acfr_std_camera_file = "auv_nav/default_yaml/ts1/SSK17-01/camera.yaml"
         sx3_camera_file = "auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml"
         biocam_camera_file = "auv_nav/default_yaml/as6/DY109/camera.yaml"
         biocam4000_15c_camera_file = "auv_nav/default_yaml/alr/jc220/camera.yaml"
         hybis_camera_file = "auv_nav/default_yaml/hybis/camera.yaml"
         ntnu_camera_file = "auv_nav/default_yaml/ntnu_stereo/tautra21/camera.yaml"
         stereo_gopro_camera_file = (
             "auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml"
         )
         voyis_camera_file = "auv_nav/default_yaml/smarty200/voyis/camera.yaml"
         rosbag_camera_file = "auv_nav/default_yaml/rosbag/grassmap/camera.yaml"
 
-        acfr_std_correct_config_file = (
-            "correct_images/default_yaml/acfr/correct_images.yaml"
-        )
-        sx3_std_correct_config_file = (
-            "correct_images/default_yaml/sx3/correct_images.yaml"
-        )
-        biocam_std_correct_config_file = (
-            "correct_images/default_yaml/biocam/correct_images.yaml"
-        )
-        biocam4000_15c_std_correct_config_file = (
-            "correct_images/default_yaml/biocam4000_15c/correct_images.yaml"
-        )
-        hybis_std_correct_config_file = (
-            "correct_images/default_yaml/hybis/correct_images.yaml"
-        )
-        ntnu_std_correct_config_file = (
-            "correct_images/default_yaml/ntnu_stereo/correct_images.yaml"
-        )
-        stereo_gopro_std_correct_config_file = (
-            "correct_images/default_yaml/stereo_gopro/correct_images.yaml"
-        )
-        voyis_std_correct_config_file = (
-            "correct_images/default_yaml/voyis/correct_images.yaml"
-        )
-        rosbag_std_correct_config_file = (
-            "correct_images/default_yaml/rosbag/correct_images.yaml"
-        )
-
         if mission.image.format == "acfr_standard":
             camera_yaml_path = root / acfr_std_camera_file
-            default_file_path_correct_config = root / acfr_std_correct_config_file
         elif mission.image.format == "seaxerocks_3":
             camera_yaml_path = root / sx3_camera_file
-            default_file_path_correct_config = root / sx3_std_correct_config_file
         elif mission.image.format == "biocam":
             camera_yaml_path = root / biocam_camera_file
-            default_file_path_correct_config = root / biocam_std_correct_config_file
         elif mission.image.format == "biocam4000_15c":
             camera_yaml_path = root / biocam4000_15c_camera_file
-            default_file_path_correct_config = (
-                root / biocam4000_15c_std_correct_config_file
-            )
         elif mission.image.format == "hybis":
             camera_yaml_path = root / hybis_camera_file
-            default_file_path_correct_config = root / hybis_std_correct_config_file
         elif mission.image.format == "ntnu_stereo":
             camera_yaml_path = root / ntnu_camera_file
-            default_file_path_correct_config = root / ntnu_std_correct_config_file
         elif mission.image.format == "stereo_gopro":
             camera_yaml_path = root / stereo_gopro_camera_file
-            default_file_path_correct_config = (
-                root / stereo_gopro_std_correct_config_file
-            )
         elif mission.image.format == "voyis":
             camera_yaml_path = root / voyis_camera_file
-            default_file_path_correct_config = root / voyis_std_correct_config_file
         elif mission.image.format == "rosbag":
             camera_yaml_path = root / rosbag_camera_file
-            default_file_path_correct_config = root / rosbag_std_correct_config_file
             camera_yaml_path.copy(camera_yaml_config_path)
             Console.info("Copied camera.yaml file to config folder. Please edit it.")
             Console.info("The file is located at", camera_yaml_config_path)
         else:
             Console.quit(
                 "There is currently no default camera file for image format",
                 mission.image.format,
```

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrections/__init__.py` & `oplab_pipeline-1.1.6/src/correct_images/corrections/__init__.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrections/attenuation.py` & `oplab_pipeline-1.1.6/src/correct_images/corrections/attenuation.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrections/debayer.py` & `oplab_pipeline-1.1.6/src/correct_images/corrections/debayer.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrections/gamma.py` & `oplab_pipeline-1.1.6/src/correct_images/corrections/gamma.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrections/manual_balance.py` & `oplab_pipeline-1.1.6/src/correct_images/corrections/manual_balance.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrections/pixel_stat.py` & `oplab_pipeline-1.1.6/src/correct_images/corrections/pixel_stat.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrections/rescale.py` & `oplab_pipeline-1.1.6/src/correct_images/corrections/rescale.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrections/undistort.py` & `oplab_pipeline-1.1.6/src/correct_images/corrections/undistort.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/corrector.py` & `oplab_pipeline-1.1.6/src/correct_images/corrector.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,19 @@
                 read_timezone(self.mission.image.timezone) * 60
                 + self.mission.image.timeoffset
             )
             self.loader.tz_offset_s = tz_offset_s
         else:
             self.loader.set_loader("default")
 
-    def parse(self, path_list, correct_config_list):
+    def parse(
+        self, path_list, correct_config_list, memmap_location=".", memmap_size_gb=50.0
+    ):
+        self.memmap_location = memmap_location
+        self.memmap_size_gb = memmap_size_gb
         # both path_list and correct_config_list are assumed to be valid + equivalent
         for i in range(len(path_list)):  # for each dive
             path = path_list[i]
             correct_config = correct_config_list[i]
 
             Console.info("Parsing dive:", path)
             # Console.info("Setting path")
@@ -541,14 +545,19 @@
                 dir_ = self.path_processed
                 json_list = list(dir_.glob("json_*"))
                 if len(json_list) == 0:
                     Console.quit(
                         "No navigation solution could be found. Please run ",
                         "auv_nav parse and process first",
                     )
+                elif len(json_list) > 1:
+                    Console.warn(
+                        "Multiple navigation solutions found. Using the first one:",
+                        json_list[0],
+                    )
                 self.distance_path = json_list[0]
                 Console.info("JSON:", self.distance_path)
             metric_path = self.path_processed / self.distance_path
             # Try if ekf exists:
             full_metric_path = metric_path / "csv" / "ekf"
             metric_file = "auv_ekf_" + self.camera_name + ".csv"
 
@@ -563,30 +572,37 @@
                     "Cannot find altitude csv file expected to be save at ",
                     self.altitude_csv_path,
                     ". Run auv_nav first.",
                 )
 
             # read dataframe for corresponding distance csv path
             dataframe = pd.read_csv(self.altitude_csv_path)
+            if len(dataframe) == 0:
+                Console.quit(
+                    f"Empty navigation csv file at {self.altitude_csv_path}. Please "
+                    "check file and rerun auv_nav if necessary."
+                )
 
             # get imagelist for given camera object
             if self.user_specified_image_list != "none":
                 path_file_list = Path(self.path_config) / self.user_specified_image_list
                 trimmed_csv_file = "trimmed_csv_" + self.camera_name + ".csv"
                 self.trimmed_csv_path = Path(self.path_config) / trimmed_csv_file
 
-                if not self.altitude_csv_path.exists():
-                    message = "Path to " + metric_file + " does not exist..."
-                    Console.quit(message)
-                else:
-                    # create trimmed csv based on user's  list of images
-                    dataframe = trim_csv_files(
-                        path_file_list,
-                        self.altitude_csv_path,
-                        self.trimmed_csv_path,
+                # create trimmed csv based on user's  list of images
+                dataframe = trim_csv_files(
+                    path_file_list,
+                    self.altitude_csv_path,
+                    self.trimmed_csv_path,
+                )
+                if len(dataframe) == 0:
+                    Console.quit(
+                        "No images left after filtering list of image altitudes from "
+                        f"{self.altitude_csv_path} with image file list provided at "
+                        f"{path_file_list}. Check both files."
                     )
 
             # Check images exist:
             valid_idx = []
             if "relative_path" not in dataframe:
                 Console.error("CSV FILE:", self.altitude_csv_path)
                 Console.quit(
@@ -595,14 +611,20 @@
             for idx, entry in enumerate(dataframe["relative_path"]):
                 if self.camera.extension == "bag":
                     valid_idx.append(idx)
                 else:
                     im_path = self.path_raw / entry
                     if im_path.exists():
                         valid_idx.append(idx)
+            if len(valid_idx) == 0:
+                Console.quit(
+                    "None of the images whose relative paths are provided in the "
+                    "navigation file exist. Check the images exits and that the "
+                    f"indicated paths are correct. Last image path checked: {im_path}"
+                )
             filtered_dataframe = dataframe.iloc[valid_idx]
             filtered_dataframe.reset_index(drop=True)
             # WARNING: if the column does not contain any 'None' entry, it will be
             # parsed as float, and the .str() accesor will fail
             filtered_dataframe["altitude [m]"] = filtered_dataframe[
                 "altitude [m]"
             ].astype(str)
@@ -665,15 +687,17 @@
             return
         elif self.distance_metric == "altitude":
             Console.info("Null distance matrix created")
             self.depth_map_list = []
             return
         elif self.distance_metric == "depth_map":
             # Load depth maps
-            path_depth = self.path_processed/"3d_reconstruction/depth_maps/gp_smoothed"
+            path_depth = (
+                self.path_processed / "3d_reconstruction/depth_maps/gp_smoothed"
+            )
             if not path_depth.exists():
                 Console.quit("Depth maps folder", path_depth, "does not exist.")
             images_to_drop = []
             for img_idx, image_path in enumerate(self.camera_image_list):
                 p = path_depth / os.path.relpath(image_path, self.path_raw)
                 p = p.with_name(p.stem + "_depthmap.npy")
                 if p.exists():
@@ -743,16 +767,15 @@
         image_size_gb = (
             self.image_channels
             * self.image_height
             * self.image_width
             * 4.0
             / (1024.0**3)
         )
-        max_bin_size_gb = 50.0
-        max_bin_size = int(max_bin_size_gb / image_size_gb)
+        max_bin_size = int(self.memmap_size_gb / image_size_gb)
 
         self.bin_band = 0.1
         hist_bins = np.arange(
             self.parse_altitude_min,
             self.parse_altitude_max + 0.5 * self.bin_band,
             self.bin_band,
         )
@@ -802,20 +825,22 @@
             images_fn, images_map = open_memmap(
                 shape=(
                     len(hist_bins) - 1,
                     self.image_height * self.image_width,
                     self.image_channels,
                 ),
                 dtype=np.float32,
+                memmap_location=self.memmap_location,
             )
             self.memmaps_to_remove.append(images_fn)
 
             distances_fn, distances_map = open_memmap(
                 shape=(len(hist_bins) - 1, self.image_height * self.image_width),
                 dtype=np.float32,
+                memmap_location=self.memmap_location,
             )
             self.memmaps_to_remove.append(distances_fn)
 
             with tqdm_joblib(
                 tqdm(
                     desc="Computing altitude histogram",
                     total=hist_bins.size - 1,
@@ -827,15 +852,15 @@
                     # program to crash when calling plt.imshow() in compute_distance_bin
                     joblib.delayed(self.compute_distance_bin)(
                         idxs,
                         idx_bin,
                         images_map,
                         distances_map,
                         max_bin_size,
-                        max_bin_size_gb,
+                        self.memmap_size_gb,
                         distance_vector,
                     )
                     for idx_bin in range(hist_bins.size - 1)
                 )
 
             # Save images map and distances map
             np.save(self.images_map_filepath, images_map)
@@ -914,14 +939,15 @@
                 shape=(
                     len(self.camera_image_list),
                     self.image_height,
                     self.image_width,
                     self.image_channels,
                 ),
                 dtype=np.float32,
+                memmap_location=self.memmap_location,
             )
             """
 
             # DEBUG: can be removed
             # Console.error("depth_map_list size", len(self.depth_map_list))
             # Console.error("camera_image_list size", len(self.camera_image_list))
             ###################################################################################################
@@ -1139,34 +1165,37 @@
 
             if self.smoothing == "mean":
                 bin_images_sample = running_mean_std(bin_images, loader=self.loader)[0]
             elif self.smoothing == "mean_trimmed":
                 memmap_filename, memmap_handle = create_memmap(
                     bin_images,
                     dimensions,
+                    self.memmap_location,
                     loader=self.loader,
                 )
                 self.memmaps_to_remove.append(memmap_filename)
                 bin_images_sample = image_mean_std_trimmed(memmap_handle)[0]
                 del memmap_handle
                 try_remove(memmap_filename)
             elif self.smoothing == "median":
                 memmap_filename, memmap_handle = create_memmap(
                     bin_images,
                     dimensions,
+                    self.memmap_location,
                     loader=self.loader,
                 )
                 self.memmaps_to_remove.append(memmap_filename)
                 bin_images_sample = median_array(memmap_handle)
                 del memmap_handle
                 try_remove(memmap_filename)
             elif self.smoothing == "ransac_mean":
                 memmap_filename, memmap_handle = create_memmap(
                     bin_images,
                     dimensions,
+                    self.memmap_location,
                     loader=self.loader,
                 )
                 self.memmaps_to_remove.append(memmap_filename)
                 bin_images_sample = ransac_mean_std(
                     memmap_handle, max_iterations=1000, threshold=0.1, sample_size=2
                 )[0]
                 del memmap_handle
```

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/acfr/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/acfr/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/biocam/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/biocam/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/hybis/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/hybis/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/rosbag/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/rosbag/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/sx3/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/sx3/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/default_yaml/voyis/correct_images.yaml` & `oplab_pipeline-1.1.6/src/correct_images/default_yaml/voyis/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/loaders/default.py` & `oplab_pipeline-1.1.6/src/correct_images/loaders/default.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/loaders/depth_map.py` & `oplab_pipeline-1.1.6/src/correct_images/loaders/depth_map.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/loaders/loader.py` & `oplab_pipeline-1.1.6/src/correct_images/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/loaders/rosbag.py` & `oplab_pipeline-1.1.6/src/correct_images/loaders/rosbag.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/loaders/xviii.py` & `oplab_pipeline-1.1.6/src/correct_images/loaders/xviii.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/parser.py` & `oplab_pipeline-1.1.6/src/correct_images/parser.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/tools/curve_fitting.py` & `oplab_pipeline-1.1.6/src/correct_images/tools/curve_fitting.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,46 +124,28 @@
     intensities_filt = []
     for altitude, intensity in zip(altitudes, intensities):
         if altitude > 0 and intensity > 0:
             altitudes_filt.append(altitude)
             intensities_filt.append(intensity)
 
     if not altitudes_filt or not intensities_filt:
-        if not altitudes_filt:
-            Console.warn(
-                "Altitudes are negative or zero in curve fitting at pixel position",
-                "x:",
-                x,
-                ", y:",
-                y,
-                "\naltitudes: ",
-                altitudes,
-                "\nintensities: ",
-                intensities,
-                "\naltitudes_filt: ",
-                altitudes_filt,
-                "\nintensities_filt: ",
-                intensities_filt,
-            )
-        if not intensities_filt:
-            Console.warn(
-                "Intensities are negative or zero in curve fitting at pixel position",
-                "x:",
-                x,
-                ", y:",
-                y,
-                "\naltitudes: ",
-                altitudes,
-                "\nintensities: ",
-                intensities,
-                "\naltitudes_filt: ",
-                altitudes_filt,
-                "\nintensities_filt: ",
-                intensities_filt,
+        note = ""
+        if x < 14 and y == 0:
+            note = (
+                ". This is expected for the first 14 pixels of the first row of BioCam "
+                "images."
             )
+        Console.warn(
+            "No valid altitudes or intensities in curve fitting at pixel position "
+            f"x: {x}, y: {y}{note}\n",
+            f"altitudes: {altitudes}\n",
+            f"intensities: {intensities}\n",
+            f"altitudes_filt: {altitudes_filt}\n",
+            f"intensities_filt: {intensities_filt}\n",
+        )
         return np.array([1, 0, 0])
 
     altitudes_filt = np.array(altitudes_filt)
     intensities_filt = np.array(intensities_filt)
 
     try:
         c_upper_bound = intensities_filt.min()
```

### Comparing `oplab_pipeline-1.1.5/src/correct_images/tools/file_handlers.py` & `oplab_pipeline-1.1.6/src/correct_images/tools/file_handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 """
 
 import uuid
 from pathlib import Path
 
 try:
     # Try using the v2 API directly to avoid a warning from imageio >= 2.16.2
-    from imageio.v2 import imwrite
+    from imageio.v2 import imread, imwrite
 except ImportError:
-    from imageio import imwrite
+    from imageio import imread, imwrite
+
 import joblib
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
 from correct_images.tools.joblib_tqdm import tqdm_joblib
 from oplab import Console
@@ -128,9 +129,31 @@
     """
 
     file = filename + "." + dest_format
     file_path = dest_path / file
     ch = image.shape[0]
     if ch == 3:
         image = image.transpose((1, 2, 0))
-    imwrite(file_path, image)
+
+    image_written_ok = False
+    i = 0
+    max_tries = 5
+    while image_written_ok is False and i < max_tries:
+        imwrite(file_path, image)
+        # Read image back to check if it was written correctly
+        try:
+            image = imread(file_path)
+        except Exception:
+            i += 1
+        else:
+            image_written_ok = True
+
+    if i >= max_tries:
+        Console.error(
+            f"Failed to write image {file_path} after {max_tries} unsuccessful attempts"
+        )
+    elif i > 0:
+        Console.warning(
+            f"Image {file_path} was written successfully after {i} failed attempt(s)"
+        )
+
     return file_path
```

### Comparing `oplab_pipeline-1.1.5/src/correct_images/tools/joblib_tqdm.py` & `oplab_pipeline-1.1.6/src/correct_images/tools/joblib_tqdm.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/correct_images/tools/memmap.py` & `oplab_pipeline-1.1.6/src/correct_images/tools/memmap.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,38 +4,43 @@
 All rights reserved.
 Licensed under the BSD 3-Clause License.
 See LICENSE.md file in the project root for full license information.
 """
 
 import uuid
 from datetime import datetime
+from pathlib import Path
 
 import cv2
 import numpy as np
 
 from oplab import Console
 
 from ..loaders import default
 
 
-def create_memmap_name() -> str:
+def create_memmap_name(memmap_location) -> str:
     filename_map = (
         "memmap_"
         + datetime.now().strftime("%Y%m%d_%H%M%S_")
         + "correct_images_"
         + Console.get_username()
         + "_"
         + str(uuid.uuid4())
         + ".map"
     )
-    return filename_map
+    memmap_location = Path(memmap_location)
+    if not memmap_location.exists():
+        memmap_location.mkdir(parents=True)
+    filename_map = memmap_location / filename_map
+    return str(filename_map)
 
 
-def create_memmap(image_list, dimensions, loader=default.loader):
-    filename_map = create_memmap_name()
+def create_memmap(image_list, dimensions, memmap_location, loader=default.loader):
+    filename_map = create_memmap_name(memmap_location)
     Console.info("Creating memmap at", filename_map)
     # If only 1 channel, do not create a 3D array
     if dimensions[-1] == 1:
         dimensions = dimensions[:-1]
     list_shape = [len(image_list)] + list(dimensions)
     size = 1
     for i in list_shape:
@@ -51,23 +56,23 @@
     for idx in range(len(image_list)):
         memmap_loader(
             image_list, image_memmap, idx, loader, dimensions[1], dimensions[0]
         )
     return filename_map, image_memmap
 
 
-def open_memmap(shape, dtype):
-    filename_map = create_memmap_name()
+def open_memmap(shape, dtype, memmap_location):
+    filename_map = create_memmap_name(memmap_location)
     Console.info("Creating memmap (open_memmap) at", filename_map)
     image_memmap = np.memmap(filename=filename_map, mode="w+", shape=shape, dtype=dtype)
     return filename_map, image_memmap
 
 
-def convert_to_memmap(array, loader=default.loader):
-    filename_map = create_memmap_name()
+def convert_to_memmap(array, memmap_location, loader=default.loader):
+    filename_map = create_memmap_name(memmap_location)
     Console.info("Creating memmap (convert_to_memmap) at", filename_map)
     image_memmap = np.memmap(
         filename=filename_map, mode="w+", shape=array.shape, dtype=array.dtype
     )
     image_memmap[:] = array[:]
     return filename_map, image_memmap
```

### Comparing `oplab_pipeline-1.1.5/src/correct_images/tools/numerical.py` & `oplab_pipeline-1.1.6/src/correct_images/tools/numerical.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/__init__.py` & `oplab_pipeline-1.1.6/src/oplab/__init__.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/camera_models.py` & `oplab_pipeline-1.1.6/src/oplab/camera_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pathlib import Path
 import math
 
 import cv2
 import numpy as np
 
-from .console import Console  # noqa
+from oplab.console import Console  # noqa
 
 
 class MonoCamera:
     """Monocular camera using OpenCV functions and parameters.
     Reads and writes calibration.yaml files
     """
```

### Comparing `oplab_pipeline-1.1.5/src/oplab/camera_system.py` & `oplab_pipeline-1.1.6/src/oplab/camera_system.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/console.py` & `oplab_pipeline-1.1.6/src/oplab/console.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/as6/DY109/camera.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/as6/DY109/camera.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 camera_system: biocam
 cameras:
   - name: cam61003146
     type: rggb
     bit_depth: 16
-    path: 'image/cam61003146_strobed'
+    path: 'image/cam61003146_strobe'
     extension: tif
     filename_to_date: YYYYMMDDxhhmmssxfffuuuxxxxxxxxxxxxxxxxxxxxxxxxxxxx.xxx
   - name: cam61004444
     type: grayscale
     bit_depth: 16
-    path: 'image/cam61004444_strobed'
+    path: 'image/cam61004444_strobe'
     extension: tif
     filename_to_date: 'YYYYMMDDxhhmmssxfffuuuxxxxxxxxxxxxxxxxxxxxxxxxxxxx.xxx'
   - name: cam61004444_laser
     type: grayscale
     bit_depth: 16
     path: 'image/cam61004444_laser'
     extension: jpg
```

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/as6/DY109/mission.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/as6/DY109/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/as6/DY109/vehicle.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/as6/DY109/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/smarty200/rk23-01/camera.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/smarty200/rk23-01/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/smarty200/rk23-01/mission.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/smarty200/rk23-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/smarty200/rk23-01/vehicle.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/smarty200/rk23-01/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml` & `oplab_pipeline-1.1.6/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/filename_to_date.py` & `oplab_pipeline-1.1.6/src/oplab/filename_to_date.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab/folder_structure.py` & `oplab_pipeline-1.1.6/src/oplab/folder_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,21 @@
         return path
     elif "processed" in path.parts:
         return change_subfolder(path, "processed", name)
     elif "raw" in path.parts:
         return change_subfolder(path, "raw", name)
     elif "configuration" in path.parts:
         return change_subfolder(path, "configuration", name)
+    elif not path.exists():
+        Console.quit(f"Folder {str(path)} does not exist.")
     else:
         Console.quit(
             "The folder",
             str(path),
-            "does not belong to any dataset",
+            "does not belong to a raw/configuration/processed dataset",
             "folder structure.",
         )
 
 
 def get_file_list(directory):
     dirpath = Path(directory)
     file_list = []
```

### Comparing `oplab_pipeline-1.1.5/src/oplab/mission.py` & `oplab_pipeline-1.1.6/src/oplab/mission.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,50 @@
     Console.error(
         "If you specified a origin frame, check that they match. Otherwise,",
         "stick to default frame names:",
     )
     Console.error("sensors: dvl ins depth usbl")
     Console.error("cameras: use the same name in mission.yaml and in vehicle.yaml")
     Console.quit("Inconsistency between mission.yaml and vehicle.yaml")
+class TimeZoneEntry:
+    def __init__(self):
+        self.timezone = 0
+        self.offset_s = 0
+        self.timeoffset_s = 0
+        self.timezone_s = 0
 
+    def load(self, node):
+        self.timezone = node.get("timezone", 0)
+        # read in timezone
+        if isinstance(self.timezone, str):
+            if self.timezone == "utc" or self.timezone == "UTC":
+                self.timezone = 0
+            elif self.timezone == "jst" or self.timezone == "JST":
+                self.timezone = 9
+            elif self.timezone == "CET" or self.timezone == "cet":
+                self.timezone = 1
+            else:
+                try:
+                    self.timezone = float(self.timezone)
+                except ValueError:
+                    Console.quit(
+                        "Error: timezone",
+                        self.timezone,
+                        "in mission.yaml not recognised,",
+                        " please enter value from UTC in",
+                        " hours",
+                    )
+
+        self.timeoffset_s = node.get("timeoffset", 0)
+        self.timezone_s = self.timezone * 60 * 60
+        self.offset_s = self.timezone_s + self.timeoffset_s
+
+    def write(self, node):
+        node["timezone"] = self.timezone
+        node["timeoffset"] = self.timeoffset_s
 
 class OriginEntry:
     def __init__(self):
         self.latitude = 0.0
         self.longitude = 0.0
         self.crs = ""
         self.date = ""
@@ -105,50 +140,15 @@
         node["type"] = self.type
         node["path"] = self.path
         node["records_laser"] = self.records_laser
         if hasattr(self, "timeoffset"):
             node["timeoffset"] = self.timeoffset
 
 
-class TimeZoneEntry:
-    def __init__(self):
-        self.timezone = 0
-        self.offset_s = 0
-        self.timeoffset_s = 0
-        self.timezone_s = 0
 
-    def load(self, node):
-        self.timezone = node.get("timezone", 0)
-        # read in timezone
-        if isinstance(self.timezone, str):
-            if self.timezone == "utc" or self.timezone == "UTC":
-                self.timezone = 0
-            elif self.timezone == "jst" or self.timezone == "JST":
-                self.timezone = 9
-            elif self.timezone == "CET" or self.timezone == "cet":
-                self.timezone = 1
-            else:
-                try:
-                    self.timezone = float(self.timezone)
-                except ValueError:
-                    Console.quit(
-                        "Error: timezone",
-                        self.timezone,
-                        "in mission.yaml not recognised,",
-                        " please enter value from UTC in",
-                        " hours",
-                    )
-
-        self.timeoffset_s = node.get("timeoffset", 0)
-        self.timezone_s = self.timezone * 60 * 60
-        self.offset_s = self.timezone_s + self.timeoffset_s
-
-    def write(self, node):
-        node["timezone"] = self.timezone
-        node["timeoffset"] = self.timeoffset_s
 
 
 class PayloadEntry(TimeZoneEntry):
     def __init__(self):
         super().__init__()
         self.path = ""
         self.format = ""
@@ -237,14 +237,17 @@
         super().__init__()
         self.format = ""
         self.filepath = ""
         self.filename = ""
         self.label = 0
         self.std_factor = 0.0
         self.std_offset = 0.0
+        self.field_id = 0 # for usbl to recognise auv
+        self.apply_depth_filter = True # for usbl to filter info using depth in usbl_filter.py
+        self.apply_north_east_filter = True # for usbl to filter info using north and east in usbl_filter.py
         self._empty = True
         self.topic = None
 
     def empty(self):
         return self._empty
 
     def load(self, node):
@@ -263,14 +266,20 @@
             self.std_factor = node["std_factor"]
         if "std_offset" in node:
             self.std_offset = node["std_offset"]
         if "origin" in node:
             self.origin = node["origin"]
         if "topic" in node:
             self.topic = node["topic"]
+        if "field_id" in node:
+            self.field_id = node["field_id"]
+        if "apply_depth_filter" in node:
+            self.apply_depth_filter = node["apply_depth_filter"]
+        if "apply_north_east_filter" in node:
+            self.apply_north_east_filter = node["apply_north_east_filter"]
 
     def write(self, node):
         super().write(node)
         node["format"] = self.format
         if "origin" in node:
             node["origin"] = self.origin
         if "topic" in node:
```

### Comparing `oplab_pipeline-1.1.5/src/oplab/vehicle.py` & `oplab_pipeline-1.1.6/src/oplab/vehicle.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/PKG-INFO` & `oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oplab-pipeline
-Version: 1.1.5
+Name: oplab_pipeline
+Version: 1.1.6
 Summary: Toolchain for AUV dive processing, camera calibration and image correction
 Home-page: https://github.com/ocean-perception/oplab_pipeline
 Author: Ocean Perception - University of Southampton
 Author-email: miquel.massot-campos@soton.ac.uk
 License: BSD
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -72,14 +72,18 @@
 This will make the commands `auv_nav`, `auv_cal` and `correct_images` available in the terminal. For more details refer to the documentation.
 
 For __development__, clone the repository, navigate to the oplab-pipeline folder and run 
 ```bash
 pip install -U --user -e .
 ```
 
+Notes:
+
+To import rosbag, using `pip install baypy`. (see the docs: https://jmscslgroup.github.io/bagpy/)
+
 ## Documentation
 The documentation is hosted in [read the docs](https://oplab-pipeline.readthedocs.io).
 
 
 ## Citation
 If you use this software, please cite the following article:
```

### Comparing `oplab_pipeline-1.1.5/src/oplab_pipeline.egg-info/SOURCES.txt` & `oplab_pipeline-1.1.6/src/oplab_pipeline.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 src/auv_nav/default_yaml/rosbag/grassmap/camera.yaml
 src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml
 src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml
 src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml
 src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml
 src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml
 src/auv_nav/default_yaml/smarty200/voyis/camera.yaml
+src/auv_nav/default_yaml/smarty200/voyis/mission.yaml
+src/auv_nav/default_yaml/smarty200/voyis/vehicle.yaml
 src/auv_nav/default_yaml/ts1/SSK17-01/camera.yaml
 src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml
 src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml
 src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml
 src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml
 src/auv_nav/localisation/__init__.py
 src/auv_nav/localisation/dead_reckoning.py
```

### Comparing `oplab_pipeline-1.1.5/src/scripts/auv_cd.sh` & `oplab_pipeline-1.1.6/src/scripts/auv_cd.sh`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/scripts/debayer_folder.py` & `oplab_pipeline-1.1.6/src/scripts/debayer_folder.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/scripts/extract_rosbag_images.py` & `oplab_pipeline-1.1.6/src/scripts/extract_rosbag_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/scripts/merge_dataset_csv.py` & `oplab_pipeline-1.1.6/src/scripts/merge_dataset_csv.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.5/src/scripts/pixel_stats_folder.py` & `oplab_pipeline-1.1.6/src/scripts/pixel_stats_folder.py`

 * *Files identical despite different names*

