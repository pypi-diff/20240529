# Comparing `tmp/pyxel_sim-2.1.1.tar.gz` & `tmp/pyxel_sim-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxel_sim-2.1.1.tar", last modified: Mon Mar 18 14:24:35 2024, max compression
+gzip compressed data, was "pyxel_sim-2.2.tar", last modified: Wed May 29 07:52:15 2024, max compression
```

## Comparing `pyxel_sim-2.1.1.tar` & `pyxel_sim-2.2.tar`

### file list

```diff
@@ -1,228 +1,230 @@
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.532801 pyxel_sim-2.1.1/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      589 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/AUTHORS.rst
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1085 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/LICENSE.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      273 2024-03-14 07:58:39.000000 pyxel_sim-2.1.1/MANIFEST.in
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8305 2024-03-18 14:24:35.531672 pyxel_sim-2.1.1/PKG-INFO
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5637 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/README.md
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7857 2024-03-18 13:21:48.000000 pyxel_sim-2.1.1/pyproject.toml
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:34.958647 pyxel_sim-2.1.1/pyxel/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1014 2024-02-27 14:01:56.000000 pyxel_sim-2.1.1/pyxel/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      623 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/__main__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      497 2024-03-18 14:24:35.537803 pyxel_sim-2.1.1/pyxel/_version.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:34.966513 pyxel_sim-2.1.1/pyxel/backends/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      448 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/backends/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2842 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/backends/asdf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6283 2024-03-11 15:18:22.000000 pyxel_sim-2.1.1/pyxel/backends/hdf5.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:34.997227 pyxel_sim-2.1.1/pyxel/calibration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1091 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/calibration/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    14665 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/calibration/algorithm.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20622 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/calibration/archipelago.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20051 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/calibration/archipelago_datatree.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    19724 2024-03-13 17:04:35.000000 pyxel_sim-2.1.1/pyxel/calibration/calibration.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3180 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/calibration/fitness.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16987 2024-03-13 17:04:35.000000 pyxel_sim-2.1.1/pyxel/calibration/fitting.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18496 2024-03-13 17:04:35.000000 pyxel_sim-2.1.1/pyxel/calibration/fitting_datatree.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2026 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/calibration/protocols.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5962 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/calibration/user_defined.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15585 2024-03-11 15:18:22.000000 pyxel_sim-2.1.1/pyxel/calibration/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.001646 pyxel_sim-2.1.1/pyxel/configuration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      493 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/configuration/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15470 2024-03-13 17:04:35.000000 pyxel_sim-2.1.1/pyxel/configuration/configuration.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.031196 pyxel_sim-2.1.1/pyxel/data_structure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1175 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/data_structure/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8856 2024-03-13 18:16:36.000000 pyxel_sim-2.1.1/pyxel/data_structure/array.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16983 2024-03-13 18:16:36.000000 pyxel_sim-2.1.1/pyxel/data_structure/charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2132 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/data_structure/image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4884 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/data_structure/persistence.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      853 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/data_structure/phase.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17317 2024-03-18 11:54:21.000000 pyxel_sim-2.1.1/pyxel/data_structure/photon.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3180 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/data_structure/pixel.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    14045 2024-03-13 18:16:36.000000 pyxel_sim-2.1.1/pyxel/data_structure/scene.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2147 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/data_structure/signal.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1310 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/data_structure/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.048846 pyxel_sim-2.1.1/pyxel/detectors/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      857 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.058221 pyxel_sim-2.1.1/pyxel/detectors/apd/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      486 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/apd/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5421 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/apd/apd.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15852 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/apd/apd_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      845 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/apd/apd_geometry.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.064074 pyxel_sim-2.1.1/pyxel/detectors/ccd/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      434 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/ccd/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5402 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/ccd/ccd.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      948 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/ccd/ccd_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9179 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/characteristics.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.071717 pyxel_sim-2.1.1/pyxel/detectors/cmos/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      438 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/cmos/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5416 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/cmos/cmos.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      956 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/cmos/cmos_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23179 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/detectors/detector.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6079 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/detectors/environment.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9133 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/detectors/geometry.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.079086 pyxel_sim-2.1.1/pyxel/detectors/mkid/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      438 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/mkid/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6870 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/mkid/mkid.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      956 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/mkid/mkid_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      442 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/optics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5081 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/detectors/readout_properties.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4105 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/evaluator.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.087873 pyxel_sim-2.1.1/pyxel/exposure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      514 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/exposure/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13640 2024-03-13 18:16:36.000000 pyxel_sim-2.1.1/pyxel/exposure/exposure.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7210 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/exposure/readout.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.092524 pyxel_sim-2.1.1/pyxel/inputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      508 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/inputs/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15449 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/inputs/loader.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.097045 pyxel_sim-2.1.1/pyxel/models/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      420 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.119028 pyxel_sim-2.1.1/pyxel/models/charge_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      613 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_collection/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      666 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_collection/collection.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9170 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_collection/diffusion.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4860 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/models/charge_collection/fixed_pattern_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1458 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_collection/full_well.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3405 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_collection/inter_pixel_capacitance.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16264 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_collection/persistence.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.152726 pyxel_sim-2.1.1/pyxel/models/charge_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      963 2024-03-18 13:27:40.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1266 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/apd_gain.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17062 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/charge_deposition.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2509 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/charge_injection.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.173003 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      357 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16755 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/cosmix.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:34.929441 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.183657 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13468 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/particle.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23322 2024-03-11 15:18:22.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/plotting.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    19714 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/simulation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3626 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/util.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13030 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/dark_current.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9394 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/dark_current_induced.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6273 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/dark_current_rule07.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.192135 pyxel_sim-2.1.1/pyxel/models/charge_generation/data/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1875 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/data/mct-stopping-power.csv
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    51083 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    50826 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2524 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2790 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/load_charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4761 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/photoelectrons.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5472 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_generation/wavelength_qe.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.232267 pyxel_sim-2.1.1/pyxel/models/charge_measurement/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      883 2024-03-18 13:21:56.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9617 2024-03-11 15:18:22.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/amplifier_crosstalk.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17515 2024-03-18 13:21:56.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/linearity.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1580 2024-03-05 19:14:53.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/measurement.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.242842 pyxel_sim-2.1.1/pyxel/models/charge_measurement/nghxrg/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      357 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/nghxrg/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13703 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/nghxrg/nghxrg.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    33408 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10291 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/non_linearity_calculation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3152 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/offset.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5242 2024-03-05 19:14:53.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/readout_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2634 2024-03-05 19:14:53.000000 pyxel_sim-2.1.1/pyxel/models/charge_measurement/reset_noise.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.257471 pyxel_sim-2.1.1/pyxel/models/charge_transfer/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      576 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_transfer/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.261915 pyxel_sim-2.1.1/pyxel/models/charge_transfer/arctic_cti/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      357 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/charge_transfer/arctic_cti/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8656 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18885 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_transfer/cdm.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2810 2024-02-21 11:31:05.000000 pyxel_sim-2.1.1/pyxel/models/charge_transfer/emccd_poisson.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4817 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/charge_transfer/emccd_poisson_cic.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.309212 pyxel_sim-2.1.1/pyxel/models/data_processing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      717 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/data_processing/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6322 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/data_processing/linear_regression.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5576 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/data_processing/mean_variance.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5458 2024-03-05 19:14:53.000000 pyxel_sim-2.1.1/pyxel/models/data_processing/remove_cosmic_rays.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3861 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/data_processing/snr.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6794 2024-03-05 19:14:53.000000 pyxel_sim-2.1.1/pyxel/models/data_processing/source_extractor.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4142 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/data_processing/statistics.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.314586 pyxel_sim-2.1.1/pyxel/models/phasing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      420 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/phasing/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.318549 pyxel_sim-2.1.1/pyxel/models/phasing/mkid_models/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    11258 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/phasing/mkid_models/SC.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.321498 pyxel_sim-2.1.1/pyxel/models/phasing/mkid_models/SCtheory/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9694 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/phasing/mkid_models/SCtheory/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6324 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/phasing/pulse_processing.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.347136 pyxel_sim-2.1.1/pyxel/models/photon_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      824 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/__init__.py
--rwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16809 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/ariel_airs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7812 2024-03-18 11:54:21.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/illumination.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2798 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/load_image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5221 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/point_spread_function.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    29534 2024-03-13 18:16:36.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/poppy.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2581 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/shot_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    19928 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/simple_collection.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3513 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/photon_collection/stripe_pattern.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.368123 pyxel_sim-2.1.1/pyxel/models/readout_electronics/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      626 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/readout_electronics/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1383 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/readout_electronics/amplification.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3548 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/readout_electronics/dead_time.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      886 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/readout_electronics/phase_conversion.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2397 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/readout_electronics/sar_adc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7159 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/readout_electronics/sar_adc_with_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3913 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/readout_electronics/simple_adc.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.373877 pyxel_sim-2.1.1/pyxel/models/scene_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      414 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/scene_generation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23914 2024-03-18 13:04:01.000000 pyxel_sim-2.1.1/pyxel/models/scene_generation/load_star_map.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.376045 pyxel_sim-2.1.1/pyxel/models/signal_transfer/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      373 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/signal_transfer/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1246 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/models/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.391023 pyxel_sim-2.1.1/pyxel/notebook/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      773 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/notebook/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16653 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/notebook/calibration.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5144 2024-03-11 15:18:22.000000 pyxel_sim-2.1.1/pyxel/notebook/html_representation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20455 2024-03-01 16:55:07.000000 pyxel_sim-2.1.1/pyxel/notebook/jupyxel.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.399617 pyxel_sim-2.1.1/pyxel/observation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      502 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/observation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    44826 2024-03-18 13:21:48.000000 pyxel_sim-2.1.1/pyxel/observation/observation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5409 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/observation/parameter_values.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3873 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/options.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.412392 pyxel_sim-2.1.1/pyxel/outputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      591 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/outputs/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5188 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/outputs/calibration_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3108 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/outputs/exposure_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4571 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/outputs/observation_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18207 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/outputs/outputs.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.432138 pyxel_sim-2.1.1/pyxel/pipelines/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      651 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/pipelines/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7310 2024-02-23 14:31:13.000000 pyxel_sim-2.1.1/pyxel/pipelines/model_function.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7433 2024-03-18 13:04:01.000000 pyxel_sim-2.1.1/pyxel/pipelines/model_group.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6531 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/pipelines/pipeline.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    11879 2024-03-18 13:21:48.000000 pyxel_sim-2.1.1/pyxel/pipelines/processor.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      102 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/py.typed
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    36718 2024-03-15 12:52:33.000000 pyxel_sim-2.1.1/pyxel/run.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4767 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/show_versions.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.433994 pyxel_sim-2.1.1/pyxel/static/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   190546 2024-03-18 11:54:21.000000 pyxel_sim-2.1.1/pyxel/static/pyxel_schema.json
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.436546 pyxel_sim-2.1.1/pyxel/templates/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4039 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/templates/_TEMPLATE.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.462251 pyxel_sim-2.1.1/pyxel/util/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      816 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/util/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3139 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/util/add_model.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1117 2024-03-18 13:04:01.000000 pyxel_sim-2.1.1/pyxel/util/caching.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2129 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/util/examples.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6391 2024-03-11 15:23:02.000000 pyxel_sim-2.1.1/pyxel/util/image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7327 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/util/materials.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2531 2024-03-11 15:18:22.000000 pyxel_sim-2.1.1/pyxel/util/memory.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3780 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/util/misc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      969 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/util/randomize.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2172 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/pyxel/util/timing.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.528695 pyxel_sim-2.1.1/pyxel_sim.egg-info/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8305 2024-03-18 14:24:34.000000 pyxel_sim-2.1.1/pyxel_sim.egg-info/PKG-INFO
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7017 2024-03-18 14:24:34.000000 pyxel_sim-2.1.1/pyxel_sim.egg-info/SOURCES.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        1 2024-03-18 14:24:34.000000 pyxel_sim-2.1.1/pyxel_sim.egg-info/dependency_links.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       41 2024-03-18 14:24:34.000000 pyxel_sim-2.1.1/pyxel_sim.egg-info/entry_points.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      500 2024-03-18 14:24:34.000000 pyxel_sim-2.1.1/pyxel_sim.egg-info/requires.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       41 2024-03-18 14:24:34.000000 pyxel_sim-2.1.1/pyxel_sim.egg-info/top_level.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       38 2024-03-18 14:24:35.533012 pyxel_sim-2.1.1/setup.cfg
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      266 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/setup.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-03-18 14:24:35.527615 pyxel_sim-2.1.1/tests/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1737 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/tests/test_evaluator.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1878 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/tests/test_options.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      456 2024-02-19 15:26:17.000000 pyxel_sim-2.1.1/tests/test_show_versions.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.065928 pyxel_sim-2.2/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      589 2024-02-19 15:26:17.000000 pyxel_sim-2.2/AUTHORS.rst
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1085 2024-02-19 15:26:17.000000 pyxel_sim-2.2/LICENSE.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      273 2024-03-14 07:58:39.000000 pyxel_sim-2.2/MANIFEST.in
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8303 2024-05-29 07:52:15.065406 pyxel_sim-2.2/PKG-INFO
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5637 2024-02-19 15:26:17.000000 pyxel_sim-2.2/README.md
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8118 2024-05-29 06:17:36.000000 pyxel_sim-2.2/pyproject.toml
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:14.991527 pyxel_sim-2.2/pyxel/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1014 2024-02-27 14:01:56.000000 pyxel_sim-2.2/pyxel/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      623 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/__main__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      495 2024-05-29 07:52:15.069300 pyxel_sim-2.2/pyxel/_version.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:14.993078 pyxel_sim-2.2/pyxel/backends/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      448 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/backends/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2842 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/backends/asdf.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6283 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/backends/hdf5.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:14.997388 pyxel_sim-2.2/pyxel/calibration/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1091 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/calibration/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    14665 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/calibration/algorithm.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    21055 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/calibration/archipelago.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20051 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/calibration/archipelago_datatree.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    19907 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/calibration/calibration.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3180 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/calibration/fitness.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16987 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/calibration/fitting.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    19121 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/calibration/fitting_datatree.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2026 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/calibration/protocols.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5962 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/calibration/user_defined.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15585 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/calibration/util.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:14.998655 pyxel_sim-2.2/pyxel/configuration/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      493 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/configuration/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15470 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/configuration/configuration.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.002839 pyxel_sim-2.2/pyxel/data_structure/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1175 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/data_structure/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8863 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/data_structure/array.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16886 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/data_structure/charge.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2132 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/data_structure/image.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4884 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/data_structure/persistence.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      853 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/data_structure/phase.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17376 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/data_structure/photon.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3180 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/data_structure/pixel.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    14045 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/data_structure/scene.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2147 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/data_structure/signal.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1310 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/data_structure/util.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.005856 pyxel_sim-2.2/pyxel/detectors/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      857 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.007209 pyxel_sim-2.2/pyxel/detectors/apd/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      486 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/apd/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5421 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/apd/apd.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15852 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/detectors/apd/apd_characteristics.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      845 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/apd/apd_geometry.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.008350 pyxel_sim-2.2/pyxel/detectors/ccd/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      434 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/ccd/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5402 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/ccd/ccd.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      948 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/ccd/ccd_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9373 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/detectors/characteristics.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.010090 pyxel_sim-2.2/pyxel/detectors/cmos/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      438 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/cmos/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5416 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/cmos/cmos.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      956 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/cmos/cmos_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23179 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/detectors/detector.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5855 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/detectors/environment.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9133 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/detectors/geometry.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.011112 pyxel_sim-2.2/pyxel/detectors/mkid/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      438 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/mkid/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6870 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/detectors/mkid/mkid.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      956 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/mkid/mkid_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      442 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/detectors/optics.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5081 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/detectors/readout_properties.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4218 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/evaluator.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.012276 pyxel_sim-2.2/pyxel/exposure/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      514 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/exposure/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13640 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/exposure/exposure.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7210 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/exposure/readout.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.012921 pyxel_sim-2.2/pyxel/inputs/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      508 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/inputs/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15511 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/inputs/loader.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.013564 pyxel_sim-2.2/pyxel/models/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      420 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.016735 pyxel_sim-2.2/pyxel/models/charge_collection/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      613 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_collection/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      666 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_collection/collection.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9170 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_collection/diffusion.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4860 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_collection/fixed_pattern_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1458 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_collection/full_well.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3405 2024-02-23 14:31:13.000000 pyxel_sim-2.2/pyxel/models/charge_collection/inter_pixel_capacitance.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16264 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_collection/persistence.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.021824 pyxel_sim-2.2/pyxel/models/charge_generation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1028 2024-05-29 06:18:13.000000 pyxel_sim-2.2/pyxel/models/charge_generation/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1266 2024-02-23 14:31:13.000000 pyxel_sim-2.2/pyxel/models/charge_generation/apd_gain.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17062 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/charge_deposition.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2509 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/charge_injection.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.024059 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      357 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16755 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/cosmix.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:14.984883 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.027290 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13468 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/particle.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23322 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/plotting.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    19714 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/simulation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3626 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/util.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10567 2024-05-29 07:33:40.000000 pyxel_sim-2.2/pyxel/models/charge_generation/dark_current.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9394 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/dark_current_induced.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6273 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/dark_current_rule07.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3625 2024-05-29 06:18:13.000000 pyxel_sim-2.2/pyxel/models/charge_generation/dark_current_saphira.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.028974 pyxel_sim-2.2/pyxel/models/charge_generation/data/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1875 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/data/mct-stopping-power.csv
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    51083 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    50826 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2524 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2790 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/load_charge.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4761 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/photoelectrons.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2374 2024-05-29 06:18:13.000000 pyxel_sim-2.2/pyxel/models/charge_generation/simple_dark_current.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5472 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_generation/wavelength_qe.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.032779 pyxel_sim-2.2/pyxel/models/charge_measurement/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      883 2024-05-29 06:17:47.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9617 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/amplifier_crosstalk.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17515 2024-05-29 06:17:47.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/linearity.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1580 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/measurement.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.033873 pyxel_sim-2.2/pyxel/models/charge_measurement/nghxrg/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      357 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/nghxrg/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13703 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/nghxrg/nghxrg.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    33408 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10291 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/non_linearity_calculation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3152 2024-02-23 14:31:13.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/offset.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5242 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/readout_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2634 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_measurement/reset_noise.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.035289 pyxel_sim-2.2/pyxel/models/charge_transfer/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      576 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_transfer/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.035859 pyxel_sim-2.2/pyxel/models/charge_transfer/arctic_cti/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      357 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/charge_transfer/arctic_cti/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8656 2024-02-23 14:31:13.000000 pyxel_sim-2.2/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18885 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/charge_transfer/cdm.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2810 2024-02-21 11:31:05.000000 pyxel_sim-2.2/pyxel/models/charge_transfer/emccd_poisson.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4817 2024-02-23 14:31:13.000000 pyxel_sim-2.2/pyxel/models/charge_transfer/emccd_poisson_cic.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.038102 pyxel_sim-2.2/pyxel/models/data_processing/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      717 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/data_processing/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6322 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/data_processing/linear_regression.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5576 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/data_processing/mean_variance.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5458 2024-03-05 19:14:53.000000 pyxel_sim-2.2/pyxel/models/data_processing/remove_cosmic_rays.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3861 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/data_processing/snr.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6794 2024-03-05 19:14:53.000000 pyxel_sim-2.2/pyxel/models/data_processing/source_extractor.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4142 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/data_processing/statistics.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.039025 pyxel_sim-2.2/pyxel/models/phasing/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      420 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/phasing/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.039354 pyxel_sim-2.2/pyxel/models/phasing/mkid_models/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    11258 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/phasing/mkid_models/SC.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.039699 pyxel_sim-2.2/pyxel/models/phasing/mkid_models/SCtheory/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9694 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/phasing/mkid_models/SCtheory/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6324 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/phasing/pulse_processing.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.043391 pyxel_sim-2.2/pyxel/models/photon_collection/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      824 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/photon_collection/__init__.py
+-rwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16810 2024-05-27 10:33:13.000000 pyxel_sim-2.2/pyxel/models/photon_collection/ariel_airs.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7812 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/photon_collection/illumination.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2798 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/photon_collection/load_image.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5221 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/photon_collection/point_spread_function.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    29534 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/photon_collection/poppy.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2581 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/photon_collection/shot_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    19928 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/photon_collection/simple_collection.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3513 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/photon_collection/stripe_pattern.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.045817 pyxel_sim-2.2/pyxel/models/readout_electronics/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      626 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/readout_electronics/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1383 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/readout_electronics/amplification.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3548 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/readout_electronics/dead_time.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      886 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/readout_electronics/phase_conversion.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2397 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/readout_electronics/sar_adc.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7159 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/readout_electronics/sar_adc_with_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3913 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/readout_electronics/simple_adc.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.046389 pyxel_sim-2.2/pyxel/models/scene_generation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      414 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/scene_generation/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23914 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/scene_generation/load_star_map.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.047264 pyxel_sim-2.2/pyxel/models/signal_transfer/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      373 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/models/signal_transfer/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1246 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/models/util.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.048800 pyxel_sim-2.2/pyxel/notebook/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      773 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/notebook/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16686 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/notebook/calibration.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5144 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/notebook/html_representation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20456 2024-05-27 10:33:13.000000 pyxel_sim-2.2/pyxel/notebook/jupyxel.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.049831 pyxel_sim-2.2/pyxel/observation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      502 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/observation/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    45572 2024-05-29 06:17:36.000000 pyxel_sim-2.2/pyxel/observation/observation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5397 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/observation/parameter_values.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3873 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/options.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.051448 pyxel_sim-2.2/pyxel/outputs/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      591 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/outputs/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5188 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/outputs/calibration_outputs.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3108 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/outputs/exposure_outputs.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4571 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/outputs/observation_outputs.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18400 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/outputs/outputs.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.053365 pyxel_sim-2.2/pyxel/pipelines/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      651 2024-05-14 18:01:05.000000 pyxel_sim-2.2/pyxel/pipelines/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7546 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/pipelines/model_function.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7416 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/pipelines/model_group.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6531 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/pipelines/pipeline.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    11879 2024-05-29 06:17:36.000000 pyxel_sim-2.2/pyxel/pipelines/processor.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      102 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/py.typed
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    36778 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/run.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4767 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/show_versions.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.053796 pyxel_sim-2.2/pyxel/static/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   190544 2024-05-24 19:32:21.000000 pyxel_sim-2.2/pyxel/static/pyxel_schema.json
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.054223 pyxel_sim-2.2/pyxel/templates/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4039 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/templates/_TEMPLATE.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.058457 pyxel_sim-2.2/pyxel/util/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      816 2024-03-11 15:23:02.000000 pyxel_sim-2.2/pyxel/util/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3139 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/util/add_model.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1117 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/util/caching.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2129 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/util/examples.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6391 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/util/image.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7327 2024-02-19 15:26:17.000000 pyxel_sim-2.2/pyxel/util/materials.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2531 2024-03-11 15:18:22.000000 pyxel_sim-2.2/pyxel/util/memory.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3780 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/util/misc.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      969 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/util/randomize.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2172 2024-05-26 11:33:47.000000 pyxel_sim-2.2/pyxel/util/timing.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.064292 pyxel_sim-2.2/pyxel_sim.egg-info/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8303 2024-05-29 07:52:14.000000 pyxel_sim-2.2/pyxel_sim.egg-info/PKG-INFO
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7126 2024-05-29 07:52:14.000000 pyxel_sim-2.2/pyxel_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        1 2024-05-29 07:52:14.000000 pyxel_sim-2.2/pyxel_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       41 2024-05-29 07:52:14.000000 pyxel_sim-2.2/pyxel_sim.egg-info/entry_points.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      500 2024-05-29 07:52:14.000000 pyxel_sim-2.2/pyxel_sim.egg-info/requires.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       55 2024-05-29 07:52:14.000000 pyxel_sim-2.2/pyxel_sim.egg-info/top_level.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       38 2024-05-29 07:52:15.065986 pyxel_sim-2.2/setup.cfg
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      266 2024-02-19 15:26:17.000000 pyxel_sim-2.2/setup.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2024-05-29 07:52:15.064049 pyxel_sim-2.2/tests/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2764 2024-05-16 06:22:20.000000 pyxel_sim-2.2/tests/test_evaluator.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1878 2024-05-26 11:33:47.000000 pyxel_sim-2.2/tests/test_options.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      456 2024-02-19 15:26:17.000000 pyxel_sim-2.2/tests/test_show_versions.py
```

### Comparing `pyxel_sim-2.1.1/AUTHORS.rst` & `pyxel_sim-2.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/LICENSE.txt` & `pyxel_sim-2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/PKG-INFO` & `pyxel_sim-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel_sim
-Version: 2.1.1
+Version: 2.2
 Summary: Pyxel detector simulation framework.
 Author-email: The Pyxel development team <pyxel@esa.int>
 License: MIT
 Project-URL: homepage, https://esa.gitlab.io/pyxel/
 Project-URL: documentation, https://esa.gitlab.io/pyxel/doc/
 Project-URL: repository, https://gitlab.com/esa/pyxel
 Project-URL: changelog, https://gitlab.com/esa/pyxel/-/releases
