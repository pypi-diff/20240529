# Comparing `tmp/srlife-2.0.0.tar.gz` & `tmp/srlife-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srlife-2.0.0.tar", last modified: Tue Oct 11 18:59:35 2022, max compression
+gzip compressed data, was "srlife-2.0.1.tar", last modified: Wed May 29 15:14:42 2024, max compression
```

## Comparing `srlife-2.0.0.tar` & `srlife-2.0.1.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.586280 srlife-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-10-11 18:58:46.000000 srlife-2.0.0/ACKNOWLEDGEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-10-11 18:58:46.000000 srlife-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-10-11 18:58:46.000000 srlife-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-11 18:59:35.586280 srlife-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-10-11 18:58:46.000000 srlife-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-10-11 18:58:46.000000 srlife-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-11 18:59:35.590280 srlife-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-10-11 18:58:46.000000 srlife-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.578280 srlife-2.0.0/srlife/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31500 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/damage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.574280 srlife-2.0.0/srlife/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.578280 srlife-2.0.0/srlife/data/damage/
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/damage/316H.xml
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/damage/740H.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/damage/800H.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/damage/A230.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/damage/A282.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/damage/A617.xml
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/damage/SiC.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.578280 srlife-2.0.0/srlife/data/deformation/
--rw-r--r--   0 runner    (1001) docker     (121)    22101 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/deformation/316H.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5426 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/deformation/740H.xml
--rw-r--r--   0 runner    (1001) docker     (121)    22107 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/deformation/800H.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/deformation/A230.xml
--rw-r--r--   0 runner    (1001) docker     (121)     7167 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/deformation/A282.xml
--rw-r--r--   0 runner    (1001) docker     (121)    22130 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/deformation/A617.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/deformation/SiC.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.578280 srlife-2.0.0/srlife/data/fluid/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/fluid/salt.xml
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/fluid/salt_SiC.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.578280 srlife-2.0.0/srlife/data/thermal/
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermal/316H.xml
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermal/740H.xml
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermal/800H.xml
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermal/A230.xml
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermal/A282.xml
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermal/A617.xml
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermal/SiC.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.578280 srlife-2.0.0/srlife/data/thermalfluid/
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermalfluid/32MgCl2-68KCl.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/data/thermalfluid/sCO2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3317 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3724 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/library.py
--rw-r--r--   0 runner    (1001) docker     (121)     9078 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/managers.py
--rw-r--r--   0 runner    (1001) docker     (121)    21766 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/materials.py
--rw-r--r--   0 runner    (1001) docker     (121)    45081 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/receiver.py
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/solverparams.py
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)    14482 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/spring.py
--rw-r--r--   0 runner    (1001) docker     (121)    39939 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/structural.py
--rw-r--r--   0 runner    (1001) docker     (121)     5940 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/system.py
--rw-r--r--   0 runner    (1001) docker     (121)    46984 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/thermal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.578280 srlife-2.0.0/srlife/thermohydraulics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/thermohydraulics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13809 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/thermohydraulics/flowpath.py
--rw-r--r--   0 runner    (1001) docker     (121)     7157 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/thermohydraulics/thermalfluid.py
--rw-r--r--   0 runner    (1001) docker     (121)     5271 2022-10-11 18:58:46.000000 srlife-2.0.0/srlife/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.578280 srlife-2.0.0/srlife.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-11 18:59:35.000000 srlife-2.0.0/srlife.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-10-11 18:59:35.000000 srlife-2.0.0/srlife.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 18:59:35.000000 srlife-2.0.0/srlife.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-11 18:59:35.000000 srlife-2.0.0/srlife.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-11 18:59:35.000000 srlife-2.0.0/srlife.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 18:59:35.000000 srlife-2.0.0/srlife.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.582280 srlife-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-10-11 18:58:46.000000 srlife-2.0.0/test/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.582280 srlife-2.0.0/test/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.582280 srlife-2.0.0/test/solvers/spring/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/spring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5422 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/spring/altsolver.py
--rw-r--r--   0 runner    (1001) docker     (121)    12321 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/spring/test_random_networks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3934 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/spring/test_spring.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.582280 srlife-2.0.0/test/solvers/thermal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/thermal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3354 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/thermal/run_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)    14491 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/thermal/test_thermal.py
--rw-r--r--   0 runner    (1001) docker     (121)     6738 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/thermal/thermalsol.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      939 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/thermal/time_1d.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1042 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/thermal/time_2d.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1072 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/thermal/time_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.582280 srlife-2.0.0/test/solvers/tube/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.586280 srlife-2.0.0/test/solvers/tube/moose-verification/
--rw-r--r--   0 runner    (1001) docker     (121)     8135 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/1d.i
--rw-r--r--   0 runner    (1001) docker     (121)   156644 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/1d_out.e
--rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/2d.i
--rw-r--r--   0 runner    (1001) docker     (121)   706960 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/2d_out.e
--rw-r--r--   0 runner    (1001) docker     (121)     8487 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/3d.i
--rw-r--r--   0 runner    (1001) docker     (121)  3260332 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/3d_out.e
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.586280 srlife-2.0.0/test/solvers/tube/moose-verification/meshes/
--rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/meshes/1d.e
--rw-r--r--   0 runner    (1001) docker     (121)    14028 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/meshes/2d.e
--rw-r--r--   0 runner    (1001) docker     (121)    99988 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/meshes/3d.e
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/moose-verification/model.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)     7568 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/run_structural_tube_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)     6233 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/test_structural_tube.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2319 2022-10-11 18:58:46.000000 srlife-2.0.0/test/solvers/tube/time.py
--rw-r--r--   0 runner    (1001) docker     (121)    21697 2022-10-11 18:58:46.000000 srlife-2.0.0/test/test_ceramic_damage.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-10-11 18:58:46.000000 srlife-2.0.0/test/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-10-11 18:58:46.000000 srlife-2.0.0/test/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (121)     9337 2022-10-11 18:58:46.000000 srlife-2.0.0/test/test_materials.py
--rw-r--r--   0 runner    (1001) docker     (121)     6840 2022-10-11 18:58:46.000000 srlife-2.0.0/test/test_receiver_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-10-11 18:58:46.000000 srlife-2.0.0/test/test_volume_calculation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-10-11 18:58:46.000000 srlife-2.0.0/test/test_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:59:35.586280 srlife-2.0.0/test/thermohydraulics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:58:46.000000 srlife-2.0.0/test/thermohydraulics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4797 2022-10-11 18:58:46.000000 srlife-2.0.0/test/thermohydraulics/test_flowpath.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-10-11 18:58:46.000000 srlife-2.0.0/test/thermohydraulics/test_thermalfluid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.029819 srlife-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 15:14:04.000000 srlife-2.0.1/ACKNOWLEDGEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 15:14:04.000000 srlife-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 15:14:04.000000 srlife-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-29 15:14:42.029819 srlife-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-29 15:14:04.000000 srlife-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 15:14:04.000000 srlife-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 15:14:42.029819 srlife-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-29 15:14:04.000000 srlife-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.017819 srlife-2.0.1/srlife/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45522 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/damage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.013818 srlife-2.0.1/srlife/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.017819 srlife-2.0.1/srlife/data/damage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/damage/316H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/damage/740H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/damage/800H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/damage/A230.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/damage/A282.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/damage/A617.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/damage/SiC.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.017819 srlife-2.0.1/srlife/data/deformation/
+-rw-r--r--   0 runner    (1001) docker     (127)    22101 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/deformation/316H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/deformation/740H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22107 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/deformation/800H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/deformation/A230.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/deformation/A282.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/deformation/A617.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/deformation/SiC.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.017819 srlife-2.0.1/srlife/data/fluid/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/fluid/salt.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/fluid/salt_SiC.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.021818 srlife-2.0.1/srlife/data/thermal/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermal/316H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermal/740H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermal/800H.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermal/A230.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermal/A282.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermal/A617.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermal/SiC.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.021818 srlife-2.0.1/srlife/data/thermalfluid/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermalfluid/32MgCl2-68KCl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/data/thermalfluid/sCO2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23543 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45081 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/solverparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/spring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39939 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/structural.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46984 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/thermal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.021818 srlife-2.0.1/srlife/thermohydraulics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/thermohydraulics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/thermohydraulics/flowpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/thermohydraulics/thermalfluid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-29 15:14:04.000000 srlife-2.0.1/srlife/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.017819 srlife-2.0.1/srlife.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-29 15:14:41.000000 srlife-2.0.1/srlife.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-29 15:14:41.000000 srlife-2.0.1/srlife.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:14:41.000000 srlife-2.0.1/srlife.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 15:14:41.000000 srlife-2.0.1/srlife.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 15:14:41.000000 srlife-2.0.1/srlife.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:14:41.000000 srlife-2.0.1/srlife.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.021818 srlife-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-29 15:14:04.000000 srlife-2.0.1/test/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.021818 srlife-2.0.1/test/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.021818 srlife-2.0.1/test/solvers/spring/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/spring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/spring/altsolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/spring/test_random_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/spring/test_spring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.021818 srlife-2.0.1/test/solvers/thermal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/thermal/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3354 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/thermal/run_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/thermal/test_thermal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/thermal/thermalsol.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      939 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/thermal/time_1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1042 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/thermal/time_2d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1072 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/thermal/time_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.025819 srlife-2.0.1/test/solvers/tube/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.029819 srlife-2.0.1/test/solvers/tube/moose-verification/
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/1d.i
+-rw-r--r--   0 runner    (1001) docker     (127)   156644 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/1d_out.e
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/2d.i
+-rw-r--r--   0 runner    (1001) docker     (127)   706960 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/2d_out.e
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/3d.i
+-rw-r--r--   0 runner    (1001) docker     (127)  3260332 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/3d_out.e
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.029819 srlife-2.0.1/test/solvers/tube/moose-verification/meshes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/meshes/1d.e
+-rw-r--r--   0 runner    (1001) docker     (127)    14028 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/meshes/2d.e
+-rw-r--r--   0 runner    (1001) docker     (127)    99988 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/meshes/3d.e
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/moose-verification/model.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7568 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/run_structural_tube_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/test_structural_tube.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-05-29 15:14:04.000000 srlife-2.0.1/test/solvers/tube/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20147 2024-05-29 15:14:04.000000 srlife-2.0.1/test/test_ceramic_damage_CARES_cyclic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-05-29 15:14:04.000000 srlife-2.0.1/test/test_ceramic_damage_CARES_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-29 15:14:04.000000 srlife-2.0.1/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-29 15:14:04.000000 srlife-2.0.1/test/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-29 15:14:04.000000 srlife-2.0.1/test/test_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-29 15:14:04.000000 srlife-2.0.1/test/test_receiver_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-29 15:14:04.000000 srlife-2.0.1/test/test_volume_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-29 15:14:04.000000 srlife-2.0.1/test/test_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:42.029819 srlife-2.0.1/test/thermohydraulics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:04.000000 srlife-2.0.1/test/thermohydraulics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-29 15:14:04.000000 srlife-2.0.1/test/thermohydraulics/test_flowpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-29 15:14:04.000000 srlife-2.0.1/test/thermohydraulics/test_thermalfluid.py
```

### Comparing `srlife-2.0.0/LICENSE` & `srlife-2.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 UChicago Argonne, LLC
+Copyright 2024 UChicago Argonne, LLC
 
 All Rights Reserved
 
 Software Name: srlife
 
 By: Argonne National Laboratory
