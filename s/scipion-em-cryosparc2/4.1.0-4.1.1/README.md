# Comparing `tmp/scipion-em-cryosparc2-4.1.0.tar.gz` & `tmp/scipion-em-cryosparc2-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryosparc2-4.1.0.tar", last modified: Mon Apr 29 13:26:26 2024, max compression
+gzip compressed data, was "scipion-em-cryosparc2-4.1.1.tar", last modified: Wed May 29 08:55:57 2024, max compression
```

## Comparing `scipion-em-cryosparc2-4.1.0.tar` & `scipion-em-cryosparc2-4.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.462176 scipion-em-cryosparc2-4.1.0/cryosparc2/
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)    32627 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.466176 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28554 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/cs2Start.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/cryosparc2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23486 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    24105 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)    16841 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_mesh_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
--rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    24600 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_ab.py
--rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_blob_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    23246 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    34102 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_patch_ctf_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_sharppening.py
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/cryosparc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47395 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/tests/test_protocols_cryosparc2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37814 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_2Dclassify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_partsubtract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14120 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/wizards.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:55:57.496783 scipion-em-cryosparc2-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-05-29 08:55:57.496783 scipion-em-cryosparc2-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:55:57.488783 scipion-em-cryosparc2-4.1.1/cryosparc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32980 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:55:57.488783 scipion-em-cryosparc2-4.1.1/cryosparc2/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/convert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28554 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/convert/cs2Start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/cryosparc2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:55:57.492783 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18226 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23486 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24105 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_flex_mesh_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14356 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24600 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_ab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_blob_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23254 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34075 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40054 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20282 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_patch_ctf_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_sharppening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:55:57.492783 scipion-em-cryosparc2-4.1.1/cryosparc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45226 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/tests/test_protocols_cryosparc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43084 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:55:57.496783 scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/viewer_2Dclassify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/viewer_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/viewer_partsubtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14120 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/viewer_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/cryosparc2/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:55:57.496783 scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-05-29 08:55:57.000000 scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-29 08:55:57.000000 scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:55:57.000000 scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-29 08:55:57.000000 scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 08:55:57.000000 scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 08:55:57.000000 scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:55:57.496783 scipion-em-cryosparc2-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-29 08:55:16.000000 scipion-em-cryosparc2-4.1.1/setup.py
```

### Comparing `scipion-em-cryosparc2-4.1.0/LICENSE` & `scipion-em-cryosparc2-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/PKG-INFO` & `scipion-em-cryosparc2-4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.1.0
+Version: 4.1.1
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -43,14 +43,20 @@
         * **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
         * **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
         
         
         **Latest plugin version**
         ==========================
         
+        **v4.1.1**
+        -----------
+        
+        * **new**        Compatibility with cryoSPARC v4.5.1
+        * **new**        Registering flex particles
+        * **new**        Integration with FlexUtils plugin
         
         **v4.1.0**
         -----------
         * **fixed**       Tolerating deletion of projects within CS as well as their folders in the file system
         
         * **new**         Add new protocols:
                             * **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
@@ -117,14 +123,20 @@
                # The root directory where cryoSPARC code and dependencies is installed.
                CRYOSPARC_HOME = <install_path>   (CRYOSPARC_DIR will work for legacy reasons)
                
                # full name of the initial admin account to be created
                CRYOSPARC_USER = <user_name>
         
                # Optional variables
+               ---------------------
+        
+               # The password with which cryoSPARC was installed.
+               # This is only required for the use of the Flexutils plugin and its
+               # connection to the 3D flex training protocol.
+               CRYOSPARC_PASSWORD = <password>
         
                #Folder (available to all workers) where scipion will create cryosparc projects
                CRYO_PROJECTS_DIR = <path> (default to <CRYOSPARC_HOME>/scipion_projects)
         
                # Specifies whether the CS installation is standalone or not. If False,
                # it is assumed that CS is installed in a cluster. If the variable is not
                # defined, by default assume that the installation is standalone and its
```

### Comparing `scipion-em-cryosparc2-4.1.0/README.rst` & `scipion-em-cryosparc2-4.1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 * **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
 * **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
 
 
 **Latest plugin version**
 ==========================
 
+**v4.1.1**
+-----------
+
+* **new**        Compatibility with cryoSPARC v4.5.1
+* **new**        Registering flex particles
+* **new**        Integration with FlexUtils plugin
 
 **v4.1.0**
 -----------
 * **fixed**       Tolerating deletion of projects within CS as well as their folders in the file system
 
 * **new**         Add new protocols:
                     * **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
@@ -107,14 +113,20 @@
        # The root directory where cryoSPARC code and dependencies is installed.
        CRYOSPARC_HOME = <install_path>   (CRYOSPARC_DIR will work for legacy reasons)
        
        # full name of the initial admin account to be created
        CRYOSPARC_USER = <user_name>
 
        # Optional variables
