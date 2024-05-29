# Comparing `tmp/scipion-em-tomo-3.6.1.tar.gz` & `tmp/scipion-em-tomo-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-tomo-3.6.1.tar", last modified: Wed Mar 27 08:58:25 2024, max compression
+gzip compressed data, was "scipion-em-tomo-3.7.0.tar", last modified: Wed May 29 07:39:59 2024, max compression
```

## Comparing `scipion-em-tomo-3.6.1.tar` & `scipion-em-tomo-3.7.0.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:58:25.785031 scipion-em-tomo-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-03-27 08:58:25.785031 scipion-em-tomo-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:58:25.773032 scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-03-27 08:58:25.000000 scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-03-27 08:58:25.000000 scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 08:58:25.000000 scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 08:58:25.000000 scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-27 08:58:25.000000 scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 08:58:25.000000 scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 08:58:25.785031 scipion-em-tomo-3.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:58:25.777032 scipion-em-tomo-3.6.1/tomo/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:58:25.777032 scipion-em-tomo-3.6.1/tomo/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/convert/mdoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)   106862 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:58:25.781031 scipion-em-tomo-3.6.1/tomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_assignTransformationTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_assign_tomo2subtomo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_assign_tomo2tomoMask.py
--rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_consensus_classes_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (127)    19825 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ctf_consensus.py
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ctf_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_extract_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_fit_ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_coordinates_from_scipion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_tomomasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_landmark_to_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_mesh_from_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27068 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_misalignTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_particles_to_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_rotate_astigmatism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_split_evenodd_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (127)    10764 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_tomo_to_mics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_consensus_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_convert_coords3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    22035 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_correct_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_estimate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)    44518 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_import_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:58:25.781031 scipion-em-tomo-3.6.1/tomo/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/templates/HIV-Dynamo-picking-STA.json.template
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/templates/HIV-Reconstruction.json.template
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/templates/HIV-Subtomogram-averaging.json.template
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/templates/HIV-tiltseries-alignment-reconstruction.json.template
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/templates/Membrane picking-with-PySeg.json.template
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/templates/Particle-picking-II.json.template
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/templates/TomoStreaming.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:58:25.785031 scipion-em-tomo-3.6.1/tomo/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45842 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/test_base_centralized_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/test_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/test_fit_vesicles.py
--rw-r--r--   0 runner    (1001) docker     (127)    58492 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/test_mesh_from_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    43179 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/test_tomo_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13338 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14680 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:58:25.785031 scipion-em-tomo-3.6.1/tomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/viewers/viewer_ctf_tomo_consensus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/viewers/viewer_split_evenodd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/viewers/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    53443 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-27 08:57:40.000000 scipion-em-tomo-3.6.1/tomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:39:59.096754 scipion-em-tomo-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-29 07:39:59.096754 scipion-em-tomo-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:39:59.084754 scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-29 07:39:59.000000 scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-29 07:39:59.000000 scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:39:59.000000 scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 07:39:59.000000 scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 07:39:59.000000 scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 07:39:59.000000 scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:39:59.096754 scipion-em-tomo-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:39:59.084754 scipion-em-tomo-3.7.0/tomo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:39:59.084754 scipion-em-tomo-3.7.0/tomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/convert/mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   110391 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:39:59.092754 scipion-em-tomo-3.7.0/tomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_assignTransformationTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_assign_tomo2subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_assign_tomo2tomoMask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_consensus_classes_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19825 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ctf_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ctf_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_extract_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_fit_ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_coordinates_from_scipion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_tomomasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_landmark_to_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_mesh_from_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27068 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_misalignTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_particles_to_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_rotate_astigmatism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_split_evenodd_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10764 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_tomo_to_mics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_consensus_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_convert_coords3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22035 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_correct_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_estimate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44518 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_import_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:39:59.092754 scipion-em-tomo-3.7.0/tomo/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/templates/HIV-Dynamo-picking-STA.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/templates/HIV-Reconstruction.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/templates/HIV-Subtomogram-averaging.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/templates/HIV-tiltseries-alignment-reconstruction.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/templates/Membrane picking-with-PySeg.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/templates/Particle-picking-II.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/templates/TomoStreaming.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:39:59.092754 scipion-em-tomo-3.7.0/tomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45899 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/test_base_centralized_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/test_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/test_fit_vesicles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58492 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/test_mesh_from_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43179 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/test_tomo_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13338 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16671 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:39:59.096754 scipion-em-tomo-3.7.0/tomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/viewers/viewer_ctf_tomo_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/viewers/viewer_split_evenodd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/viewers/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53443 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-29 07:39:32.000000 scipion-em-tomo-3.7.0/tomo/wizards.py
```

### Comparing `scipion-em-tomo-3.6.1/LICENSE` & `scipion-em-tomo-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/PKG-INFO` & `scipion-em-tomo-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-tomo
-Version: 3.6.1
+Version: 3.7.0
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
@@ -76,15 +76,15 @@
         
             scipion installp -p local/path/to/scipion-em-tomo --devel
         
         
         **Configuration variables**
         ===========================
         