```

### Comparing `srlife-2.0.0/PKG-INFO` & `srlife-2.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: srlife
-Version: 2.0.0
+Version: 2.0.1
 Summary: Evaluate the structural life of a solar receiver
 Home-page: https://github.com/Argonne-National-Laboratory/srlife
 Author: Argonne National Laboratory
 Author-email: messner@anl.gov
-License: UNKNOWN
-Description: # srlife: solar receiver life estimation tool
-        
-        ![Test Status](https://github.com/Argonne-National-Laboratory/srlife/workflows/tests/badge.svg?branch=master) ![Documentation Status](https://readthedocs.org/projects/srlife/badge/?version=latest)
-        
-        This python package evaluates the structural life of tubular solar receivers against
-        creep rupture, fatigue, and creep-fatigue damage modes.
-        
-        Full documentation is available [here](https://srlife.readthedocs.io/).
-        
-        ## Prerequisites
-        
-        The package itself is pure python, however it relies on several additional
-        python packages listed in [requirements.txt](requirements.txt).
-        Note that srlife uses Python3.
-        
-        ## License
-        
-        The package is provided under an MIT license found in the
-        [LICENSE](LICENSE) file.
-        
 Keywords: materials structures modeling
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# srlife: solar receiver life estimation tool
+
+![Test Status](https://github.com/Argonne-National-Laboratory/srlife/workflows/tests/badge.svg?branch=master) ![Documentation Status](https://readthedocs.org/projects/srlife/badge/?version=latest)
+
+This python package evaluates the structural life of tubular solar receivers against
+creep rupture, fatigue, and creep-fatigue damage modes.
+
+Full documentation is available [here](https://srlife.readthedocs.io/).
+
+## Prerequisites
+
+The package itself is pure python, however it relies on several additional
+python packages listed in [requirements.txt](requirements.txt).
+Note that srlife uses Python3.
+
+## License
+
+The package is provided under an MIT license found in the
+[LICENSE](LICENSE) file.
```

### Comparing `srlife-2.0.0/README.md` & `srlife-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/setup.py` & `srlife-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open(os.path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
   long_description = f.read()
 
 setup (
     # Name of the project
     name = 'srlife',
     # Version
-    version = '2.0.0',
+    version = '2.0.1',
     # One line-description
     description = "Evaluate the structural life of a solar receiver",
     # README
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     # Project webpage
     url='https://github.com/Argonne-National-Laboratory/srlife',
```

### Comparing `srlife-2.0.0/srlife/damage.py` & `srlife-2.0.1/srlife/damage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # pylint: disable=no-member
 """
   This module contains methods for calculating the reliability and
   creep-fatigue damage given completely-solved tube results and
   damage material properties
 """
-
 import numpy as np
 import numpy.linalg as la
 import scipy.optimize as opt
 import multiprocess
 
 
 class WeibullFailureModel:
@@ -16,22 +15,25 @@
 
     Determines principal stresses from mandel stress
 
     Determines tube reliability and overall reliability by taking input of
     element log reliabilities from respective Weibull failure model
     """
 
+    tolerance = 1.0e-16
+
     def __init__(self, pset, *args, cares_cutoff=True):
         """Initialize the Weibull Failure Model
 
         Boolean:
         cares_cutoff:    condition for forcing reliability as unity in case of
                         high compressive stresses
         """
         self.cares_cutoff = cares_cutoff
+        self.shear_sensitive = pset.get_default("shear_sensitive", True)
 
     def calculate_principal_stress(self, stress):
         """
         Calculate the principal stresses from Mandel vector and converts
         to conventional notation
         """
         if stress.ndim == 2:
@@ -55,62 +57,84 @@
         mults = [1.0, 1.0, 1.0, np.sqrt(2), np.sqrt(2), np.sqrt(2)]
 
         # Converting mandel notation to conventional notation
         for i, (grp, m) in enumerate(zip(inds, mults)):
             for a, b in grp:
                 tensor[..., a, b] = stress[..., i] / m
 
-        return la.eigvalsh(tensor)
+        # return la.eigvalsh(tensor)
+        pstress = la.eigvalsh(tensor)
+
+        if self.cares_cutoff:
+            pmax = np.max(pstress, axis=2)
+            pmin = np.min(pstress, axis=2)
+            remove = np.abs(pmin / (pmax + self.tolerance)) > 3.0
+            pstress[remove] = 0.0
+
+        return pstress
 
     def determine_reliability(
-        self, receiver, material, nthreads=1, decorator=lambda x, n: x
+        self, receiver, material, time, nthreads=1, decorator=lambda x, n: x
     ):
         """
         Determine the reliability of the tubes in the receiver by calculating individual
         material point reliabilities and finding the minimum of all points.
 
         Parameters:
           receiver        fully-solved receiver object
           material        material model to use
+          time (float):   time in service
 
         Additional Parameters:
           nthreads        number of threads
           decorator       progress bar
         """
         with multiprocess.Pool(nthreads) as p:
             results = list(
                 decorator(
                     p.imap(
-                        lambda x: self.tube_log_reliability(x, material, receiver),
+                        lambda x: self.tube_log_reliability(
+                            x, material, receiver, time
+                        ),
                         receiver.tubes,
                     ),
                     receiver.ntubes,
                 )
             )
 
         p_tube = np.array([res[0] for res in results])
         tube_fields = [res[1] for res in results]
 
         # Tube reliability is the minimum of all the time steps
         tube = np.min(p_tube, axis=1)
 
-        # Overall reliability is the minimum of the sum
-        overall = np.min(np.sum(p_tube, axis=0))
+        # Panel reliability
+        tube_multipliers = np.array(
+            [
+                [t.multiplier_val for (ti, t) in p.tubes.items()]
+                for (pi, p) in receiver.panels.items()
+            ]
+        )
+        panel = np.sum(tube.reshape(receiver.npanels, -1) * tube_multipliers, axis=1)
+
+        # Overall reliability
+        overall = np.sum(panel)
 
         # Add the field to the tubes
         for tubei, field in zip(receiver.tubes, tube_fields):
             tubei.add_quadrature_results("log_reliability", field)
 
         # Convert back from log-prob as we go
         return {
             "tube_reliability": np.exp(tube),
+            "panel_reliability": np.exp(panel),
             "overall_reliability": np.exp(overall),
         }
 
-    def tube_log_reliability(self, tube, material, receiver):
+    def tube_log_reliability(self, tube, material, receiver, time):
         """
         Calculate the log reliability of a single tube
         """
         volumes = tube.element_volumes()
 
         stresses = np.transpose(
             np.mean(
@@ -127,30 +151,31 @@
                 axis=-1,
             ),
             axes=(1, 2, 0),
         )
 
         temperatures = np.mean(tube.quadrature_results["temperature"], axis=-1)
 
+        # Figure out the number of repetitions of the load cycle
+        if receiver.days != 1:
+            raise RuntimeError(
+                "Time dependent reliability requires the load cycle"
+                "be a single, representative cycle"
+            )
+
         # Do it this way so we can vectorize
         inc_prob = self.calculate_element_log_reliability(
-            stresses, temperatures, volumes, material
+            tube.times, stresses, temperatures, volumes, material, time
         )
 
-        # CARES/LIFE cutoff
-        if self.cares_cutoff:
-            pstress = self.calculate_principal_stress(stresses).reshape(-1, 3)
-            pmax = np.max(pstress, axis=1)
-            pmin = np.min(pstress, axis=1)
-            remove = np.abs(pmin / (pmax + 1.0e-16)) > 3.0
-            mod_prob = inc_prob.flatten()
-            mod_prob[remove] = 0.0
-            inc_prob = mod_prob.reshape(inc_prob.shape)
-
         # Return the sums as a function of time along with the field itself
+        inc_prob = np.array(list(inc_prob) * len(tube.times)).reshape(
+            len(tube.times), -1
+        )
+
         return np.sum(inc_prob, axis=1), np.transpose(
             np.stack((inc_prob, inc_prob)), axes=(1, 2, 0)
         )
 
 
 class CrackShapeIndependent(WeibullFailureModel):
     """
@@ -282,222 +307,361 @@
         # Normal stress
         sigma_n = self.calculate_normal_stress(mandel_stress)
 
         # Total stress
         sigma = self.calculate_total_stress(mandel_stress)
 
         # Shear stress
-        with np.errstate(invalid="ignore"):
-            return np.sqrt(sigma**2 - sigma_n**2)
+        return np.sqrt(sigma**2 - sigma_n**2)
 
     def calculate_flattened_eq_stress(
-        self, mandel_stress, temperatures, material, A, dalpha, dbeta
+        self,
+        time,
+        mandel_stress,
+        temperatures,
+        material,
+        tot_time,
+        A,
+        dalpha,
+        dbeta,
     ):
         """
         Calculate the integral of equivalent stresses given the material
         properties and integration limits
 
         Parameters:
+          time:           time instance variable for each stress/temperature
           mandel_stress:  element stresses in Mandel convention
           temperatures:   element temperatures
-          material        material model to use
+          material:       material model object with required data that includes
+                          Weibull scale parameter (svals) and Weibull modulus (mvals)
+                          and fatigue parameters Bv and Nv
+          tot_time:       total service time used as input to calculate reliability
 
         Additional Parameters:
           A:              mesh grid of vectorized angle values
           dalpha:         increment of angle alpha to be used in evaluating integral
           dbeta:          increment of angle beta to be used in evaluating integral
         """
+
+        # Material parameters
         self.temperatures = temperatures
         self.material = material
         self.mandel_stress = mandel_stress
-        self.mvals = self.material.modulus(temperatures)
-
-        # Principal stresses
-        pstress = self.calculate_principal_stress(mandel_stress)
+        self.mvals = material.modulus(temperatures)
+        Nv = material.Nv(temperatures)
+        Bv = material.Bv(temperatures)
+
+        # Temperature average values
+        mavg = np.mean(self.mvals, axis=0)
+        Nvavg = np.mean(Nv, axis=0)
+        Bvavg = np.mean(Bv, axis=0)
 
         # Projected equivalent stresses
         sigma_e = self.calculate_eq_stress(
             mandel_stress, self.temperatures, self.material
         )
 
-        # Suppressing warning given when negative numbers are raised to rational numbers
-        with np.errstate(invalid="ignore"):
-            # Defining area integral element wise
-            integral = (
-                (sigma_e ** self.mvals[..., None, None])
-                * np.sin(self.A)
-                * self.dalpha
-                * self.dbeta
+        # Max principal stresss over all time steps for each element
+        sigma_e_max = np.max(sigma_e, axis=0)
+
+        # Calculating ratio of cyclic stress to max cyclic stress (in one cycle)
+        # for time-independent and time-dependent cases
+        if np.all(time == 0):
+            sigma_e_0 = sigma_e
+        else:
+            sigma_e[sigma_e < 0] = 0
+            g = (
+                np.trapz(
+                    (sigma_e / (sigma_e_max + self.tolerance))
+                    ** Nvavg[..., None, None],
+                    time,
+                    axis=0,
+                )
+                / time[-1]
             )
 
+            # Time dependent equivalent stress
+            sigma_e_0 = (
+                (
+                    ((sigma_e_max ** Nvavg[..., None, None]) * g * tot_time)
+                    / Bvavg[..., None, None]
+                )
+                + (sigma_e_max ** (Nvavg[..., None, None] - 2))
+            ) ** (1 / (Nvavg[..., None, None] - 2))
+
+        # Defining area integral element wise
+        integral = (
+            (sigma_e_0 ** mavg[..., None, None])
+            * np.sin(self.A)
+            * self.dalpha
+            * self.dbeta
+        )
+
         # Flatten the last axis and calculate the mean of the positive values along that axis
-        if pstress.ndim == 2:
-            flat = integral.reshape(
-                integral.shape[:1] + (-1,)
-            )  # when no time steps involved
-        elif pstress.ndim == 3:
-            flat = integral.reshape(
-                integral.shape[:2] + (-1,)
-            )  # when time steps involved
-
-        # Suppressing warning to ignoring initial NaN values
-        with np.errstate(invalid="ignore"):
-            # Summing over area integral elements ignoring NaN values
-            flat = np.nansum(flat, axis=-1)
+        flat = integral.reshape(integral.shape[:-2] + (-1,))
 
+        # Summing over area integral elements ignoring NaN values
+        flat = np.nansum(flat, axis=-1)
         return flat
 
     def calculate_element_log_reliability(
-        self, mandel_stress, temperatures, volumes, material
+        self, time, mandel_stress, temperatures, volumes, material, tot_time
     ):
         """
         Calculate the element log reliability given the equivalent stress
 
         Parameters:
-          mandel_stress:  element stresses in Mandel convention
-          temperatures:   element temperatures
-          volumes:        element volumes
-          material:       material model  object with required data
+          mandel_stress:    element stresses in Mandel convention
+          temperatures:     element temperatures
+          volumes:          element volumes
+          material:         material model object with required data that includes
+                            Weibull scale parameter (svals), Weibull modulus (mvals)
+                            and uniaxial and polyaxial crack density coefficient (kvals,kpvals)
+          shear_sensitive:  shear sensitivity condition for evaluating normalized
+                            crack density coefficient (kbar) using a
+                            numerically (when True) or using a fixed expression (when False)
         """
         self.temperatures = temperatures
         self.material = material
         self.mandel_stress = mandel_stress
 
         # Material parameters
-        self.svals = self.material.strength(temperatures)
-        self.mvals = self.material.modulus(temperatures)
-        self.kvals = self.svals ** (-self.mvals)
-        self.kpvals = (2 * self.mvals + 1) * self.kvals
+        svals = material.strength(temperatures)
+        mvals = material.modulus(temperatures)
+        kvals = svals ** (-mvals)
+
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+        kavg = np.mean(kvals, axis=0)
+
+        # shear_sensitive = True
+
+        if self.shear_sensitive is True:
+            kbar = self.calculate_kbar(
+                self.temperatures, self.material, self.A, self.dalpha, self.dbeta
+            )
+        else:
+            kbar = 2 * mavg + 1
+
+        kpvals = kbar * kavg
 
         # Equivalent stress raied to exponent mv
         flat = (
             self.calculate_flattened_eq_stress(
+                time,
                 mandel_stress,
                 self.temperatures,
                 self.material,
+                tot_time,
                 self.A,
                 self.dalpha,
                 self.dbeta,
             )
-        ) ** (1 / self.mvals)
+        ) ** (1 / mavg)
 
-        return -(2 * self.kpvals / np.pi) * (flat**self.mvals) * volumes
+        return -(2 * kpvals / np.pi) * (flat**mavg) * volumes
 
 
 class PIAModel(CrackShapeIndependent):
     """
     Principal of independent action failure model
 
     Calculates reliability using only tensile stresses
     that are assumed to act independently on cracks
     """
 
     def calculate_element_log_reliability(
-        self, mandel_stress, temperatures, volumes, material
+        self, time, mandel_stress, temperatures, volumes, material, tot_time
     ):
         """
         Calculate the element log reliability
 
         Parameters:
+          time:           time instance variable for each stress/temperature
           mandel_stress:  element stresses in Mandel convention
           temperatures:   element temperatures
           volumes:        element volumes
           material:       material model object with required data that includes
-                          Weibull scale parameter (svals) and Weibull modulus (mvals)
+                          Weibull scale parameter (svals), Weibull modulus (mvals)
+                          and fatigue parameters (Bv,Nv)
+          tot_time:       total service time used as input to calculate reliability
         """
+
+        # Principal stresses
+        pstress = self.calculate_principal_stress(mandel_stress)
+
         # Material parameters
         svals = material.strength(temperatures)
         mvals = material.modulus(temperatures)
         kvals = svals ** (-mvals)
+        Nv = material.Nv(temperatures)
+        Bv = material.Bv(temperatures)
 
-        # Principal stresses
-        pstress = self.calculate_principal_stress(mandel_stress)
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+        kavg = np.mean(kvals, axis=0)
+        Nvavg = np.mean(Nv, axis=0)
+        Bvavg = np.mean(Bv, axis=0)
 
         # Only tension
         pstress[pstress < 0] = 0
 
-        return -kvals * np.sum(pstress ** mvals[..., None], axis=-1) * volumes
+        # Max principal stresss over all time steps for each element
+        pstress_max = np.max(pstress, axis=0)
+
+        # Calculating ratio of cyclic stress to max cyclic stress (in one cycle)
+        # for time-independent and time-dependent cases
+        if np.all(time == 0):
+            pstress_0 = pstress
+        else:
+            g = (
+                np.trapz(
+                    (pstress / (pstress_max + 1.0e-14)) ** Nvavg[..., None],
+                    time,
+                    axis=0,
+                )
+                / time[-1]
+            )
+
+            # Time dependent principal stress
+            pstress_0 = (
+                (pstress_max ** Nvavg[..., None] * g * tot_time) / Bvavg[..., None]
+                + (pstress_max ** (Nvavg[..., None] - 2))
+            ) ** (1 / (Nvavg[..., None] - 2))
+
+        return -kavg * np.sum(pstress_0 ** mavg[..., None], axis=-1) * volumes
 
 
 class WNTSAModel(CrackShapeIndependent):
     """
     Weibull normal tensile average failure model
 
     Evaluates an average normal tensile stress (acting on the cracks) integrated over the
     area of a sphere, and uses it to calculate the element reliability
     """
 
-    def calculate_avg_normal_stress(self, mandel_stress, temperatures, material):
+    def calculate_avg_normal_stress(
+        self, time, mandel_stress, temperatures, material, tot_time
+    ):
         """
         Calculate the average normal tensile stresses from the pricipal stresses
 
         Parameters:
           mandel_stress:  element stresses in Mandel convention
           temperatures:   element temperatures
-          material:       material model object with required data
+          material:       material model object with required data that includes
+                          Weibull scale parameter (svals), Weibull modulus (mvals)
+                          and fatigue parameters (Bv,Nv)
+          tot_time:       total service time used as input to calculate reliability
         """
+
         # Material parameters
+        self.temperatures = temperatures
+        self.material = material
+        self.mandel_stress = mandel_stress
+
         mvals = material.modulus(temperatures)
+        Nv = material.Nv(temperatures)
+        Bv = material.Bv(temperatures)
 
-        # Principal stresses
-        pstress = self.calculate_principal_stress(mandel_stress)
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+        Nvavg = np.mean(Nv, axis=0)
+        Bvavg = np.mean(Bv, axis=0)
 
-        # Normal stress
+        # Time dependent Normal stress
         sigma_n = self.calculate_normal_stress(mandel_stress)
 
-        # Area integral; suppressing warning given when negative numbers are raised
-        # to rational numbers
-        with np.errstate(invalid="ignore"):
-            integral = (
-                (sigma_n ** mvals[..., None, None])
-                * np.sin(self.A)
-                * self.dalpha
-                * self.dbeta
-            ) / (4 * np.pi)
+        # Considering only tensile stresses
+        sigma_n[sigma_n < 0] = 0
+
+        # Max normal stresss over all time steps for each element
+        sigma_n_max = np.max(sigma_n, axis=0)
+
+        # Calculating ratio of cyclic stress to max cyclic stress (in one cycle)
+        # for time-independent and time-dependent cases
+        if np.all(time == 0):
+            sigma_n_0 = sigma_n
+        else:
+            g = (
+                np.trapz(
+                    (sigma_n / (sigma_n_max + self.tolerance))
+                    ** Nvavg[..., None, None],
+                    time,
+                    axis=0,
+                )
+                / time[-1]
+            )
+
+            # Time dependent equivalent stress
+            sigma_n_0 = (
+                (
+                    ((sigma_n_max ** Nvavg[..., None, None]) * g * tot_time)
+                    / Bvavg[..., None, None]
+                )
+                + (sigma_n_max ** (Nvavg[..., None, None] - 2))
+            ) ** (1 / (Nvavg[..., None, None] - 2))
+
+        integral = (
+            (sigma_n_0 ** mavg[..., None, None])
+            * np.sin(self.A)
+            * self.dalpha
+            * self.dbeta
+        ) / (4 * np.pi)
 
         # Flatten the last axis and calculate the mean of the positive values along that axis
-        if pstress.ndim == 2:
-            flat = integral.reshape(
-                integral.shape[:1] + (-1,)
-            )  # when no time steps involved
-        elif pstress.ndim == 3:
-            flat = integral.reshape(
-                integral.shape[:2] + (-1,)
-            )  # when time steps involved
-
-        # Suppressing warning to ignoring initial NaN values
-        with np.errstate(invalid="ignore"):
-            # Average stress
-            return np.nansum(np.where(flat >= 0.0, flat, np.nan), axis=-1)
+        flat = integral.reshape(integral.shape[:-2] + (-1,))
+
+        # Average stress from summing while ignoring NaN values
+        return np.nansum(np.where(flat >= 0.0, flat, np.nan), axis=-1)
 
     def calculate_element_log_reliability(
-        self, mandel_stress, temperatures, volumes, material
+        self, time, mandel_stress, temperatures, volumes, material, tot_time
     ):
         """
         Calculate the element log reliability
 
         Parameters:
-          mandel_stress:  element stresses in Mandel convention
-          temperatures:   element temperatures
-          volumes:        element volumes
-          material:       material model  object with required data
+          mandel_stress:    element stresses in Mandel convention
+          temperatures:     element temperatures
+          volumes:          element volumes
+          material:         material model object with required data that includes
+                            Weibull scale parameter (svals), Weibull modulus (mvals)
+                            and uniaxial and polyaxial crack density coefficient (kvals,kpvals)
+          tot_time:       total time at which to calculate reliability
         """
+        self.temperatures = temperatures
+        self.material = material
+        self.mandel_stress = mandel_stress
 
         # Material parameters
         svals = material.strength(temperatures)
         mvals = material.modulus(temperatures)
         kvals = svals ** (-mvals)
-        kpvals = (2 * mvals + 1) * kvals
+
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+        kavg = np.mean(kvals, axis=0)
+
+        # Polyaxial Batdorf crack density coefficient
+        kpvals = (2 * mavg + 1) * kavg
 
         # Average normal tensile stress raied to exponent mv
         avg_nstress = (
-            self.calculate_avg_normal_stress(mandel_stress, temperatures, material)
-        ) ** (1 / mvals)
+            self.calculate_avg_normal_stress(
+                time,
+                mandel_stress,
+                self.temperatures,
+                self.material,
+                tot_time,
+            )
+        ) ** (1 / mavg)
 
-        return -kpvals * (avg_nstress**mvals) * volumes
+        return -kpvals * (avg_nstress**mavg) * volumes
 
 
 class MTSModelGriffithFlaw(CrackShapeDependent):
     """
     Maximum tensile stess failure model with a Griffith flaw
 
     Evaluates an equivalent stress (acting on the cracks) using the normal and
@@ -513,14 +677,53 @@
 
         # Shear stress
         tau = self.calculate_shear_stress(mandel_stress)
 
         # Projected equivalent stress
         return 0.5 * (sigma_n + np.sqrt((sigma_n**2) + (tau**2)))
 
+    def calculate_kbar(self, temperatures, material, A, dalpha, dbeta):
+        """
+        Calculate the evaluating normalized crack density coefficient (kbar)
+        using the Weibull scale parameter (svals), Weibull modulus (mvals),
+        poisson ratio (nu)
+        """
+
+        self.temperatures = temperatures
+        self.material = material
+
+        # Weibull modulus
+        mvals = self.material.modulus(temperatures)
+
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+
+        # Evaluating integral for kbar
+        integral2 = 2 * (
+            (
+                (
+                    0.5
+                    * (
+                        ((np.cos(self.A)) ** 2)
+                        + np.sqrt(
+                            ((np.cos(self.A)) ** 4)
+                            + (((np.sin(self.A)) ** 2) * ((np.cos(self.A)) ** 2))
+                        )
+                    )
+                )
+                ** mavg[..., None, None]
+            )
+            * np.sin(self.A)
+            * self.dalpha
+            * self.dbeta
+        )
+        kbar = np.pi / np.sum(integral2, axis=(1, 2))
+
+        return kbar
+
 
 class MTSModelPennyShapedFlaw(CrackShapeDependent):
     """
     Maximum tensile stess failure model with a penny shaped flaw
 
     Evaluates an equivalent stress (acting on the cracks) using the normal and
     shear stresses in the maximum tensile stress fracture criterion for a penny shaped flaw
@@ -531,23 +734,76 @@
         Calculate the average normal tensile stresses from the normal and shear stresses
 
         Additional parameter:
         nu:     Poisson ratio
         """
 
         # Material parameters
-        nu = material.nu(temperatures).flat[0]
+        nu = np.mean(material.nu(temperatures), axis=0)
 
+        # Normal stress
         sigma_n = self.calculate_normal_stress(mandel_stress)
+
+        # Shear stress
         tau = self.calculate_shear_stress(mandel_stress)
+
         # Projected equivalent stress
         return 0.5 * (
-            sigma_n + np.sqrt((sigma_n**2) + ((tau / (1 - (0.5 * nu))) ** 2))
+            sigma_n
+            + np.sqrt((sigma_n**2) + ((tau / (1 - (0.5 * nu[..., None, None]))) ** 2))
         )
 
+    def calculate_kbar(self, temperatures, material, A, dalpha, dbeta):
+        """
+        Calculate the evaluating normalized crack density coefficient (kbar)
+
+        Parameters:
+        temperatures:   element temperatures
+        material:       material model object with required data that includes
+                        Weibull modulus (mvals), poisson ratio (nu)
+        """
+
+        self.temperatures = temperatures
+        self.material = material
+
+        # Weibull modulus
+        mvals = self.material.modulus(temperatures)
+
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+
+        # Material parameters
+        nu = np.mean(material.nu(temperatures), axis=0)
+
+        # Evaluating integral for kbar
+        integral2 = 2 * (
+            (
+                (
+                    0.5
+                    * (
+                        ((np.cos(self.A)) ** 2)
+                        + np.sqrt(
+                            ((np.cos(self.A)) ** 4)
+                            + (
+                                ((np.sin(2 * self.A)) ** 2)
+                                / (2 - (nu[..., None, None] ** 2))
+                            )
+                        )
+                    )
+                )
+                ** mavg[..., None, None]
+            )
+            * np.sin(self.A)
+            * self.dalpha
+            * self.dbeta
+        )
+        kbar = np.pi / np.sum(integral2, axis=(1, 2))
+
+        return kbar
+
 
 class CSEModelGriffithFlaw(CrackShapeDependent):
     """
     Coplanar strain energy failure model with a Griffith flaw
 
     Evaluates an equivalent stress (acting on the cracks) using the normal and
     shear stresses in the coplanar strain energy fracture criterion
@@ -563,14 +819,44 @@
 
         # Shear stress
         tau = self.calculate_shear_stress(mandel_stress)
 
         # Projected equivalent stress
         return np.sqrt((sigma_n**2) + (tau**2))
 
+    def calculate_kbar(self, temperatures, material, A, dalpha, dbeta):
+        """
+        Calculate the evaluating normalized crack density coefficient (kbar)
+
+        Parameters:
+        temperatures:   element temperatures
+        material:       material model object with required data that includes
+                        Weibull modulus (mvals)
+        """
+
+        self.temperatures = temperatures
+        self.material = material
+
+        # Weibull modulus
+        mvals = self.material.modulus(temperatures)
+
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+
+        # Evaluating integral for kbar
+        integral2 = 2 * (
+            ((np.cos(self.A)) ** mavg[..., None, None])
+            * np.sin(self.A)
+            * self.dalpha
+            * self.dbeta
+        )
+        kbar = np.pi / np.sum(integral2, axis=(1, 2))
+
+        return kbar
+
 
 class CSEModelPennyShapedFlaw(CrackShapeDependent):
     """
     Coplanar strain energy failure model with a penny shaped flaw
 
     Evaluates an equivalent stress (acting on the cracks) using the normal and
     shear stresses in the coplanar strain energy fracture criterion
@@ -582,24 +868,68 @@
         Calculate the equivalent stresses from the normal and shear stresses
 
         Additional parameter:
         nu:     Poisson ratio
         """
 
         # Material parameters
-        nu = material.nu(temperatures).flat[0]
+        nu = np.mean(material.nu(temperatures), axis=0)
 
         # Normal stress
         sigma_n = self.calculate_normal_stress(mandel_stress)
 
         # Shear stress
         tau = self.calculate_shear_stress(mandel_stress)
 
         # Projected equivalent stress
-        return np.sqrt((sigma_n**2) + (tau / (1 - (0.5 * nu))) ** 2)
+        return np.sqrt((sigma_n**2) + (tau / (1 - (0.5 * nu[..., None, None]))) ** 2)
+
+    def calculate_kbar(self, temperatures, material, A, dalpha, dbeta):
+        """
+        Calculate the evaluating normalized crack density coefficient (kbar)
+
+        Parameters:
+        temperatures:   element temperatures
+        material:       material model object with required data that includes
+                        Weibull modulus (mvals), poisson ratio (nu)
+        """
+
+        self.temperatures = temperatures
+        self.material = material
+
+        # Weibull modulus
+        mvals = self.material.modulus(temperatures)
+
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+
+        # Material parameters
+        nu = np.mean(material.nu(temperatures), axis=0)
+
+        # Evaluating integral for kbar
+        integral2 = 2 * (
+            (
+                (
+                    np.sqrt(
+                        ((np.cos(self.A)) ** 4)
+                        + (
+                            ((np.sin(2 * self.A)) ** 2)
+                            / ((2 - nu[..., None, None]) ** 2)
+                        )
+                    )
+                )
+                ** mavg[..., None, None]
+            )
+            * np.sin(self.A)
+            * self.dalpha
+            * self.dbeta
+        )
+        kbar = np.pi / np.sum(integral2, axis=(1, 2))
+
+        return kbar
 
 
 class SMMModelGriffithFlaw(CrackShapeDependent):
     """
     Shetty mixed-mod failure model with a Griffith flaw
 
     Evaluates an equivalent stress (acting on the cracks) using the normal and
@@ -608,28 +938,79 @@
     """
 
     def calculate_eq_stress(self, mandel_stress, temperatures, material):
         """
         Calculate the equivalent stresses from the normal and shear stresses
 
         Additional parameters:
-        cbar:   Emperical constant
+        cbar:   Shetty model empirical constant (cbar)
         """
 
         # Material parameters
-        cbar = material.c_bar(temperatures).flat[0]
+        cbar = np.mean(material.c_bar(temperatures), axis=0)
 
         # Normal stress
         sigma_n = self.calculate_normal_stress(mandel_stress)
 
         # Shear stress
         tau = self.calculate_shear_stress(mandel_stress)
 
         # Projected equivalent stress
-        return 0.5 * (sigma_n + np.sqrt((sigma_n**2) + ((2 * tau / cbar) ** 2)))
+        return 0.5 * (
+            sigma_n + np.sqrt((sigma_n**2) + ((2 * tau / cbar[..., None, None]) ** 2))
+        )
+
+    def calculate_kbar(self, temperatures, material, A, dalpha, dbeta):
+        """
+        Calculate the evaluating normalized crack density coefficient (kbar)
+
+        Parameters:
+        temperatures:   element temperatures
+        material:       material model object with required data that includes
+                        Weibull modulus (mvals), poisson ratio (nu),
+                        Shetty model empirical constant (cbar)
+        """
+
+        self.temperatures = temperatures
+        self.material = material
+
+        # Weibull modulus
+        mvals = self.material.modulus(temperatures)
+
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+
+        # Material parameters
+        cbar = np.mean(material.c_bar(temperatures), axis=0)
+
+        # Evaluating integral for kbar
+        integral2 = 2 * (
+            (
+                (
+                    0.5
+                    * (
+                        ((np.cos(self.A)) ** 2)
+                        + np.sqrt(
+                            ((np.cos(self.A)) ** 4)
+                            + (
+                                ((np.sin(2 * self.A)) ** 2)
+                                / (cbar[..., None, None] ** 2)
+                            )
+                        )
+                    )
+                )
+                ** mavg[..., None, None]
+            )
+            * np.sin(self.A)
+            * self.dalpha
+            * self.dbeta
+        )
+        kbar = np.pi / np.sum(integral2, axis=(1, 2))
+
+        return kbar
 
 
 class SMMModelPennyShapedFlaw(CrackShapeDependent):
     """
     Shetty mixed mode failure model with a penny shaped flaw
 
     Evaluates an equivalent stress (acting on the cracks) using the normal and
@@ -639,32 +1020,89 @@
 
     def calculate_eq_stress(self, mandel_stress, temperatures, material):
         """
         Calculate the equivalent stresses from the normal and shear stresses
 
         Additional parameters:
         nu:     Poisson ratio
-        cbar:   Emperical constant
+        cbar:   Shetty model empirical constant (cbar)
         """
 
         # Material parameters
-        nu = material.nu(temperatures).flat[0]
-        cbar = material.c_bar(temperatures).flat[0]
+        nu = np.mean(material.nu(temperatures), axis=0)
+        cbar = np.mean(material.c_bar(temperatures), axis=0)
 
         # Normal stress
         sigma_n = self.calculate_normal_stress(mandel_stress)
 
         # Shear stress
         tau = self.calculate_shear_stress(mandel_stress)
 
         # Projected equivalent stress
         return 0.5 * (
-            sigma_n + np.sqrt((sigma_n**2) + ((4 * tau / (cbar * (2 - nu))) ** 2))
+            sigma_n
+            + np.sqrt(
+                (sigma_n**2)
+                + ((4 * tau / (cbar[..., None, None] * (2 - nu[..., None, None]))) ** 2)
+            )
         )
 
+    def calculate_kbar(self, temperatures, material, A, dalpha, dbeta):
+        """
+        Calculate the evaluating normalized crack density coefficient (kbar)
+
+        Parameters:
+        temperatures:   element temperatures
+        material:       material model object with required data that includes
+                        Weibull modulus (mvals), poisson ratio (nu),
+                        Shetty model empirical constant (cbar)
+        """
+
+        self.temperatures = temperatures
+        self.material = material
+
+        # Weibull modulus
+        mvals = self.material.modulus(temperatures)
+
+        # Temperature average values
+        mavg = np.mean(mvals, axis=0)
+
+        # Material parameters
+        nu = np.mean(material.nu(temperatures), axis=0)
+        cbar = np.mean(material.c_bar(temperatures), axis=0)
+
+        # Evaluating integral for kbar
+        integral2 = 2 * (
+            (
+                (
+                    0.5
+                    * (
+                        ((np.cos(self.A)) ** 2)
+                        + np.sqrt(
+                            ((np.cos(self.A)) ** 4)
+                            + (
+                                (4 * ((np.sin(2 * self.A)) ** 2))
+                                / (
+                                    (cbar[..., None, None] ** 2)
+                                    * ((nu[..., None, None] - 2) ** 2)
+                                )
+                            )
+                        )
+                    )
+                )
+                ** mavg[..., None, None]
+            )
+            * np.sin(self.A)
+            * self.dalpha
+            * self.dbeta
+        )
+        kbar = np.pi / np.sum(integral2, axis=(1, 2))
+
+        return kbar
+
 
 class DamageCalculator:
     """
     Parent class for all damage calculators, handling common iteration
     and scaling options
     """
```

### Comparing `srlife-2.0.0/srlife/data/damage/316H.xml` & `srlife-2.0.1/srlife/data/damage/316H.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/damage/740H.xml` & `srlife-2.0.1/srlife/data/damage/740H.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/damage/800H.xml` & `srlife-2.0.1/srlife/data/damage/800H.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/damage/A230.xml` & `srlife-2.0.1/srlife/data/damage/A230.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/damage/A282.xml` & `srlife-2.0.1/srlife/data/damage/A282.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/damage/A617.xml` & `srlife-2.0.1/srlife/data/damage/A617.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/deformation/316H.xml` & `srlife-2.0.1/srlife/data/deformation/316H.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/deformation/740H.xml` & `srlife-2.0.1/srlife/data/deformation/740H.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/deformation/800H.xml` & `srlife-2.0.1/srlife/data/deformation/800H.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/deformation/A230.xml` & `srlife-2.0.1/srlife/data/deformation/A230.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/deformation/A282.xml` & `srlife-2.0.1/srlife/data/deformation/A282.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/deformation/A617.xml` & `srlife-2.0.1/srlife/data/deformation/A617.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/fluid/salt.xml` & `srlife-2.0.1/srlife/data/fluid/salt.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/thermal/740H.xml` & `srlife-2.0.1/srlife/data/thermal/740H.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/thermal/SiC.xml` & `srlife-2.0.1/srlife/data/thermal/SiC.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/data/thermalfluid/sCO2.xml` & `srlife-2.0.1/srlife/data/thermalfluid/sCO2.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/helpers.py` & `srlife-2.0.1/srlife/helpers.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/library.py` & `srlife-2.0.1/srlife/library.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/managers.py` & `srlife-2.0.1/srlife/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,39 +133,46 @@
         return self.damage_model.determine_life(
             self.receiver,
             self.damage_material,
             nthreads=self.nthreads,
             decorator=self.progress_decorator,
         )
 
-    def solve_reliability(self):
+    def solve_reliability(self, time):
         """User interface: solve everything and return receiver reliability
 
         The trigger for everything: solve the complete problem and report the
         best-estimate reliability.
 
+        Args:
+            time (float): time at which to report reliability
+
         Returns:
           float:  Reliability between 0 and 1
         """
         self.solve_heat_transfer()
         self.solve_structural()
 
-        return self.calculate_reliability()
+        return self.calculate_reliability(time)
 
-    def calculate_reliability(self):
+    def calculate_reliability(self, time):
         """Calculate reliability from the results
 
+        Args:
+            time (float): time at which to report reliability
+
         Returns:
           float:    Reliability between 0 and 1
         """
         if self.progress:
             print("Calculating reliability :")
         return self.damage_model.determine_reliability(
             self.receiver,
             self.damage_material,
+            time,
             nthreads=self.nthreads,
             decorator=self.progress_decorator,
         )
 
     def solve_heat_transfer(self):
         """Solve heat transfer for the receiver
 
@@ -201,15 +208,15 @@
                 self.progress_decorator(
                     p.imap(
                         lambda x: self.thermal_solver.solve(
                             x,
                             self.thermal_material,
                             self.fluid_material,
                             **merge_dicts(
-                                h.args_for_thermal_solver(self.receiver, x)
+                                h.args_for_tube_thermal_solver(self.receiver, x)
                                 for h in self.heuristics
                             )
                         ),
                         self.tubes,
                     ),
                     self.ntubes,
                 )
```

### Comparing `srlife-2.0.0/srlife/materials.py` & `srlife-2.0.1/srlife/materials.py`

 * *Files 7% similar despite different names*

```diff
@@ -494,15 +494,15 @@
             )
 
         for i in range(np.size(T, axis=0)):
             if temp <= T[i]:
                 polysum = 0.0
                 if erange <= cutoff[i]:
                     erange = cutoff[i][0][0]
-                for (b, m) in zip(a[i][0], n[i][0]):
+                for b, m in zip(a[i][0], n[i][0]):
                     polysum += b * np.log10(erange) ** m
                 break
 
         return 10**polysum
 
     def time_to_rupture(self, pname, temp, stress):
         """
@@ -525,15 +525,15 @@
         if stress.shape != temp.shape:
             raise ValueError("Stress and temperature must have the same shape!")
 
         zeros = stress == 0.0
         not_zeros = np.logical_not(zeros)
 
         res = np.zeros(stress.shape)
-        for (b, m) in zip(a, n):
+        for b, m in zip(a, n):
             res[not_zeros] += b * np.log10(stress[not_zeros]) ** m
         res[not_zeros] = 10.0 ** (res[not_zeros] / temp[not_zeros] - C)
         res[zeros] = np.inf
 
         return res
 
     def inside_envelope(self, pname, damage_fatigue, damage_creep):
@@ -698,37 +698,49 @@
     """
     Ceramic material where:
 
     1) Weibull strength depends on temperature
     2) Weibull modulus depends on temperature
     3) Constant c_bar parameter
     4) Constant Poisson's ratio