+       ---------------------
+
+       # The password with which cryoSPARC was installed.
+       # This is only required for the use of the Flexutils plugin and its
+       # connection to the 3D flex training protocol.
+       CRYOSPARC_PASSWORD = <password>
 
        #Folder (available to all workers) where scipion will create cryosparc projects
        CRYO_PROJECTS_DIR = <path> (default to <CRYOSPARC_HOME>/scipion_projects)
 
        # Specifies whether the CS installation is standalone or not. If False,
        # it is assumed that CS is installed in a cluster. If the variable is not
        # defined, by default assume that the installation is standalone and its
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/__init__.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,31 +27,33 @@
 
 import os
 import pwem as em
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
-__version__ = '4.1.0'
+__version__ = '4.1.1'
 _references = ['Punjani2017', 'Brubaker2017', 'daniel_asarnow_2019_3576630']
 _logo = 'cryosparc2_logo.png'
 
 
 class Plugin(em.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-cryosparc2"
     _homeVar = CRYOSPARC_HOME
     _pathVars = [CRYOSPARC_HOME]
-    _supportedVersions = [V3_0_0, V3_0_1, V3_1_0, V3_2_0, V3_3_0, V3_3_1,
-                          V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
+    _supportedVersions = SUPORTED_VERSIONS
 
     @classmethod
     def _defineVariables(cls):
         cls._defineVar(CRYOSPARC_HOME, os.environ.get(CRYOSPARC_DIR, ""))
         cls._defineVar(CRYO_PROJECTS_DIR, "scipion_projects")
+        cls._defineVar(CRYOSPARC_PASSWORD, None, description='The password with which cryoSPARC was installed. '
+                                                             'This is only required for the use of the Flexutils '
+                                                             'plugin and its connection to the 3D flex training protocol.')
+        cls._defineVar(CRYOSPARC_USER, None, description='This is the email with which cryoSPARC was installed.')
 
     @classmethod
     def getPyemEnvActivation(cls):
         return PYEM_ACTIVATION_CMD
 
     @classmethod
     def getEnviron(cls):
@@ -70,22 +72,33 @@
         neededProgs = ['wget']
         if not condaActivationCmd:
             neededProgs.append('conda')
 
         return neededProgs
 
     @classmethod
+    def getUserPassword(cls):
+        """Get the user password taking into account the environment variable"""
+        return cls.getVar(CRYOSPARC_PASSWORD)
+
+    @classmethod
+    def getUser(cls):
+        """Get the user email taking into account the environment variable"""
+        return cls.getVar(CRYOSPARC_USER)
+
+    @classmethod
     def addPyemPackage(cls, env):
         PYEM_INSTALLED = f"pyem_{PYEM_VERSION}_installed"
         ENV_NAME = getPyemEnvName(PYEM_VERSION)
 
         installCmd = ["pip uninstall -y pyem && ",
                       cls.getCondaActivationCmd(),
+                      f'conda env remove -n pyem-23.01.25 && ',
                       f'conda create -y -n {ENV_NAME} python=3.8 -c conda-forge -c anaconda && ',
-                      f'conda activate {ENV_NAME} && pip install git+https://github.com/asarnow/pyem.git@47cf8f70488500be5988b4db1b6ef7002916e0e0 && pip install numpy==1.23.5']
+                      f'conda activate {ENV_NAME} && pip install git+https://github.com/asarnow/pyem.git@0394d5bf6096377ca7cc7b6dd74484f1f40f37a8 && pip install numpy==1.23.5']
 
         # install pyem
         #installCmd.append('pip install git+https://github.com/asarnow/pyem.git@47cf8f70488500be5988b4db1b6ef7002916e0e0')
 
         # Flag installation finished
         installCmd.append(f'&& touch {PYEM_INSTALLED}')
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/bibtex.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/constants.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 # Root folder where cryosparc is installed, we will look here for the client
 CRYOSPARC_HOME = 'CRYOSPARC_HOME'
 CRYOSPARC_DIR = 'CRYOSPARC_DIR'  # Legacy, replaced by CRYOSPARC_HOME
 # Optional: Folder where cryosparc projects will be created
 CRYO_PROJECTS_DIR = 'CRYO_PROJECTS_DIR'
 CRYOSPARC_USER = 'CRYOSPARC_USER'
+CRYOSPARC_PASSWORD = 'CRYOSPARC_PASSWORD'
 CRYOSPARC_USE_SSD = 'CRYOSPARC_USE_SSD'
 CRYOSPARC_MASTER = 'cryosparc_master'
 CRYOSPARC_STANDALONE_INSTALLATION = 'CRYOSPARC_STANDALONE_INSTALLATION'
 CRYOSPARC_DEFAULT_LANE = 'CRYOSPARC_DEFAULT_LANE'
 CRYOSPARC_VERSION_FILE = 'version'
 CRYOSPARC_CONFIG_FILE = 'config.sh'
 CRYOSPARC_LICENSE_ID_VARIABLE = 'CRYOSPARC_LICENSE_ID'
@@ -48,15 +49,15 @@
 
 
 def getPyemEnvName(version):
     return 'pyem-%s' % version
 
 
 # pyem environment variables
-PYEM_VERSION = '23.01.25'  # This is our made up version
+PYEM_VERSION = '17.05.24'  # This is our made up version
 PYEM_ACTIVATION_CMD = 'conda activate %s' % (getPyemEnvName(PYEM_VERSION))
 
 # Supported versions:
 V_UNKNOWN = 'v0.0.0'
 V3_0_0 = 'v3.0.0'
 V3_0_1 = 'v3.0.1'
 V3_1_0 = 'v3.1.0'
@@ -72,14 +73,20 @@
 V4_1_1 = 'V4.1.1'
 V4_1_2 = 'V4.1.2'
 V4_2_0 = 'V4.2.0'
 V4_2_1 = 'V4.2.1'
 V4_3_1 = 'V4.3.1'
 V4_4_0 = 'V4.4.0'
 V4_4_1 = 'V4.4.1'
+V4_5_1 = 'V4.5.1'
+
+SUPORTED_VERSIONS = [V3_0_0, V3_0_1, V3_1_0, V3_2_0, V3_3_0, V3_3_1,
+                     V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
+                     V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0,
+                     V4_4_1, V4_5_1]
 
 # Symmetry dict
 CS_SYM_NAME = dict()
 CS_SYM_NAME[SYM_CYCLIC] = 'Cn'
 CS_SYM_NAME[SYM_DIHEDRAL_Y] = 'Dn'
 CS_SYM_NAME[SYM_TETRAHEDRAL] = 'T'
 CS_SYM_NAME[SYM_OCTAHEDRAL] = 'O'
@@ -148,14 +155,18 @@
 ALL_MAPS = 3
 
 OBJCMD_CLASSAVG_PROJS = 'Show class-averages/projections'
 OBJCMD_PROJS = 'Show only projections'
 OBJCMD_INITVOL = 'Show initial random volume'
 
 
+# FlexHub program
+CRYOSPARCFLEX = "cryoSPARC"
+
+
 # METADATA
 
 class RELIONCOLUMNS(enum.Enum):
     rlnOriginX = 'rlnOriginX'  # RLN_ORIENT_ORIGIN_X
     rlnOriginY = 'rlnOriginY'  # RLN_ORIENT_ORIGIN_Y
     rlnAngleRot = 'rlnAngleRot'  # RLN_ORIENT_ROT
     rlnAnglePsi = 'rlnAnglePsi'  # RLN_ORIENT_PSI
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/convert/__init__.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/convert/convert.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/convert/cs2Start.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/convert/cs2Start.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/convert/dataimport.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/cryosparc2_logo.png` & `scipion-em-cryosparc2-4.1.1/cryosparc2/cryosparc2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/__init__.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_base.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         """ Create the input file in STAR format as expected by Relion.
         If the input particles comes from Relion, just link the file.
         """
         imgSet = self._getInputParticles()
         if imgSet is not None:
             # Create links to binary files and write the relion .star file
             writeSetOfParticles(imgSet, self._getFileName('input_particles'),
-                                self._getTmpPath())
+                                self._getPath())
             self._importParticles()
 
         volume = self._getInputVolume()
         if volume is not None:
             self._importVolume()
 
         mask = self._getInputMask()
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc2d.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_classification.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_classification.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from pwem.objects import Volume
 from pyworkflow import BETA
-from pyworkflow.protocol.params import (PointerParam, FloatParam, IntParam,
-                                        BooleanParam, FileParam, StringParam)
+from pyworkflow.protocol.params import PointerParam
 from . import ProtCryosparcBase
 from ..convert import *
 from ..utils import *
 from ..constants import *
 
 
 class ProtCryoSparc3DFlexDataPrepare(ProtCryosparcBase):
@@ -39,15 +37,15 @@
     Prepares particles for use in 3DFlex training and reconstruction. At the same
     way,  Takes in a consensus (rigid) refinement density map, plus optionally
      a segmentation and generates a tetrahedral mesh for 3DFlex.
     """
     _label = '3D flex data prepare'
     _devStatus = BETA
     _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1,
-                          V4_4_0, V4_4_1]
+                          V4_4_0, V4_4_1, V4_5_1]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_mesh_prepare.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_flex_mesh_prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from pyworkflow import BETA
-from pyworkflow.protocol.params import (PointerParam, FloatParam, IntParam,
-                                        BooleanParam, FileParam, StringParam)
+from pyworkflow.protocol.params import (PointerParam, FloatParam, BooleanParam, FileParam, StringParam)
 from . import ProtCryosparcBase
 from ..convert import *
 from ..utils import *
 from ..constants import *
 
 
 class ProtCryoSparc3DFlexMeshPrepare(ProtCryosparcBase):
@@ -39,15 +38,15 @@
     Prepares particles for use in 3DFlex training and reconstruction. At the same
     way,  Takes in a consensus (rigid) refinement density map, plus optionally
      a segmentation and generates a tetrahedral mesh for 3DFlex.
     """
     _label = '3D flex mesh prepare'
     _devStatus = BETA
     _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1,
-                          V4_4_0, V4_4_1]
+                          V4_4_0, V4_4_1, V4_5_1]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 from pwem.objects import Volume
 from pyworkflow import BETA