-        **NAPARI_ENV_ACTIVATION** (default = conda activate napari-0.4.4):
+        **NAPARI_ENV_ACTIVATION** (default = conda activate napari-0.4.17):
         Command to activate napari environment (used by other tomo plugins).
         
         
         Buildbot status
         ---------------
         
         Status devel version:
```

### Comparing `scipion-em-tomo-3.6.1/README.rst` & `scipion-em-tomo-3.7.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     scipion installp -p local/path/to/scipion-em-tomo --devel
 
 
 **Configuration variables**
 ===========================
 
-**NAPARI_ENV_ACTIVATION** (default = conda activate napari-0.4.4):
+**NAPARI_ENV_ACTIVATION** (default = conda activate napari-0.4.17):
 Command to activate napari environment (used by other tomo plugins).
 
 
 Buildbot status
 ---------------
 
 Status devel version:
```

### Comparing `scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/PKG-INFO` & `scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-tomo
-Version: 3.6.1
+Version: 3.7.0
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
@@ -76,15 +76,15 @@
         
             scipion installp -p local/path/to/scipion-em-tomo --devel
         
         
         **Configuration variables**
         ===========================
         
-        **NAPARI_ENV_ACTIVATION** (default = conda activate napari-0.4.4):
+        **NAPARI_ENV_ACTIVATION** (default = conda activate napari-0.4.17):
         Command to activate napari environment (used by other tomo plugins).
         
         
         Buildbot status
         ---------------
         
         Status devel version:
```

### Comparing `scipion-em-tomo-3.6.1/scipion_em_tomo.egg-info/SOURCES.txt` & `scipion-em-tomo-3.7.0/scipion_em_tomo.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+CHANGES.txt
 LICENSE
+MANIFEST.in
 README.rst
+requirements.txt
 setup.py
 scipion_em_tomo.egg-info/PKG-INFO
 scipion_em_tomo.egg-info/SOURCES.txt
 scipion_em_tomo.egg-info/dependency_links.txt
 scipion_em_tomo.egg-info/entry_points.txt
 scipion_em_tomo.egg-info/requires.txt
 scipion_em_tomo.egg-info/top_level.txt
```

### Comparing `scipion-em-tomo-3.6.1/setup.py` & `scipion-em-tomo-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/__init__.py` & `scipion-em-tomo-3.7.0/tomo/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # **************************************************************************
 
 import os
 import pwem
 from .constants import (NAPARI_ENV_ACTIVATION, NAPARI_ACTIVATION_CMD,
                         getNaparyEnvName, NAPARI_DEF_VER)
 
-__version__ = '3.6.1'
+__version__ = '3.7.0'
 _logo = "icon.png"
 _references = []
 
 
 class Plugin(pwem.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-tomo"
 
@@ -60,15 +60,16 @@
     def addNapariPackage(cls, env, version, default=False):
         ENV_NAME = getNaparyEnvName(version)
         NAPARI_INSTALLED = f"napari_{version}_installed"
         installCmd = [cls.getCondaActivationCmd(),
                       f'conda create -y -n {ENV_NAME} -c conda-forge',
                       f'python=3.10 napari={version} pyqt pip &&',
                       f'conda activate {ENV_NAME} &&',
-                      'pip install napari-tomotwin napari-boxmanager']
+                      'pip install napari-tomotwin napari-boxmanager',
+                      'napari-clusters-plotter@git+https://github.com/BiAPoL/napari-clusters-plotter.git@095d9e8']
 
         # Flag installation finished
         installCmd.append(f'&& touch {NAPARI_INSTALLED}')
 
         napari_commands = [(" ".join(installCmd), NAPARI_INSTALLED)]
 
         envPath = os.environ.get('PATH', "")