```

### Comparing `pyxel_sim-2.1.1/README.md` & `pyxel_sim-2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyproject.toml` & `pyxel_sim-2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 ignore_errors = true
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = [
     "--showlocals",
     "--capture=no",
+    "--log-cli-level=ERROR",
     "-vv",
     "--ignore=old_code"
 ]
 markers = [
     "deprecated: marks tests as deprecated (deselect with '-m \"not deprecated\"')",
 ]
 [tool.pydocstyle]
@@ -222,28 +223,34 @@
 [tool.doc8]
 ignore = ["D001", "D002", "D004", "D005"]
 
 [tool.bandit]
 exclude_dirs = ["pyxel/_version.py"]
 
 [tool.codespell]
-ignore-words-list = "acn,sade,te"
+ignore-words-list = "acn,sade,te,Tennant"
 skip = "pyxel/_version.py,*.fits,pyxel/models/phasing/mkid_models/*"
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "debug",
     "raise NotImplementedError",
+    "if TYPE_CHECKING:",
+    "class .*\\bProtocol\\):",
+    "if not hv.Store.renderers",
 ]
 
 [tool.coverage.run]
 omit = [
+    "pyxel/models/phasing/mkid_models/*",
     "pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py",
     "pyxel/models/charge_generation/tars/plotting.py",
+    "pyxel/_version.py",
+    "tests/*",
 ]
 
 [tool.ruff.lint]
 select = [
     "A",        # flake8-builtins
     "B",        # flake8-bugbear
     "E",        # pycodestyle
@@ -278,14 +285,15 @@
     "TRY301",   # Abstract `raise` to an inner function
     "PTH207",   # Replace 'glob' with 'Path.glob' or 'Path.rglob'
     "SIM108",   # Use ternary operator
     "SIM114",   # Combine 'if' branches using logical 'or' operator
     "SIM117",   # Use a single 'with' statement with multiple contexts
     "SIM300",   # Yoda conditions are discouraged
     "PERF203",  # try-except within a loop incurs performance overhead
+    "UP037",    # Remove quotes from type annotation
 ]
 
 exclude = ["_TEMPLATE.py", "_version.py"]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = [
     "D100",     # Missing docstring in public module
```

### Comparing `pyxel_sim-2.1.1/pyxel/__init__.py` & `pyxel_sim-2.2/pyxel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/__main__.py` & `pyxel_sim-2.2/pyxel/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/backends/asdf.py` & `pyxel_sim-2.2/pyxel/backends/asdf.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/backends/hdf5.py` & `pyxel_sim-2.2/pyxel/backends/hdf5.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/__init__.py` & `pyxel_sim-2.2/pyxel/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/algorithm.py` & `pyxel_sim-2.2/pyxel/calibration/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/archipelago.py` & `pyxel_sim-2.2/pyxel/calibration/archipelago.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Sub-package to create 'archipelagos'."""
 import logging
+import warnings
 from collections.abc import Mapping, Sequence
 from concurrent.futures.thread import ThreadPoolExecutor
 from timeit import default_timer as timer
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import dask.array as da
 import numpy as np
@@ -27,18 +28,22 @@
     from dask.delayed import Delayed
     from numpy.typing import ArrayLike
 
     from pyxel.exposure import Readout
 
 
 # TODO: Deprecate this class ?
-class ArchipelagoLogs:
+class ArchipelagoLogs:  # pragma: no cover
     """Keep log information from all algorithms in an archipelago."""
 
     def __init__(self, algo_type: AlgorithmType, num_generations: int):
+        warnings.warn(
+            "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
+        )
+
         try:
             import pygmo as pg
         except ModuleNotFoundError as exc:
             raise ModuleNotFoundError(
                 "Missing optional package 'pygmo'.\n"
                 "Please install it with 'pip install pyxel-sim[calibration]' "
                 "or 'pip install pyxel-sim[all]'"
@@ -114,16 +119,20 @@
 
 def extract_data_3d(
     df_results: pd.DataFrame,
     rows: int,
     cols: int,
     times: int,
     readout_times: np.ndarray,
-) -> xr.Dataset:
+) -> xr.Dataset:  # pragma: no cover
     """Extract 'photon', 'charge', 'pixel', 'signal' and 'image' arrays from several delayed dynamic results."""
+    warnings.warn(
+        "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
+    )
+
     lst: list[xr.Dataset] = []
     for _, row in df_results.iterrows():
         island: int = row["island"]
         id_processor: int = row["id_processor"]
         result: Mapping[str, Delayed] = row["processor"].result
 
         photon_delayed: Delayed = result["photon"]
@@ -181,15 +190,15 @@
     if not isinstance(ds, xr.Dataset):
         raise TypeError("Expected a Dataset.")
 
     return ds
 
 
 # TODO: Rename to PyxelArchipelago. See #335
-class MyArchipelago:
+class MyArchipelago:  # pragma: no cover
     """User-defined Archipelago."""
 
     def __init__(
         self,
         num_islands: int,
         udi: IslandProtocol,
         algorithm: Algorithm,
@@ -197,14 +206,18 @@
         pop_size: int,
         bfe: Optional[Callable] = None,
         topology: Optional[Callable] = None,
         pygmo_seed: Optional[int] = None,
         parallel: bool = True,
         with_bar: bool = False,
     ):
+        warnings.warn(
+            "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
+        )
+
         try:
             import pygmo as pg
         except ModuleNotFoundError as exc:
             raise ModuleNotFoundError(
                 "Missing optional package 'pygmo'.\n"
                 "Please install it with 'pip install pyxel-sim[calibration]' "
                 "or 'pip install pyxel-sim[all]'"
```

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/archipelago_datatree.py` & `pyxel_sim-2.2/pyxel/calibration/archipelago_datatree.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/calibration.py` & `pyxel_sim-2.2/pyxel/calibration/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         """TBW."""
         self._weights = value
 
     def get_problem(
         self,
         processor: Processor,
         output_dir: Optional[Path],
-    ) -> ModelFitting:
+    ) -> ModelFitting:  # pragma: no cover
         """Convert a 'processor' object into a Pygmo Problem.
 
         Examples
         --------
         Create a 'Pygmo Problem'
         >>> calibration = Calibration(...)
         >>> problem = calibration.get_problem(processor=..., output_dir=...)
@@ -373,14 +373,18 @@
         Create a decision vector
         >>> problem.get_bounds()
         >>> decision_vector = [...]
 
         Compute fitness
         >>> problem.fitness(decision_vector)
         """
+        warnings.warn(
+            "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
+        )
+
         problem = ModelFitting(
             processor=processor,
             variables=self.parameters,
             readout=self.readout,
             calibration_mode=CalibrationMode(self.calibration_mode),
             simulation_output=self.result_type,
             generations=self.algorithm.generations,
@@ -401,15 +405,15 @@
         return problem
 
     def _run_calibration_deprecated(
         self,
         processor: Processor,
         output_dir: Optional[Path],
         with_progress_bar: bool = True,
-    ) -> tuple["xr.Dataset", "pd.DataFrame", "pd.DataFrame"]:
+    ) -> tuple["xr.Dataset", "pd.DataFrame", "pd.DataFrame"]:  # pragma: no cover
         """Run calibration pipeline."""
         warnings.warn(
             "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
         )
 
         try:
             import pygmo as pg
@@ -551,15 +555,15 @@
         return data_tree
 
     def _post_processing(
         self,
         ds: "xr.Dataset",
         df_processors: "pd.DataFrame",
         output: Optional["CalibrationOutputs"],
-    ) -> Sequence[Delayed]:
+    ) -> Sequence[Delayed]:  # pragma: no cover
         warnings.warn(
             "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
         )
 
         if output:
             filenames: Sequence[Delayed] = output._save_processors_deprecated(
                 processors=df_processors
```

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/fitness.py` & `pyxel_sim-2.2/pyxel/calibration/fitness.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/fitting.py` & `pyxel_sim-2.2/pyxel/calibration/fitting.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/fitting_datatree.py` & `pyxel_sim-2.2/pyxel/calibration/fitting_datatree.py`

 * *Files 4% similar despite different names*

```diff
@@ -321,14 +321,20 @@
                 f"Simulation mode: {self.sim_output!r} not implemented"
             )
 
         simulated_data = data[self.sim_output]
         if not isinstance(simulated_data, xr.DataArray):
             raise TypeError("Expected a 'DataArray'")
 
+        if "y" not in simulated_data.dims or "x" not in simulated_data.dims:
+            raise ValueError(
+                f"Missing dimensions 'y' or 'x' in container '{self.sim_output:s}'. "
+                f"{simulated_data=}"
+            )
+
         if self.sim_fit_range is not None:
             simulated_data = simulated_data.isel(indexers=self.sim_fit_range.to_dict())
 
         return simulated_data
 
     def _calculate_fitness(
         self,
@@ -437,18 +443,25 @@
 
                 overall_fitness += self._calculate_fitness(
                     simulated_data=simulated_data,
                     target_data=target_data,
                     weighting=weighting,  # TODO: 'weighting' should be a 'DataArray'
                 )
 
-        except Exception:
+        except Exception as exc:
             logging.exception(
-                "Catch an exception in 'fitness' for ModelFitting: %r.", self
+                "Catch an exception in 'fitness' for ModelFitting: %r with decision vector: %r.",
+                self,
+                decision_vector_1d,
             )
+            print(f"--- 3 - {exc=}, {exc.__notes__}")
+            # logging.warning('--- 3.1')
+            # logging.error('--- 3.1')
+            # logging.handlers[0].flush()
+
             raise
 
         return [overall_fitness]
 
     def convert_to_parameters(self, decisions_vector: "ArrayLike") -> np.ndarray:
         """Convert a decision version from Pygmo2 to parameters.
 
@@ -473,15 +486,15 @@
                 start = a
                 stop = a + b
                 parameters[..., start:stop] = np.power(10, parameters[..., start:stop])
             a += b
 
         return parameters
 
-    def apply_parameters(
+    def _apply_parameters(
         self, processor: Processor, parameter: np.ndarray
     ) -> "DataTree":
         """Create a new ``Processor`` with new parameters."""
         new_processor = self.update_processor(parameter=parameter, processor=processor)
 
         data_tree: "DataTree" = run_pipeline(
             processor=new_processor,
@@ -492,25 +505,27 @@
 
         return data_tree
 
     def apply_parameters_to_processors(
         self, parameters: "xr.DataArray"
     ) -> pd.DataFrame:
         """TBW."""
-        assert "island" in parameters.dims
-        assert "param_id" in parameters.dims
+        if "island" not in parameters.dims:
+            raise KeyError("Missing dimension 'island'")
+        if "param_id" not in parameters.dims:
+            raise KeyError("Missing dimension 'param_id'")
 
         lst = []
         for id_processor, processor in enumerate(self.param_processor_list):
             delayed_processor = delayed(processor)
 
             for idx_island, params_array in parameters.groupby("island"):
-                params: np.ndarray = params_array.data  # type
+                params: np.ndarray = params_array.to_numpy()
 
-                result_datatree: DataTree = delayed(self.apply_parameters)(
+                result_datatree: DataTree = delayed(self._apply_parameters)(
                     processor=delayed_processor, parameter=params
                 )
 
                 lst.append(
                     {
                         "island": idx_island,
                         "id_processor": id_processor,
```

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/protocols.py` & `pyxel_sim-2.2/pyxel/calibration/protocols.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/user_defined.py` & `pyxel_sim-2.2/pyxel/calibration/user_defined.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/calibration/util.py` & `pyxel_sim-2.2/pyxel/calibration/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/configuration/configuration.py` & `pyxel_sim-2.2/pyxel/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/__init__.py` & `pyxel_sim-2.2/pyxel/data_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/array.py` & `pyxel_sim-2.2/pyxel/data_structure/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,9 +282,9 @@
 
         .. image:: _static/photon_plot.png
         """
         import matplotlib.pyplot as plt
 
         arr: xr.DataArray = self.to_xarray()
 
-        arr.plot(robust=robust)
+        arr.plot.imshow(robust=robust)
         plt.title(self.NAME)
```

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/charge.py` & `pyxel_sim-2.2/pyxel/data_structure/charge.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,42 +163,30 @@
             "velocity_ver": init_ver_velocity,
             "velocity_hor": init_hor_velocity,
             "velocity_z": init_z_velocity,
         }
 
         return pd.DataFrame(new_charges)
 
-    def convert_df_to_array(self):
+    def convert_df_to_array(self) -> np.ndarray:
         """Convert charge dataframe to an array.
 
         Charge in the detector volume is collected and assigned to the nearest pixel.
         """
         # Late import to speedup start-up time
-        import numba
+        from numba import njit
 
-        @numba.jit(nopython=True)
+        @njit
         def df_to_array(
             array: np.ndarray,
-            charge_per_pixel: list,
-            pixel_index_ver: list,
-            pixel_index_hor: list,
-        ) -> np.ndarray:
-            """Assign charge in dataframe to nearest pixel.
-
-            Parameters
-            ----------
-            array: ndarray
-            charge_per_pixel: list
-            pixel_index_ver: list
-            pixel_index_hor:list
-
-            Returns
-            -------
-            ndarray
-            """
+            charge_per_pixel: np.ndarray,
+            pixel_index_ver: np.ndarray,
+            pixel_index_hor: np.ndarray,
+        ) -> np.ndarray:  # pragma: no cover
+            """Assign charges in dataframe to nearest pixel."""
             for i, charge_value in enumerate(charge_per_pixel):
                 array[pixel_index_ver[i], pixel_index_hor[i]] += charge_value
             return array
 
         array = np.zeros((self._geo.row, self._geo.col))
 
         charge_per_pixel = self.get_frame_values(quantity="number")
@@ -210,15 +198,20 @@
         ).astype(int)
         pixel_index_hor = np.floor_divide(
             charge_pos_hor, self._geo.pixel_horz_size
         ).astype(int)
 
         # Changing = to += since charge dataframe is reset, the pixel array need to be
         # incremented, we can't do the whole operation on each iteration
-        return df_to_array(array, charge_per_pixel, pixel_index_ver, pixel_index_hor)
+        return df_to_array(
+            array=array,
+            charge_per_pixel=charge_per_pixel,
+            pixel_index_ver=pixel_index_ver,
+            pixel_index_hor=pixel_index_hor,
+        )
 
     @staticmethod
     def convert_array_to_df(
         array: np.ndarray,
         num_rows: int,
         num_cols: int,
         pixel_vertical_size: float,
@@ -464,15 +457,15 @@
             List of particle ids: ``[0, 12, 321]``
 
         Returns
         -------
         array
         """
         if id_list:
-            df: pd.DataFrame = self._frame.query("index in %s" % id_list)
+            df: pd.DataFrame = self._frame.query(f"index in {id_list}")
         else:
             df = self._frame
 
         array: np.ndarray = df[quantity].values
 
         return array
 
@@ -499,10 +492,10 @@
         Parameters
         ----------
         id_list : Sequence of int
             List of particle ids: ``[0, 12, 321]``
         """
         if id_list:
             # TODO: Check carefully if 'inplace' is needed. This could break lot of things.
-            self._frame.query("index not in %s" % id_list, inplace=True)
+            self._frame.query(f"index not in {id_list}", inplace=True)
         else:
             self._frame = self.EMPTY_FRAME.copy()
```

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/image.py` & `pyxel_sim-2.2/pyxel/data_structure/image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/persistence.py` & `pyxel_sim-2.2/pyxel/data_structure/persistence.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/phase.py` & `pyxel_sim-2.2/pyxel/data_structure/phase.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/photon.py` & `pyxel_sim-2.2/pyxel/data_structure/photon.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import numpy as np
 import xarray as xr
 from typing_extensions import Self
 
 from pyxel.util import convert_unit, get_size
 
 if TYPE_CHECKING:
+    from matplotlib.pyplot import AxesImage
+
     from pyxel.detectors import Geometry
 
 
 class Photon:
     """Photon class designed to handle the storage of monochromatic (unit: ph or multi-wavelength photons (unit ph/nm).
 
     Monochromatic photons are stored in a 2D Numpy array and
@@ -517,15 +519,15 @@
                 "units": "nm",
                 "long_name": "Wavelength",
             }
             data_3d.attrs = {"units": convert_unit("Ph/nm"), "long_name": "Photon"}
 
             return data_3d
 
-    def plot(self, robust: bool = True) -> None:
+    def plot(self, robust: bool = True) -> "AxesImage":
         """Plot the array using Matplotlib.
 
         Parameters
         ----------
         robust : bool, optional
             If True, the colormap is computed with 2nd and 98th percentile
             instead of the extreme values.
@@ -534,12 +536,12 @@
         --------
         >>> detector.photon.plot()
 
         .. image:: _static/photon_plot.png
         """
         arr: xr.DataArray = self.to_xarray()
 
-        return arr.plot(robust=robust)
+        return arr.plot.imshow(robust=robust)
 
     def empty(self) -> None:
         """Empty the data container."""
         self._array = None
```

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/pixel.py` & `pyxel_sim-2.2/pyxel/data_structure/pixel.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/scene.py` & `pyxel_sim-2.2/pyxel/data_structure/scene.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/signal.py` & `pyxel_sim-2.2/pyxel/data_structure/signal.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/data_structure/util.py` & `pyxel_sim-2.2/pyxel/data_structure/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/__init__.py` & `pyxel_sim-2.2/pyxel/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/apd/apd.py` & `pyxel_sim-2.2/pyxel/detectors/apd/apd.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/apd/apd_characteristics.py` & `pyxel_sim-2.2/pyxel/detectors/apd/apd_characteristics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/apd/apd_geometry.py` & `pyxel_sim-2.2/pyxel/detectors/apd/apd_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/ccd/ccd.py` & `pyxel_sim-2.2/pyxel/detectors/ccd/ccd.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/ccd/ccd_geometry.py` & `pyxel_sim-2.2/pyxel/detectors/ccd/ccd_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/characteristics.py` & `pyxel_sim-2.2/pyxel/detectors/characteristics.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 
-from collections.abc import Iterable, Mapping
+from collections.abc import Iterable, Mapping, Sequence
 from typing import Optional
 
 import numpy as np
 from toolz import dicttoolz
 
 from pyxel.util import get_size
 
@@ -40,30 +40,35 @@
         quantum_efficiency: Optional[float] = None,  # unit: NA
         charge_to_volt_conversion: Optional[float] = None,  # unit: volt/electron
         pre_amplification: Optional[float] = None,  # unit: V/V
         full_well_capacity: Optional[float] = None,  # unit: electron
         adc_bit_resolution: Optional[int] = None,
         adc_voltage_range: Optional[tuple[float, float]] = None,  # unit: V
     ):
-        if quantum_efficiency and not (0.0 <= quantum_efficiency <= 1.0):
+        if quantum_efficiency is not None and not (0.0 <= quantum_efficiency <= 1.0):
             raise ValueError("'quantum_efficiency' must be between 0.0 and 1.0.")
         if charge_to_volt_conversion and not (
             0.0 <= charge_to_volt_conversion <= 100.0
         ):
             raise ValueError(
                 "'charge_to_volt_conversion' must be between 0.0 and 100.0."
             )
-        if pre_amplification and not (0.0 <= pre_amplification <= 10000.0):
+        if pre_amplification is not None and not (0.0 <= pre_amplification <= 10_000.0):
             raise ValueError("'pre_amplification' must be between 0.0 and 10000.0.")
-        if full_well_capacity and not (0.0 <= full_well_capacity <= 1.0e7):
+        if full_well_capacity is not None and not (0.0 <= full_well_capacity <= 1.0e7):
             raise ValueError("'full_well_capacity' must be between 0 and 1e7.")
-        if adc_bit_resolution and not (4 <= adc_bit_resolution <= 64):
+        if adc_bit_resolution is not None and not (4 <= adc_bit_resolution <= 64):
             raise ValueError("'adc_bit_resolution' must be between 4 and 64.")
-        if adc_voltage_range and not len(adc_voltage_range) == 2:
-            raise ValueError("Voltage range must have length of 2.")
+
+        if adc_voltage_range is not None:
+            if not isinstance(adc_voltage_range, Sequence):
+                raise TypeError("Voltage range must have length of 2.")
+
+            if len(adc_voltage_range) != 2:
+                raise ValueError("Voltage range must have length of 2.")
 
         self._quantum_efficiency = quantum_efficiency
         self._charge_to_volt_conversion = charge_to_volt_conversion
         self._pre_amplification = pre_amplification
         self._full_well_capacity = full_well_capacity
 
         if adc_voltage_range is None:
@@ -88,110 +93,111 @@
             and self._adc_voltage_range == other._adc_voltage_range
             and self._adc_bit_resolution == other._adc_bit_resolution
         )
 
     @property
     def quantum_efficiency(self) -> float:
         """Get Quantum efficiency."""
-        if self._quantum_efficiency:
-            return self._quantum_efficiency
-        else:
+        if self._quantum_efficiency is None:
             raise ValueError(
                 "'quantum_efficiency' not specified in detector characteristics."
             )
 
+        return self._quantum_efficiency
+
     @quantum_efficiency.setter
     def quantum_efficiency(self, value: float) -> None:
         """Set Quantum efficiency."""
-        if np.min(value) < 0.0 and np.max(value) <= 1.0:
+        # TODO: Refactor this
+        if np.min(value) < 0.0 or np.max(value) > 1.0:
             raise ValueError("'quantum_efficiency' values must be between 0.0 and 1.0.")
 
         self._quantum_efficiency = value
 
     @property
     def charge_to_volt_conversion(self) -> float:
         """Get charge to volt conversion parameter."""
-        if self._charge_to_volt_conversion:
-            return self._charge_to_volt_conversion
-        else:
+        if self._charge_to_volt_conversion is None:
             raise ValueError(
                 "'charge_to_volt_conversion' not specified in detector characteristics."
             )
 
+        return self._charge_to_volt_conversion
+
     @charge_to_volt_conversion.setter
     def charge_to_volt_conversion(self, value: float) -> None:
         """Set charge to volt conversion parameter."""
         if not (0.0 <= value <= 100.0):
             raise ValueError(
                 "'charge_to_volt_conversion' must be between 0.0 and 100.0."
             )
         self._charge_to_volt_conversion = value
 
     @property
     def pre_amplification(self) -> float:
         """Get voltage pre-amplification gain."""
-        if self._pre_amplification:
-            return self._pre_amplification
-        else:
+        if self._pre_amplification is None:
             raise ValueError(
                 "'pre_amplification' not specified in detector characteristics."
             )
 
+        return self._pre_amplification
+
     @pre_amplification.setter
     def pre_amplification(self, value: float) -> None:
         """Set voltage pre-amplification gain.."""
-        if not (0.0 <= value <= 10000.0):
+        if not (0.0 <= value <= 10_000.0):
             raise ValueError("'pre_amplification' must be between 0.0 and 10000.0.")
 
         self._pre_amplification = value
 
     @property
     def adc_bit_resolution(self) -> int:
         """Get bit resolution of the Analog-Digital Converter."""
-        if self._adc_bit_resolution:
-            return self._adc_bit_resolution
-        else:
+        if self._adc_bit_resolution is None:
             raise ValueError(
                 "'adc_bit_resolution' not specified in detector characteristics."
             )
 
+        return self._adc_bit_resolution
+
     @adc_bit_resolution.setter
     def adc_bit_resolution(self, value: int) -> None:
         """Set bit resolution of the Analog-Digital Converter."""
         self._adc_bit_resolution = value
 
     @property
     def adc_voltage_range(self) -> tuple[float, float]:
         """Get voltage range of the Analog-Digital Converter."""
-        if self._adc_voltage_range:
-            return self._adc_voltage_range
-        else:
+        if self._adc_voltage_range is None:
             raise ValueError(
                 "'adc_voltage_range' not specified in detector characteristics."
             )
 
+        return self._adc_voltage_range
+
     @adc_voltage_range.setter
     def adc_voltage_range(self, value: tuple[float, float]) -> None:
         """Set voltage range of the Analog-Digital Converter."""
         self._adc_voltage_range = value
 
     @property
     def full_well_capacity(self) -> float:
         """Get Full well capacity."""
-        if self._full_well_capacity:
-            return self._full_well_capacity
-        else:
+        if self._full_well_capacity is None:
             raise ValueError(
                 "'full_well_capacity' not specified in detector characteristics."
             )
 
+        return self._full_well_capacity
+
     @full_well_capacity.setter
     def full_well_capacity(self, value: float) -> None:
         """Set Full well capacity."""
-        if value not in range(10000001):
+        if not (0 <= value <= 10_000_000):
             raise ValueError("'full_well_capacity' must be between 0 and 1e+7.")
 
         self._full_well_capacity = value
 
     @property
     def system_gain(self) -> float:
         """Get system gain."""
```

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/cmos/cmos.py` & `pyxel_sim-2.2/pyxel/detectors/cmos/cmos.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/cmos/cmos_geometry.py` & `pyxel_sim-2.2/pyxel/detectors/cmos/cmos_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/detector.py` & `pyxel_sim-2.2/pyxel/detectors/detector.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/environment.py` & `pyxel_sim-2.2/pyxel/detectors/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,25 @@
     """Information about multi-wavelength."""
 
     cut_on: float
     cut_off: float
     resolution: int
 
     def __post_init__(self):
-        assert 0 < self.cut_on <= self.cut_off
-        assert self.resolution > 0
+        if self.cut_on <= 0:
+            raise ValueError(f"'cut_on' must be > 0. {self.cut_on=}")
+
+        if self.cut_on > self.cut_off:
+            raise ValueError(
+                "'cut_off' must be bigger than 'cut_on'. "
+                f"{self.cut_on=}, {self.cut_off=}"
+            )
+
+        if self.resolution <= 0:
+            raise ValueError(f"'resolution' must be > 0. {self.resolution=}")
 
     def to_dict(self) -> dict:
         return {
             "cut_on": self.cut_on,
             "cut_off": self.cut_off,
             "resolution": self.resolution,
         }
@@ -65,26 +74,20 @@
     """
 
     def __init__(
         self,
         temperature: Optional[float] = None,
         wavelength: Union[float, WavelengthHandling, None] = None,
     ):
-        if isinstance(temperature, (int, float)) and not (0.0 <= temperature <= 1000.0):
+        if isinstance(temperature, (int, float)) and not (0.0 < temperature <= 1000.0):
             raise ValueError("'temperature' must be between 0.0 and 1000.0.")
 
         if isinstance(wavelength, (int, float)) and not (wavelength > 0.0):
             raise ValueError("'wavelength' must be strictly positive.")
 
-        if isinstance(wavelength, WavelengthHandling):
-            if not (wavelength.cut_on < wavelength.cut_off):
-                raise ValueError("'cut_on' must be strictly inferior to 'cut_off'.")
-            if not (wavelength.resolution > 0):
-                raise ValueError("'resolution' must be strictly positive and not 0.")
-
         self._temperature: Optional[float] = (
             float(temperature) if temperature is not None else None
         )
 
         self._wavelength: Union[float, WavelengthHandling, None] = (
             float(wavelength) if isinstance(wavelength, (int, float)) else wavelength
         )
@@ -101,47 +104,43 @@
             and self._temperature == other._temperature
             and self._wavelength == other._wavelength
         )
 
     @property
     def temperature(self) -> float:
         """Get Temperature of the detector."""
-        if self._temperature:
-            return self._temperature
-        else:
+        if self._temperature is None:
             raise ValueError("'temperature' not specified in detector environment.")
 
+        return self._temperature
+
     @temperature.setter
     def temperature(self, value: float) -> None:
         """Set Temperature of the detector."""
-        if not (0.0 <= value <= 1000.0):
+        if not (0.0 < value <= 1000.0):
             raise ValueError("'temperature' must be between 0.0 and 1000.0.")
 
         self._temperature = value
 
     @property
     def wavelength(self) -> Union[float, WavelengthHandling]:
         """Get wavelength of the detector."""
         if self._wavelength is None:
             raise ValueError("'wavelength' not specified in detector environment.")
+
         return self._wavelength
 
     @wavelength.setter
-    def wavelength(self, value: Union[float, WavelengthHandling]) -> None:
+    def wavelength(self, value: Union[int, float, WavelengthHandling]) -> None:
         """Set wavelength of the detector."""
-        if isinstance(value, float) and not (value > 0.0):
-            raise ValueError("'wavelength' must be strictly positive.")
-
-        elif isinstance(value, WavelengthHandling):
-            if not (value.cut_on < value.cut_off):
-                raise ValueError("'cut_on' must be strictly inferior to 'cut_off'.")
-            if not (value.resolution > 0):
-                raise ValueError("'resolution' must be strictly positive and not 0.")
-        else:
-            raise ValueError("A WavelengthHandling object or a float must be provided.")
+        if isinstance(value, (int, float)):
+            if value <= 0.0:
+                raise ValueError("'wavelength' must be strictly positive.")
+        elif not isinstance(value, WavelengthHandling):
+            raise TypeError("A WavelengthHandling object or a float must be provided.")
 
         self._wavelength = value
 
     @property
     def numbytes(self) -> int:
         """Recursively calculates object size in bytes using Pympler library.
 
@@ -152,19 +151,20 @@
         """
         self._numbytes = get_size(self)
         return self._numbytes
 
     def to_dict(self) -> Mapping:
         """Get the attributes of this instance as a `dict`."""
         if self._wavelength is None:
-            wavelength_dict = {}
+            wavelength_dict: dict[str, Union[int, float, dict]] = {}
         elif isinstance(self._wavelength, (int, float)):
             wavelength_dict = {"wavelength": self._wavelength}
         else:
-            wavelength_dict = self._wavelength.to_dict()
+            wavelength_dict = {"wavelength": self._wavelength.to_dict()}
+
         return {"temperature": self._temperature} | wavelength_dict
 
     @classmethod
     def from_dict(cls, dct: Mapping) -> Self:
         """Create a new instance of `Geometry` from a `dict`."""
 
         value = dct.get("wavelength")
```

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/geometry.py` & `pyxel_sim-2.2/pyxel/detectors/geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/mkid/mkid.py` & `pyxel_sim-2.2/pyxel/detectors/mkid/mkid.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/mkid/mkid_geometry.py` & `pyxel_sim-2.2/pyxel/detectors/mkid/mkid_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/detectors/readout_properties.py` & `pyxel_sim-2.2/pyxel/detectors/readout_properties.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/evaluator.py` & `pyxel_sim-2.2/pyxel/evaluator.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,44 +15,52 @@
 
 import numpy as np
 
 __all__ = ["evaluate_reference", "eval_range", "eval_entry"]
 
 
 def evaluate_reference(reference_str: str) -> Callable:
-    """Evaluate a module's class, function, or constant.
+    """Evaluate a reference to a module's class or function.
 
-    :param str reference_str: the python expression to
-        evaluate or retrieve the module attribute reference to.
+    Parameters
+    ----------
+    reference_str : str
+        The python expression to evaluate or retrieve the module attribute reference to.
         This is usually a reference to a class or a function.
-    :return: the module attribute or object.
-    :rtype: object
-    :raises ModuleNotFoundError: if reference_str cannot be evaluated to a callable.
+
+    Returns
+    -------
+    Callable
+        A reference to the class or function.
+
+    Raises
+    ------
+    ModuleNotFoundError
+        raised if reference_str cannot be evaluated to a callable.
     """
     if not reference_str:
         raise ImportError("Empty string cannot be evaluated")
 
     if "." not in reference_str:
         raise ImportError("Missing module path")
 
     # reference to a module class, function, or constant
     module_str, function_str = reference_str.rsplit(".", 1)
     try:
         module = importlib.import_module(module_str)
 
         reference: Callable = getattr(module, function_str)
-        assert callable(reference)
+        if not callable(reference):
+            raise TypeError(f"{reference_str!r} is not a callable")
 
         # if isinstance(reference, type):
         #     # this is a class type, instantiate it using default arguments.
         #     reference = reference()
     except ModuleNotFoundError as exc:
-        raise ModuleNotFoundError(
-            f"Cannot import module: {module_str!r}. exc: {exc}"
-        ) from exc
+        raise ModuleNotFoundError(f"Cannot import module: {module_str!r}.") from exc
     except AttributeError as ex:
         raise ImportError(
             f"Module: {module_str!r}, does not contain {function_str!r}"
         ) from ex
 
     return reference
```

### Comparing `pyxel_sim-2.1.1/pyxel/exposure/__init__.py` & `pyxel_sim-2.2/pyxel/exposure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/exposure/exposure.py` & `pyxel_sim-2.2/pyxel/exposure/exposure.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/exposure/readout.py` & `pyxel_sim-2.2/pyxel/exposure/readout.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/inputs/loader.py` & `pyxel_sim-2.2/pyxel/inputs/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,22 +302,21 @@
             raise FileNotFoundError(f"Input file '{full_filename}' can not be found.")
 
         url_path: str = str(full_filename)
     else:
         url_path = filename
 
     if suffix.startswith(".fits"):
-        from astropy.io import fits
         from astropy.table import Table
 
-        with fits.open(url_path) as hdus:
-            if data_path is None:
-                data_path = 0
-            assert isinstance(data_path, int)
-            assert isinstance(hdus[data_path], (fits.TableHDU, fits.BinTableHDU))
+        # with fits.open(url_path) as hdus:
+        #     if data_path is None:
+        #         data_path = 0
+        #     assert isinstance(data_path, int)
+        #     assert isinstance(hdus[data_path], (fits.TableHDU, fits.BinTableHDU))
         table: pd.DataFrame = Table.read(url_path, hdu=data_path).to_pandas()
         if rename_cols:
             col_new = {value: key for key, value in rename_cols.items()}
             table_data = table.rename(columns=col_new)[list(rename_cols)]
         else:
             table_data = table
 
@@ -328,18 +327,20 @@
                 dims = []
                 for ax in range(len(table.columns)):
                     for key, value in rename_cols.items():
                         if value == ax:
                             dims.append(key)
                             break
                     else:
-                        raise ValueError
+                        raise KeyError(f"Missing columns. {rename_cols=}")
 
                 table.columns = dims
                 table_data = table.copy()
+            else:
+                table_data = table
 
     elif suffix.startswith((".txt", ".data", ".csv")):
         with open(url_path) as file_handler:
             data: str = file_handler.read()
         valid_delimiters: Sequence[str] = ("\t", " ", ",", "|", ";")
         valid_delimiters_str = "".join(valid_delimiters)
 
@@ -351,15 +352,15 @@
 
         delimiter: str = dialect.delimiter
 
         if delimiter not in valid_delimiters:
             raise ValueError(f"Cannot find the separator. {delimiter=!r}")
 
         with StringIO(data) as file_handler:
-            if suffix.startswith("csv"):
+            if suffix.startswith(".csv"):
                 table = pd.read_csv(
                     file_handler,
                     delimiter=delimiter,
                     header=0 if header else None,
                     usecols=rename_cols.values() if rename_cols else None,
                 )
             else:
```

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_collection/__init__.py` & `pyxel_sim-2.2/pyxel/models/charge_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_collection/collection.py` & `pyxel_sim-2.2/pyxel/models/charge_collection/collection.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_collection/diffusion.py` & `pyxel_sim-2.2/pyxel/models/charge_collection/diffusion.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_collection/fixed_pattern_noise.py` & `pyxel_sim-2.2/pyxel/models/charge_collection/fixed_pattern_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_collection/full_well.py` & `pyxel_sim-2.2/pyxel/models/charge_collection/full_well.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_collection/inter_pixel_capacitance.py` & `pyxel_sim-2.2/pyxel/models/charge_collection/inter_pixel_capacitance.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_collection/persistence.py` & `pyxel_sim-2.2/pyxel/models/charge_collection/persistence.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/__init__.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,15 @@
 
 # flake8: noqa
 from .charge_injection import charge_blocks
 from .dark_current_rule07 import dark_current_rule07
 from .load_charge import load_charge
 from .photoelectrons import simple_conversion, conversion_with_qe_map
 from .cosmix.cosmix import cosmix
+from .simple_dark_current import simple_dark_current
 from .dark_current_induced import radiation_induced_dark_current
-from .dark_current import dark_current, simple_dark_current, dark_current_saphira
+from .dark_current import dark_current
+from .dark_current_saphira import dark_current_saphira
 from .apd_gain import apd_gain
 from .charge_deposition import charge_deposition
 from .charge_deposition import charge_deposition_in_mct
 from .wavelength_qe import apply_qe_curve, conversion_with_3d_qe_map
```

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/apd_gain.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/apd_gain.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/charge_deposition.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/charge_deposition.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/charge_injection.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/charge_injection.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/cosmix.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/cosmix.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/particle.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/particle.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/plotting.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/plotting.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/simulation.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/simulation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/cosmix/util.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/cosmix/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/dark_current_induced.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/dark_current_induced.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/dark_current_rule07.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/dark_current_rule07.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/data/mct-stopping-power.csv` & `pyxel_sim-2.2/pyxel/models/charge_generation/data/mct-stopping-power.csv`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt` & `pyxel_sim-2.2/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt` & `pyxel_sim-2.2/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv` & `pyxel_sim-2.2/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/load_charge.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/load_charge.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/photoelectrons.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/photoelectrons.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_generation/wavelength_qe.py` & `pyxel_sim-2.2/pyxel/models/charge_generation/wavelength_qe.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/__init__.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/amplifier_crosstalk.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/amplifier_crosstalk.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/linearity.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/linearity.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/measurement.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/measurement.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/nghxrg/nghxrg.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/nghxrg/nghxrg.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/non_linearity_calculation.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/non_linearity_calculation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/offset.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/offset.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/readout_noise.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/readout_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_measurement/reset_noise.py` & `pyxel_sim-2.2/pyxel/models/charge_measurement/reset_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_transfer/__init__.py` & `pyxel_sim-2.2/pyxel/models/charge_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py` & `pyxel_sim-2.2/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_transfer/cdm.py` & `pyxel_sim-2.2/pyxel/models/charge_transfer/cdm.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_transfer/emccd_poisson.py` & `pyxel_sim-2.2/pyxel/models/charge_transfer/emccd_poisson.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/charge_transfer/emccd_poisson_cic.py` & `pyxel_sim-2.2/pyxel/models/charge_transfer/emccd_poisson_cic.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/data_processing/__init__.py` & `pyxel_sim-2.2/pyxel/models/data_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/data_processing/linear_regression.py` & `pyxel_sim-2.2/pyxel/models/data_processing/linear_regression.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/data_processing/mean_variance.py` & `pyxel_sim-2.2/pyxel/models/data_processing/mean_variance.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/data_processing/remove_cosmic_rays.py` & `pyxel_sim-2.2/pyxel/models/data_processing/remove_cosmic_rays.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/data_processing/snr.py` & `pyxel_sim-2.2/pyxel/models/data_processing/snr.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/data_processing/source_extractor.py` & `pyxel_sim-2.2/pyxel/models/data_processing/source_extractor.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/data_processing/statistics.py` & `pyxel_sim-2.2/pyxel/models/data_processing/statistics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/phasing/mkid_models/SC.py` & `pyxel_sim-2.2/pyxel/models/phasing/mkid_models/SC.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/phasing/mkid_models/SCtheory/__init__.py` & `pyxel_sim-2.2/pyxel/models/phasing/mkid_models/SCtheory/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/phasing/pulse_processing.py` & `pyxel_sim-2.2/pyxel/models/phasing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/__init__.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/ariel_airs.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/ariel_airs.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     Parameters
     ----------
     wavelength : quantity array
         Wavelength. Unit: usually micron. Dimension: small_n.
     flux : quantity array
         Flux. Unit: ph/s/m2/micron. Dimension: big_n.
     psf_wavelength : quantity array
-        Point Spead Function per wavelength.
+        Point Spread Function per wavelength.
 
     Returns
     -------
     flux : quantity array
         Flux. UNit: photon/s. Dimension: nw.
     """
```

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/illumination.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/illumination.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/load_image.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/load_image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/point_spread_function.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/point_spread_function.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/poppy.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/poppy.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/shot_noise.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/shot_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/simple_collection.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/simple_collection.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/photon_collection/stripe_pattern.py` & `pyxel_sim-2.2/pyxel/models/photon_collection/stripe_pattern.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/readout_electronics/__init__.py` & `pyxel_sim-2.2/pyxel/models/readout_electronics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/readout_electronics/amplification.py` & `pyxel_sim-2.2/pyxel/models/readout_electronics/amplification.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/readout_electronics/dead_time.py` & `pyxel_sim-2.2/pyxel/models/readout_electronics/dead_time.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/readout_electronics/phase_conversion.py` & `pyxel_sim-2.2/pyxel/models/readout_electronics/phase_conversion.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/readout_electronics/sar_adc.py` & `pyxel_sim-2.2/pyxel/models/readout_electronics/sar_adc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/readout_electronics/sar_adc_with_noise.py` & `pyxel_sim-2.2/pyxel/models/readout_electronics/sar_adc_with_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/readout_electronics/simple_adc.py` & `pyxel_sim-2.2/pyxel/models/readout_electronics/simple_adc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/scene_generation/load_star_map.py` & `pyxel_sim-2.2/pyxel/models/scene_generation/load_star_map.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/models/util.py` & `pyxel_sim-2.2/pyxel/models/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/notebook/__init__.py` & `pyxel_sim-2.2/pyxel/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/notebook/calibration.py` & `pyxel_sim-2.2/pyxel/notebook/calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,17 +403,17 @@
     return best
 
 
 def champion_heatmap(
     ds: "xr.Dataset",
     num_bins: int = 100,
     logx: bool = False,
-    parameter_range: Optional[list] = None,
-    island_range: Optional[list] = None,
-    ind_range: Optional[list] = None,
+    parameter_range: Optional[tuple[int, int]] = None,
+    island_range: Optional[tuple[int, int]] = None,
+    ind_range: Optional[tuple[int, int]] = None,
 ) -> "hv.Points":
     """Plot a heatmap of champion parameters vs fitness.
 
     Parameters
     ----------
     ds: Dataset
         Result dataset.
```

### Comparing `pyxel_sim-2.1.1/pyxel/notebook/html_representation.py` & `pyxel_sim-2.2/pyxel/notebook/html_representation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/notebook/jupyxel.py` & `pyxel_sim-2.2/pyxel/notebook/jupyxel.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         color_norm = pm.Selector(objects=["linear", "log"], doc="foo")
         color_map = pm.Selector(
             objects={
                 "fire": cc.fire,
                 "gray": cc.gray,  # linear colormaps, for plotting magnitudes
                 "blues": cc.blues,  # linear colormaps, for plotting magnitudes
                 "colorwheel": cc.colorwheel,  # cyclic colormaps for cyclic quantities like orientation or phase
-                "coolwarm": cc.coolwarm,  # diverging colormap, for plotting magnitude increasing or decreasin from a central point
+                "coolwarm": cc.coolwarm,  # diverging colormap, for plotting magnitude increasing or decreasing from a central point
                 "rainbow": cc.rainbow4,  # To highlight local differences in sequential data
                 "isoluminant": cc.isolum,  # To highlight low spatial-frequency information
             }
         )
         flip_yaxis = pm.Boolean(default=True)
 
         # Histogram
```

### Comparing `pyxel_sim-2.1.1/pyxel/observation/observation.py` & `pyxel_sim-2.2/pyxel/observation/observation.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,24 +85,32 @@
 
 def _get_short_name_with_model(name: str) -> str:
     _, _, model_name, _, param_name = name.split(".")
 
     return f"{model_name}.{param_name}"
 
 
-def _get_final_short_name(name: str, param_type: ParameterType) -> str:
+def _get_final_short_name(
+    name: str, param_type: ParameterType
+) -> str:  # pragma: no cover
+    warnings.warn(
+        "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
+    )
+
     if param_type == ParameterType.Simple:
         return name
     elif param_type == ParameterType.Multi:
         return _id(name)
     else:
         raise NotImplementedError
 
 
-def _get_short_dimension_names(types: Mapping[str, ParameterType]) -> Mapping[str, str]:
+def _get_short_dimension_names(
+    types: Mapping[str, ParameterType]
+) -> Mapping[str, str]:  # pragma: no cover
     warnings.warn(
         "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
     )
     # Create potential names for the dimensions
     potential_dim_names: dict[str, str] = {}
     for param_name, param_type in types.items():
         short_name: str = short(param_name)
@@ -231,15 +239,15 @@
     def result_type(self) -> ResultId:
         """TBW."""
         return self._result_type
 
     @result_type.setter
     def result_type(self, value: ResultId) -> None:
         """TBW."""
-        self._result_type = value
+        self._result_type = get_result_id(value)
 
     @property
     def pipeline_seed(self) -> Optional[int]:
         """TBW."""
         return self._pipeline_seed
 
     @pipeline_seed.setter
@@ -381,15 +389,15 @@
             self._product_indices(), itertools.product(*all_steps)
         ):
             parameter_dict = {}
             for key, value in zip(keys, params):
                 parameter_dict.update({key: value})
             yield indices, parameter_dict
 
-    def _parameter_it(self) -> Iterator[tuple]:
+    def _parameter_it(self) -> Iterator[tuple]:  # pragma: no cover
         """Return the method for generating parameters based on parametric mode."""
         warnings.warn(
             "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
         )
         if self.parameter_mode == ParameterMode.Product:
             yield from self._product_parameters()
 
@@ -444,15 +452,15 @@
             ]
 
         else:
             raise ValueError("Parametric mode not specified.")
 
     def _processors_it(
         self, processor: "Processor"
-    ) -> Iterator[tuple["Processor", Union[int, tuple[int]], dict]]:
+    ) -> Iterator[tuple["Processor", Union[int, tuple[int]], dict]]:  # pragma: no cover
         """Generate processors with different product parameters.
 
         Parameters
         ----------
         processor: Processor
 
         Yields
@@ -478,15 +486,15 @@
         """Check for each step if parameters can be used as dataset coordinates (1D, simple) or not (multi)."""
         for step in self.enabled_steps:
             self.parameter_types.update({step.key: step.type})
         return self.parameter_types
 
     def _run_debug_mode_deprecated(
         self, processor: "Processor"
-    ) -> tuple[list["Processor"], "xr.Dataset"]:
+    ) -> tuple[list["Processor"], "xr.Dataset"]:  # pragma: no cover
         """Run observation pipelines in debug mode and return list of processors and parameter logs.
 
         Parameters
         ----------
         processor: Processor
 
         Returns
