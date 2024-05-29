# Comparing `tmp/gempy_engine-2024.1.4.tar.gz` & `tmp/gempy_engine-2024.1.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempy_engine-2024.1.4.tar", last modified: Fri May 17 07:15:45 2024, max compression
+gzip compressed data, was "gempy_engine-2024.1.4b0.tar", last modified: Wed May 29 14:29:41 2024, max compression
```

## Comparing `gempy_engine-2024.1.4.tar` & `gempy_engine-2024.1.4b0.tar`

### file list

```diff
@@ -1,313 +1,313 @@
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.200174 gempy_engine-2024.1.4/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      260 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4/.env.example
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1832 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/.gitignore
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.160174 gempy_engine-2024.1.4/.vscode/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      463 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/.vscode/launch.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)      523 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/AUTHORS.rst
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13879 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/LICENSE
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2837 2024-05-17 07:15:45.200174 gempy_engine-2024.1.4/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1144 2023-08-11 08:35:11.000000 gempy_engine-2024.1.4/README.md
--rw-r--r--   0 leguark   (1000) leguark   (1000)   260403 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/apibinary.le
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.160174 gempy_engine-2024.1.4/gempy_engine/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.160174 gempy_engine-2024.1.4/gempy_engine/API/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/API/_version.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.160174 gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4516 2023-11-21 09:51:13.000000 gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/_dual_contouring.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2205 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/_experimental_water_tight_DC_1.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3206 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/_interpolate_on_edges.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      114 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/_mask_buffer.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7237 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/multi_scalar_dual_contouring.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.160174 gempy_engine-2024.1.4/gempy_engine/API/interp_single/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/interp_single/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6236 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/API/interp_single/_interp_scalar_field.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5559 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/API/interp_single/_interp_single_feature.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12592 2024-05-16 14:21:50.000000 gempy_engine-2024.1.4/gempy_engine/API/interp_single/_multi_scalar_field_manager.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3368 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/API/interp_single/_octree_generation.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4202 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/API/interp_single/interp_features.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.160174 gempy_engine-2024.1.4/gempy_engine/API/model/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/model/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2929 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/API/model/model_api.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.160174 gempy_engine-2024.1.4/gempy_engine/API/server/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1338 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/server/2features.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1356 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/server/2features_inclined.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/server/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1193 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/server/_old_example.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4176 2023-09-15 12:25:48.000000 gempy_engine-2024.1.4/gempy_engine/API/server/_process_output.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1923 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/API/server/_server_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1252 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/server/example.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3942 2023-11-14 16:11:18.000000 gempy_engine-2024.1.4/gempy_engine/API/server/main_server_pro.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      223 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/API/server/test_compute.http
--rw-r--r--   0 leguark   (1000) leguark   (1000)       61 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      417 2024-05-17 07:15:45.000000 gempy_engine-2024.1.4/gempy_engine/_version.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1571 2024-05-16 15:17:02.000000 gempy_engine-2024.1.4/gempy_engine/config.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.160174 gempy_engine-2024.1.4/gempy_engine/core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    14539 2024-05-16 14:26:31.000000 gempy_engine-2024.1.4/gempy_engine/core/backend_tensor.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/core/data/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      308 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4203 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/centered_grid.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       44 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4/gempy_engine/core/data/continue_epoch.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1314 2023-10-05 13:36:58.000000 gempy_engine-2024.1.4/gempy_engine/core/data/custom_segmentation_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1279 2023-10-05 11:49:56.000000 gempy_engine-2024.1.4/gempy_engine/core/data/dual_contouring_data.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      602 2023-09-14 08:17:23.000000 gempy_engine-2024.1.4/gempy_engine/core/data/dual_contouring_mesh.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6150 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/engine_grid.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2951 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4/gempy_engine/core/data/exported_fields.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      442 2023-09-05 11:04:18.000000 gempy_engine-2024.1.4/gempy_engine/core/data/exported_structs.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      383 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/generic_grid.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      173 2023-10-06 08:38:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/geophysics_input.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3503 2023-08-17 12:00:28.000000 gempy_engine-2024.1.4/gempy_engine/core/data/input_data_descriptor.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1745 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/internal_structs.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5280 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/interp_output.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3045 2023-10-05 13:51:07.000000 gempy_engine-2024.1.4/gempy_engine/core/data/interpolation_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9088 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/interpolation_input.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1550 2023-08-17 13:49:03.000000 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/faults.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2627 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/kernel_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3541 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/orientations.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/server/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/server/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1000 2023-08-11 11:40:58.000000 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/server/input_parser.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      145 2023-08-09 08:33:04.000000 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/solvers.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2278 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/surface_points.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      430 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/core/data/matrices_sizes.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1660 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/octree_level.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/core/data/options/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      180 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/options/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2326 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/options/evaluation_options.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9427 2024-05-16 15:18:40.000000 gempy_engine-2024.1.4/gempy_engine/core/data/options/interpolation_options.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3373 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/options/kernel_options.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      104 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/options/temp_interpolation_values.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/core/data/output/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/output/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      275 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/output/blocks_value_type.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9923 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/core/data/raw_arrays_solution.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6874 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/regular_grid.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4824 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/scalar_field_output.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4904 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/solutions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      198 2023-07-24 09:17:59.000000 gempy_engine-2024.1.4/gempy_engine/core/data/stack_relation_type.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4996 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/stacks_structure.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2587 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/core/data/tensors_structure.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10868 2023-09-05 14:24:09.000000 gempy_engine-2024.1.4/gempy_engine/core/data/transforms.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1286 2024-04-15 13:51:26.000000 gempy_engine-2024.1.4/gempy_engine/core/utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2058 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/dev_notes.md
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/activator/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/activator/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2608 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/activator/activator_interface.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6245 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/activator/torch_activation.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/data_preprocess/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/data_preprocess/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2402 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/data_preprocess/_input_preparation.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1651 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/data_preprocess/data_preprocess_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/dual_contouring/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/dual_contouring/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11313 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/modules/dual_contouring/dual_contouring_interface.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11330 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/dual_contouring/fancy_triangulation.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/evaluator/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/evaluator/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3330 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/evaluator/generic_evaluator.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2599 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4/gempy_engine/modules/evaluator/symbolic_evaluator.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/geophysics/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-06 08:07:32.000000 gempy_engine-2024.1.4/gempy_engine/modules/geophysics/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1929 2023-10-09 08:58:18.000000 gempy_engine-2024.1.4/gempy_engine/modules/geophysics/fw_gravity.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2021 2023-10-09 08:27:43.000000 gempy_engine-2024.1.4/gempy_engine/modules/geophysics/gravity_gradient.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      867 2023-10-05 12:31:28.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_b_vector_assembler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8286 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_covariance_assembler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2950 2023-10-05 09:41:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4237 2023-11-07 11:42:44.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_kernel_constructors.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1347 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_kernel_selectors.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12656 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_kernels_assembler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2519 2023-08-11 11:19:33.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_pykeops_cov_compiler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9218 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_structs.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3548 2023-08-16 13:29:03.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_test_assembler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      976 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11918 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_vectors_preparation.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1493 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/kernel_constructor_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      434 2023-09-05 12:48:43.000000 gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/README.md
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5913 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/_curvature_analysis.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1217 2023-09-06 08:37:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/_octree_common.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3635 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/_octree_internals.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6583 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/octrees_topology_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/solver/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/solver/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2139 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4/gempy_engine/modules/solver/_conjugate_gradient.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6535 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4/gempy_engine/modules/solver/_custom_pykeops_solver.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11136 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4/gempy_engine/modules/solver/_kernel_solve_autograd.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11945 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4/gempy_engine/modules/solver/_kernel_solver_from_lazy_tensor.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5324 2024-05-16 14:10:20.000000 gempy_engine-2024.1.4/gempy_engine/modules/solver/solver_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/topology/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/topology/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/gempy_engine/modules/topology/topology _interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/modules/weights_cache/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4/gempy_engine/modules/weights_cache/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3489 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/modules/weights_cache/weights_cache_interface.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1565 2023-10-05 08:11:53.000000 gempy_engine-2024.1.4/gempy_engine/optional_dependencies.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/plugins/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 07:51:38.000000 gempy_engine-2024.1.4/gempy_engine/plugins/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/gempy_engine/plugins/plotting/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 07:51:56.000000 gempy_engine-2024.1.4/gempy_engine/plugins/plotting/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3976 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/gempy_engine/plugins/plotting/helper_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5609 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/gempy_engine/plugins/plotting/helper_functions_pyvista.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.200174 gempy_engine-2024.1.4/gempy_engine.egg-info/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2837 2024-05-17 07:15:45.000000 gempy_engine-2024.1.4/gempy_engine.egg-info/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13837 2024-05-17 07:15:45.000000 gempy_engine-2024.1.4/gempy_engine.egg-info/SOURCES.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-05-17 07:15:45.000000 gempy_engine-2024.1.4/gempy_engine.egg-info/dependency_links.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)      257 2024-05-17 07:15:45.000000 gempy_engine-2024.1.4/gempy_engine.egg-info/requires.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2024-05-17 07:15:45.000000 gempy_engine-2024.1.4/gempy_engine.egg-info/top_level.txt
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.170174 gempy_engine-2024.1.4/requirements/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      184 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4/requirements/dev-requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       28 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4/requirements/optional-requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       29 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4/requirements/requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       80 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4/requirements/server-requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2024-05-17 07:15:45.200174 gempy_engine-2024.1.4/setup.cfg
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2593 2024-05-16 14:10:20.000000 gempy_engine-2024.1.4/setup.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      251 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/test.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)   260148 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/test.le
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.180174 gempy_engine-2024.1.4/tests/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.180174 gempy_engine-2024.1.4/tests/SKIP_tensor_flow/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/SKIP_tensor_flow/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2532 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/SKIP_tensor_flow/test_backend_tensor.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2883 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/SKIP_tensor_flow/test_tensorflow.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      693 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/SKIP_tensor_flow/test_tf.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.180174 gempy_engine-2024.1.4/tests/SKIP_test_large_data/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/SKIP_test_large_data/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    16424 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/SKIP_test_large_data/plot_scipy.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.180174 gempy_engine-2024.1.4/tests/benchmark/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.150174 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.180174 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11112 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/NoOptsFewInput_8f0c757cc42cb56628256f233c1f66523a634aa1_20221014_121041_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11141 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/NoOptsMidInput_bd95d1107e2c3779eb123cd694479ea62bd111a9_20221014_122235_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9897 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt1FewInput_1f1b37c12217371ea50b4e1cb46fc464049d14a7_20221015_120122_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9900 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt1MidInput_67ff73c1220d60ab1b284243a043aa6b73d4ee00_20221014_202857_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11127 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl3_1bf3c987df2b548a2edfc18b5f283f0acf466df7_20221015_150147_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10536 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl5_f9f08e62a3aa03c3d2089fb55b3ed4bcc1c46f15_20221016_104901_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9153 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl6_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124647_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11131 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2MidInputOctLvl3_1bf3c987df2b548a2edfc18b5f283f0acf466df7_20221015_150632_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9153 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt3FewInputOctLvl5_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124154_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9153 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt3FewInputOctLvl6_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124502_uncommited-changes.json
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3794 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/benchmark/README.md
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/benchmark/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4234 2023-11-14 16:11:18.000000 gempy_engine-2024.1.4/tests/benchmark/one_fault_model.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2449 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/benchmark/profile_runner.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3344 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/benchmark/test_benchmark_one_feature.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2050 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/conftest.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.180174 gempy_engine-2024.1.4/tests/data/
--rw-r--r--   0 leguark   (1000) leguark   (1000)   204949 2023-08-11 08:57:48.000000 gempy_engine-2024.1.4/tests/data/Moureze_Points.csv
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.180174 gempy_engine-2024.1.4/tests/fixtures/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8156 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/fixtures/complex_geometries.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.180174 gempy_engine-2024.1.4/tests/fixtures/graben_data/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1240 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9a_Fault_relations_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4468 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9a_Fault_relations_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4468 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9a_Finite_Fault_relations_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1401 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9b_Fault_relations_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4654 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9b_Fault_relations_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1179 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/fixtures/grids.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6498 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/fixtures/heavy_models.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.190174 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/05_toy_fold_unconformity_interfaces.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      299 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/05_toy_fold_unconformity_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      139 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/fixture_model_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1856 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/fixture_model_surfaces.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)       87 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model1_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)       89 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model1_orientations_scaled.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)  3000128 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model1_scaled.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)      232 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model1_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      268 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model1_surface_points_scaled.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)       87 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model2_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      659 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model2_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)       97 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model3_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      121 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model3_orientations_scaled.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1845 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model3_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3167 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model3_surface_points_scaled-2.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      211 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model4_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      227 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model4_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      163 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model5_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      409 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model5_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      168 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model6_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      715 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model6_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)      237 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model7_orientations.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1853 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model7_surface_points.csv
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2840 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/fixtures/simple_geometries.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    21434 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/fixtures/simple_models.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      123 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/pytest.ini
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.190174 gempy_engine-2024.1.4/tests/test_common/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.190174 gempy_engine-2024.1.4/tests/test_common/test_api/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_api/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.190174 gempy_engine-2024.1.4/tests/test_common/test_api/test_faults/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_api/test_faults/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6882 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_api/test_faults/test_faults_graben.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11460 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_api/test_faults/test_one_fault.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1749 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_common/test_api/test_output_to_subsurface.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5876 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_api/test_public_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.190174 gempy_engine-2024.1.4/tests/test_common/test_core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       72 2023-07-12 07:31:14.000000 gempy_engine-2024.1.4/tests/test_common/test_core/test_data_classes.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.190174 gempy_engine-2024.1.4/tests/test_common/test_dependencies/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_dependencies/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      542 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_dependencies/pykeops_test_compiler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    18780 2023-08-11 08:42:39.000000 gempy_engine-2024.1.4/tests/test_common/test_dependencies/test_pykeops.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.190174 gempy_engine-2024.1.4/tests/test_common/test_integrations/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_integrations/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4178 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_integrations/test_external_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3394 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_integrations/test_interpolate_model.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2102 2023-09-06 11:22:27.000000 gempy_engine-2024.1.4/tests/test_common/test_integrations/test_kernels.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8007 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_integrations/test_multi_fields.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6468 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_integrations/test_multi_fields_dual_contouring.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1285 2023-09-06 07:48:11.000000 gempy_engine-2024.1.4/tests/test_common/test_integrations/test_multiple_grids.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      290 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_common/test_integrations/test_options.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.190174 gempy_engine-2024.1.4/tests/test_common/test_modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.200174 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1300 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cartesian_selector.pickle
--rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cov.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cov_grad.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cov_grad_sp.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cov_sp.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9055 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/distance_matrices.pickle
--rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/drift.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)   100184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/gx.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)   100184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/gy.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)   100184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/gz.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)   100128 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/test_activator.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/test_kernel_numeric2.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)    49280 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/test_octree_leaf.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)   100184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/zx.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3806 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_activator.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    27926 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_dual.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6234 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_exporter.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2109 2023-11-15 12:52:50.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_geophysics.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.200174 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      118 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/TestPykeopsNumPyEqual.test_distance_matrices.dif_ref_ref.approved.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    25216 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/one_fault_test_data.npy
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10345 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       64 2023-10-05 14:31:56.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.test_b_vector..approved.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       64 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.test_b_vector.approved.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)      109 2023-09-06 09:30:56.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.test_covariance_cubic_kernel.axis=1.approved.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5020 2023-10-05 14:50:19.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3341 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_universal.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9540 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_octrees.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1779 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_solver.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       29 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_topology.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      896 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_common/test_modules/test_weight_caching.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.200174 gempy_engine-2024.1.4/tests/test_common/test_prototyping/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_prototyping/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9854 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_common/test_prototyping/test_broadcasting.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       52 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4/tests/test_installation.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:15:45.200174 gempy_engine-2024.1.4/tests/test_pytorch/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-05 07:48:25.000000 gempy_engine-2024.1.4/tests/test_pytorch/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4808 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_pytorch/test_pytorch_gradients.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      366 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4/tests/test_pytorch/test_pytorch_installation.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2416 2023-10-05 14:42:20.000000 gempy_engine-2024.1.4/tests/verify_helper.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.639065 gempy_engine-2024.1.4b0/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      260 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4b0/.env.example
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1832 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/.gitignore
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/.vscode/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      463 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/.vscode/launch.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      523 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/AUTHORS.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    13879 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/LICENSE
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2839 2024-05-29 14:29:41.639065 gempy_engine-2024.1.4b0/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1144 2023-08-11 08:35:11.000000 gempy_engine-2024.1.4b0/README.md
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   260403 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/apibinary.le
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/gempy_engine/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/gempy_engine/API/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/API/_version.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4516 2023-11-21 09:51:13.000000 gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/_dual_contouring.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2205 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/_experimental_water_tight_DC_1.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3206 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/_interpolate_on_edges.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      114 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/_mask_buffer.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7237 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/multi_scalar_dual_contouring.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6236 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/_interp_scalar_field.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5559 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/_interp_single_feature.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12592 2024-05-16 14:21:50.000000 gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/_multi_scalar_field_manager.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3368 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/_octree_generation.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4202 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/interp_features.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/gempy_engine/API/model/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/model/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2929 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/API/model/model_api.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/gempy_engine/API/server/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1338 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/2features.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1356 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/2features_inclined.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1193 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/_old_example.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4176 2023-09-15 12:25:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/_process_output.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1923 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/_server_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1252 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/example.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3942 2023-11-14 16:11:18.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/main_server_pro.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      223 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/API/server/test_compute.http
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       61 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      419 2024-05-29 14:29:41.000000 gempy_engine-2024.1.4b0/gempy_engine/_version.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1571 2024-05-16 15:17:02.000000 gempy_engine-2024.1.4b0/gempy_engine/config.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/gempy_engine/core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    14539 2024-05-16 14:26:31.000000 gempy_engine-2024.1.4b0/gempy_engine/core/backend_tensor.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/core/data/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      308 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4203 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/centered_grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       44 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/continue_epoch.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1314 2023-10-05 13:36:58.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/custom_segmentation_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1279 2023-10-05 11:49:56.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/dual_contouring_data.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      602 2023-09-14 08:17:23.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/dual_contouring_mesh.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6150 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/engine_grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2951 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/exported_fields.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      442 2023-09-05 11:04:18.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/exported_structs.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      383 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/generic_grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      173 2023-10-06 08:38:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/geophysics_input.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3503 2023-08-17 12:00:28.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/input_data_descriptor.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1745 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/internal_structs.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5280 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/interp_output.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3045 2023-10-05 13:51:07.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/interpolation_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9088 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/interpolation_input.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1550 2023-08-17 13:49:03.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/faults.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2627 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/kernel_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3541 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/orientations.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/server/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/server/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1000 2023-08-11 11:40:58.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/server/input_parser.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      145 2023-08-09 08:33:04.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/solvers.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2278 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/surface_points.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      430 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/matrices_sizes.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1660 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/octree_level.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/core/data/options/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      180 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/options/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2326 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/options/evaluation_options.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9427 2024-05-16 15:18:40.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/options/interpolation_options.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3373 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/options/kernel_options.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      104 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/options/temp_interpolation_values.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/core/data/output/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/output/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      275 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/output/blocks_value_type.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9923 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/raw_arrays_solution.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6874 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/regular_grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4824 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/scalar_field_output.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4904 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/solutions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      198 2023-07-24 09:17:59.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/stack_relation_type.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4996 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/stacks_structure.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2587 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/tensors_structure.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10868 2023-09-05 14:24:09.000000 gempy_engine-2024.1.4b0/gempy_engine/core/data/transforms.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1286 2024-04-15 13:51:26.000000 gempy_engine-2024.1.4b0/gempy_engine/core/utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2058 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/dev_notes.md
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/modules/activator/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/activator/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2608 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/activator/activator_interface.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6245 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/activator/torch_activation.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/modules/data_preprocess/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/data_preprocess/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2402 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/data_preprocess/_input_preparation.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1651 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/data_preprocess/data_preprocess_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/modules/dual_contouring/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/dual_contouring/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11313 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/dual_contouring/dual_contouring_interface.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11330 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/dual_contouring/fancy_triangulation.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/modules/evaluator/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/evaluator/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3330 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/evaluator/generic_evaluator.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2599 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/evaluator/symbolic_evaluator.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.599065 gempy_engine-2024.1.4b0/gempy_engine/modules/geophysics/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-06 08:07:32.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/geophysics/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1929 2023-10-09 08:58:18.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/geophysics/fw_gravity.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2021 2023-10-09 08:27:43.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/geophysics/gravity_gradient.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      867 2023-10-05 12:31:28.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_b_vector_assembler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8286 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_covariance_assembler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2950 2023-10-05 09:41:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4237 2023-11-07 11:42:44.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_kernel_constructors.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1347 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_kernel_selectors.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12656 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_kernels_assembler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2519 2023-08-11 11:19:33.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_pykeops_cov_compiler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9218 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_structs.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3548 2023-08-16 13:29:03.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_test_assembler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      976 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11918 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_vectors_preparation.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1493 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/kernel_constructor_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      434 2023-09-05 12:48:43.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/README.md
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5913 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/_curvature_analysis.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1217 2023-09-06 08:37:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/_octree_common.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3604 2024-05-29 14:24:49.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/_octree_internals.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6583 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/octrees_topology_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/gempy_engine/modules/solver/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/solver/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2139 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/solver/_conjugate_gradient.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6535 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/solver/_custom_pykeops_solver.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11136 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/solver/_kernel_solve_autograd.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11945 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/solver/_kernel_solver_from_lazy_tensor.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5324 2024-05-16 14:10:20.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/solver/solver_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/gempy_engine/modules/topology/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/topology/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/topology/topology _interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/gempy_engine/modules/weights_cache/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-04-12 09:01:44.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/weights_cache/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3489 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/modules/weights_cache/weights_cache_interface.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1565 2023-10-05 08:11:53.000000 gempy_engine-2024.1.4b0/gempy_engine/optional_dependencies.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/gempy_engine/plugins/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 07:51:38.000000 gempy_engine-2024.1.4b0/gempy_engine/plugins/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/gempy_engine/plugins/plotting/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 07:51:56.000000 gempy_engine-2024.1.4b0/gempy_engine/plugins/plotting/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3976 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/gempy_engine/plugins/plotting/helper_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5609 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/gempy_engine/plugins/plotting/helper_functions_pyvista.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.639065 gempy_engine-2024.1.4b0/gempy_engine.egg-info/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2839 2024-05-29 14:29:41.000000 gempy_engine-2024.1.4b0/gempy_engine.egg-info/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    13837 2024-05-29 14:29:41.000000 gempy_engine-2024.1.4b0/gempy_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-05-29 14:29:41.000000 gempy_engine-2024.1.4b0/gempy_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      257 2024-05-29 14:29:41.000000 gempy_engine-2024.1.4b0/gempy_engine.egg-info/requires.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2024-05-29 14:29:41.000000 gempy_engine-2024.1.4b0/gempy_engine.egg-info/top_level.txt
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/requirements/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      184 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4b0/requirements/dev-requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       28 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4b0/requirements/optional-requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       29 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4b0/requirements/requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       80 2024-05-16 14:04:45.000000 gempy_engine-2024.1.4b0/requirements/server-requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2024-05-29 14:29:41.639065 gempy_engine-2024.1.4b0/setup.cfg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2593 2024-05-16 14:10:20.000000 gempy_engine-2024.1.4b0/setup.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      251 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/test.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   260148 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/test.le
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/tests/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/tests/SKIP_tensor_flow/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/SKIP_tensor_flow/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2532 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/SKIP_tensor_flow/test_backend_tensor.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2883 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/SKIP_tensor_flow/test_tensorflow.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      693 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/SKIP_tensor_flow/test_tf.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/tests/SKIP_test_large_data/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/SKIP_test_large_data/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    16424 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/SKIP_test_large_data/plot_scipy.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/tests/benchmark/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.589065 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.609065 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11112 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/NoOptsFewInput_8f0c757cc42cb56628256f233c1f66523a634aa1_20221014_121041_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11141 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/NoOptsMidInput_bd95d1107e2c3779eb123cd694479ea62bd111a9_20221014_122235_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9897 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt1FewInput_1f1b37c12217371ea50b4e1cb46fc464049d14a7_20221015_120122_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9900 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt1MidInput_67ff73c1220d60ab1b284243a043aa6b73d4ee00_20221014_202857_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11127 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl3_1bf3c987df2b548a2edfc18b5f283f0acf466df7_20221015_150147_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10536 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl5_f9f08e62a3aa03c3d2089fb55b3ed4bcc1c46f15_20221016_104901_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9153 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl6_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124647_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11131 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2MidInputOctLvl3_1bf3c987df2b548a2edfc18b5f283f0acf466df7_20221015_150632_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9153 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt3FewInputOctLvl5_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124154_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9153 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt3FewInputOctLvl6_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124502_uncommited-changes.json
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3794 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/benchmark/README.md
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/benchmark/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4234 2023-11-14 16:11:18.000000 gempy_engine-2024.1.4b0/tests/benchmark/one_fault_model.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2449 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/benchmark/profile_runner.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3344 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/benchmark/test_benchmark_one_feature.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2050 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/conftest.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.619065 gempy_engine-2024.1.4b0/tests/data/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   204949 2023-08-11 08:57:48.000000 gempy_engine-2024.1.4b0/tests/data/Moureze_Points.csv
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.619065 gempy_engine-2024.1.4b0/tests/fixtures/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8156 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/fixtures/complex_geometries.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.619065 gempy_engine-2024.1.4b0/tests/fixtures/graben_data/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1240 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9a_Fault_relations_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4468 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9a_Fault_relations_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4468 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9a_Finite_Fault_relations_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1401 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9b_Fault_relations_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4654 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9b_Fault_relations_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1179 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/fixtures/grids.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6498 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/fixtures/heavy_models.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/05_toy_fold_unconformity_interfaces.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      299 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/05_toy_fold_unconformity_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      139 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/fixture_model_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1856 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/fixture_model_surfaces.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       87 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model1_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       89 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model1_orientations_scaled.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)  3000128 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model1_scaled.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      232 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model1_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      268 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model1_surface_points_scaled.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       87 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model2_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      659 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model2_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       97 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model3_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      121 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model3_orientations_scaled.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1845 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model3_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3167 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model3_surface_points_scaled-2.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      211 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model4_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      227 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model4_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      163 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model5_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      409 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model5_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      168 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model6_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      715 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model6_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      237 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model7_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1853 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model7_surface_points.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2840 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    21434 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/fixtures/simple_models.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      123 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/pytest.ini
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/test_common/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/test_common/test_api/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_api/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/test_common/test_api/test_faults/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_api/test_faults/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6882 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_api/test_faults/test_faults_graben.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11460 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_api/test_faults/test_one_fault.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1749 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_common/test_api/test_output_to_subsurface.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5876 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_api/test_public_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/test_common/test_core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       72 2023-07-12 07:31:14.000000 gempy_engine-2024.1.4b0/tests/test_common/test_core/test_data_classes.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/test_common/test_dependencies/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_dependencies/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      542 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_dependencies/pykeops_test_compiler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    18780 2023-08-11 08:42:39.000000 gempy_engine-2024.1.4b0/tests/test_common/test_dependencies/test_pykeops.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4178 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_external_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3394 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_interpolate_model.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2102 2023-09-06 11:22:27.000000 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_kernels.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8007 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_multi_fields.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6468 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_multi_fields_dual_contouring.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1285 2023-09-06 07:48:11.000000 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_multiple_grids.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      290 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_options.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/test_common/test_modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.629065 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1300 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cartesian_selector.pickle
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cov.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cov_grad.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cov_grad_sp.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cov_sp.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9055 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/distance_matrices.pickle
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/drift.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   100184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/gx.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   100184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/gy.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   100184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/gz.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   100128 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/test_activator.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      776 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/test_kernel_numeric2.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    49280 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/test_octree_leaf.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   100184 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/zx.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3806 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_activator.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    27926 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_dual.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6234 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_exporter.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2109 2023-11-15 12:52:50.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_geophysics.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.639065 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      118 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/TestPykeopsNumPyEqual.test_distance_matrices.dif_ref_ref.approved.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    25216 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/one_fault_test_data.npy
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10345 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       64 2023-10-05 14:31:56.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.test_b_vector..approved.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       64 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.test_b_vector.approved.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      109 2023-09-06 09:30:56.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.test_covariance_cubic_kernel.axis=1.approved.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5020 2023-10-05 14:50:19.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3341 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_universal.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9540 2024-05-16 14:33:22.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_octrees.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1779 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_solver.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       29 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_topology.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      896 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_weight_caching.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.639065 gempy_engine-2024.1.4b0/tests/test_common/test_prototyping/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_prototyping/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9854 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_common/test_prototyping/test_broadcasting.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       52 2023-06-18 07:50:48.000000 gempy_engine-2024.1.4b0/tests/test_installation.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-29 14:29:41.639065 gempy_engine-2024.1.4b0/tests/test_pytorch/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-05 07:48:25.000000 gempy_engine-2024.1.4b0/tests/test_pytorch/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4808 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_pytorch/test_pytorch_gradients.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      366 2024-05-16 14:02:52.000000 gempy_engine-2024.1.4b0/tests/test_pytorch/test_pytorch_installation.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2416 2023-10-05 14:42:20.000000 gempy_engine-2024.1.4b0/tests/verify_helper.py
```

### Comparing `gempy_engine-2024.1.4/.gitignore` & `gempy_engine-2024.1.4b0/.gitignore`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/AUTHORS.rst` & `gempy_engine-2024.1.4b0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/LICENSE` & `gempy_engine-2024.1.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/PKG-INFO` & `gempy_engine-2024.1.4b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gempy_engine
-Version: 2024.1.4
+Version: 2024.1.4b0
 Summary: A Python package for GemPy
 Home-page: https://github.com/gempy-project/gempy_engine
 Author: Miguel de la Varga
 Author-email: miguel@terranigma-solutions.com
 License: EUPL-1.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gempy_engine-2024.1.4/README.md` & `gempy_engine-2024.1.4b0/README.md`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/apibinary.le` & `gempy_engine-2024.1.4b0/apibinary.le`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/_dual_contouring.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/_dual_contouring.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/_experimental_water_tight_DC_1.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/_experimental_water_tight_DC_1.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/_interpolate_on_edges.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/_interpolate_on_edges.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/dual_contouring/multi_scalar_dual_contouring.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/dual_contouring/multi_scalar_dual_contouring.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/interp_single/_interp_scalar_field.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/_interp_scalar_field.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/interp_single/_interp_single_feature.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/_interp_single_feature.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/interp_single/_multi_scalar_field_manager.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/_multi_scalar_field_manager.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/interp_single/_octree_generation.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/_octree_generation.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/interp_single/interp_features.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/interp_single/interp_features.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/model/model_api.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/model/model_api.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/server/2features.json` & `gempy_engine-2024.1.4b0/gempy_engine/API/server/2features.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/server/2features_inclined.json` & `gempy_engine-2024.1.4b0/gempy_engine/API/server/2features_inclined.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/server/_old_example.json` & `gempy_engine-2024.1.4b0/gempy_engine/API/server/_old_example.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/server/_process_output.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/server/_process_output.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/server/_server_functions.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/server/_server_functions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/server/example.json` & `gempy_engine-2024.1.4b0/gempy_engine/API/server/example.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/API/server/main_server_pro.py` & `gempy_engine-2024.1.4b0/gempy_engine/API/server/main_server_pro.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/config.py` & `gempy_engine-2024.1.4b0/gempy_engine/config.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/backend_tensor.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/backend_tensor.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/centered_grid.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/centered_grid.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/custom_segmentation_functions.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/custom_segmentation_functions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/dual_contouring_data.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/dual_contouring_data.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/dual_contouring_mesh.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/dual_contouring_mesh.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/engine_grid.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/engine_grid.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/exported_fields.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/exported_fields.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/input_data_descriptor.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/input_data_descriptor.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/internal_structs.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/internal_structs.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/interp_output.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/interp_output.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/interpolation_functions.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/interpolation_functions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/interpolation_input.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/interpolation_input.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/faults.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/faults.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/kernel_functions.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/kernel_functions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/orientations.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/orientations.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/server/input_parser.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/server/input_parser.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/kernel_classes/surface_points.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/kernel_classes/surface_points.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/octree_level.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/octree_level.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/options/evaluation_options.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/options/evaluation_options.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/options/interpolation_options.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/options/interpolation_options.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/options/kernel_options.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/options/kernel_options.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/raw_arrays_solution.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/raw_arrays_solution.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/regular_grid.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/regular_grid.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/scalar_field_output.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/scalar_field_output.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/solutions.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/solutions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/stacks_structure.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/stacks_structure.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/tensors_structure.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/tensors_structure.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/data/transforms.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/data/transforms.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/core/utils.py` & `gempy_engine-2024.1.4b0/gempy_engine/core/utils.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/dev_notes.md` & `gempy_engine-2024.1.4b0/gempy_engine/dev_notes.md`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/activator/activator_interface.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/activator/activator_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/activator/torch_activation.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/activator/torch_activation.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/data_preprocess/_input_preparation.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/data_preprocess/_input_preparation.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/data_preprocess/data_preprocess_interface.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/data_preprocess/data_preprocess_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/dual_contouring/dual_contouring_interface.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/dual_contouring/dual_contouring_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/dual_contouring/fancy_triangulation.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/dual_contouring/fancy_triangulation.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/evaluator/generic_evaluator.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/evaluator/generic_evaluator.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/evaluator/symbolic_evaluator.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/evaluator/symbolic_evaluator.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/geophysics/fw_gravity.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/geophysics/fw_gravity.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/geophysics/gravity_gradient.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/geophysics/gravity_gradient.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_b_vector_assembler.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_b_vector_assembler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_covariance_assembler.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_covariance_assembler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_kernel_constructors.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_kernel_constructors.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_kernel_selectors.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_kernel_selectors.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_kernels_assembler.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_kernels_assembler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_pykeops_cov_compiler.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_pykeops_cov_compiler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_structs.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_structs.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_test_assembler.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_test_assembler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_utils.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_utils.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/_vectors_preparation.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/_vectors_preparation.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/kernel_constructor/kernel_constructor_interface.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/kernel_constructor/kernel_constructor_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/_curvature_analysis.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/_curvature_analysis.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/_octree_common.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/_octree_common.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/_octree_internals.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/_octree_internals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import torch