-from pyworkflow.protocol.params import (PointerParam,  IntParam,  BooleanParam)
+from pyworkflow.protocol.params import (PointerParam,  BooleanParam)
 from . import ProtCryosparcBase
 from ..convert import *
 from ..utils import *
 from ..constants import *
 
 
 class ProtCryoSparc3DFlexReconstruction(ProtCryosparcBase):
@@ -39,15 +39,15 @@
     particles and performs high-resolution refinement using L-BFGS under
     the 3DFlex model. This is the stage at which improvements to density
     in high-res regions are computed. Outputs two half-maps that can be used
     for FSC validation, sharpening, and other downstream tasks.
     """
     _label = '3D flex reconstruction'
     _devStatus = BETA
-    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
+    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1, V4_5_1]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,35 +20,43 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+from enum import Enum
 
+from pwem import getMatchingFiles
+from pwem.objects import ParticleFlex, SetOfParticles, SetOfParticlesFlex
+from pwem.protocols import ProtFlexBase
 from pyworkflow import BETA
 from pyworkflow.protocol import LEVEL_ADVANCED
-from pyworkflow.protocol.params import (PointerParam, FloatParam, IntParam,
+from pyworkflow.protocol.params import (PointerParam, FloatParam,
                                         BooleanParam)
 from . import ProtCryosparcBase
 from ..convert import *
 from ..utils import *
 from ..constants import *
 
 
-class ProtCryoSparc3DFlexTraining(ProtCryosparcBase):
+class outputs(Enum):
+    Particles = SetOfParticles
+
+class ProtCryoSparc3DFlexTraining(ProtCryosparcBase, ProtFlexBase):
     """
     Uses a mesh and prepared particles (at a downsampled resolution) to train
     a 3DFlex model. Parameters control the number of latent dimensions,
     size of the model, and training hyperparameters. This job outputs
     checkpoints during training.
     """
     _label = '3D flex training'
     _devStatus = BETA
-    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
+    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1, V4_5_1]
+    _possibleOutputs = outputs
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
@@ -149,15 +157,15 @@
                            "coordinates are very concentrated around (0,0) "
                            "then this value should be decreased.")
 
         form.addParam('flex_latent_prior_pow', FloatParam, default=4.0,
                       label="Latent centering pow",
                       expertLevel=LEVEL_ADVANCED)
 
-        form.addParam('flex_latent_ext_init', BooleanParam, default=False,
+        form.addParam('flex_latent_ext_init', BooleanParam, default=True,
                       label="Initialize latents from input",
                       expertLevel=LEVEL_ADVANCED)
 
         """
         job.param_add('flex_train', "flex_latent_ext_init_idxs",base_value=None,   title="Initialize latents input indices",  param_type="string", desc="Comma separated list of (zero-based) indices for which input components to use for initializing latent coordinates. This list should be the same length as the latent dimension specified.")
 
         job.param_add('flex_train', "flex_force_restart", base_value=False,  title="Restart training",  param_type="boolean", desc="Force restart of training even if a model with trained checkpoint is connected.", hidden=True)
@@ -176,15 +184,74 @@
         self._insertFunctionStep(self.createOutputStep)
 
     def trainingStep(self):
         self.info(pwutils.yellowStr("3D Flex Training started..."))
         self.doRun3DFlexTraining()
 
     def createOutputStep(self):
-        pass
+        self._initializeUtilsVariables()
+        self.info(pwutils.yellowStr("Creating the output..."))
+
+        csOutputFolder = os.path.join(self.projectDir.get(),
+                                      self.run3DFlexTrainJob.get())
+
+        pattern = csOutputFolder + '/*latents*'
+        csParticlesName = os.path.basename(getMatchingFiles(pattern, True)[-1])
+
+        pattern = csOutputFolder + '/*train_checkpoint*.tar'
+        trainModelRar = os.path.basename(getMatchingFiles(pattern, True)[-1])
+
+        pattern = csOutputFolder + '/*train_checkpoint*.cs'
+        trainModelCs = os.path.basename(getMatchingFiles(pattern, True)[-1])
+
+
+        # Copy the CS output particles to extra folder
+        copyFiles(csOutputFolder, self._getExtraPath(), files=[csParticlesName, trainModelRar, trainModelCs])
+        csPartFile = os.path.join(self._getExtraPath(), csParticlesName)
+
+        # Taking the zvalues from the .cs file using numpy
+        arr = np.load(csPartFile)
+        zValues = [[arr[i][j] for j in range(2, len(arr[i]), 2)] for i in range(len(arr))]
+
+        inputSet = self.input3DFlexDataPrepareProt.get()._getInputParticles()
+        outImgSet = SetOfParticlesFlex.create(self._getPath(), suffix='', progName=CRYOSPARCFLEX)
+
+        outImgSet.copyInfo(inputSet)
+        outImgSet.setHasCTF(inputSet.hasCTF())
+        outImgSet.getFlexInfo().setProgName(CRYOSPARCFLEX)
+        outImgSet.getFlexInfo().setAttr('projectId', str(self.projectName.get()))
+        outImgSet.getFlexInfo().setAttr('workSpaceId', str(self.workSpaceName.get()))
+        outImgSet.getFlexInfo().setAttr('trainJobId', str(self.run3DFlexTrainJob.get()))
+        outImgSet.getFlexInfo().setAttr('projectPath', self.projectDir.get())
+
+        for particle, zValue in zip(inputSet, zValues):
+            outParticle = ParticleFlex(progName=CRYOSPARCFLEX)
+            outParticle.copyInfo(particle)
+            outParticle.getFlexInfo().setProgName(CRYOSPARCFLEX)
+
+            outParticle.setZFlex(list(zValue))
+
+            outImgSet.append(outParticle)
+
+        self._defineOutputs(**{outputs.Particles.name: outImgSet})
+        self._defineSourceRelation(inputSet, outImgSet)
+
+        # This is an example to create a latent trajectory in order to launch the flex generator job
+        # arr = np.stack([zValues[20], zValues[21]], axis=0)
+        # latentTrajectoryJob = customLatentTrajectory(arr,
+        #                                              str(self.projectName.get()),
+        #                                              str(self.workSpaceName.get()),
+        #                                              str(self.run3DFlexTrainJob.get()))
+        #
+        # flexGeneratorJob = runFlexGeneratorJob(str(self.run3DFlexTrainJob.get()),
+        #                                        latentTrajectoryJob,
+        #                                        str(self.projectName.get()),
+        #                                        str(self.workSpaceName.get()))
+
+
 
     def _defineParamsName(self):
         """ Define a list with 3D Flex Training parameters names"""
         self._paramsName = ['flex_K', 'flex_num_layers', 'flex_num_layers',
                         'flex_hidden_units', 'flex_lr_flex_init',
                         'flex_lr_flex_final', 'flex_lr_density_init',
                         'flex_lr_density_final', 'flex_sv_lam',
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3d_variability.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3d_variability.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 from pyworkflow import BETA
 from pyworkflow.protocol.params import (PointerParam, FloatParam, Positive,
-                                        IntParam, BooleanParam, EnumParam)
+                                        BooleanParam, EnumParam)
 from pwem.objects import Volume
 from pwem.protocols import ProtRefine3D
 
 from . import ProtCryosparcBase
 from ..convert import *
 from ..utils import *
 from ..constants import *
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_ab.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_ab.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_blob_picker.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_blob_picker.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     Wrapper protocol for the Cryosparc's per-particle Global CTF refinement.
     Performs per-exposure-group CTF parameter refinement of higher-order
     aberrations, against a given 3D reference
     """
     _label = 'global ctf refinement'
     _className = "ctf_refine_global"
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
+                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1, V4_5_1]
     newParamsName = []
 
     def _initialize(self):
         self._createFilenameTemplates()
 
     def _createFilenameTemplates(self):
         """ Centralize how files are called. """
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,25 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from pkg_resources import parse_version
-
 from pwem import SCIPION_SYM_NAME
 
 import pyworkflow.utils as pwutils
-from pyworkflow import BETA
 from pyworkflow.object import String
 from pyworkflow.protocol.params import (FloatParam, Positive, IntParam,
                                         BooleanParam, EnumParam, PointerParam)
 
 from .protocol_cryosparc_homogeneous_refine import ProtCryoSparc3DHomogeneousRefine
 from ..utils import (getSymmetry, enqueueJob, waitForCryosparc,
                      clearIntermediateResults, addComputeSectionParams,
-                     cryosparcValidate, gpusValidate, getCryosparcVersion)
+                     cryosparcValidate, gpusValidate)
 from ..constants import *
 
 
 class ProtCryoSparcHelicalRefine3D(ProtCryoSparc3DHomogeneousRefine):
     """ Reconstruct and refine a homogeneous helical assembly, with or without
     imposition and refinement of symmetry parameters. Helical Refinement (BETA)
     uses an algorithm that is conceptually similar to Egelman's Iterative