+    5) Fatigue exponent parameter Nv depends on temperature
+    6) Faitgue parameter Bv depends on temperature
     """
 
     def __init__(
         self,
         s_temperatures,
         strengths,
         m_temperatures,
         modulus,
         c_bar,
         nu,
+        Nv_temperatures,
+        Nvvals,
+        Bv_temperatures,
+        Bvvals,
         *args,
         **kwargs
     ):
         super().__init__(*args, **kwargs)
 
-        self.s0 = inter.interp1d(s_temperatures, strengths)
         self.s_temperatures = s_temperatures
         self.strengths = strengths
+        self.s0 = inter.interp1d(s_temperatures, strengths)
         self.m_temperatures = m_temperatures
         self.mvals = modulus
         self.m = inter.interp1d(m_temperatures, modulus)
         self.C = c_bar
         self.nu_val = nu
+        self.Nv_temperatures = Nv_temperatures
+        self.Nvvals = Nvvals
+        self.Nv = inter.interp1d(Nv_temperatures, Nvvals)
+        self.Bv_temperatures = Bv_temperatures
+        self.Bvvals = Bvvals
+        self.Bv = inter.interp1d(Bv_temperatures, Bvvals)
 
     def strength(self, T):
         """
         Weibull strength as a function of temperature
         """
         return self.s0(T)
 
@@ -752,47 +764,74 @@
         Poisson's ratio as a function of temperature
         """
         if np.isscalar(T):
             return self.nu_val
         else:
             return self.nu_val * np.ones(T.shape)
 