@@ -568,15 +576,17 @@
             ):
                 raise ValueError(
                     "Either define 'custom' as parametric mode or "
                     "do not use '_' character in 'values' field"
                 )
 
     # ruff: noqa: C901
-    def _run_observation_deprecated(self, processor: "Processor") -> ObservationResult:
+    def _run_observation_deprecated(
+        self, processor: "Processor"
+    ) -> ObservationResult:  # pragma: no cover
         """Run the observation pipelines.
 
         Parameters
         ----------
         processor : Processor
 
         Returns
@@ -858,15 +868,15 @@
         ],
         dimension_names: Mapping[str, str],
         processor: "Processor",
         x: range,
         y: range,
         times: np.ndarray,
         types: Mapping[str, ParameterType],
-    ) -> "xr.Dataset":
+    ) -> "xr.Dataset":  # pragma: no cover
         warnings.warn(
             "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
         )
 
         index, parameter_dict, n = index_and_parameter
 
         new_processor = create_new_processor(
@@ -959,15 +969,15 @@
             ParametersType,
             int,
         ],
         processor: "Processor",
         x: range,
         y: range,
         times: np.ndarray,
-    ):
+    ):  # pragma: no cover
         warnings.warn(
             "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
         )
 
         index, parameter_dict, n = index_and_parameter
 
         new_processor = create_new_processor(
@@ -1008,15 +1018,15 @@
         ],
         dimension_names: Mapping[str, str],
         processor: "Processor",
         x: range,
         y: range,
         times: np.ndarray,
         types: Mapping[str, ParameterType],
-    ):
+    ):  # pragma: no cover
         warnings.warn(
             "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
         )
 
         index, parameter_dict, n = index_and_parameter
 
         new_processor = create_new_processor(
@@ -1076,27 +1086,33 @@
 
     for key in parameter_dict:
         new_processor.set(key=key, value=parameter_dict[key])
 
     return new_processor
 
 
-def _id(s: str) -> str:
+def _id(s: str) -> str:  # pragma: no cover
     """Add _id to the end of a string."""
+    warnings.warn(
+        "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
+    )
+
     out = s + "_id"
     return out
 
 
 def short(s: str) -> str:
     """Split string with . and return the last element."""
     out = s.split(".")[-1]
     return out
 
 
-def log_parameters(processor_id: int, parameter_dict: dict) -> "xr.Dataset":
+def log_parameters(
+    processor_id: int, parameter_dict: dict
+) -> "xr.Dataset":  # pragma: no cover
     """Return parameters in the current processor in a xarray dataset.
 
     Parameters
     ----------
     processor_id: int
     parameter_dict: dict
 