@@ -50,15 +47,15 @@
     the same maximum likelihood framework, accelerated branch-and-bound
     alignment algorithm, and optional Non-Uniform regularization as used in
     other cryoSPARC refinement jobs.
     """
     _label = '3D helical refinement'
     _fscColumns = 4
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1, V4_5_1]
     _className = "helix_refine"
 
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputParticles', PointerParam,
                       pointerClass='SetOfParticles',
                       label="Input particles", important=True,
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """
     _label = 'homogeneous reconstruction'
     _className = "homo_reconstruct"
     _devStatus = NEW
     _fscColumns = 6
     _protCompatibility = [V3_3_0, V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2,
                           V4_0_3, V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1,
-                          V4_3_1, V4_4_0, V4_4_1]
+                          V4_3_1, V4_4_0, V4_4_1, V4_5_1]
     ewsParamsName = []
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
         """ Centralize how files are called. """
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 # **************************************************************************
 import os
 import emtable
 from pkg_resources import parse_version
 
 import pwem.objects as pwobj
 import pyworkflow.utils as pwutils
-from pwem.convert import moveParticlesInsideUnitCell, getSymmetryMatrices, \
-    getUnitCell
+from pwem.convert import getSymmetryMatrices, getUnitCell
 from pwem.convert.symmetry import moveParticleInsideUnitCell
 from pyworkflow.protocol.params import *
 
 from .protocol_base import ProtCryosparcBase
 from ..convert import (convertCs2Star, createItemMatrix,
                        setCryosparcAttributes)
 from ..utils import (addSymmetryParam, addComputeSectionParams,
@@ -56,15 +55,15 @@
         the fly.
     """
     _label = '3D homogeneous refinement'
     _fscColumns = 6
     _className = "homo_refine_new"
     ewsParamsName = []
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
+                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1, V4_5_1]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import os
 
 import emtable
 from pkg_resources import parse_version
 
 import pyworkflow.utils as pwutils
 from pwem.objects import VolumeMask
-from pyworkflow import BETA
 from pyworkflow.object import String
 from pyworkflow.protocol.params import (FloatParam, LEVEL_ADVANCED,
                                         PointerParam, MultiPointerParam,
                                         CsvList, Positive, IntParam,
                                         BooleanParam, EnumParam)
 
 from .protocol_base import ProtCryosparcBase
@@ -57,23 +56,23 @@
     implements a version of 3D classification without alignment — a
     classification routine that can complement the existing Heterogeneous
     Refinement job in finding new discrete classes of data.
     """
     _label = '3D Classification'
     _className = "class_3D"
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1, V4_5_1]
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
         """ Centralize how files are called. """
         myDict = {
-            'input_particles': self._getTmpPath('input_particles.star'),
+            'input_particles': self._getPath('input_particles.star'),
             'out_particles': self._getExtraPath('output_particle.star'),
             'stream_log': self._getPath() + '/stream.log',
             'out_class': self._getExtraPath() + '/output_class.star'
         }
         self._updateFilenamesDict(myDict)
 
     def _defineParams(self, form):
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,44 +24,42 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 
 import emtable
-from pkg_resources import parse_version
 
 from pwem import ALIGN_PROJ
 from pwem.protocols import ProtOperateParticles
 
 import pyworkflow.utils as pwutils
-from pyworkflow import NEW
 from pyworkflow.object import String
 from pyworkflow.protocol.params import (PointerParam, FloatParam, IntParam,
                                         Positive, BooleanParam, EnumParam)
 from pwem.objects import Volume
 
 from .protocol_base import ProtCryosparcBase
 from ..convert import (convertCs2Star, createItemMatrix,
                        setCryosparcAttributes)
 from ..utils import (addComputeSectionParams, calculateNewSamplingRate,
                      cryosparcValidate, gpusValidate, enqueueJob,
                      waitForCryosparc, clearIntermediateResults,
-                     addSymmetryParam, getCryosparcVersion, getSymmetry,
+                     addSymmetryParam, getSymmetry,
                      fixVolume, copyFiles, getOutputPreffix)
 from ..constants import *
 
 
 class ProtCryoSparcLocalRefine(ProtCryosparcBase, ProtOperateParticles):
     """ Signal subtraction protocol of cryoSPARC.
         Subtract projections of a masked volume from particles.
         """
     _label = 'local refinement'
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0,  V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1, V4_5_1]
     _className = "new_local_refine"
     _fscColumns = 6
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_part_subtract.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_part_subtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_patch_ctf_estimation.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_patch_ctf_estimation.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_sharppening.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_sharppening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols.conf` & `scipion-em-cryosparc2-4.1.1/cryosparc2/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/tests/__init__.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/tests/test_protocols_cryosparc2.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/tests/test_protocols_cryosparc2.py`

 * *Files 3% similar despite different names*

```diff
@@ -341,14 +341,16 @@
             prot3DHomoRefinement = self.newProtocol(ProtCryoSparc3DHomogeneousRefine)
 
             prot3DHomoRefinement.inputParticles.set(self.protImportPart.outputParticles)
             prot3DHomoRefinement.referenceVolume.set(self.protImportVol.outputVolume)
             prot3DHomoRefinement.symmetryGroup.set(SYM_CYCLIC)
             prot3DHomoRefinement.symmetryOrder.set(1)
             prot3DHomoRefinement.compute_use_ssd.set(False)
+            prot3DHomoRefinement.refine_defocus_refine.set(False)
+            prot3DHomoRefinement.refine_ctf_global_refine.set(False)
             prot3DHomoRefinement.setObjLabel(label)
             self.launchProtocol(prot3DHomoRefinement)
 
             # Check the outputs, sampling rate,...
             self.assertIsNotNone(prot3DHomoRefinement.outputVolume)
             self.assertEqual(prot3DHomoRefinement.outputVolume.getSamplingRate(),
                              self.protImportPart.outputParticles.getSamplingRate())
@@ -361,53 +363,15 @@
             self.assertTrue(outputParticles.hasCTF())
             self.assertEqual(outputParticles.getSize(),
                              self.protImportPart.outputParticles.getSize())
 
         _runCryosparctest3DHomogeneousRefinement(label="Cryosparc 3D homogeneous refinement")
 
 