```

### Comparing `scipion-em-tomo-3.6.1/tomo/constants.py` & `scipion-em-tomo-3.7.0/tomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/convert/__init__.py` & `scipion-em-tomo-3.7.0/tomo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/convert/convert.py` & `scipion-em-tomo-3.7.0/tomo/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/convert/mdoc.py` & `scipion-em-tomo-3.7.0/tomo/convert/mdoc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/icon.png` & `scipion-em-tomo-3.7.0/tomo/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/objects.py` & `scipion-em-tomo-3.7.0/tomo/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import logging
+from sqlite3 import OperationalError
+from typing import Dict, Tuple, Any, Optional, Union
 
 from pwem import ALIGN_NONE
 
 logger = logging.getLogger(__name__)
 
 import csv
 import math
@@ -126,14 +128,18 @@
         R[:3, :3] = M[:3, :3]
         Mi = np.linalg.inv(M)
         return R @ R @ Mi
 
 
 class TiltImageBase:
     """ Base class for TiltImageM and TiltImage. """
+    TS_ID_FIELD = '_tsId'
+    TILT_ANGLE_FIELD = '_tiltAngle'
+    ACQ_ORDER_FIELD = '_acqOrder'
+    INDEX_FIELD = '_index'
 
     def __init__(self, tsId=None, tiltAngle=None, acquisitionOrder=None, **kwargs):
         self._tiltAngle = Float(tiltAngle)
         self._tsId = String(tsId)
         self._acqOrder = Integer(acquisitionOrder)
         self._oddEvenFileNames = CsvList(pType=str)  # IMPORTANT: The odd is the first one and the even the second one
 
@@ -141,14 +147,15 @@
         return not self._oddEvenFileNames.isEmpty()
 
     def getOddEven(self):
         return self._oddEvenFileNames
 
     def getOdd(self):
         return self._oddEvenFileNames[0]
+
     def getEven(self):
         return self._oddEvenFileNames[1]
 
     def setOdd(self, fnOdd):
         self._oddEvenFileNames[0] = fnOdd
 
     def setEven(self, fnEven):
@@ -195,15 +202,15 @@
     """ Tilt image """
 
     def __init__(self, location=None, **kwargs):
         data.Image.__init__(self, location, **kwargs)
         TiltImageBase.__init__(self, **kwargs)
 
     def clone(self):
-        return  super().clone(copyEnable=True)
+        return super().clone(copyEnable=True)
 
     def copyInfo(self, other, copyId=False, copyTM=True, copyStatus=True):
         data.Image.copyInfo(self, other)
         TiltImageBase.copyInfo(self, other, copyId=copyId, copyTM=copyTM)
         if copyStatus:
             self.setEnabled(other.isEnabled())
 
@@ -326,32 +333,43 @@
         # Do nothing on close, since the db will be closed by SetOfTiltSeries
         pass
 
     def getScannedPixelSize(self):
         mag = self._acquisition.getMagnification()
         return self._samplingRate.get() * 1e-4 * mag
 
-    def generateTltFile(self, tltFilePath, reverse=False):
+    def generateTltFile(self, tltFilePath, reverse=False, excludeViews=False, presentAcqOrders=None):
         """ Generates an angle file in .tlt format in the specified location. If reverse is set to true the angles in
         file are sorted in the opposite order.
         :param tltFilePath: String containing the path where the file is created.
         :param reverse: Boolean indicating if the angle list must be reversed.
+        :param excludeViews: boolean used to indicate if the tlt file should contain only the data concerning
+        the non-excluded views (True) or all of them (False).
+        :param presentAcqOrders: set containing the present acq orders in both the given TS and CTFTomoSeries. Used to
+        filter the tilt angles that will be written in the tlt file generated. The parameter excludedViews is ignored
+        if presentAcqOrders is provided, as the excluded views info may have been used to generate the presentAcqOrders
+        (see tomo > utils > getCommonTsAndCtfElements)
         """
 
-        angleList = []
-
-        for ti in self.iterItems(orderBy="_tiltAngle"):
-            angleList.append(ti.getTiltAngle())
-
+        if presentAcqOrders:
+            angleList = [ti.getTiltAngle() for ti in self.iterItems(orderBy=TiltImage.TILT_ANGLE_FIELD) if
+                         ti.getAcquisitionOrder() in presentAcqOrders]
+        else:
+            angleList = []
+            for ti in self.iterItems(orderBy=TiltImage.TILT_ANGLE_FIELD):
+                if excludeViews and not ti.isEnabled():
+                    continue
+                angleList.append(ti.getTiltAngle())
         if reverse:
             angleList.reverse()
 
         with open(tltFilePath, 'w') as f:
             f.writelines("%.3f\n" % angle for angle in angleList)
 