+    def fatigue_Nv(self, T):
+        """
+        Fatigue exponent parameter as a function of temperature
+        """
+        return self.Nv(T)
+
+    def fatigue_Bv(self, T):
+        """
+        Fatigue parameter as a function of temperature
+        """
+        return self.Bv(T)
+
     @classmethod
     def load(cls, node):
         """
         Load a Ceramic material from a file
 
         Parameters:
           node:    node with model
         """
         strength = node.find("strength")
-        c_bar = node.find("c_bar")
         s_temps = strength.find("temperatures")
         svals = strength.find("values")
+
         m = node.find("modulus")
         m_temps = m.find("temperatures")
         mvals = m.find("values")
+
+        c_bar = node.find("c_bar")
         nu = node.find("nu")
 
+        Nv = node.find("fatigue_Nv")
+        Nv_temps = Nv.find("temperatures")
+        Nvvals = Nv.find("values")
+
+        Bv = node.find("fatigue_Bv")
+        Bv_temps = Bv.find("temperatures")
+        Bvvals = Bv.find("values")
+
         return StandardCeramicMaterial(
             np.array(list(map(float, s_temps.text.strip().split()))),
             np.array(list(map(float, svals.text.strip().split()))),
             np.array(list(map(float, m_temps.text.strip().split()))),
             np.array(list(map(float, mvals.text.strip().split()))),
             float(c_bar.text),
             float(nu.text),
+            np.array(list(map(float, Nv_temps.text.strip().split()))),
+            np.array(list(map(float, Nvvals.text.strip().split()))),
+            np.array(list(map(float, Bv_temps.text.strip().split()))),
+            np.array(list(map(float, Bvvals.text.strip().split()))),
         )
 
     def save(self, fname, modelname):
         """
         Save to a particular file under a particular model name
         """
         root = ET.Element("models")
 
         base = ET.SubElement(root, modelname, {"type": "StandardModel"})