-# class TestCryosparcNonUniformRefine3D(TestCryosparcBase):
-#
-#     @classmethod
-#     def setUpClass(cls):
-#         setupTestProject(cls)
-#         setupTestProject(cls)
-#         dataProject = 'grigorieff'
-#         dataset = DataSet.getDataSet(dataProject)
-#         TestCryosparcBase.setData()
-#         particlesPattern = dataset.getFile('particles.sqlite')
-#         cls.protImportPart = cls.runImportParticleCryoSPARC(cls.partFn2)
-#         cls.protImportVolumeVol = cls.runImportVolumesCryoSPARC(cls.volFn)
-#
-#     def testCryosparcNonUniformRefine3D(self):
-#         def _runCryosparctestNonUniformRefine3D(label=''):
-#             protNonUniform3DRefinement = self.newProtocol(ProtCryoSparcNonUniformRefine3D)
-#             protNonUniform3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
-#             protNonUniform3DRefinement.referenceVolume.set(self.protImportVolumeVol.outputVolume)
-#             protNonUniform3DRefinement.symmetryGroup.set(SYM_CYCLIC)
-#             protNonUniform3DRefinement.symmetryOrder.set(1)
-#             protNonUniform3DRefinement.compute_use_ssd.set(False)
-#             protNonUniform3DRefinement.setObjLabel(label)
-#             self.launchProtocol(protNonUniform3DRefinement)
-#
-#             # Check the outputs, dimensions, sampling rate,...
-#             self.assertIsNotNone(protNonUniform3DRefinement.outputVolume)
-#             self.assertEqual(protNonUniform3DRefinement.outputVolume.getSamplingRate(),
-#                              self.protImportPart.outputParticles.getSamplingRate())
-#
-#             outputParticles = protNonUniform3DRefinement.outputParticles
-#             self.assertIsNotNone(outputParticles)
-#             self.assertEqual(outputParticles.getSamplingRate(),
-#                              self.protImportPart.outputParticles.getSamplingRate())
-#             self.assertTrue(outputParticles.hasAlignmentProj())
-#             self.assertTrue(outputParticles.hasCTF())
-#             self.assertEqual(outputParticles.getSize(),
-#                              self.protImportPart.outputParticles.getSize())
-#
-#         _runCryosparctestNonUniformRefine3D(label="Cryosparc Non-Uniform 3D refinement")
+
 
 
 class TestCryosparcNewNonUniformRefine3D(TestCryosparcBase):
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
@@ -423,14 +387,16 @@
         def _runCryosparctestNewNonUniformRefine3D(label=''):
             protNewNonUniform3DRefinement = self.newProtocol(ProtCryoSparcNewNonUniformRefine3D)
             protNewNonUniform3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             protNewNonUniform3DRefinement.referenceVolume.set(self.protImportVolumeVol.outputVolume)
             protNewNonUniform3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             protNewNonUniform3DRefinement.symmetryOrder.set(1)
             protNewNonUniform3DRefinement.compute_use_ssd.set(False)
+            protNewNonUniform3DRefinement.refine_defocus_refine.set(False)
+            protNewNonUniform3DRefinement.refine_ctf_global_refine.set(False)
             protNewNonUniform3DRefinement.setObjLabel(label)
             self.launchProtocol(protNewNonUniform3DRefinement)
 
             # Check the outputs, dimensions, sampling rate,...
             self.assertIsNotNone(protNewNonUniform3DRefinement.outputVolume)
             self.assertEqual(protNewNonUniform3DRefinement.outputVolume.getSamplingRate(),
                              self.protImportPart.outputParticles.getSamplingRate())
@@ -505,26 +471,30 @@
             # Launch a first refinement protocol
             protNonUniform3DRefinement = self.newProtocol(ProtCryoSparcNewNonUniformRefine3D)
             protNonUniform3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             protNonUniform3DRefinement.referenceVolume.set(self.protImportVolumeVol.outputVolume)
             protNonUniform3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             protNonUniform3DRefinement.symmetryOrder.set(1)
             protNonUniform3DRefinement.compute_use_ssd.set(False)
+            protNonUniform3DRefinement.refine_defocus_refine.set(False)
+            protNonUniform3DRefinement.refine_ctf_global_refine.set(False)
             protNonUniform3DRefinement.setObjLabel("protNonUniform3DRefinement_1")
             self.launchProtocol(protNonUniform3DRefinement)
             self.assertIsNotNone(protNonUniform3DRefinement.outputVolume)
 
             # Launch a second refinement protocol
             protNonUniform3DRefinement1 = self.newProtocol(ProtCryoSparcNewNonUniformRefine3D)
 
             protNonUniform3DRefinement1.inputParticles.set(self.protImportPart.outputParticles)
             protNonUniform3DRefinement1.referenceVolume.set(self.protImportVolumeVol.outputVolume)
             protNonUniform3DRefinement1.symmetryGroup.set(SYM_CYCLIC)
             protNonUniform3DRefinement1.symmetryOrder.set(1)
             protNonUniform3DRefinement1.compute_use_ssd.set(False)
+            protNonUniform3DRefinement1.refine_defocus_refine.set(False)
+            protNonUniform3DRefinement1.refine_ctf_global_refine.set(False)
             protNonUniform3DRefinement1.setObjLabel("protNonUniform3DRefinement_2")
             self.launchProtocol(protNonUniform3DRefinement1)
             self.assertIsNotNone(protNonUniform3DRefinement1.outputVolume)
 
             unionProt = self.newProtocol(ProtUnionSet)
             # Set the input volumes
             unionProt.inputSets.append(protNonUniform3DRefinement.outputParticles)
@@ -578,14 +548,16 @@
             # Launch a refinement protocol
             protNonUniform3DRefinement = self.newProtocol(ProtCryoSparcNewNonUniformRefine3D)
             protNonUniform3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             protNonUniform3DRefinement.referenceVolume.set(self.protImportVol.outputVolume)
             protNonUniform3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             protNonUniform3DRefinement.symmetryOrder.set(1)
             protNonUniform3DRefinement.compute_use_ssd.set(False)
+            protNonUniform3DRefinement.refine_defocus_refine.set(False)
+            protNonUniform3DRefinement.refine_ctf_global_refine.set(False)
             protNonUniform3DRefinement.setObjLabel("protNonUniform3DRefinement")
             self.launchProtocol(protNonUniform3DRefinement)
             self.assertIsNotNone(protNonUniform3DRefinement.outputVolume)
 
             protParticlesSubtract = self.newProtocol(ProtCryoSparcSubtract)
 
             prot3DRefinement = self.newProtocol(ProtCryoSparcLocalRefine)
@@ -628,14 +600,16 @@
             protSharppening = self.newProtocol(ProtCryoSparcSharppening)
             prot3DRefinement = self.newProtocol(ProtCryoSparc3DHomogeneousRefine)
             prot3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             prot3DRefinement.referenceVolume.set(self.protImportVol.outputVolume)
             prot3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             prot3DRefinement.symmetryOrder.set(1)
             prot3DRefinement.compute_use_ssd.set(False)
+            prot3DRefinement.refine_defocus_refine.set(False)
+            prot3DRefinement.refine_ctf_global_refine.set(False)
             self.launchProtocol(prot3DRefinement)
             
             protSharppening.refVolume.set(prot3DRefinement.outputVolume)
             protSharppening.sharp_bfactor.set(-80)
             protSharppening.compute_use_ssd.set(False)
             self.launchProtocol(protSharppening)
 