@@ -1123,15 +1139,15 @@
 
 
 def parameter_to_dataset(
     parameter_dict: dict,
     dimension_names: Mapping[str, str],
     index: int,
     coordinate_name: str,
-) -> "xr.Dataset":
+) -> "xr.Dataset":  # pragma: no cover
     """Return a specific parameter dataset from a parameter dictionary.
 
     Parameters
     ----------
     parameter_dict: dict
     dimension_names
     index: int
@@ -1166,15 +1182,17 @@
     parameter = parameter.assign_coords({short_coord_name_id: index})
     parameter = parameter.expand_dims(dim=short_coord_name_id)
     parameter_ds[short_coord_name] = parameter
 
     return parameter_ds
 
 
-def _add_custom_parameters_deprecated(ds: "xr.Dataset", index: int) -> "xr.Dataset":
+def _add_custom_parameters_deprecated(
+    ds: "xr.Dataset", index: int
+) -> "xr.Dataset":  # pragma: no cover
     """Add coordinate "index" to the dataset.
 
     Parameters
     ----------
     ds: Dataset
     index: int
 
@@ -1238,15 +1256,15 @@
 def _add_sequential_parameters_deprecated(
     ds: "xr.Dataset",
     parameter_dict: ParametersType,
     dimension_names: Mapping[str, str],
     index: int,
     coordinate_name: str,
     types: Mapping[str, ParameterType],
-) -> "xr.Dataset":
+) -> "xr.Dataset":  # pragma: no cover
     """Add true coordinates or index to sequential mode dataset.
 
     Parameters
     ----------
     ds : Dataset
     parameter_dict : dict
     dimension_names
@@ -1272,21 +1290,21 @@
     elif types[coordinate_name] == ParameterType.Multi:
         ds = ds.assign_coords({short_name: index})
         ds = ds.expand_dims(dim=short_name)
 
     return ds
 
 
-def _add_product_parameters_deprecated(
+def _add_product_parameters_deprecated(  # pragma: no cover
     ds: "xr.Dataset",
     parameter_dict: ParametersType,
     dimension_names: Mapping[str, str],
     indices: tuple[int, ...],
     types: Mapping[str, ParameterType],
-) -> "xr.Dataset":
+) -> "xr.Dataset":  # pragma: no cover
     """Add true coordinates or index to product mode dataset.
 
     Parameters
     ----------
     ds: Dataset
     parameter_dict: dict
     indices: tuple