+
         strength = ET.SubElement(base, "strength")
         temps = ET.SubElement(strength, "temperatures")
         temps.text = " ".join(map(str, self.s_temperatures))
         svals = ET.SubElement(strength, "values")
         svals.text = " ".join(map(str, self.strengths))
 
         m = ET.SubElement(base, "modulus")
@@ -803,9 +842,21 @@
 
         c_bar = ET.SubElement(base, "c_bar")
         c_bar.text = str(self.C)
 
         nu = ET.SubElement(base, "nu")
         nu.text = str(self.nu_val)
 
+        Nv = ET.SubElement(base, "fatigue_Nv")
+        Nvtemps = ET.SubElement(Nv, "temperatures")
+        Nvtemps.text = " ".join(map(str, self.Nv_temperatures))
+        Nvvals = ET.SubElement(Nv, "values")
+        Nvvals.text = " ".join(map(str, self.Nvvals))
+
+        Bv = ET.SubElement(base, "fatigue_Bv")
+        Bvtemps = ET.SubElement(Bv, "temperatures")
+        Bvtemps.text = " ".join(map(str, self.Bv_temperatures))
+        Bvvals = ET.SubElement(Bv, "values")
+        Bvvals.text = " ".join(map(str, self.Bvvals))
+
         tree = ET.ElementTree(element=root)
         tree.write(fname)