+
     def hasOrigin(self):
         """ Method indicating if the TiltSeries object has a defined origin. """
 
         return self._origin is not None
 
     def setOrigin(self, newOrigin):
         """ Method to set the origin of the TiltSeries object.
@@ -771,15 +789,15 @@
             orderByTs: optional orderBy value for iterating over TiltSeries
             updateTsCallback: optional callback after TiltSeries is created
             orderByTi: optional orderBy value for iterating over TiltImages
             updateTiCallback: optional callback after TiltImage is created
             itemSelectedCallback: Optional, callback receiving an item and
                 returning true if it has to be copied
         """
-        
+
         if itemSelectedCallback is None:
             itemSelectedCallback = data.SetOfImages.isItemEnabled
 
         for i, ts in enumerate(inputTs.iterItems(orderBy=orderByTs)):
             if itemSelectedCallback(ts):
                 tsOut = self.ITEM_TYPE()
                 tsOut.copyInfo(ts)
@@ -789,15 +807,15 @@
                 self.append(tsOut)
                 for j, ti in enumerate(ts.iterItems(orderBy=orderByTi)):
                     tiOut = tsOut.ITEM_TYPE()
                     tiOut.copyInfo(ti)
                     tiOut.setAcquisition(ti.getAcquisition())
                     tiOut.copyObjId(ti)
                     tiOut.setLocation(ti.getLocation())
-                    tiOut.setEnabled(ti.isEnabled()) # Clone disabled tilt images
+                    tiOut.setEnabled(ti.isEnabled())  # Clone disabled tilt images
                     if updateTiCallback:
                         updateTiCallback(j, ts, ti, tsOut, tiOut)
                     tsOut.append(tiOut)
 
                 self.update(tsOut)
 
     def update(self, item: TiltSeriesBase):
@@ -824,17 +842,15 @@
         return self._samplingRate.get() * 1e-4 * mag
 
     def getTiltSeriesFromTsId(self, tsId):
         return self[{"_tsId": tsId}]
 
     def getTSIds(self):
         """ Returns al the Tilt series ids involved in the set."""
-        tsIds = self.aggregate(["MAX"], TiltSeries.TS_ID_FIELD, [TiltSeries.TS_ID_FIELD])
-        tsIds = [d[TiltSeries.TS_ID_FIELD] for d in tsIds]
-        return tsIds
+        return self.getUniqueValues(TiltSeries.TS_ID_FIELD)
 
 
 class SetOfTiltSeries(SetOfTiltSeriesBase):
     ITEM_TYPE = TiltSeries
 
     def _dimStr(self):
         """ Return the string representing the dimensions. """
@@ -1148,14 +1164,18 @@
              self._dimStr(), tomoStr, sampling, self._appendStreamState())
         return s
 
     def update(self, item: Tomogram):
         self._hasOddEven.set(item.hasHalfMaps())
         super().update(item)
 
+    def getTSIds(self):
+        """ Returns al the Tilt series ids involved in the set."""
+        return self.getUniqueValues(Tomogram.TS_ID_FIELD)
+
 
 class TomoMask(Tomogram):
     """ Object used to represent segmented tomograms
     """
 
     def __init__(self, **kwargs):
         Tomogram.__init__(self, **kwargs)
@@ -1638,17 +1658,15 @@
     def append(self, item: Coordinate3D):
         if self.getBoxSize() is None and item._boxSize:
             self.setBoxSize(item._boxSize)
         super().append(item)
 
     def getTSIds(self):
         """ Returns all the TS ID (tomoId) present in this set"""
-        volIds = self.aggregate(["MAX"], Coordinate3D.TOMO_ID_ATTR, [Coordinate3D.TOMO_ID_ATTR])
-        volIds = [d[Coordinate3D.TOMO_ID_ATTR] for d in volIds]
-        return volIds
+        return self.getUniqueValues(Coordinate3D.TOMO_ID_ATTR)
 
 
 class SubTomogram(data.Volume):
     """The coordinate associated to each subtomogram is not scaled. To do that, the coordinates and the subtomograms
     sampling rates should be compared (because of how the extraction protocol works). But when shifts are applied to
     the coordinates, it has to be considered that if we're operating with coordinates coming from subtomogrmas, those
     shifts will be scaled, but if the coordinates come from coordinates, they won't be."""