@@ -1315,15 +1333,19 @@
 
         else:
             raise NotImplementedError
 
     return ds
 
 
-def to_tuples(data: Iterable) -> tuple:
+def to_tuples(data: Iterable) -> tuple:  # pragma: no cover
+    warnings.warn(
+        "Deprecated. Will be removed in Pyxel 2.0", DeprecationWarning, stacklevel=1
+    )
+
     lst: list = []
     for el in data:
         if isinstance(el, Iterable) and not isinstance(el, str):
             lst.append(to_tuples(el))
         else:
             lst.append(el)
 
@@ -1399,15 +1421,15 @@
     return data_tree
 
 
 def compute_final_sequential_dataset(
     list_of_index_and_parameter: list,
     list_of_datasets: list,
     dimension_names: Mapping[str, str],
-) -> dict[str, "xr.Dataset"]:
+) -> dict[str, "xr.Dataset"]:  # pragma: no cover
     """Return a dictionary of result datasets where keys are different parameters.
 
     Parameters
     ----------
     list_of_index_and_parameter: list
     list_of_datasets: list
     dimension_names
```

### Comparing `pyxel_sim-2.1.1/pyxel/observation/parameter_values.py` & `pyxel_sim-2.2/pyxel/observation/parameter_values.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,25 +48,25 @@
         ] = None,
         enabled: bool = True,
         logarithmic: bool = False,
     ):
         # TODO: maybe use numpy to check multi-dimensional input lists
         # Check YAML input (not real values yet) and define parameter type
         if values == "_":
-            self.type: ParameterType = ParameterType("multi")
+            self.type: ParameterType = ParameterType.Multi
         elif isinstance(values, str) and "numpy" in values:
-            self.type = ParameterType("simple")
+            self.type = ParameterType.Simple
         elif isinstance(values, abc.Sequence) and any(
             [(el == "_" or isinstance(el, abc.Sequence)) for el in values]
         ):
-            self.type = ParameterType("multi")
+            self.type = ParameterType.Multi
         elif isinstance(values, abc.Sequence) and all(
             [isinstance(el, (Number, str)) for el in values]
         ):
-            self.type = ParameterType("simple")
+            self.type = ParameterType.Simple
         else:
             raise ValueError("Parameter values cannot be initiated with those values.")
 
         if "sampling.start_time" in key:
             key = "detector.sampling_properties.start_time"
 
         # unique identifier to the step. example: 'detector.geometry.row'
```

### Comparing `pyxel_sim-2.1.1/pyxel/options.py` & `pyxel_sim-2.2/pyxel/options.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/outputs/__init__.py` & `pyxel_sim-2.2/pyxel/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/outputs/calibration_outputs.py` & `pyxel_sim-2.2/pyxel/outputs/calibration_outputs.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/outputs/exposure_outputs.py` & `pyxel_sim-2.2/pyxel/outputs/exposure_outputs.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/outputs/observation_outputs.py` & `pyxel_sim-2.2/pyxel/outputs/observation_outputs.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/outputs/outputs.py` & `pyxel_sim-2.2/pyxel/outputs/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,43 +116,45 @@
 
     def __repr__(self):
         cls_name: str = self.__class__.__name__
 
         if self._current_output_folder is None:
             return f"{cls_name}<NO OUTPUT DIR>"
         else:
-            return f"{cls_name}<output_dir={self.current_output_folder!r}>"
+            return f"{cls_name}<output_dir='{self.current_output_folder!s}'>"
 
     @property
     def current_output_folder(self) -> Path:
         """Get directory where all outputs are saved."""
         if self._current_output_folder is None:
-            raise RuntimeError
+            raise RuntimeError("'current_output_folder' is not defined.")
 
         return self._current_output_folder
 
     @property
     def output_folder(self) -> Path:
         return self._output_folder
 
     @output_folder.setter
     def output_folder(self, folder: Union[str, Path]) -> None:
         if not isinstance(folder, (str, Path)):
-            raise TypeError
+            raise TypeError(
+                "Wrong type for parameter 'folder'. Expecting 'str' or 'Path'."
+            )
 
         self._output_folder = Path(folder)
 
     @property
     def custom_dir_name(self) -> str:
         return self._custom_dir_name
 
     @custom_dir_name.setter
     def custom_dir_name(self, name: str) -> None:
         if not isinstance(name, str):
-            raise TypeError
+            raise TypeError("Wrong type for parameter 'name'. Expecting 'str'.")
 
         self._custom_dir_name = name
 
     def create_output_folder(self) -> None:
         self._current_output_folder = create_output_directory(
             output_folder=self._output_folder,
             custom_dir_name=self._custom_dir_name,
```

### Comparing `pyxel_sim-2.1.1/pyxel/pipelines/__init__.py` & `pyxel_sim-2.2/pyxel/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/pipelines/model_function.py` & `pyxel_sim-2.2/pyxel/pipelines/model_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 import inspect
+import sys
 import warnings
 from collections.abc import Mapping, MutableMapping
 from typing import TYPE_CHECKING, Any, Callable, Optional
 
 from pyxel.evaluator import evaluate_reference
 
 if TYPE_CHECKING:
@@ -52,15 +53,15 @@
     >>> arguments["three"] = 3
     KeyError: 'No argument named three !'
     >>> arguments.three = 3
     AttributeError: 'No argument named three !'
     """
 
     def __init__(self, input_arguments: dict[str, Any]):