@@ -669,22 +643,25 @@
 
             prot3DRefinement = self.newProtocol(ProtCryoSparc3DHomogeneousRefine)
             prot3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             prot3DRefinement.referenceVolume.set(self.protImportVol.outputVolume)
             prot3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             prot3DRefinement.symmetryOrder.set(1)
             prot3DRefinement.compute_use_ssd.set(False)
+            prot3DRefinement.refine_defocus_refine.set(False)
+            prot3DRefinement.refine_ctf_global_refine.set(False)
             self.launchProtocol(prot3DRefinement)
 
             # Create a 3D Mask using xmipp
             protXmippCreate3DMask = self.runCreate3DMask(prot3DRefinement.outputVolume)
 
             protGlobalCtfRefinement.inputParticles.set(prot3DRefinement.outputParticles)
             protGlobalCtfRefinement.refVolume.set(prot3DRefinement.outputVolume)
             protGlobalCtfRefinement.refMask.set(protXmippCreate3DMask.outputMask)
+            protGlobalCtfRefinement.crg_min_res_A.set(400)
             protGlobalCtfRefinement.compute_use_ssd.set(False)
             self.launchProtocol(protGlobalCtfRefinement)
 
             return protGlobalCtfRefinement
 
         def _checkAsserts(cryosparcProt):
             self.assertIsNotNone(cryosparcProt.outputParticles,
@@ -714,22 +691,25 @@
 
             prot3DRefinement = self.newProtocol(ProtCryoSparc3DHomogeneousRefine)
             prot3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             prot3DRefinement.referenceVolume.set(self.protImportVol.outputVolume)
             prot3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             prot3DRefinement.symmetryOrder.set(1)
             prot3DRefinement.compute_use_ssd.set(False)
+            prot3DRefinement.refine_defocus_refine.set(False)
+            prot3DRefinement.refine_ctf_global_refine.set(False)
             self.launchProtocol(prot3DRefinement)
 
             # Create a 3D Mask using xmipp
             protXmippCreate3DMask = self.runCreate3DMask(prot3DRefinement.outputVolume)
 
             protLocalCtfRefinement.inputParticles.set(prot3DRefinement.outputParticles)
             protLocalCtfRefinement.refVolume.set(prot3DRefinement.outputVolume)
             protLocalCtfRefinement.refMask.set(protXmippCreate3DMask.outputMask)
+            protLocalCtfRefinement.crl_min_res_A.set(400)
             protLocalCtfRefinement.compute_use_ssd.set(False)
             self.launchProtocol(protLocalCtfRefinement)
 
             return protLocalCtfRefinement
 
         def _checkAsserts(cryosparcProt):
             self.assertIsNotNone(cryosparcProt.outputParticles,
@@ -759,14 +739,16 @@
 
             prot3DRefinement = self.newProtocol(ProtCryoSparc3DHomogeneousRefine)
             prot3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             prot3DRefinement.referenceVolume.set(self.protImportVol.outputVolume)
             prot3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             prot3DRefinement.symmetryOrder.set(1)
             prot3DRefinement.compute_use_ssd.set(False)
+            prot3DRefinement.refine_defocus_refine.set(False)
+            prot3DRefinement.refine_ctf_global_refine.set(False)
             self.launchProtocol(prot3DRefinement)
 
             protSymExp.inputParticles.set(prot3DRefinement.outputParticles)
             protSymExp.symmetryGroup.set(SYM_CYCLIC)
             protSymExp.symmetryOrder.set(4)
             protSymExp.compute_use_ssd.set(False)
             self.launchProtocol(protSymExp)
@@ -779,59 +761,14 @@
             self.assertEqual(cryosparcProt.outputParticles.getSize(),
                              self.protImportPart.outputParticles.getSize()*4)
 
         cryosparcProtGpu = _runCryosparctestSymetryExpansion(label="Cryosparc Symmetry Expansion")
         _checkAsserts(cryosparcProtGpu)
 
 
-# class TestCryosparcNaiveLocalRefine(TestCryosparcBase):
-#
-#     @classmethod
-#     def setUpClass(cls):
-#         setupTestProject(cls)
-#         setupTestProject(cls)
-#         dataProject = 'grigorieff'
-#         dataset = DataSet.getDataSet(dataProject)
-#         TestCryosparcBase.setData()
-#         particlesPattern = dataset.getFile('particles.sqlite')
-#         cls.protImportPart = cls.runImportParticleCryoSPARC(cls.partFn2)
-#         cls.protImportVol = cls.runImportVolumesCryoSPARC(cls.volFn)
-#
-#     def testCryosparcNaiveLocalRefine(self):
-#         def _runCryosparctestNaiveLocalRefine(label=''):
-#
-#             protLocalRefine = self.newProtocol(ProtCryoSparcNaiveLocalRefine)
-#
-#             prot3DRefinement = self.newProtocol(ProtCryoSparcRefine3D)
-#             prot3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
-#             prot3DRefinement.referenceVolume.set(self.protImportVol.outputVolume)
-#             prot3DRefinement.symmetryGroup.set(SYM_CYCLIC)
-#             prot3DRefinement.symmetryOrder.set(1)
-#             prot3DRefinement.compute_use_ssd.set(False)
-#             self.launchProtocol(prot3DRefinement)
-#
-#             # Create a 3D Mask using xmipp
-#             protXmippCreate3DMask = self.runCreate3DMask(prot3DRefinement.outputVolume)
-#
-#             protLocalRefine.inputParticles.set(prot3DRefinement.outputParticles)
-#             protLocalRefine.refVolume.set(prot3DRefinement.outputVolume)
-#             protLocalRefine.refMask.set(protXmippCreate3DMask.outputMask)
-#             protLocalRefine.compute_use_ssd.set(False)
-#             self.launchProtocol(protLocalRefine)
-#
-#             return protLocalRefine
-#
-#         def _checkAsserts(cryosparcProt):
-#             self.assertIsNotNone(cryosparcProt.outputParticles,
-#                                  "There was a problem with Cryosparc subtract projection")
-#
-#         cryosparcProtGpu = _runCryosparctestNaiveLocalRefine(label="Cryosparc Local Refine")
-#         _checkAsserts(cryosparcProtGpu)
-
-
 class TestCryosparcLocalRefine(TestCryosparcBase):
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         setupTestProject(cls)
         dataProject = 'grigorieff'
@@ -848,14 +785,16 @@
 
             prot3DRefinement = self.newProtocol(ProtCryoSparc3DHomogeneousRefine)
             prot3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             prot3DRefinement.referenceVolume.set(self.protImportVol.outputVolume)
             prot3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             prot3DRefinement.symmetryOrder.set(1)
             prot3DRefinement.compute_use_ssd.set(False)
+            prot3DRefinement.refine_defocus_refine.set(False)
+            prot3DRefinement.refine_ctf_global_refine.set(False)
             self.launchProtocol(prot3DRefinement)
 
             # Create a 3D Mask using xmipp
             protXmippCreate3DMask = self.runCreate3DMask(prot3DRefinement.outputVolume)
 
             protLocalRefine.inputParticles.set(prot3DRefinement.outputParticles)
             protLocalRefine.refVolume.set(prot3DRefinement.outputVolume)
@@ -895,14 +834,16 @@
 
             prot3DRefinement = self.newProtocol(ProtCryoSparc3DHomogeneousRefine)
             prot3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             prot3DRefinement.referenceVolume.set(self.protImportVol.outputVolume)
             prot3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             prot3DRefinement.symmetryOrder.set(1)
             prot3DRefinement.compute_use_ssd.set(False)
+            prot3DRefinement.refine_defocus_refine.set(False)
+            prot3DRefinement.refine_ctf_global_refine.set(False)
             self.launchProtocol(prot3DRefinement)
 
             protHomogeneousReconst = self.newProtocol(ProtCryoSparcHomogeneousReconstruct)
             protHomogeneousReconst.inputParticles.set(prot3DRefinement.outputParticles)
             protHomogeneousReconst.refMask.set(self.protXmippCreate3DMask.outputMask)
             self.launchProtocol(protHomogeneousReconst)
 
@@ -934,38 +875,44 @@
             # Launch a first refinement protocol
             protNonUniform3DRefinement = self.newProtocol(ProtCryoSparcNewNonUniformRefine3D)
             protNonUniform3DRefinement.inputParticles.set(self.protImportPart.outputParticles)
             protNonUniform3DRefinement.referenceVolume.set(self.protImportVolumeVol.outputVolume)
             protNonUniform3DRefinement.symmetryGroup.set(SYM_CYCLIC)
             protNonUniform3DRefinement.symmetryOrder.set(1)
             protNonUniform3DRefinement.compute_use_ssd.set(False)
+            protNonUniform3DRefinement.refine_defocus_refine.set(False)
+            protNonUniform3DRefinement.refine_ctf_global_refine.set(False)
             protNonUniform3DRefinement.setObjLabel("protNonUniform3DRefinement_1")
             self.launchProtocol(protNonUniform3DRefinement)
             self.assertIsNotNone(protNonUniform3DRefinement.outputVolume)
 
             # Launch a second refinement protocol
             protNonUniform3DRefinement1 = self.newProtocol(ProtCryoSparcNewNonUniformRefine3D)
 
             protNonUniform3DRefinement1.inputParticles.set(self.protImportPart.outputParticles)
             protNonUniform3DRefinement1.referenceVolume.set(self.protImportVolumeVol.outputVolume)
             protNonUniform3DRefinement1.symmetryGroup.set(SYM_CYCLIC)
             protNonUniform3DRefinement1.symmetryOrder.set(1)
             protNonUniform3DRefinement1.compute_use_ssd.set(False)
+            protNonUniform3DRefinement1.refine_defocus_refine.set(False)
+            protNonUniform3DRefinement1.refine_ctf_global_refine.set(False)
             protNonUniform3DRefinement1.setObjLabel("protNonUniform3DRefinement_2")
             self.launchProtocol(protNonUniform3DRefinement1)
             self.assertIsNotNone(protNonUniform3DRefinement1.outputVolume)
 
             # Launch a second refinement protocol
             protNonUniform3DRefinement2 = self.newProtocol(ProtCryoSparcNewNonUniformRefine3D)
 
             protNonUniform3DRefinement2.inputParticles.set(self.protImportPart.outputParticles)
             protNonUniform3DRefinement2.referenceVolume.set(self.protImportVolumeVol.outputVolume)
             protNonUniform3DRefinement2.symmetryGroup.set(SYM_CYCLIC)
             protNonUniform3DRefinement2.symmetryOrder.set(1)
             protNonUniform3DRefinement2.compute_use_ssd.set(False)
+            protNonUniform3DRefinement2.refine_defocus_refine.set(False)
+            protNonUniform3DRefinement2.refine_ctf_global_refine.set(False)
             protNonUniform3DRefinement2.setObjLabel("protNonUniform3DRefinement_3")
             self.launchProtocol(protNonUniform3DRefinement2)
             self.assertIsNotNone(protNonUniform3DRefinement2.outputVolume)
 
             # Launch a join set
             unionProt = self.newProtocol(ProtUnionSet)
             # Set the input volumes
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/tests/test_utils.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/utils.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,18 +167,21 @@
         logger.info(pwutils.yellowStr("cryoSPARC %s is newer than those we've tested %s. Instead of blocking the "
                                 "execution, we are allowing this to run assuming compatibility is not broken."
                                 "If it fails, please consider:\n A - upgrade the plugin, there might be an update.\n "
                                 "B - downgrade cryosparc version.\n C - Contact plugin maintainers"
                                 " at https://github.com/scipion-em/scipion-em-cryosparc2"
                                 % (cryosparcVersion, str(supportedVersions).replace('\'', ''))))
 
-    if cryosparcVersion >= parse_version(V4_1_0) and not userExist(os.environ.get(CRYOSPARC_USER)):
-        return ["You need to define the cryoSPARC user variable "
-                "(CRYOSPARC_USER) in the Scipion config file. Note that the "
-                "cryoSPARC username is the email address."]
+    if cryosparcVersion >= parse_version(V4_1_0):
+        if not os.environ.get(CRYOSPARC_USER):
+            return ["You need to define the cryoSPARC user variable "
+                    "(CRYOSPARC_USER) in the Scipion config file. Note that the "
+                    "cryoSPARC username is the email address."]
+        elif not userExist(os.environ.get(CRYOSPARC_USER)):
+            return ["The user defined in the Scipion config file does not exist within CS."]
 
     return []
 
 
 def gpusValidate(gpuList, checkSingleGPU=False):
     """
     Validate a gpu list
@@ -361,14 +364,15 @@
 def getProjectInformation(project_uid, info='project_dir'):
     """
     Get information about a single project
     :param project_uid: the id of the project
     :return: the information related to the project that's stored in the database
     """
     import ast
+    from cryosparc.tools import CryoSPARC
     getProject_cmd = (getCryosparcProgram() +
                                 ' %sget_project("%s")%s '
                                 % ("'", str(project_uid), "'"))
 
     project_info = runCmd(getProject_cmd, printCmd=False)
     dictionary = ast.literal_eval(project_info[1])
     return str(dictionary[info])
@@ -440,15 +444,15 @@
     returns the new uid of the job that was created
     """
     print(pwutils.yellowStr("Importing particles..."), flush=True)
     className = "import_particles"
     params = {"particle_meta_path": str(os.path.join(os.getcwd(),
                                                      protocol._getFileName('input_particles'))),
               "particle_blob_path": str(os.path.join(os.getcwd(),
-                                                     protocol._getTmpPath())),
+                                                     protocol._getPath())),
               "psize_A": str(protocol._getInputParticles().getSamplingRate())
               }
 
     import_particles = enqueueJob(className, protocol.projectName, protocol.workSpaceName,
                                   str(params).replace('\'', '"'), '{}', protocol.lane)
 
     waitForCryosparc(protocol.projectName.get(), import_particles.get(),
@@ -649,27 +653,125 @@
                                ("'", projectName, jobId,
                                 lane, user, "'"))
     runCmd(enqueue_job_cmd)
 
     return jobId
 
 
