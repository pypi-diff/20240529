# Comparing `tmp/gnssrefl-3.3.0.tar.gz` & `tmp/gnssrefl-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-3.3.0.tar", last modified: Wed May 22 20:14:08 2024, max compression
+gzip compressed data, was "gnssrefl-3.3.1.tar", last modified: Wed May 29 00:11:27 2024, max compression
```

## Comparing `gnssrefl-3.3.0.tar` & `gnssrefl-3.3.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.361307 gnssrefl-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-22 20:14:08.361307 gnssrefl-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.337307 gnssrefl-3.3.0/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.337307 gnssrefl-3.3.0/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/filesizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnssir_cl_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44629 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    50908 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)    50896 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (127)   202799 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)    40683 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/make_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/max_resolve_RH_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/mjd.py
--rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    43423 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57874 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    25817 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinex_coords.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/sd_libs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    61269 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.337307 gnssrefl-3.3.0/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 20:14:08.000000 gnssrefl-3.3.0/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:14:08.361307 gnssrefl-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:14:08.361307 gnssrefl-3.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-22 20:14:01.000000 gnssrefl-3.3.0/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:11:27.468349 gnssrefl-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 00:11:19.000000 gnssrefl-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 00:11:19.000000 gnssrefl-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-29 00:11:27.464349 gnssrefl-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-29 00:11:19.000000 gnssrefl-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:11:27.440349 gnssrefl-3.3.1/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:11:27.440349 gnssrefl-3.3.1/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/filesizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gnssir_cl_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44629 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50908 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)    50896 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (127)   202763 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40683 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    24562 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/max_resolve_RH_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/mjd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20890 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43423 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57906 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25817 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/rinex_coords.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38842 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/sd_libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61269 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:11:27.440349 gnssrefl-3.3.1/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-29 00:11:27.000000 gnssrefl-3.3.1/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-29 00:11:27.000000 gnssrefl-3.3.1/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:11:27.000000 gnssrefl-3.3.1/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-29 00:11:27.000000 gnssrefl-3.3.1/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 00:11:27.000000 gnssrefl-3.3.1/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 00:11:27.000000 gnssrefl-3.3.1/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 00:11:27.468349 gnssrefl-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:11:27.464349 gnssrefl-3.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-29 00:11:20.000000 gnssrefl-3.3.1/test/test_rinex2snr.py
```

### Comparing `gnssrefl-3.3.0/LICENSE` & `gnssrefl-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/PKG-INFO` & `gnssrefl-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.3.0
+Version: 3.3.1
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.3.0 
+# gnssrefl v3.3.1 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.3.0/README.md` & `gnssrefl-3.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gnssrefl v3.3.0 
+# gnssrefl v3.3.1 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.3.0/gnssrefl/EGM96.py` & `gnssrefl-3.3.1/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/check_rinex_file.py` & `gnssrefl-3.3.1/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/computemp1mp2.py` & `gnssrefl-3.3.1/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/daily_avg.py` & `gnssrefl-3.3.1/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/daily_avg_cl.py` & `gnssrefl-3.3.1/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-3.3.1/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/decipher_argt.py` & `gnssrefl-3.3.1/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/download_ioc.py` & `gnssrefl-3.3.1/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/download_noaa.py` & `gnssrefl-3.3.1/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/download_orbits.py` & `gnssrefl-3.3.1/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/download_psmsl.py` & `gnssrefl-3.3.1/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/download_rinex.py` & `gnssrefl-3.3.1/gnssrefl/download_rinex.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,21 +264,27 @@
 
     for d in range(doy, doy_end+1):
         # RINEX Version 3
         if version == 3:
             print('Request ', station, year, d, archive, samplerate, stream)
             if rate == 'high':
                 if archive == 'cddis':
-                    if debug:
-                        print('seek highrate data at CDDIS')
-                    ch.cddis_highrate(station, year, d, 0, stream, 1)
+                    bad_day = g.cddis_restriction(year, doy,'cddis')
+                    print('seek highrate data at CDDIS')
+                    if bad_day:
+                        rnx_filename, foundit = ch.cddis_highrate_tar(station, year, d, 0, stream, 1)
+                    else:
+                        rnx_filename, foundit = ch.cddis_highrate(station, year, d, 0, stream, 1)
                 if archive == 'bkg':                               