-        self._arguments: dict[str, Any] = input_arguments
+        self._arguments: dict[str, Any] = dict(input_arguments)
 
     def __setitem__(self, key, value):
         if key not in self._arguments:
             raise KeyError(f"No argument named {key} !")
 
         self._arguments[key] = value
 
@@ -108,15 +109,14 @@
 
     # def __deepcopy__(self, memo) -> "Arguments":
     #     """TBW."""
     #     return Arguments(deepcopy(self._arguments))
 
 
 # TODO: Improve this class. See issue #132.
-# TODO: Add unit tests #182
 class ModelFunction:
     """Create a wrapper function around a Model function.
 
     Parameters
     ----------
     func : str
         Full name of the model to use with this ModelFunction.
@@ -168,14 +168,15 @@
     def __init__(
         self,
         func: str,
         name: str,
         arguments: Optional[dict] = None,
         enabled: bool = True,
     ):
+        # TODO: Remove this !
         if inspect.isclass(func):
             raise AttributeError("Cannot pass a class to ModelFunction.")
 
         self._func_name: str = func
         self._func: Optional[Callable] = None
 
         self._name: str = name
@@ -206,15 +207,21 @@
         """TBW."""
         return self._arguments
 
     @property
     def func(self) -> Callable:
         """TBW."""
         if self._func is None:
-            self._func = evaluate_reference(self._func_name)
+            try:
+                self._func = evaluate_reference(self._func_name)
+            except Exception as exc:
+                if sys.version_info >= (3, 11):
+                    exc.add_note(f"Cannot retrieve function from {self._func_name!r}'")
+
+                raise
 
         if hasattr(self._func, "__deprecated__"):
             # This will be visible by the user
             msg = self._func.__deprecated__
             warnings.warn(msg, FutureWarning, stacklevel=2)
 
         return self._func
```

### Comparing `pyxel_sim-2.1.1/pyxel/pipelines/model_group.py` & `pyxel_sim-2.2/pyxel/pipelines/model_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 if TYPE_CHECKING:
     from pyxel.detectors import Detector
 
 
 # TODO: These methods could also be as a `abc.Sequence` with magical methods:
 #       __getitem__, __iter__, __len__, __contains__, ...
-#       See #181
 class ModelGroup:
     """Manage a collection of model functions.
 
     Parameters
     ----------
     models : Sequence of ``ModelFunction``
         Sequence of model functions belonging to the group.