```

### Comparing `srlife-2.0.0/srlife/receiver.py` & `srlife-2.0.1/srlife/receiver.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/solverparams.py` & `srlife-2.0.1/srlife/solverparams.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/solvers.py` & `srlife-2.0.1/srlife/solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
   Nonlinear solvers and other accessories
 """
 
 import numpy as np
 import numpy.linalg as la
 
+
 # pylint: disable=too-many-branches
 def newton(
     RJ,
     x0,
     rel_tol=1.0 - 6,
     abs_tol=1.0e-8,
     miters=20,
```

### Comparing `srlife-2.0.0/srlife/spring.py` & `srlife-2.0.1/srlife/spring.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/structural.py` & `srlife-2.0.1/srlife/structural.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/system.py` & `srlife-2.0.1/srlife/system.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/thermal.py` & `srlife-2.0.1/srlife/thermal.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife/thermohydraulics/flowpath.py` & `srlife-2.0.1/srlife/thermohydraulics/flowpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import numpy as np
 import numpy.linalg as la
 import scipy.interpolate as inter
 import scipy.sparse as sp
 import scipy.sparse.linalg as spla
 
-from jax.config import config
+import jax
 
-config.update("jax_enable_x64", True)
+jax.config.update("jax_enable_x64", True)
 import jax.numpy as jnp
 from jax import jacfwd
 
 
 class StartLink:
     """Starting link in the chain, gives the first temperature"""
```

### Comparing `srlife-2.0.0/srlife/thermohydraulics/thermalfluid.py` & `srlife-2.0.1/srlife/thermohydraulics/thermalfluid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pylint: disable=no-member, wrong-import-position
 """
     Thermal-fluid specific material classes
 """
 import xml.etree.ElementTree as ET
 
-from jax.config import config
+import jax
 
-config.update("jax_enable_x64", True)
+jax.config.update("jax_enable_x64", True)
 import jax.numpy as jnp
 
 from srlife import materials
 
 
 class ThermalFluidMaterial:
     """Thermal fluid material properties