-                    if debug:
-                        print('seek highrate data at BKG')
-                    rnx_filename,foundit = ch.bkg_highrate(station, year, d, 0,stream,dec,bkg)
+                    print('seek highrate data at BKG')
+                    bad_day = g.cddis_restriction(year, doy,'bkg')
+                    if bad_day:
+                        rnx_filename,foundit = ch.bkg_highrate_tar(station, year, d, 0,stream,dec,bkg)
+                    else:
+                        rnx_filename,foundit = ch.bkg_highrate(station, year, d, 0,stream,dec,bkg)
                 if archive == 'ga':
                     if debug:
                         print('seek highrate data at GA')
                     deleteOld = True
                     r2, foundit = g.ga_highrate(station,year,d,dec,deleteOld)
             else:
                 if archive == 'all':
```

### Comparing `gnssrefl-3.3.0/gnssrefl/download_teqc.py` & `gnssrefl-3.3.1/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/download_tides.py` & `gnssrefl-3.3.1/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/download_unr.py` & `gnssrefl-3.3.1/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/download_wsv.py` & `gnssrefl-3.3.1/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/filesizes.py` & `gnssrefl-3.3.1/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gnssir_cl.py` & `gnssrefl-3.3.1/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gnssir_cl_old.py` & `gnssrefl-3.3.1/gnssrefl/gnssir_cl_old.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gnssir_input.py` & `gnssrefl-3.3.1/gnssrefl/gnssir_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gnssir_v2.py` & `gnssrefl-3.3.1/gnssrefl/gnssir_v2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gnsssnr.f` & `gnssrefl-3.3.1/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gnsssnrbigger.f` & `gnssrefl-3.3.1/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gps.py` & `gnssrefl-3.3.1/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -6365,15 +6365,15 @@
     """
     CDDIS has announced a restructuring of their archive.
     After 6 months files are tarred. It would be ok for the code
     to accommodate this change, but it will have to come from the community.
     If six months has passed since you ran the code, a warning will come to the 
     screen and the code will exit.
 
-    updated now that i realize BKG does the same thing
+    Updated now that i realize BKG does the same thing
 
     Parameters
     ----------
     iyear : int
         year you want to download from CDDIS
     idoy : int
         day of year you want to download from CDDIS
@@ -6399,16 +6399,16 @@
     # input date
     idate = iyear + idoy/365.25
 
     if (tdate - idate) > 0.5:
         # i.e. half a year is six months
         bad_day =  True
         print(archive.upper() + ' does not allow direct access to their high-rate data for this day and year. ')
-        print('They now tar files six months after the data archived - but force you to merge them. I have installed a solution for CDDIS.')
-        print('It would be nice if someone would make a similar fix for BKG')
+        print('They now tar files six months after the data archived - but force you to merge them.')
+        print('I have installed a solution for this problem for CDDIS and BKG.')
 
     else:
         bad_day = False
 
 
     return bad_day
```

### Comparing `gnssrefl-3.3.0/gnssrefl/gpssnr.f` & `gnssrefl-3.3.1/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gpsweek.py` & `gnssrefl-3.3.1/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/gpt_1wA.pickle` & `gnssrefl-3.3.1/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/highrate.py` & `gnssrefl-3.3.1/gnssrefl/highrate.py`

 * *Files 8% similar despite different names*

```diff
@@ -571,7 +571,136 @@
         searchpath = station.upper() + streamID + cyyyy + cdoy + '*.sha512.txt'
         cm = 'rm -rf ' + searchpath
         subprocess.call(cm,shell=True)
 
     s2=time.time()
     print('That download/merge experience took ', int(s2-s1), ' seconds.')
     return rinexname,  fexist
+
+def bkg_highrate_tar(station, year, month, day,stream,dec_rate,bkg):
+    """
+    picks up a highrate RINEX 3 file from BKG, merges and decimates it.
+    requires gfzrnx
+
+    Parameters
+    ----------
+    station : str
+        9 ch station name 
+    year : int
+        full year
+    month : integer
+        month or day of year if day set to 0
+    day : int
+        day of the month
+    stream : str
+        R or S
+    dec_rate : int
+        decimation rate in seconds
+    bkg : str
+        file directory at BKG (igs or euref)
+
+    Returns
+    -------
+    file_name24 : str
+        name of merged rinex file
+    fexist : boolean
+        whether file exists
+
+    """
+    fexist  = False
+    version = 3
+    crnxpath = g.hatanaka_version()
+    gexe = g.gfz_version()
+    alpha='abcdefghijklmnopqrstuvwxyz'
+    # if doy is input
+    if day == 0:
+        doy=month
+        d = g.doy2ymd(year,doy);
+        month = d.month; day = d.day
+    doy,cdoy,cyyyy,cyy = g.ymd2doy(year,month,day); 
+
+    if not os.path.isfile(crnxpath):
+        g.hatanaka_warning(); return
+
+    if not os.path.isfile(gexe):
+        print('You need to install gfzrnx to use high-rate RINEX data in my code.')
+        return '', fexist
+
+#    https://igs.bkg.bund.de/root_ftp/EUREF/highrate/2022/233/a/VLIS00NLD_R_20222330000_15M_01S_MO.crx.gz
+# 	VLIS00NLD_R_20231220000_01D_01S_MO.crx.tar.gz
+    gns = 'https://igs.bkg.bund.de/root_ftp/' + bkg + '/highrate/'
+    streamID  = '_' + stream + '_'
+    # base directory name
+    dirname = gns + cyyyy + '/'+ cdoy + '/' 
+    xend = '0000_01D_01S_MO'
+    #print('looking for files in: ', dirname)
+    file_name = station.upper() + streamID + cyyyy + cdoy + xend + '.crx'
+    file_name1 = file_name + '.tar.gz'
+    print(dirname + file_name1)
+    if not os.path.isfile(file_name + '.tar'):
+        s1=time.time()
+        s = g.replace_wget(dirname+file_name1, file_name1)
+        s2=time.time()
+        print('That file took ', int(s2-s1), ' seconds to download')
+        if os.path.isfile(file_name1):
+            subprocess.call(['gunzip',file_name1]) # unzip
+            subprocess.call(['tar','-xf', file_name + '.tar'])
+        else:
+            print('Something is wrong with tar download')
+            return '', False
+
+    fileF = 0
+    for h in range(0,24):
+        # subdirectory
+        ch = '{:02d}'.format(h)
+        print('Hour: ', ch)
+        for e in ['00', '15', '30', '45']:
+            crnx_name = station.upper() + streamID + cyyyy + cdoy + ch + e + '_15M_01S_MO.crx'
+            oname = crnx_name[:-3] + 'rnx'
+            print(oname)
+
+            if os.path.isfile(oname):
+                fileF = fileF + 1
+                print('You already have ', oname, ' so no need to make it ')
+                if os.path.isfile(crnx_name):
+                    subprocess.call(['rm',crnx_name])  
+            else:
+                if os.path.isfile(crnx_name):
+                    subprocess.call([crnxpath,crnx_name])  
+                    if os.path.isfile(oname):
+                        fileF = fileF + 1
+                        subprocess.call(['rm',crnx_name])  
+                else:
+                    print('File does not exist', oname)
+
+    searchP = station.upper() + streamID + cyyyy + cdoy + '*15M*MO.rnx'
+    print('Found ', fileF,' 15 minute files')
+
+
+    outfile = station.upper() + streamID + cyyyy + cdoy + '.tmp'
+    crate = '{:02d}'.format(dec_rate)
+
+    file_name24 = station.upper() + streamID + cyyyy + cdoy + '0000_01D_01S_MO.rnx'
+    print('Final name of RINEX 3 file ', file_name24)
+
+    if os.path.isfile(outfile):
+        print('you already merged')
+        fexist = True
+    else:
+        if (fileF > 0):
+            s1= time.time()
+            subprocess.call([gexe,'-finp', searchP, '-fout', outfile, '-vo','3', '-smp', crate, '-f','-q'])
+            fexist = True
+            s2=time.time()
+            print('That merging/decimating experience took ', int(s2-s1), ' seconds.')
+            print('remove 15 minute files')
+            cm = 'rm ' + station.upper() + streamID + cyyyy + cdoy + '*15M_01S_MO.rnx'
+            subprocess.call(cm,shell=True)
+
+    if fexist:
+        print('Now change the output name: ', file_name24)
+        subprocess.call(['mv', outfile, file_name24])
+        subprocess.call(['rm', file_name+'.tar'])
+    else:
+        file_name24 = ''
+
+    return file_name24,  fexist
```

### Comparing `gnssrefl-3.3.0/gnssrefl/installexe_cl.py` & `gnssrefl-3.3.1/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/invsnr_cl.py` & `gnssrefl-3.3.1/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/invsnr_input.py` & `gnssrefl-3.3.1/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/karnak_libraries.py` & `gnssrefl-3.3.1/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/kelly.py` & `gnssrefl-3.3.1/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/llh2xyz.py` & `gnssrefl-3.3.1/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/make_meta.py` & `gnssrefl-3.3.1/gnssrefl/make_meta.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/max_resolve_RH_cl.py` & `gnssrefl-3.3.1/gnssrefl/max_resolve_RH_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/nmea2snr.py` & `gnssrefl-3.3.1/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/nmea2snr_cl.py` & `gnssrefl-3.3.1/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/nyquist_libs.py` & `gnssrefl-3.3.1/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/phase_functions.py` & `gnssrefl-3.3.1/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/prn2gps.py` & `gnssrefl-3.3.1/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/query_unr.py` & `gnssrefl-3.3.1/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/quickLook_cl.py` & `gnssrefl-3.3.1/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/quickLook_function2.py` & `gnssrefl-3.3.1/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/quickPhase.py` & `gnssrefl-3.3.1/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/quicklib.py` & `gnssrefl-3.3.1/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/quickplt.py` & `gnssrefl-3.3.1/gnssrefl/quickplt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/read_snr_files.py` & `gnssrefl-3.3.1/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/refl_zones.py` & `gnssrefl-3.3.1/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/refl_zones_cl.py` & `gnssrefl-3.3.1/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/refraction.py` & `gnssrefl-3.3.1/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/rh_plot.py` & `gnssrefl-3.3.1/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/rinex2snr.py` & `gnssrefl-3.3.1/gnssrefl/rinex2snr.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
                                 if screenstats:
                                     print('RINEX 2 file derived from the GA archive should now exist:', r2)
                             if archive == 'cddis':
                                 bad_day = g.cddis_restriction(year, doy,'cddis')
                                 if not bad_day:
                                     rnx_filename,foundit = ch.cddis_highrate(station9ch, year, doy, 0,stream,dec_rate)
                                 else: 
-                                    print('Check the tar version')
+                                    print('Check for the tar version')
                                     rnx_filename,foundit = ch.cddis_highrate_tar(station9ch, year, doy, 0,stream,dec_rate)
                                     print(rnx_filename, ' returned from tar version')
                                 if not foundit:
                                     print('No high-rate RINEX data will be downloaded')
                                     foundit = False; fexists = False; rnx_file = ''
                                 else:
                                     if screenstats:
@@ -309,19 +309,19 @@
                                     fexists = g.new_rinex3_rinex2(rnx_filename,r2,dec_rate)
                             if archive == 'bkg':
                                 # this is confusing - so the bkg variable is either IGS or EUREF
                                 bad_day = g.cddis_restriction(year, doy,'bkg')
                                 if not bad_day:
                                     rnx_filename,foundit = ch.bkg_highrate(station9ch, year, doy, 0,stream,dec_rate,bkg)
                                 else:
-                                    print('No high-rate RINEX data will be downloaded')
-                                    foundit = False; fexists = False; rnx_file = ''
+                                    print('Will try the tar version ')
+                                    rnx_filename,foundit = ch.bkg_highrate_tar(station9ch, year, doy, 0,stream,dec_rate,bkg)
                                 if foundit:
                                     if screenstats:
-                                        print('The RINEX 3 file has been downloaded from the BKG and merged. Try to make ', r2)
+                                        print('The RINEX 3 file has been downloaded from the BKG and merged. Now try to make ', r2)
                                     fexists = g.new_rinex3_rinex2(rnx_filename,r2,dec_rate)
                             if archive == 'ignes':
                                 bad_day = g.cddis_restriction(year, doy,'bkg')
                                 if not bad_day:
                                     rnx_filename,foundit = ch.esp_highrate(station9ch, year, doy, 0,stream,dec_rate)
                                 else:
                                     print('No high-rate RINEX data will be downloaded')
```

### Comparing `gnssrefl-3.3.0/gnssrefl/rinex2snr_cl.py` & `gnssrefl-3.3.1/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/rinex3_rinex2.py` & `gnssrefl-3.3.1/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/rinex3_snr.py` & `gnssrefl-3.3.1/gnssrefl/rinex3_snr.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,13 +79,15 @@
         print('found version 2 rinex')
         isnr = 66;  rate = 30; idoy = int(cdoy); iyear = int(year)
         rate = '30'; dec_rate = 0; archive = 'unavco' ; fortran = False; translator = 'hybrid'
         year_list = [iyear]; doy_list = [idoy]; rate = 'low';   nol = True; overwrite = False; srate = 30; mk = False; skipit = 1
         strip = False; stream = 'S'  ; bkg = 'IGS' # many of these are fake values because the file has already been translated to rinex2
         gzip = True
         screenstats = False
-        r.run_rinex2snr(station, year_list, doy_list, isnr, orbtype, rate,dec_rate,archive,fortran,nol,
-                overwrite,translator,srate,mk,skipit,stream,strip,bkg,screenstats,gzip)
+        # removed fortran and skipit inputs ...  and got rid of the year and doy lists
+        # 2024 may 28
+        r.run_rinex2snr(station, iyear, idoy, isnr, orbtype, rate,dec_rate,archive,nol,
+                overwrite,translator,srate,mk,stream,strip,bkg,screenstats,gzip)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gnssrefl-3.3.0/gnssrefl/rinex_coords.py` & `gnssrefl-3.3.1/gnssrefl/rinex_coords.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/rinpy.py` & `gnssrefl-3.3.1/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-3.3.1/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/sd_libs.py` & `gnssrefl-3.3.1/gnssrefl/sd_libs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1056,15 +1056,20 @@
         xm = [y.month for y in dlist]; xd = [y.day for y in dlist]
         xh = [y.hour for y in dlist]; xmin = [y.minute for y in dlist]
         xs = [y.second for y in dlist]
 
         if (Ngdiff > 0):
             for i in range(0,Ngdiff):
                 if ii[i]:
-                    e0 = mjd[i] ; e1 = mjd[i+1] # beginning and ending of the gap
+                    try:
+                        e0 = mjd[i] ; e1 = mjd[i+1] # beginning and ending of the gap
+                    except:
+                        # alerted to this problem by Felipe Nievinski.  
+                        print('>>>>  DUNNO, some problem with the spline - maybe gap at end of day',mjd[i])
+                        continue
                     bad_indices = (mjd_new > e0) & (mjd_new < e1 )
                     spline_new[bad_indices] = np.nan
                     mjd_new_obstimes[bad_indices] = np.datetime64("NaT")
 
     # write the spline values to a file, with gaps removed
         for i in range(0,N_new):
             if not np.isnan(spline_new[i]):
```

### Comparing `gnssrefl-3.3.0/gnssrefl/smoosh.py` & `gnssrefl-3.3.1/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/smoosh_snr.py` & `gnssrefl-3.3.1/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/snow_functions.py` & `gnssrefl-3.3.1/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/snowdepth_cl.py` & `gnssrefl-3.3.1/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/spline_functions.py` & `gnssrefl-3.3.1/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/subdaily.py` & `gnssrefl-3.3.1/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/subdaily_cl.py` & `gnssrefl-3.3.1/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/utils.py` & `gnssrefl-3.3.1/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/veg_multiyr.py` & `gnssrefl-3.3.1/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/vwc_cl.py` & `gnssrefl-3.3.1/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/vwc_input.py` & `gnssrefl-3.3.1/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/xnmeasnr.f` & `gnssrefl-3.3.1/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/xyz2llh.py` & `gnssrefl-3.3.1/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/ydoy.py` & `gnssrefl-3.3.1/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl/ymd.py` & `gnssrefl-3.3.1/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-3.3.1/gnssrefl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.3.0
+Version: 3.3.1
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.3.0 
+# gnssrefl v3.3.1 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.3.0/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-3.3.1/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-3.3.1/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/pyproject.toml` & `gnssrefl-3.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.3.0/setup.py` & `gnssrefl-3.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "simplekml",
     "earthscope-sdk",
     "jupyterlab",
     "ipywidgets"
 ]
 setup(
     name="gnssrefl",
-    version="3.3.0",
+    version="3.3.1",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-3.3.0/test/test_gps.py` & `gnssrefl-3.3.1/test/test_gps.py`

 * *Files identical despite different names*