```

### Comparing `pyxel_sim-2.1.1/pyxel/pipelines/pipeline.py` & `pyxel_sim-2.2/pyxel/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/pipelines/processor.py` & `pyxel_sim-2.2/pyxel/pipelines/processor.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/run.py` & `pyxel_sim-2.2/pyxel/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     from pyxel.outputs import CalibrationOutputs, ExposureOutputs, ObservationOutputs
 
 
 def exposure_mode(
     exposure: "Exposure",
     detector: Detector,
     pipeline: "DetectionPipeline",
-) -> "xr.Dataset":
+) -> "xr.Dataset":  # pragma: no cover
     """Run an 'exposure' pipeline.
 
     .. deprecated:: 1.14
         `exposure_mode` will be removed in pyxel 2.0.0, it is replaced by `pyxel.run_mode`.
 
     For more information, see :ref:`exposure_mode`.
 
@@ -189,15 +189,15 @@
     return result
 
 
 def observation_mode(
     observation: "Observation",
     detector: Detector,
     pipeline: "DetectionPipeline",
-) -> "ObservationResult":
+) -> "ObservationResult":  # pragma: no cover
     """Run an 'observation' pipeline.
 
     .. deprecated:: 1.14
         `observation_mode` will be removed in pyxel 2.0.0, it is replaced by `pyxel.run_mode`.
 
     For more information, see :ref:`observation_mode`.
 