-import warnings
 from typing import List, Optional
 
 from gempy_engine.core.backend_tensor import BackendTensor
 from gempy_engine.core.data.octree_level import OctreeLevel
 import numpy as np
 
 from gempy_engine.core.data.engine_grid import EngineGrid
```

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/octrees_topology/octrees_topology_interface.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/octrees_topology/octrees_topology_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/solver/_conjugate_gradient.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/solver/_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/solver/_custom_pykeops_solver.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/solver/_custom_pykeops_solver.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/solver/_kernel_solve_autograd.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/solver/_kernel_solve_autograd.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/solver/_kernel_solver_from_lazy_tensor.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/solver/_kernel_solver_from_lazy_tensor.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/solver/solver_interface.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/solver/solver_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/modules/weights_cache/weights_cache_interface.py` & `gempy_engine-2024.1.4b0/gempy_engine/modules/weights_cache/weights_cache_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/optional_dependencies.py` & `gempy_engine-2024.1.4b0/gempy_engine/optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/plugins/plotting/helper_functions.py` & `gempy_engine-2024.1.4b0/gempy_engine/plugins/plotting/helper_functions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine/plugins/plotting/helper_functions_pyvista.py` & `gempy_engine-2024.1.4b0/gempy_engine/plugins/plotting/helper_functions_pyvista.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/gempy_engine.egg-info/PKG-INFO` & `gempy_engine-2024.1.4b0/gempy_engine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gempy_engine
-Version: 2024.1.4
+Version: 2024.1.4b0
 Summary: A Python package for GemPy
 Home-page: https://github.com/gempy-project/gempy_engine
 Author: Miguel de la Varga
 Author-email: miguel@terranigma-solutions.com
 License: EUPL-1.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gempy_engine-2024.1.4/gempy_engine.egg-info/SOURCES.txt` & `gempy_engine-2024.1.4b0/gempy_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/setup.py` & `gempy_engine-2024.1.4b0/setup.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/test.le` & `gempy_engine-2024.1.4b0/test.le`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/SKIP_tensor_flow/test_backend_tensor.py` & `gempy_engine-2024.1.4b0/tests/SKIP_tensor_flow/test_backend_tensor.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/SKIP_tensor_flow/test_tensorflow.py` & `gempy_engine-2024.1.4b0/tests/SKIP_tensor_flow/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/SKIP_tensor_flow/test_tf.py` & `gempy_engine-2024.1.4b0/tests/SKIP_tensor_flow/test_tf.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/SKIP_test_large_data/plot_scipy.py` & `gempy_engine-2024.1.4b0/tests/SKIP_test_large_data/plot_scipy.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/NoOptsFewInput_8f0c757cc42cb56628256f233c1f66523a634aa1_20221014_121041_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/NoOptsFewInput_8f0c757cc42cb56628256f233c1f66523a634aa1_20221014_121041_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/NoOptsMidInput_bd95d1107e2c3779eb123cd694479ea62bd111a9_20221014_122235_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/NoOptsMidInput_bd95d1107e2c3779eb123cd694479ea62bd111a9_20221014_122235_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt1FewInput_1f1b37c12217371ea50b4e1cb46fc464049d14a7_20221015_120122_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt1FewInput_1f1b37c12217371ea50b4e1cb46fc464049d14a7_20221015_120122_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt1MidInput_67ff73c1220d60ab1b284243a043aa6b73d4ee00_20221014_202857_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt1MidInput_67ff73c1220d60ab1b284243a043aa6b73d4ee00_20221014_202857_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl3_1bf3c987df2b548a2edfc18b5f283f0acf466df7_20221015_150147_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl3_1bf3c987df2b548a2edfc18b5f283f0acf466df7_20221015_150147_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl5_f9f08e62a3aa03c3d2089fb55b3ed4bcc1c46f15_20221016_104901_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl5_f9f08e62a3aa03c3d2089fb55b3ed4bcc1c46f15_20221016_104901_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl6_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124647_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2FewInputOctLvl6_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124647_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2MidInputOctLvl3_1bf3c987df2b548a2edfc18b5f283f0acf466df7_20221015_150632_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt2MidInputOctLvl3_1bf3c987df2b548a2edfc18b5f283f0acf466df7_20221015_150632_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt3FewInputOctLvl5_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124154_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt3FewInputOctLvl5_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124154_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt3FewInputOctLvl6_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124502_uncommited-changes.json` & `gempy_engine-2024.1.4b0/tests/benchmark/.benchmarks/Linux-CPython-3.10-64bit/Opt3FewInputOctLvl6_865d9d22d7eb360de24c4dcc101106383e2ea6ec_20221016_124502_uncommited-changes.json`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/README.md` & `gempy_engine-2024.1.4b0/tests/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/one_fault_model.py` & `gempy_engine-2024.1.4b0/tests/benchmark/one_fault_model.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/profile_runner.py` & `gempy_engine-2024.1.4b0/tests/benchmark/profile_runner.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/benchmark/test_benchmark_one_feature.py` & `gempy_engine-2024.1.4b0/tests/benchmark/test_benchmark_one_feature.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/conftest.py` & `gempy_engine-2024.1.4b0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/data/Moureze_Points.csv` & `gempy_engine-2024.1.4b0/tests/data/Moureze_Points.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/complex_geometries.py` & `gempy_engine-2024.1.4b0/tests/fixtures/complex_geometries.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9a_Fault_relations_orientations.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9a_Fault_relations_orientations.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9a_Fault_relations_surface_points.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9a_Fault_relations_surface_points.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9a_Finite_Fault_relations_surface_points.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9a_Finite_Fault_relations_surface_points.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9b_Fault_relations_orientations.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9b_Fault_relations_orientations.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/graben_data/Tutorial_ch1-9b_Fault_relations_surface_points.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/graben_data/Tutorial_ch1-9b_Fault_relations_surface_points.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/grids.py` & `gempy_engine-2024.1.4b0/tests/fixtures/grids.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/heavy_models.py` & `gempy_engine-2024.1.4b0/tests/fixtures/heavy_models.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_geometries/fixture_model_surfaces.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/fixture_model_surfaces.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model1_scaled.npy` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model1_scaled.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model2_surface_points.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model2_surface_points.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model3_surface_points.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model3_surface_points.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model3_surface_points_scaled-2.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model3_surface_points_scaled-2.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model6_surface_points.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model6_surface_points.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_geometries/model7_surface_points.csv` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries/model7_surface_points.csv`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_geometries.py` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_geometries.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/fixtures/simple_models.py` & `gempy_engine-2024.1.4b0/tests/fixtures/simple_models.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_api/test_faults/test_faults_graben.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_api/test_faults/test_faults_graben.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_api/test_faults/test_one_fault.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_api/test_faults/test_one_fault.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_api/test_output_to_subsurface.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_api/test_output_to_subsurface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_api/test_public_interface.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_api/test_public_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_dependencies/pykeops_test_compiler.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_dependencies/pykeops_test_compiler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_dependencies/test_pykeops.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_dependencies/test_pykeops.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_integrations/test_external_functions.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_external_functions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_integrations/test_interpolate_model.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_interpolate_model.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_integrations/test_kernels.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_kernels.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_integrations/test_multi_fields.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_multi_fields.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_integrations/test_multi_fields_dual_contouring.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_multi_fields_dual_contouring.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_integrations/test_multiple_grids.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_integrations/test_multiple_grids.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cartesian_selector.pickle` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cartesian_selector.pickle`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cov.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cov.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cov_grad.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cov_grad.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cov_grad_sp.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cov_grad_sp.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/cov_sp.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/cov_sp.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/distance_matrices.pickle` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/distance_matrices.pickle`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/drift.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/drift.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/gx.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/gx.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/gy.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/gy.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/gz.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/gz.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/test_activator.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/test_activator.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/test_kernel_numeric2.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/test_kernel_numeric2.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/test_octree_leaf.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/test_octree_leaf.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/solutions/zx.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/solutions/zx.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_activator.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_activator.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_dual.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_dual.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_exporter.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_exporter.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_geophysics.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_geophysics.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/one_fault_test_data.npy` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/one_fault_test_data.npy`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_octrees.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_octrees.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_solver.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_solver.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_modules/test_weight_caching.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_modules/test_weight_caching.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_common/test_prototyping/test_broadcasting.py` & `gempy_engine-2024.1.4b0/tests/test_common/test_prototyping/test_broadcasting.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/test_pytorch/test_pytorch_gradients.py` & `gempy_engine-2024.1.4b0/tests/test_pytorch/test_pytorch_gradients.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2024.1.4/tests/verify_helper.py` & `gempy_engine-2024.1.4b0/tests/verify_helper.py`

 * *Files identical despite different names*