```

### Comparing `srlife-2.0.0/srlife/writers.py` & `srlife-2.0.1/srlife/writers.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/srlife.egg-info/PKG-INFO` & `srlife-2.0.1/srlife.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: srlife
-Version: 2.0.0
+Version: 2.0.1
 Summary: Evaluate the structural life of a solar receiver
 Home-page: https://github.com/Argonne-National-Laboratory/srlife
 Author: Argonne National Laboratory
 Author-email: messner@anl.gov
-License: UNKNOWN
-Description: # srlife: solar receiver life estimation tool
-        
-        ![Test Status](https://github.com/Argonne-National-Laboratory/srlife/workflows/tests/badge.svg?branch=master) ![Documentation Status](https://readthedocs.org/projects/srlife/badge/?version=latest)
-        
-        This python package evaluates the structural life of tubular solar receivers against
-        creep rupture, fatigue, and creep-fatigue damage modes.
-        
-        Full documentation is available [here](https://srlife.readthedocs.io/).
-        
-        ## Prerequisites
-        
-        The package itself is pure python, however it relies on several additional
-        python packages listed in [requirements.txt](requirements.txt).
-        Note that srlife uses Python3.
-        
-        ## License
-        
-        The package is provided under an MIT license found in the
-        [LICENSE](LICENSE) file.
-        
 Keywords: materials structures modeling
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# srlife: solar receiver life estimation tool
+
+![Test Status](https://github.com/Argonne-National-Laboratory/srlife/workflows/tests/badge.svg?branch=master) ![Documentation Status](https://readthedocs.org/projects/srlife/badge/?version=latest)
+
+This python package evaluates the structural life of tubular solar receivers against
+creep rupture, fatigue, and creep-fatigue damage modes.
+
+Full documentation is available [here](https://srlife.readthedocs.io/).
+
+## Prerequisites
+
+The package itself is pure python, however it relies on several additional
+python packages listed in [requirements.txt](requirements.txt).
+Note that srlife uses Python3.
+
+## License
+
+The package is provided under an MIT license found in the
+[LICENSE](LICENSE) file.
```

### Comparing `srlife-2.0.0/srlife.egg-info/SOURCES.txt` & `srlife-2.0.1/srlife.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 srlife/data/thermal/SiC.xml
 srlife/data/thermalfluid/32MgCl2-68KCl.xml
 srlife/data/thermalfluid/sCO2.xml
 srlife/thermohydraulics/__init__.py
 srlife/thermohydraulics/flowpath.py
 srlife/thermohydraulics/thermalfluid.py
 test/helpers.py
-test/test_ceramic_damage.py
+test/test_ceramic_damage_CARES_cyclic.py
+test/test_ceramic_damage_CARES_static.py
 test/test_helpers.py
 test/test_material_library.py
 test/test_materials.py
 test/test_receiver_data.py
 test/test_volume_calculation.py
 test/test_writers.py
 test/solvers/__init__.py
```

### Comparing `srlife-2.0.0/test/helpers.py` & `srlife-2.0.1/test/helpers.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/spring/altsolver.py` & `srlife-2.0.1/test/solvers/spring/altsolver.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/spring/test_random_networks.py` & `srlife-2.0.1/test/solvers/spring/test_random_networks.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/spring/test_spring.py` & `srlife-2.0.1/test/solvers/spring/test_spring.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/thermal/run_verification.py` & `srlife-2.0.1/test/solvers/thermal/run_verification.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/thermal/test_thermal.py` & `srlife-2.0.1/test/solvers/thermal/test_thermal.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/thermal/thermalsol.py` & `srlife-2.0.1/test/solvers/thermal/thermalsol.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/thermal/time_1d.py` & `srlife-2.0.1/test/solvers/thermal/time_1d.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/thermal/time_2d.py` & `srlife-2.0.1/test/solvers/thermal/time_2d.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/thermal/time_3d.py` & `srlife-2.0.1/test/solvers/thermal/time_3d.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/1d.i` & `srlife-2.0.1/test/solvers/tube/moose-verification/1d.i`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/1d_out.e` & `srlife-2.0.1/test/solvers/tube/moose-verification/1d_out.e`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/2d.i` & `srlife-2.0.1/test/solvers/tube/moose-verification/2d.i`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/2d_out.e` & `srlife-2.0.1/test/solvers/tube/moose-verification/2d_out.e`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/3d.i` & `srlife-2.0.1/test/solvers/tube/moose-verification/3d.i`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/3d_out.e` & `srlife-2.0.1/test/solvers/tube/moose-verification/3d_out.e`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/meshes/1d.e` & `srlife-2.0.1/test/solvers/tube/moose-verification/meshes/1d.e`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/meshes/2d.e` & `srlife-2.0.1/test/solvers/tube/moose-verification/meshes/2d.e`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/meshes/3d.e` & `srlife-2.0.1/test/solvers/tube/moose-verification/meshes/3d.e`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/moose-verification/model.xml` & `srlife-2.0.1/test/solvers/tube/moose-verification/model.xml`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/run_structural_tube_verification.py` & `srlife-2.0.1/test/solvers/tube/run_structural_tube_verification.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/test_structural_tube.py` & `srlife-2.0.1/test/solvers/tube/test_structural_tube.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/solvers/tube/time.py` & `srlife-2.0.1/test/solvers/tube/time.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/test_helpers.py` & `srlife-2.0.1/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/test_material_library.py` & `srlife-2.0.1/test/test_material_library.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/test_materials.py` & `srlife-2.0.1/test/test_materials.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,33 +186,33 @@
         fcycles = self.structmat.cycles_to_fail(self.fatigue_pname, self.T, self.erange)
 
         a = np.array([-9.2e-01, -3.8e00, -8.4e00, -4.1e00])
         n = np.array([3, 2, 1, 0])
         cutoff = 1.5e-3
         sum = 0
         if self.erange <= cutoff:
-            for (b, m) in zip(a, n):
+            for b, m in zip(a, n):
                 sum += b * np.log10(cutoff) ** m
         else:
-            for (b, m) in zip(a, n):
+            for b, m in zip(a, n):
                 sum += b * np.log10(self.erange) ** m
         return 10**sum
 
         self.assertTrue(np.isclose(sum, fcycles))
 
     def test_rupturetime(self):
         rtime = self.structmat.time_to_rupture(
             self.rupture_pname, np.array([self.T]), np.array([self.stress])
         )[0]
 
         C = 17.16
         a = np.array([-1475.23, 7289.41, -16642.64, 35684.60])
         n = np.array([3, 2, 1, 0])
         sum = 0
-        for (b, m) in zip(a, n):
+        for b, m in zip(a, n):
             sum += b * np.log10(self.stress) ** m
         sum = 10 ** (sum / self.T - C)
 
         self.assertTrue(np.isclose(sum, rtime))
 
     def test_inside_envelope(self):
         """
@@ -244,17 +244,30 @@
     def setUp(self):
         self.Ts = np.array([25.0, 800.0, 1000.0, 1200.0, 1400.0, 1500.0])
         self.s0s = np.array([507.0, 467.0, 528.0, 570.0, 746.0, 461.0])
         self.mTs = np.array([25.0, 1500.0])
         self.ms = np.array([10.7, 9.2])
         self.c_bar = 1.5
         self.nu = 0.17
+        self.NvTs = np.array([25.0, 1000.0, 1500.0])
+        self.Nvs = np.array([30.0, 30.0, 30.0])
+        self.BvTs = np.array([25.0, 1000.0, 1500.0])
+        self.Bvs = np.array([320.0, 320.0, 320.0])
 
         self.mat = materials.StandardCeramicMaterial(
-            self.Ts, self.s0s, self.mTs, self.ms, self.c_bar, self.nu
+            self.Ts,
+            self.s0s,
+            self.mTs,
+            self.ms,
+            self.c_bar,
+            self.nu,
+            self.NvTs,
+            self.Nvs,
+            self.BvTs,
+            self.Bvs,
         )
 
     def test_strength(self):
         ifn = inter.interp1d(self.Ts, self.s0s)
         T = 1099.1
 
         a = self.mat.strength(T)
@@ -282,20 +295,44 @@
     def test_nu(self):
         T = 1099.1
 
         a = self.mat.nu(T)
         b = self.nu
         self.assertAlmostEqual(a, b)
 
+    def test_Nv(self):
+        ifn = inter.interp1d(self.NvTs, self.Nvs)
+        T = 1099.1
+
+        a = self.mat.Nv(T)
+        b = ifn(T)
+
+        self.assertAlmostEqual(a, b)
+
+    def test_Bv(self):
+        ifn = inter.interp1d(self.BvTs, self.Bvs)
+        T = 1099.1
+
+        a = self.mat.Bv(T)
+        b = ifn(T)
+
+        self.assertAlmostEqual(a, b)
+
     def test_store_receover(self):
         tfile = tempfile.mktemp()
         self.mat.save(tfile, "blah")
         test = materials.CeramicMaterial.load(tfile, "blah")
 
         self.assertTrue(np.allclose(test.s_temperatures, self.Ts))
         self.assertTrue(np.allclose(test.strengths, self.s0s))
 
         self.assertTrue(np.allclose(test.m_temperatures, self.mTs))
         self.assertTrue(np.allclose(test.mvals, self.ms))
 
         self.assertTrue(np.isclose(test.C, self.c_bar))
         self.assertTrue(np.isclose(test.nu_val, self.nu))
+
+        self.assertTrue(np.allclose(test.Nv_temperatures, self.NvTs))
+        self.assertTrue(np.allclose(test.Nvvals, self.Nvs))
+
+        self.assertTrue(np.allclose(test.Bv_temperatures, self.BvTs))
+        self.assertTrue(np.allclose(test.Bvvals, self.Bvs))
```

### Comparing `srlife-2.0.0/test/test_receiver_data.py` & `srlife-2.0.1/test/test_receiver_data.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/test_volume_calculation.py` & `srlife-2.0.1/test/test_volume_calculation.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/test_writers.py` & `srlife-2.0.1/test/test_writers.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/thermohydraulics/test_flowpath.py` & `srlife-2.0.1/test/thermohydraulics/test_flowpath.py`

 * *Files identical despite different names*

### Comparing `srlife-2.0.0/test/thermohydraulics/test_thermalfluid.py` & `srlife-2.0.1/test/thermohydraulics/test_thermalfluid.py`

 * *Files identical despite different names*