@@ -258,15 +258,15 @@
 
 
 def calibration_mode(
     calibration: "Calibration",
     detector: Detector,
     pipeline: "DetectionPipeline",
     compute_and_save: bool = True,
-) -> tuple["xr.Dataset", pd.DataFrame, pd.DataFrame, Sequence]:
+) -> tuple["xr.Dataset", pd.DataFrame, pd.DataFrame, Sequence]:  # pragma: no cover
     """Run a 'calibration' pipeline.
 
     .. deprecated:: 1.14
         `calibration_mode` will be removed in pyxel 2.0.0, it is replaced by `pyxel.run_mode`.
 
     For more information, see :ref:`calibration_mode`.
```

### Comparing `pyxel_sim-2.1.1/pyxel/show_versions.py` & `pyxel_sim-2.2/pyxel/show_versions.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/static/pyxel_schema.json` & `pyxel_sim-2.2/pyxel/static/pyxel_schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999641891272%*

 * *Differences: {"'definitions'": "{'ModelChargeGenerationSimpleDarkCurrent': {'properties': {'arguments': "*

 * *                  "{'properties': {'dark_rate': {'description': 'Dark current, in e⁻/pixel/second, "*

 * *                  "which is the way manufacturers typically report it.'}}}}}}"}*

```diff
@@ -3587,15 +3587,15 @@
             "additionalProperties": false,
             "description": "Simulate dark current in a detector.",
             "properties": {
                 "arguments": {
                     "additionalProperties": false,
                     "properties": {
                         "dark_rate": {
-                            "description": "Dark current, in electrons/pixel/second, which is the way manufacturers typically report it.",
+                            "description": "Dark current, in e\u207b/pixel/second, which is the way manufacturers typically report it.",
                             "title": "dark_rate",
                             "type": "number"
                         },
                         "seed": {
                             "default": null,
                             "title": "seed",
                             "type": [
```

### Comparing `pyxel_sim-2.1.1/pyxel/templates/_TEMPLATE.py` & `pyxel_sim-2.2/pyxel/templates/_TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/__init__.py` & `pyxel_sim-2.2/pyxel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/add_model.py` & `pyxel_sim-2.2/pyxel/util/add_model.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/caching.py` & `pyxel_sim-2.2/pyxel/util/caching.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/examples.py` & `pyxel_sim-2.2/pyxel/util/examples.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/image.py` & `pyxel_sim-2.2/pyxel/util/image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/materials.py` & `pyxel_sim-2.2/pyxel/util/materials.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/memory.py` & `pyxel_sim-2.2/pyxel/util/memory.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/misc.py` & `pyxel_sim-2.2/pyxel/util/misc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/randomize.py` & `pyxel_sim-2.2/pyxel/util/randomize.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel/util/timing.py` & `pyxel_sim-2.2/pyxel/util/timing.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-2.1.1/pyxel_sim.egg-info/PKG-INFO` & `pyxel_sim-2.2/pyxel_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel_sim
-Version: 2.1.1
+Version: 2.2
 Summary: Pyxel detector simulation framework.
 Author-email: The Pyxel development team <pyxel@esa.int>
 License: MIT
 Project-URL: homepage, https://esa.gitlab.io/pyxel/
 Project-URL: documentation, https://esa.gitlab.io/pyxel/doc/
 Project-URL: repository, https://gitlab.com/esa/pyxel
 Project-URL: changelog, https://gitlab.com/esa/pyxel/-/releases
```

### Comparing `pyxel_sim-2.1.1/pyxel_sim.egg-info/SOURCES.txt` & `pyxel_sim-2.2/pyxel_sim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,18 @@
 pyxel/models/charge_generation/__init__.py
 pyxel/models/charge_generation/apd_gain.py
 pyxel/models/charge_generation/charge_deposition.py
 pyxel/models/charge_generation/charge_injection.py
 pyxel/models/charge_generation/dark_current.py
 pyxel/models/charge_generation/dark_current_induced.py
 pyxel/models/charge_generation/dark_current_rule07.py
+pyxel/models/charge_generation/dark_current_saphira.py
 pyxel/models/charge_generation/load_charge.py
 pyxel/models/charge_generation/photoelectrons.py
+pyxel/models/charge_generation/simple_dark_current.py
 pyxel/models/charge_generation/wavelength_qe.py
 pyxel/models/charge_generation/cosmix/__init__.py
 pyxel/models/charge_generation/cosmix/cosmix.py
 pyxel/models/charge_generation/cosmix/particle.py
 pyxel/models/charge_generation/cosmix/plotting.py
 pyxel/models/charge_generation/cosmix/simulation.py
 pyxel/models/charge_generation/cosmix/util.py
```

### Comparing `pyxel_sim-2.1.1/tests/test_options.py` & `pyxel_sim-2.2/tests/test_options.py`

 * *Files identical despite different names*