@@ -2253,29 +2271,32 @@
 
     def hasAlgebraicDesc(self):
         return self._algebraicDesc is not None
 
 
 class CTFTomo(data.CTFModel):
     """ Represents a generic CTF model for a tilt-image. """
+    ACQ_ORDER_FIELD = '_acqOrder'
+    INDEX_FIELD = '_index'
 
-    def __init__(self, **kwargs):
-        data.CTFModel.__init__(self, **kwargs)
-        self._index = Integer(kwargs.get('index', None))
+    def __init__(self, index=None, acqOrder=None, **kwargs):
+        super().__init__(**kwargs)
+        self._index = Integer(index)
+        self._acqOrder = Integer(acqOrder)
 
     def copyInfo(self, other, copyId=False):
         """ Copy info is similar to clone, but is often used to tranfer data from other type of objects with same attributes"""
         self.copy(other, copyId=copyId)
 
     def clone(self, copyEnable=True):
         return super().clone(copyEnable=copyEnable)
 
     def copy(self, other, copyId=True, ignoreAttrs=[], copyEnable=True):
         self.copyAttributes(other, '_defocusU', '_defocusV', '_defocusAngle', '_defocusRatio', '_psdFile',
-                            '_resolution', '_fitQuality', '_index')
+                            '_resolution', '_fitQuality', self.INDEX_FIELD, self.ACQ_ORDER_FIELD)
 
         if copyEnable:
             self.setEnabled(other.isEnabled())
 
         if other.hasPhaseShift():
             self.setPhaseShift(other.getPhaseShift())
 
@@ -2309,18 +2330,24 @@
         newCTFTomo = CTFTomo()
         newCTFTomo.copyAttributes(ctfModel, '_defocusU', '_defocusV',
                                   '_defocusAngle', '_defocusRatio', '_psdFile',
                                   '_resolution', '_fitQuality')
         return newCTFTomo
 
     def getIndex(self):
-        return self._index
+        return self._index.get()
 
     def setIndex(self, value):
-        self._index = Integer(value)
+        self._index.set(value)
+
+    def getAcquisitionOrder(self):
+        return self._acqOrder.get()
+
+    def setAcquisitionOrder(self, value):
+        self._acqOrder.set(value)
 
     def getCutOnFreq(self):
         return self._cutOnFreq
 
     def setCutOnFreq(self, value):
         self._cutOnFreq = Float(value)
 
@@ -2557,14 +2584,15 @@
         " Standardize the input values "
         self.standardize()
 
 
 class CTFTomoSeries(data.EMSet):
     """ Represents a set of CTF models belonging to the same tilt-series. """
     ITEM_TYPE = CTFTomo
+    TS_ID_FIELD = '_tsId'
 
     def __init__(self, **kwargs):
         data.EMSet.__init__(self, **kwargs)
         self._tiltSeriesPointer = Pointer(kwargs.get('tiltSeriesPointer', None))
         self._tsId = String(kwargs.get('tsId', None))
         self._isDefocusUDeviationInRange = Boolean(True)
         self._isDefocusVDeviationInRange = Boolean(True)
@@ -2693,14 +2721,48 @@
 
     def calculateDefocusUDeviation(self, defocusUTolerance=20):
         pass
 
     def calculateDefocusVDeviation(self, defocusVTolerance=20):
         pass
 