+def customLatentTrajectory(latentsPoints, projectId, workspaceId, trainingJobId):
+    """Output the trajectory as a new output in CryoSPARC.
+       The resulting trajectory may be used as input to the 3D Flex Generator job
+       to generate a volume series along the trajectory."""
+    from cryosparc.tools import CryoSPARC
+
+    credentials = _getCredentials()
+    if not credentials[0]:
+        logger.error("Error obtaining cryoSPARC's credentials: %s" % credentials[1])
+        raise Exception("Error obtaining cryoSPARC's credentials: %s" % credentials[1])
+
+    credentials = credentials[1]
+    cs = CryoSPARC(license=credentials['license'],
+                   host=credentials['host'],
+                   base_port=int(credentials['base_port']),
+                   email=credentials['email'],
+                   password=credentials['password'])
+
+    project = cs.find_project(projectId)
+    particles = project.find_job(trainingJobId).load_output("particles")
+    numComponents = int(len([x for x in particles.fields() if "components_mode" in x]) / 2)
+    slot_spec = [{"dtype": "components", "prefix": f"components_mode_{k}", "required": True} for k in
+                 range(numComponents)]
+    job = project.create_external_job(workspaceId, "Custom Latents")
+    job.connect("particles", trainingJobId, "particles", slots=slot_spec)
+
+    if len(latentsPoints.shape) == 1:
+        latentsPoints = latentsPoints[None, ...]
+
+    latentsDSet = job.add_output(
+        type="particle",
+        name="latents",
+        slots=slot_spec,
+        title="Latents",
+        alloc=len(latentsPoints),
+    )
+
+    for k in range(numComponents):
+        latentsDSet[f"components_mode_{k}/component"] = k
+        latentsDSet[f"components_mode_{k}/value"] = latentsPoints[:, k]
+
+    # Save the output
+    with job.run():
+        job.save_output("latents", latentsDSet)
+
+    return job.uid
+
+
+def runFlexGeneratorJob(trainingJobId, customLatentsJobId, projectId, workspaceId, gpu=0, lane='default'):
+    """Generate a volume series along the trajectory using a flex model."""
+    className = "flex_generate"
+    gpusToUse = [gpu]
+    input_group_connect = {"flex_model": "%s.flex_model" % trainingJobId,
+                           "latents": "%s.latents" % customLatentsJobId}
+    params = {}
+
+    run3DFlexGeneratorJob = enqueueJob(className,
+                                       projectId,
+                                       workspaceId,
+                                       str(params).replace('\'', '"'),
+                                       str(input_group_connect).replace('\'', '"'),
+                                       lane, gpusToUse)
+
+    waitForCryosparc(projectId,
+                     run3DFlexGeneratorJob,
+                     "An error occurred in the 3D Flex Training process. "
+                     "Please, go to cryoSPARC software for more "
+                     "details.")
+    clearIntermediateResults(projectId,
+                             run3DFlexGeneratorJob)
+
+    return run3DFlexGeneratorJob
+
+
+def generateFlexVolumes(latentsPoints, projectId, workspaceId, trainingJobId, gpu=0):
+    """Load particle latent coordinates from a 3D Flex Training job and use the 3D Flex Generator job to
+        generate a volume series along the trajectory.
+        This method allows(FlexUtils plugin) visualizing specific regions or pathways through the latent conformational distribution
+        of the particle."""
+    try:
+        latentTrajectoryJob = customLatentTrajectory(latentsPoints,
+                                                     projectId,
+                                                     workspaceId,
+                                                     trainingJobId)
+        flexGeneratorJob = runFlexGeneratorJob(trainingJobId,
+                                               latentTrajectoryJob,
+                                               projectId,
+                                               workspaceId,
+                                               gpu)
+
+        return flexGeneratorJob
+    except Exception as ex:
+        raise Exception("Error generating the flex volume : %s" % ex)
+
+
 def runCmd(cmd, printCmd=True):