+    def getCtfTomoFromTi(self, ti: TiltImage, onlyEnabled: bool = True) -> Optional[CTFTomo]:
+        """Get the corresponding CTFModel from a given tilt-image. If there's no match, it returns None.
+        :param ti: Tilt-image.
+        :param onlyEnabled: boolean used to indicate the matching behaves in terms of the value the attribute
+        _objEnabled from both ti and the matching CTFModel attribute:
+            - If True (default), the CTFModel found is returned only if both the ti and the CTFModel are enabled.
+            - If False, the CTFModel found is returned no matter the value of _objEnabled.
+        """
+        if onlyEnabled and not ti.isEnabled():
+            logger.debug('The introduced tilt-image is not enabled and working with onlyEnabled = True')
+            return None
+        try:
+            # The method getItem raises an exception of type:
+            #   - sqlite3.OperationalError if the key is not found
+            #   - UnboundLocalError if the value is not found
+            ctfTomo = self.getItem(CTFTomo.ACQ_ORDER_FIELD, ti.getAcquisitionOrder())
+        except UnboundLocalError:
+            return None
+        except OperationalError:
+            try:
+                ctfTomo = self.getItem(CTFTomo.INDEX_FIELD, ti.getIndex())
+                logger.warning('WARNING! The current CTF series does not have the attribute "acquisition order" '
+                               '(_acqOrder). The matching between the CTF and the tilt-image is carried out '
+                               'using the index --> LESS RELIABLE. CHECK THE RESULTS CAREFULLY')
+            except (OperationalError, UnboundLocalError):
+                logger.warning(f'No CTF found in the current CTF series {self.getTsId()} that matches the '
+                               f'given tilt-image of tsId = {ti.getTsId()}.')
+                return None
+
+        if ctfTomo.isEnabled() or not onlyEnabled:
+            return ctfTomo
+        else:
+            return None
+
 
 class SetOfCTFTomoSeries(data.EMSet):
     """ Represents a set of CTF model series belonging to the same set of tilt-series. """
     ITEM_TYPE = CTFTomoSeries
     USE_CREATE_COPY_FOR_SUBSET = True
 
     def __init__(self, **kwargs):
@@ -2727,15 +2789,14 @@
 
                 for j, ctf in enumerate(ctfSerie.iterItems()):
                     ctfOut = ctf.clone()
                     ctfSerieOut.append(ctfOut)
 
                 self.update(ctfSerieOut)
 
-
     def getSetOfTiltSeries(self, pointer=False):
         """ Return the tilt-series associated with this CTF model series. """
         return self._setOfTiltSeriesPointer.get() if not pointer else self._setOfTiltSeriesPointer
 
     def setSetOfTiltSeries(self, setOfTiltSeries):
         """ Set the tilt-series from which this CTF model series were estimated.
         :param setOfTiltSeries: Either a TiltSeries object or a pointer to it.
@@ -2808,14 +2869,18 @@
     def _getTiltSeriesFromTsId(self, tsId):
         if self._idDict:
             return self._idDict.get(tsId, None)
         else:
             self._idDict = {ts.getTsId(): ts.clone(ignoreAttrs=[]) for ts in self.getSetOfTiltSeries()}
             return self._idDict.get(tsId, None)
 
+    def getTSIds(self):
+        """ Returns al the Tilt series ids involved in the set."""
+        return self.getUniqueValues(CTFTomoSeries.TS_ID_FIELD)
+
 
 class TiltSeriesCoordinate(data.EMObject):
     """This class holds the (x,y,z) positions, in angstroms, and other information
     associated with a coordinate related to a tilt series"""
 
     def __init__(self, **kwargs):
         data.EMObject.__init__(self, **kwargs)
```

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/__init__.py` & `scipion-em-tomo-3.7.0/tomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_alignment_assign.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_assignTransformationTS.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_assignTransformationTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_assign_tomo2subtomo.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_assign_tomo2subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_assign_tomo2tomoMask.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_assign_tomo2tomoMask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_base.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_compose_TS.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_compose_TS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_consensus_classes_subtomo.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_consensus_classes_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ctf_consensus.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ctf_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ctf_validate.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ctf_validate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_extract_coordinates.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_fit_ellipsoid.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_fit_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_coordinates.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_coordinates_from_scipion.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_coordinates_from_scipion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_ctf.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_subtomograms.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_tomograms.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_import_tomomasks.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_import_tomomasks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_landmark_to_2d.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_landmark_to_2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_mesh_from_segmentation.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_mesh_from_segmentation.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_misalignTS.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_misalignTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_particles_to_subtomograms.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_particles_to_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_rotate_astigmatism.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_rotate_astigmatism.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_split_evenodd_subtomos.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_split_evenodd_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_tomo_to_mics.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_tomo_to_mics.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_base.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_consensus_alignment.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_consensus_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_convert_coords3d.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_convert_coords3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_correct_motion.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_correct_motion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_estimate_ctf.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_estimate_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_import.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols/protocol_ts_import_coordinates.py` & `scipion-em-tomo-3.7.0/tomo/protocols/protocol_ts_import_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/protocols.conf` & `scipion-em-tomo-3.7.0/tomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/templates/HIV-Dynamo-picking-STA.json.template` & `scipion-em-tomo-3.7.0/tomo/templates/HIV-Dynamo-picking-STA.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/templates/HIV-Reconstruction.json.template` & `scipion-em-tomo-3.7.0/tomo/templates/HIV-Reconstruction.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/templates/HIV-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.7.0/tomo/templates/HIV-Subtomogram-averaging.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/templates/HIV-tiltseries-alignment-reconstruction.json.template` & `scipion-em-tomo-3.7.0/tomo/templates/HIV-tiltseries-alignment-reconstruction.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/templates/Membrane picking-with-PySeg.json.template` & `scipion-em-tomo-3.7.0/tomo/templates/Membrane picking-with-PySeg.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/templates/Particle-picking-II.json.template` & `scipion-em-tomo-3.7.0/tomo/templates/Particle-picking-II.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/templates/TomoStreaming.json.template` & `scipion-em-tomo-3.7.0/tomo/templates/TomoStreaming.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/__init__.py` & `scipion-em-tomo-3.7.0/tomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/test_base_centralized_layer.py` & `scipion-em-tomo-3.7.0/tomo/tests/test_base_centralized_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         testAcq = testAcq[tsId] if type(testAcq) is dict else testAcq
         self.assertAlmostEqual(testAcq.getMagnification(), currentAcq.getMagnification(), delta=1)
         self.assertAlmostEqual(testAcq.getVoltage(), currentAcq.getVoltage(), delta=1)
         self.assertAlmostEqual(testAcq.getSphericalAberration(), currentAcq.getSphericalAberration(), delta=0.01)
         self.assertAlmostEqual(testAcq.getDoseInitial(), currentAcq.getDoseInitial(), delta=0.01)
         self.assertAlmostEqual(testAcq.getDosePerFrame(), currentAcq.getDosePerFrame(), delta=0.01)
         self.assertAlmostEqual(testAcq.getAccumDose(), currentAcq.getAccumDose(), delta=0.01)
-        self.assertAlmostEqual(testAcq.getTiltAxisAngle(), currentAcq.getTiltAxisAngle(), delta=0.01)
+        self.assertAlmostEqual(testAcq.getTiltAxisAngle(), currentAcq.getTiltAxisAngle(), delta=0.5)
         self.assertAlmostEqual(testAcq.getAngleMin(), currentAcq.getAngleMin(), delta=0.01)
         self.assertAlmostEqual(testAcq.getAngleMax(), currentAcq.getAngleMax(), delta=0.01)
         self.assertAlmostEqual(testAcq.getStep(), currentAcq.getStep(), delta=0.1)
 
     # CTF ##############################################################################################################
     def checkCTFs(self, inCtfSet, expectedSetSize=-1, expectedPsdFile=None, excludedViewsDict=None, streamState=2):
         """
@@ -727,14 +727,15 @@
             self.assertTrue(enb, msg='TsId = %s: %s %i was expected to be Enabled' % (tsId, objType, ind))
 
     def checkCtfTomo(self, ctf, isExcluded, expectPsdFile):
         defocusU = ctf.getDefocusU()
         defocusV = ctf.getDefocusV()
         defocusAngle = ctf.getDefocusAngle()
         defocusVals = [defocusU, defocusV, defocusAngle]
+        self.assertGreater(ctf.getAcquisitionOrder(), -1)
         if isExcluded:
             expectedDefocusU = -999
             expectedDefocusV = -1
             expectedDefocusAngle = -999
             self.assertTrue(np.allclose(np.array(defocusVals),
                                         np.array([expectedDefocusU, expectedDefocusV, expectedDefocusAngle])))
         else:
```

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/test_compose_TS.py` & `scipion-em-tomo-3.7.0/tomo/tests/test_compose_TS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/test_fit_vesicles.py` & `scipion-em-tomo-3.7.0/tomo/tests/test_fit_vesicles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/test_import.py` & `scipion-em-tomo-3.7.0/tomo/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/test_mesh_from_segmentation.py` & `scipion-em-tomo-3.7.0/tomo/tests/test_mesh_from_segmentation.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/test_objects.py` & `scipion-em-tomo-3.7.0/tomo/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/test_tomo_base.py` & `scipion-em-tomo-3.7.0/tomo/tests/test_tomo_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/tests/test_transformations.py` & `scipion-em-tomo-3.7.0/tomo/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/utils.py` & `scipion-em-tomo-3.7.0/tomo/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,23 +25,26 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 import re
 import importlib
+from typing import List, Set
+
 import numpy as np
 import math
 import logging
 logger = logging.getLogger(__name__)
 
 import pyworkflow.utils as pwutils
 
 import tomo.constants as const
-from tomo.objects import SetOfCoordinates3D, SetOfSubTomograms, SetOfTiltSeries, Coordinate3D, SubTomogram, TiltSeries
+from tomo.objects import SetOfCoordinates3D, SetOfSubTomograms, SetOfTiltSeries, Coordinate3D, SubTomogram, TiltSeries, \
+    CTFTomoSeries, TiltImage, CTFTomo
 
 
 def existsPlugin(plugin):
     return importlib.util.find_spec(plugin)
 
 
 def _getUniqueFileName(pattern, filename, filePaths=None):
@@ -404,7 +407,39 @@
     if scaleFactor != 1:  # It can be lower (smaller source) or higher (bigger source) than one
         shifts = np.array([inTrMatrix[0, 3], inTrMatrix[1, 3], inTrMatrix[2, 3]])
         scaledShifts = scaleFactor * shifts
         inTrMatrix[0, 3] = scaledShifts[0]
         inTrMatrix[1, 3] = scaledShifts[1]
         inTrMatrix[2, 3] = scaledShifts[2]
     return inTrMatrix
+
+
+def getCommonTsAndCtfElements(ts: TiltSeries, ctfTomoSeries: CTFTomoSeries, onlyEnabled: bool = True) -> Set[int]:
+    """Given a tilt-series and a CTFTomoSeries, it finds the common elements present and enabled in both sets, and
+    returns a list with the corresponding acquisition orders or indices, if acquisition order is not present in the
+    CTFTomoSeries introduced (old versions, backwards compatibility). By default, it takes the common active elements,
+    but it may take common elements no matter if they're enabled or not by setting the input onlyEnabled to False.
+    """
+    # Attribute _acqOrder was recently added to CTFTomo, so it will be used to discriminate
+    ctfTomoSeries._getMapper()  # Avoid finding closed mappers when combining cached sets of sets (TS, CTF) and
+    # calls to getFirstItem(). The second closes the first and so on
+    firstCtfTomo = ctfTomoSeries.getFirstItem()
+    acqOrder = getattr(firstCtfTomo, CTFTomo.ACQ_ORDER_FIELD, None)
+    if acqOrder:
+        msgStr = 'acquisition order'
+        if onlyEnabled:
+            tsAcqOrderSet = {ti.getAcquisitionOrder() for ti in ts if ti.isEnabled()}
+            ctfAcqOrderSet = {ctf.getAcquisitionOrder() for ctf in ctfTomoSeries if ctf.isEnabled()}
+        else:
+            tsAcqOrderSet = {ti.getAcquisitionOrder() for ti in ts}
+            ctfAcqOrderSet = {ctf.getAcquisitionOrder() for ctf in ctfTomoSeries}
+    else:
+        msgStr = 'index'
+        if onlyEnabled:
+            tsAcqOrderSet = {ti.getIndex() for ti in ts if ti.isEnabled()}
+            ctfAcqOrderSet = {ctf.getIndex() for ctf in ctfTomoSeries if ctf.isEnabled()}
+        else:
+            tsAcqOrderSet = {ti.getIndex() for ti in ts}
+            ctfAcqOrderSet = {ctf.getIndex() for ctf in ctfTomoSeries}
+
+    logger.debug(f'getCommonTsAndCtfElements: tsId = {ts.getTsId()}, matching used field is {msgStr}')
+    return tsAcqOrderSet & ctfAcqOrderSet
```

### Comparing `scipion-em-tomo-3.6.1/tomo/viewers/__init__.py` & `scipion-em-tomo-3.7.0/tomo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/viewers/viewer_ctf_tomo_consensus.py` & `scipion-em-tomo-3.7.0/tomo/viewers/viewer_ctf_tomo_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/viewers/viewer_split_evenodd.py` & `scipion-em-tomo-3.7.0/tomo/viewers/viewer_split_evenodd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/viewers/viewers_data.py` & `scipion-em-tomo-3.7.0/tomo/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/viewers/views.py` & `scipion-em-tomo-3.7.0/tomo/viewers/views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/viewers/views_tkinter_tree.py` & `scipion-em-tomo-3.7.0/tomo/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.6.1/tomo/wizards.py` & `scipion-em-tomo-3.7.0/tomo/wizards.py`

 * *Files identical despite different names*