-    """ Runs a command and check its exit code. If different than 0 it raises an exception
+    """ Runs a command and check its exit code. If different from 0 it raises an exception
     :parameter cmd command to run
     :parameter printCmd (default True) prints the command"""
     import subprocess
     if printCmd:
         logger.info(pwutils.greenStr("Running: %s" % cmd))
+    else:
+        logger.debug(pwutils.greenStr("Running: %s" % cmd))
+
     exitCode, cmdOutput = subprocess.getstatusoutput(cmd)
 
     if exitCode != 0:
         raise Exception("%s failed --> Exit code %s, message %s" % (cmd, exitCode, cmdOutput))
 
-    return exitCode, cmdOutput
+    return exitCode, cmdOutput.split('\n')[-1]
 
 
 def waitForCryosparc(projectName, jobId, failureMessage):
     """ Waits for cryosparc to finish or fail a job
     :parameter projectName: Cryosparc project name
     :parameter jobId: cryosparc job id
     :parameter failureMessage: Message for the exception thrown in case job fails
@@ -798,14 +900,41 @@
     """Get the user Id taking into account the user email"""
     import ast
     getUser_cmd = (getCryosparcProgram() + ' %sGetUser("%s")%s' % ("'", email, "'"))
     user = runCmd(getUser_cmd, printCmd=False)
     return ast.literal_eval(user[1])['_id']
 
 
+def _getCredentials():
+    licence = _getLicenceFromFile()
+    if licence is None:
+        return False, 'Error obtaining cryoSPARC license'
+
+    csIsRunning = isCryosparcRunning()
+    if csIsRunning:
+        hostName = getCryosparcEnvInformation('master_hostname')
+        basePort = getCryosparcEnvInformation('port_app')
+
+        email = Plugin.getUser()
+        if email is None:
+            return False, 'Error obtaining the cryoSPARC user'
+
+        password = Plugin.getUserPassword()
+        if password is None:
+            return False, 'Error obtaining the %s password ' % email
+
+        return True, {'license': licence,
+                    'host': hostName,
+                    'base_port': basePort,
+                    'email': email,
+                    'password': password}
+
+    return False, 'Cryosparc is not running'
+
+
 def getSchedulerLanes():
     """
      Returns a list of lanes that are registered with the master scheduler
      list of dicts -- information about each lane
      """
     _csLanes = ['default']
     _defaultLane = _csLanes[0]
```

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/__init__.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_2Dclassify.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/viewer_2Dclassify.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_initialmodel.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/viewer_initialmodel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_partsubtract.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/viewer_partsubtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_refinement.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/viewers/viewer_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/cryosparc2/wizards.py` & `scipion-em-cryosparc2-4.1.1/cryosparc2/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/PKG-INFO` & `scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.1.0
+Version: 4.1.1
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -43,14 +43,20 @@
         * **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
         * **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
         
         
         **Latest plugin version**
         ==========================
         
+        **v4.1.1**
+        -----------
+        
+        * **new**        Compatibility with cryoSPARC v4.5.1
+        * **new**        Registering flex particles
+        * **new**        Integration with FlexUtils plugin
         
         **v4.1.0**
         -----------
         * **fixed**       Tolerating deletion of projects within CS as well as their folders in the file system
         
         * **new**         Add new protocols:
                             * **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
@@ -117,14 +123,20 @@
                # The root directory where cryoSPARC code and dependencies is installed.
                CRYOSPARC_HOME = <install_path>   (CRYOSPARC_DIR will work for legacy reasons)
                
                # full name of the initial admin account to be created
                CRYOSPARC_USER = <user_name>
         
                # Optional variables
+               ---------------------
+        
+               # The password with which cryoSPARC was installed.
+               # This is only required for the use of the Flexutils plugin and its
+               # connection to the 3D flex training protocol.
+               CRYOSPARC_PASSWORD = <password>
         
                #Folder (available to all workers) where scipion will create cryosparc projects
                CRYO_PROJECTS_DIR = <path> (default to <CRYOSPARC_HOME>/scipion_projects)
         
                # Specifies whether the CS installation is standalone or not. If False,
                # it is assumed that CS is installed in a cluster. If the variable is not
                # defined, by default assume that the installation is standalone and its
```

### Comparing `scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/SOURCES.txt` & `scipion-em-cryosparc2-4.1.1/scipion_em_cryosparc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.1.0/setup.py` & `scipion-em-cryosparc2-4.1.1/setup.py`

 * *Files identical despite different names*

