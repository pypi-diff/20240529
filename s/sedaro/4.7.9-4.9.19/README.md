# Comparing `tmp/sedaro-4.7.9.tar.gz` & `tmp/sedaro-4.9.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedaro-4.7.9.tar", last modified: Tue Oct 17 20:12:32 2023, max compression
+gzip compressed data, was "sedaro-4.9.19.tar", last modified: Mon Jan 15 19:09:57 2024, max compression
```

## Comparing `sedaro-4.7.9.tar` & `sedaro-4.9.19.tar`

### file list

```diff
@@ -1,391 +1,659 @@
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.803264 sedaro-4.7.9/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    34889 2023-08-03 13:50:30.000000 sedaro-4.7.9/LICENSE
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15810 2023-10-17 20:12:32.802993 sedaro-4.7.9/PKG-INFO
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14933 2023-10-05 19:07:26.000000 sedaro-4.7.9/README.md
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      857 2023-10-17 20:12:20.000000 sedaro-4.7.9/pyproject.toml
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)       38 2023-10-17 20:12:32.803307 sedaro-4.7.9/setup.cfg
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.721991 sedaro-4.7.9/src/
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.727007 sedaro-4.7.9/src/sedaro/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      104 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro/__init__.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.728575 sedaro-4.7.9/src/sedaro/branches/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      126 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro/branches/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10946 2023-10-17 19:28:57.000000 sedaro-4.7.9/src/sedaro/branches/agent_template_branch.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.729099 sedaro-4.7.9/src/sedaro/branches/blocks/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)       59 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro/branches/blocks/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4530 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro/branches/blocks/block.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5374 2023-10-17 19:28:57.000000 sedaro-4.7.9/src/sedaro/branches/blocks/block_type.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5777 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro/branches/branch.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3507 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro/branches/common.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.730010 sedaro-4.7.9/src/sedaro/branches/scenario_branch/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)       44 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro/branches/scenario_branch/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2298 2023-10-17 19:28:57.000000 sedaro-4.7.9/src/sedaro/branches/scenario_branch/scenario_branch.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    25720 2023-10-17 19:28:57.000000 sedaro-4.7.9/src/sedaro/branches/scenario_branch/sim_client.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8297 2023-10-05 02:03:05.000000 sedaro-4.7.9/src/sedaro/branches/scenario_branch/study_client.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1100 2023-10-17 19:28:57.000000 sedaro-4.7.9/src/sedaro/exceptions.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2067 2023-10-05 19:16:40.000000 sedaro-4.7.9/src/sedaro/plain_request.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.731470 sedaro-4.7.9/src/sedaro/results/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      186 2023-10-05 02:03:05.000000 sedaro-4.7.9/src/sedaro/results/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5303 2023-10-05 02:03:05.000000 sedaro-4.7.9/src/sedaro/results/agent.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3685 2023-10-05 02:03:05.000000 sedaro-4.7.9/src/sedaro/results/block.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6792 2023-10-05 19:16:40.000000 sedaro-4.7.9/src/sedaro/results/series.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5135 2023-10-05 02:03:05.000000 sedaro-4.7.9/src/sedaro/results/simulation_result.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5082 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro/results/study.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3613 2023-10-05 02:03:05.000000 sedaro-4.7.9/src/sedaro/results/utils.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2788 2023-10-05 19:16:40.000000 sedaro-4.7.9/src/sedaro/sedaro_api_client.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      638 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro/settings.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4109 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro/utils.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.727753 sedaro-4.7.9/src/sedaro.egg-info/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15810 2023-10-17 20:12:32.000000 sedaro-4.7.9/src/sedaro.egg-info/PKG-INFO
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    19363 2023-10-17 20:12:32.000000 sedaro-4.7.9/src/sedaro.egg-info/SOURCES.txt
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)        1 2023-10-17 20:12:32.000000 sedaro-4.7.9/src/sedaro.egg-info/dependency_links.txt
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      150 2023-10-17 20:12:32.000000 sedaro-4.7.9/src/sedaro.egg-info/requires.txt
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)       26 2023-10-17 20:12:32.000000 sedaro-4.7.9/src/sedaro.egg-info/top_level.txt
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.732812 sedaro-4.7.9/src/sedaro_base_client/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2215 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    59948 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/api_client.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.734237 sedaro-4.7.9/src/sedaro_base_client/apis/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      214 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5474 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/path_to_api.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.737857 sedaro-4.7.9/src/sedaro_base_client/apis/paths/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      245 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      102 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/data_id.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      430 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_branch_id.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      152 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_branch_id_changes_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      155 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_branch_id_commits_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      156 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_branch_id_committed_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      150 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_branch_id_export_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      148 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_branch_id_saved_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      160 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_branch_id_share_auth_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      159 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_branch_id_template.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      200 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_branches_current_branch_id_merge_incoming_branch_id.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      130 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_repositories_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      143 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_repositories__import.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      367 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/models_repositories_repository_id.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      271 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      294 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_job_id.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      288 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_study_.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      311 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_study_job_id.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      350 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/apis/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1071 2023-09-18 00:28:53.000000 sedaro-4.7.9/src/sedaro_base_client/apis/tag_to_api.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.739395 sedaro-4.7.9/src/sedaro_base_client/apis/tags/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      446 2023-09-18 00:28:53.000000 sedaro-4.7.9/src/sedaro_base_client/apis/tags/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3075 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/tags/branches_api.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1909 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/tags/data_api.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2120 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/tags/externals_api.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2805 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/tags/jobs_api.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1954 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/tags/meta_models_api.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2361 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/apis/tags/repositories_api.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16766 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/configuration.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5946 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/exceptions.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.794138 sedaro-4.7.9/src/sedaro_base_client/model/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      352 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/model/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11313 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/agent.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8319 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/agent_group.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2891 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/agent_parameters.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4227 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_algorithm100.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4227 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_algorithm105.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4225 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_algorithm95.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3994 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4230 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_field_of_view141.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4231 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_field_of_view146.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4231 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_field_of_view147.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4164 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors110.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4164 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors115.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4162 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors20.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4162 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors51.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4162 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors56.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4505 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_algorithm110.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4337 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_attitude14.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4331 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40182 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4499 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_sensors84.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35964 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/antenna.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    30814 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/area_target.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12690 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/averaging_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4064 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/base_dissipations.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23966 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/battery.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12899 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/battery_cell.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41922 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/battery_pack.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5540 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/battery_pack_dissipations.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12664 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/body_frame_vector.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2578 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/body_frame_vector_types.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14677 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/body_in_fov_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8491 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_changes_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4732 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_create.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5454 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_merge.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4899 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_merge_conflicts_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11637 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8984 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_scenario_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8988 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_spacecraft_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9004 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_terrestrial_vehicle_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4699 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_update.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3929 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/branch_verify_password.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    20962 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/bus_regulator.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3114 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/categories.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3543 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/celestial_pointing_directions.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    26003 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/celestial_target.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15901 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/celestial_vector.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18804 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/circular_field_of_view.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7431 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/classical_orbital_elements.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6846 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/clock_config.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    33524 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/component.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4885 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/component_dissipations.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2633 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/component_parameters.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16199 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/component_to_scalar_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14440 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/compound_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2621 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/compound_operators.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3043 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/condition_relationship.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2544 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/configuration_types.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4979 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/conflicts_obj.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4070 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/constant_power_params.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3996 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/constant_resistance_params.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43142 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/cooler.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16336 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/cooperative_transmit_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5989 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/crud_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7542 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/data_bus.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11115 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/data_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10876 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/data_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3916 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/data_service_response.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4397 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/data_set.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13597 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/data_storage.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5080 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/data_type.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4328 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/deleted_entity.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    42150 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/direction_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5203 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/distance_algorithm158.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5029 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/distance_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5199 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/distance_sensors126.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5197 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/distance_sensors72.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5197 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/distance_sensors99.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5081 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/duration_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5257 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/duration_field_of_view61.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5243 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/duration_load68.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode20.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode22.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode24.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode32.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode34.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    34947 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/dynamically_loaded_component.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18419 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/ekf_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12952 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/elapsed_time_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5516 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/entity_delete_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2580 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/eps_output_types.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5831 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/equatorial_circular_reference_orbit.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5538 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/external_state_set_request.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23989 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/fixed_surface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7263 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/frame_vector_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10947 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/fuel_reservoir.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    44547 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/fully_reg_det_power_processor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7591 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/fully_reg_det_topology_params.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    19639 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/generic_ad_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22065 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/generic_od_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5152 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/geostationary_reference_orbit.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6637 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/geostationary_transfer_reference_orbit.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18419 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/gps_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35993 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/ground_target.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3388 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/group_rollers.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41624 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/heater.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4822 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/http_validation_error.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7077 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/ideal_orbital_attitude_dynamics.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2817 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/initial_state_def_type.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2584 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/input_types.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11693 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/internal_data_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5816 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/iss_reference_orbit.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    36024 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/laser_comm_module.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14577 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/load_state.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3961 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/local_pointing_directions.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17430 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/local_vector.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16492 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/lock_pointing_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    45698 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/magnetorquer.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15440 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/max_align_pointing_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13417 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/mekf_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3893 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/message_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4470 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/model_crud_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35326 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/modem.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22312 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/operational_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    42999 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/optical_attitude_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    21289 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/orbit.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4464 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/orbital_attitude_dynamics.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7282 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/orbital_elements_data.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2552 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/orders.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5688 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/panel_dissipations.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12025 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/passive_pointing_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16308 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/passive_transmit_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14459 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/per_round_external_state.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    44550 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/photovoltaic_power_processor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15069 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/pid_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6517 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/polar_circular_reference_orbit.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3539 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/polynomial_ephemeris_body.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11706 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/position_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40126 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/position_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17013 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/power_load.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    39497 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/power_processor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6539 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/processor_dissipations.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    44547 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/quasi_reg_det_power_processor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7671 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/quasi_reg_det_topology_params.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8982 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/quaternion_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2987 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/range_relationship.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    46525 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/reaction_wheel.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16250 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/receive_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22308 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/rectangular_field_of_view.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5831 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/repo_create_req.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4442 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/repo_import_req.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8993 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/repo_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5275 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/repo_update_req.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2536 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/representation.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17063 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/resistance_load.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11205 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/same_target_multi_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2801 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/satellite_parameters.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14109 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/satellite_to_satellite_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15563 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/satellite_to_scalar_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14814 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/satellite_to_target_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13261 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/scan_field_of_view_articulation_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9496 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/scenario.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13272 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/scenario_model_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5123 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/scenario_model_root.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10009 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/scenario_model_update_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35845 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3164 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/services_model_spec_models_simulation_job_statuses.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3159 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/services_model_spec_models_study_job_statuses.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2662 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/side_categories.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10735 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/simulation_job.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    46079 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/single_conv_hybrid_power_processor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5791 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/single_conv_hybrid_topology_params.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    46065 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/single_conv_mppt_power_processor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4762 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/single_conv_mppt_topology_params.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12990 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/sliding_mode_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15935 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/solar_array.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9841 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/solar_cell.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    49258 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/solar_panel.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3436 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/sort_values.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    38549 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/space_target.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    71781 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spacecraft.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    75557 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spacecraft_model_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    67434 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spacecraft_model_root.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22512 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spacecraft_model_update_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23021 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spacecraft_operational_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4757 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/speed_algorithm163.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4583 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/speed_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4753 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/speed_sensors137.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4811 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spherical_angles.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41533 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spherical_fuel_tank.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43035 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spherocylinder_fuel_tank.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14478 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/spontaneous_external_state.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4769 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/state_vector.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10776 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/static_field_of_view_articulation_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6407 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/static_thrust_control_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6914 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/study_job.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11851 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/subsystem.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6412 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/sun_synchronous_circular_orbit.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    30072 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/sun_tracking_surface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15155 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/surface_material.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43557 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_attitude_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17460 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_group.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13395 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_group_in_fov_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23003 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_group_to_satellite_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    24281 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_group_to_scalar_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23404 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_group_to_target_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13687 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_group_vector.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8151 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_in_fov_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3962 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_parameters.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40729 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_position_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41782 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_range_rate_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41770 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_range_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16092 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_to_scalar_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15249 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_to_target_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13702 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/target_vector.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10893 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/temp_controller_state.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4756 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/temperature_base323.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4492 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_attitude_dynamics.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    24590 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_vehicle.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    28366 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_vehicle_model_res.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    20243 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_vehicle_model_root.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17002 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_vehicle_update_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7707 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/thermal_design_layout.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22629 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/thermal_interface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13212 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/thermal_interface_material.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40833 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/thruster.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12881 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/time_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3815 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/tle.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10661 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/tracking_field_of_view_articulation_mode.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12536 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/triad_algorithm.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    46044 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/two_conv_mppt_power_processor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7639 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/two_conv_mppt_topology_params.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2855 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/types.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8009 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/validation_error.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4725 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/vector.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8255 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/vector_in_fov_condition.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    39027 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/vector_sensor.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    30743 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/vector_tracking_surface.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    24018 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/waypoint_path_with_duration.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23255 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/waypoint_path_with_speed.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    21203 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/model/waypoint_path_with_timestamps.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.794331 sedaro-4.7.9/src/sedaro_base_client/models/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18754 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/models/__init__.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.794528 sedaro-4.7.9/src/sedaro_base_client/paths/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1821 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/paths/__init__.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.794969 sedaro-4.7.9/src/sedaro_base_client/paths/data_id/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      309 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/data_id/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13227 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/data_id/get.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.795997 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      345 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10272 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/delete.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10153 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/get.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14210 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/patch.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14214 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/post.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.796342 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_changes_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      363 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_changes_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10314 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_changes_/get.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.796687 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_commits_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      363 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_commits_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12511 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_commits_/post.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.797057 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_committed_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      367 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_committed_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10325 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_committed_/get.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.797399 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_export_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      361 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_export_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9952 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_export_/get.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.797749 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_saved_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      359 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_saved_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10285 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_saved_/get.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.798101 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      368 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14418 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/post.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.798432 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_template/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      363 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_template/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18207 2023-09-18 00:28:53.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_template/patch.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.799093 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      411 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16399 2023-09-18 00:28:53.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.799543 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      335 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12039 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_/post.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.800021 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories__import/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      349 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories__import/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12237 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories__import/post.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.800634 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_repository_id/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      361 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_repository_id/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10280 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_repository_id/delete.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10201 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_repository_id/get.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14262 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_repository_id/patch.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.801026 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      373 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14785 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12446 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.801403 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      385 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10611 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10530 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.801864 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      385 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13157 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/get.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12413 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/post.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.802269 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      397 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10551 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/delete.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10455 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/get.py
-drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2023-10-17 20:12:32.802678 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)      427 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/__init__.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13881 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/get.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15793 2023-08-03 13:50:30.000000 sedaro-4.7.9/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/patch.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12103 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/rest.py
--rw-r--r--   0 sebastianwelsh   (501) staff       (20)    99090 2023-10-05 19:16:41.000000 sedaro-4.7.9/src/sedaro_base_client/schemas.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.757652 sedaro-4.9.19/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    34889 2023-08-03 13:50:30.000000 sedaro-4.9.19/LICENSE
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15810 2024-01-15 19:09:57.757137 sedaro-4.9.19/PKG-INFO
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14879 2024-01-15 18:29:29.000000 sedaro-4.9.19/README.md
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      889 2024-01-15 19:09:31.000000 sedaro-4.9.19/pyproject.toml
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)       38 2024-01-15 19:09:57.757714 sedaro-4.9.19/setup.cfg
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.379461 sedaro-4.9.19/src/
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.392336 sedaro-4.9.19/src/sedaro/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      104 2023-08-03 13:50:30.000000 sedaro-4.9.19/src/sedaro/__init__.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.410287 sedaro-4.9.19/src/sedaro/branches/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      126 2023-08-03 13:50:30.000000 sedaro-4.9.19/src/sedaro/branches/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13607 2024-01-15 18:17:22.000000 sedaro-4.9.19/src/sedaro/branches/agent_template_branch.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.411898 sedaro-4.9.19/src/sedaro/branches/blocks/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)       59 2023-08-03 13:50:30.000000 sedaro-4.9.19/src/sedaro/branches/blocks/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4553 2024-01-15 18:27:07.000000 sedaro-4.9.19/src/sedaro/branches/blocks/block.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5374 2023-11-24 01:06:16.000000 sedaro-4.9.19/src/sedaro/branches/blocks/block_type.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5777 2023-10-05 19:16:41.000000 sedaro-4.9.19/src/sedaro/branches/branch.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3608 2023-11-24 01:07:05.000000 sedaro-4.9.19/src/sedaro/branches/common.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.414115 sedaro-4.9.19/src/sedaro/branches/scenario_branch/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)       44 2023-08-03 13:50:30.000000 sedaro-4.9.19/src/sedaro/branches/scenario_branch/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3415 2024-01-15 18:20:09.000000 sedaro-4.9.19/src/sedaro/branches/scenario_branch/scenario_branch.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    31125 2024-01-15 17:39:36.000000 sedaro-4.9.19/src/sedaro/branches/scenario_branch/sim_client.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8297 2023-10-05 02:03:05.000000 sedaro-4.9.19/src/sedaro/branches/scenario_branch/study_client.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1100 2023-10-17 19:28:57.000000 sedaro-4.9.19/src/sedaro/exceptions.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2067 2023-10-05 19:16:40.000000 sedaro-4.9.19/src/sedaro/plain_request.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.417593 sedaro-4.9.19/src/sedaro/results/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      186 2023-10-05 02:03:05.000000 sedaro-4.9.19/src/sedaro/results/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5303 2023-10-05 02:03:05.000000 sedaro-4.9.19/src/sedaro/results/agent.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3685 2023-10-05 02:03:05.000000 sedaro-4.9.19/src/sedaro/results/block.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6792 2023-10-05 19:16:40.000000 sedaro-4.9.19/src/sedaro/results/series.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5618 2024-01-15 17:39:36.000000 sedaro-4.9.19/src/sedaro/results/simulation_result.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5082 2023-10-05 19:16:41.000000 sedaro-4.9.19/src/sedaro/results/study.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4649 2024-01-15 17:39:36.000000 sedaro-4.9.19/src/sedaro/results/utils.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2878 2024-01-15 17:39:36.000000 sedaro-4.9.19/src/sedaro/sedaro_api_client.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      638 2023-10-05 19:16:41.000000 sedaro-4.9.19/src/sedaro/settings.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4201 2024-01-15 17:39:36.000000 sedaro-4.9.19/src/sedaro/utils.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.756279 sedaro-4.9.19/src/sedaro.egg-info/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15810 2024-01-15 19:09:57.000000 sedaro-4.9.19/src/sedaro.egg-info/PKG-INFO
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    34372 2024-01-15 19:09:57.000000 sedaro-4.9.19/src/sedaro.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)        1 2024-01-15 19:09:57.000000 sedaro-4.9.19/src/sedaro.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      173 2024-01-15 19:09:57.000000 sedaro-4.9.19/src/sedaro.egg-info/requires.txt
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)       26 2024-01-15 19:09:57.000000 sedaro-4.9.19/src/sedaro.egg-info/top_level.txt
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.421024 sedaro-4.9.19/src/sedaro_base_client/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2215 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    59948 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/api_client.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.423390 sedaro-4.9.19/src/sedaro_base_client/apis/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      214 2024-01-15 18:05:29.000000 sedaro-4.9.19/src/sedaro_base_client/apis/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5474 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/apis/path_to_api.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.432942 sedaro-4.9.19/src/sedaro_base_client/apis/paths/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      245 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      102 2024-01-15 18:05:22.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/data_id.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      430 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_branch_id.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      152 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_branch_id_changes_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      155 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_branch_id_commits_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      156 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_branch_id_committed_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      150 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_branch_id_export_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      148 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_branch_id_saved_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      160 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_branch_id_share_auth_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      159 2024-01-15 18:05:27.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_branch_id_template.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      200 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_branches_current_branch_id_merge_incoming_branch_id.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      130 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_repositories_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      143 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_repositories__import.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      367 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/models_repositories_repository_id.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      271 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      294 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_job_id.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      288 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_study_.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      311 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_study_job_id.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      350 2024-01-15 18:05:24.000000 sedaro-4.9.19/src/sedaro_base_client/apis/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1071 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/apis/tag_to_api.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.436396 sedaro-4.9.19/src/sedaro_base_client/apis/tags/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      446 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/apis/tags/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3075 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/apis/tags/branches_api.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1909 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/apis/tags/data_api.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2120 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/apis/tags/externals_api.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2805 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/apis/tags/jobs_api.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1954 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/apis/tags/meta_models_api.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2361 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/apis/tags/repositories_api.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16766 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/configuration.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5946 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/exceptions.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.712100 sedaro-4.9.19/src/sedaro_base_client/model/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      352 2024-01-15 18:05:29.000000 sedaro-4.9.19/src/sedaro_base_client/model/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11313 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/agent.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11075 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/agent.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8319 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/agent_group.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8069 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/agent_group.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2891 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/agent_parameters.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2660 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/agent_parameters.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4227 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm100.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4087 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm100.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4227 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm105.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4087 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm105.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4225 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm95.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4085 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm95.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3994 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3994 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4230 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view141.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4091 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view141.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4231 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view146.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4091 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view146.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4231 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view147.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4091 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view147.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4164 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors110.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4083 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors110.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4164 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors115.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4083 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors115.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4162 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors20.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4081 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors20.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4162 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors51.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4081 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors51.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4162 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors56.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4081 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors56.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4505 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_algorithm110.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4424 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_algorithm110.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4337 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_attitude14.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4337 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_attitude14.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4331 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4331 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40182 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    39318 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4499 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_sensors84.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4418 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_sensors84.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35964 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/antenna.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35130 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/antenna.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    30814 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/area_target.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    30246 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/area_target.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12690 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/averaging_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12424 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/averaging_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4064 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/base_dissipations.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3983 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/base_dissipations.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23966 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/battery.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22859 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/battery.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12899 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/battery_cell.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11929 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/battery_cell.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41922 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/battery_pack.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40728 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/battery_pack.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5540 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/battery_pack_dissipations.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5297 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/battery_pack_dissipations.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12664 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/body_frame_vector.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12403 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/body_frame_vector.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2578 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/body_frame_vector_types.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2431 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/body_frame_vector_types.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14677 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/body_in_fov_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14409 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/body_in_fov_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8491 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_changes_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8491 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_changes_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4732 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_create.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4585 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_create.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5454 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_merge.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5181 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_merge.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4899 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_merge_conflicts_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4899 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_merge_conflicts_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11637 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11490 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8984 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_scenario_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8837 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_scenario_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8988 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_spacecraft_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8841 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_spacecraft_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9004 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_terrestrial_vehicle_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8857 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_terrestrial_vehicle_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4699 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_update.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4552 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_update.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3929 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_verify_password.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3929 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/branch_verify_password.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    20962 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/bus_regulator.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    20546 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/bus_regulator.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3114 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/categories.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2819 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/categories.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3543 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/celestial_pointing_directions.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3142 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/celestial_pointing_directions.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    26003 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/celestial_target.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    25675 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/celestial_target.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15901 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/celestial_vector.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15715 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/celestial_vector.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18804 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/circular_field_of_view.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18534 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/circular_field_of_view.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7431 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/classical_orbital_elements.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6737 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/classical_orbital_elements.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6846 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/clock_config.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6668 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/clock_config.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    33524 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/component.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    32686 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/component.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4885 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/component_dissipations.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4723 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/component_dissipations.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2633 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/component_parameters.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2458 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/component_parameters.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16199 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/component_to_scalar_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15915 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/component_to_scalar_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14440 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/compound_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14176 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/compound_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2621 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/compound_operators.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2476 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/compound_operators.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3043 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/condition_relationship.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2764 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/condition_relationship.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2544 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/configuration_types.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2413 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/configuration_types.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4979 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/conflicts_obj.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4979 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/conflicts_obj.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4070 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/constant_power_params.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3989 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/constant_power_params.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3996 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/constant_resistance_params.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3996 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/constant_resistance_params.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43142 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/cooler.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    42148 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/cooler.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16336 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/cooperative_transmit_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15968 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/cooperative_transmit_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5989 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/crud_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5989 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/crud_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7542 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_bus.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7219 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_bus.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11115 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10778 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10876 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10630 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3916 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_service_response.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3916 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_service_response.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4397 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_set.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4397 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_set.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13597 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_storage.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12929 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_storage.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5080 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_type.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4834 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/data_type.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4328 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/deleted_entity.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4328 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/deleted_entity.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    42150 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/direction_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41299 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/direction_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5203 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_algorithm158.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5122 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_algorithm158.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5029 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5029 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5199 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors126.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5118 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors126.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5197 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors72.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5116 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors72.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5197 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors99.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5116 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors99.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5081 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5081 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5257 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_field_of_view61.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5176 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_field_of_view61.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5243 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_load68.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5162 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_load68.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode20.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5184 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode20.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode22.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5184 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode22.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode24.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5184 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode24.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode32.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5184 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode32.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5265 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode34.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5184 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode34.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    34947 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/dynamically_loaded_component.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    34073 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/dynamically_loaded_component.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18419 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/ekf_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17913 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/ekf_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12952 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/elapsed_time_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12681 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/elapsed_time_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5516 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/entity_delete_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5516 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/entity_delete_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2580 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/eps_output_types.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2429 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/eps_output_types.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5831 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/equatorial_circular_reference_orbit.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5433 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/equatorial_circular_reference_orbit.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5538 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/external_state_set_request.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5538 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/external_state_set_request.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23989 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/fixed_surface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23360 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/fixed_surface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7263 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/frame_vector_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7059 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/frame_vector_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10947 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/fuel_reservoir.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10404 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/fuel_reservoir.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    44547 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/fully_reg_det_power_processor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43673 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/fully_reg_det_power_processor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7591 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/fully_reg_det_topology_params.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7186 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/fully_reg_det_topology_params.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    19639 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/generic_ad_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    19372 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/generic_ad_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22065 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/generic_od_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    21546 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/generic_od_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5152 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/geostationary_reference_orbit.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4853 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/geostationary_reference_orbit.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6637 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/geostationary_transfer_reference_orbit.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6107 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/geostationary_transfer_reference_orbit.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18419 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/gps_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17913 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/gps_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35993 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/ground_target.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35671 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/ground_target.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3388 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/group_rollers.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3023 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/group_rollers.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41624 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/heater.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40711 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/heater.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4822 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/http_validation_error.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4822 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/http_validation_error.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7077 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/ideal_orbital_attitude_dynamics.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6863 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/ideal_orbital_attitude_dynamics.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2817 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/initial_state_def_type.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2600 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/initial_state_def_type.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2584 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/input_types.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2429 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/input_types.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11693 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/internal_data_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11339 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/internal_data_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5816 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/iss_reference_orbit.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5395 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/iss_reference_orbit.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    36024 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/laser_comm_module.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35172 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/laser_comm_module.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14577 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/load_state.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14204 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/load_state.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3961 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/local_pointing_directions.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3374 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/local_pointing_directions.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17430 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/local_vector.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17184 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/local_vector.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16492 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/lock_pointing_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16229 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/lock_pointing_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    45698 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/magnetorquer.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    44647 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/magnetorquer.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15440 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/max_align_pointing_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15168 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/max_align_pointing_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13417 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/mekf_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13161 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/mekf_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3893 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/message_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3893 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/message_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4470 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/model_crud_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4470 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/model_crud_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35326 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/modem.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    34496 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/modem.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22312 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/operational_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    21973 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/operational_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    42999 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/optical_attitude_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    42135 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/optical_attitude_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    21289 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/orbit.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    20713 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/orbit.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4464 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/orbital_attitude_dynamics.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4261 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/orbital_attitude_dynamics.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7282 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/orbital_elements_data.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7282 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/orbital_elements_data.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2552 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/orders.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2411 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/orders.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5688 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/panel_dissipations.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5445 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/panel_dissipations.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12025 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/passive_pointing_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11756 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/passive_pointing_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16308 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/passive_transmit_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15948 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/passive_transmit_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14459 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/per_round_external_state.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14259 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/per_round_external_state.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    44550 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/photovoltaic_power_processor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43676 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/photovoltaic_power_processor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15069 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/pid_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14491 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/pid_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6517 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/polar_circular_reference_orbit.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5999 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/polar_circular_reference_orbit.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3539 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/polynomial_ephemeris_body.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3138 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/polynomial_ephemeris_body.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11706 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/position_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11298 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/position_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40126 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/position_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    39277 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/position_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17013 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/power_load.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16640 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/power_load.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    39497 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/power_processor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    38648 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/power_processor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6539 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/processor_dissipations.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6215 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/processor_dissipations.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    44547 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/quasi_reg_det_power_processor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43673 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/quasi_reg_det_power_processor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7671 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/quasi_reg_det_topology_params.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7266 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/quasi_reg_det_topology_params.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8982 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/quaternion_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8710 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/quaternion_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2987 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/range_relationship.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2684 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/range_relationship.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    46525 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/reaction_wheel.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    45273 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/reaction_wheel.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16250 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/receive_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15907 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/receive_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22308 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/rectangular_field_of_view.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22032 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/rectangular_field_of_view.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5831 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/repo_create_req.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5683 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/repo_create_req.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4442 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/repo_import_req.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4442 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/repo_import_req.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8993 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/repo_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8845 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/repo_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5275 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/repo_update_req.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5127 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/repo_update_req.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2536 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/representation.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2407 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/representation.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17063 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/resistance_load.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16680 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/resistance_load.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11205 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/same_target_multi_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10925 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/same_target_multi_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2801 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/satellite_parameters.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2592 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/satellite_parameters.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14109 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_satellite_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13819 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_satellite_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15563 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_scalar_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15279 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_scalar_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14814 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_target_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14530 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_target_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13261 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scan_field_of_view_articulation_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12965 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scan_field_of_view_articulation_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9496 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scenario.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9325 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scenario.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13272 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13083 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5123 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_root.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4932 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_root.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10009 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_update_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10009 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_update_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35845 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    35013 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3164 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/services_model_spec_models_simulation_job_statuses.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2861 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/services_model_spec_models_simulation_job_statuses.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3159 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/services_model_spec_models_study_job_statuses.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2856 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/services_model_spec_models_study_job_statuses.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2662 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/side_categories.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2495 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/side_categories.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10735 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/simulation_job.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10735 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/simulation_job.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    46079 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/single_conv_hybrid_power_processor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    45195 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/single_conv_hybrid_power_processor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5791 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/single_conv_hybrid_topology_params.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     5548 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/single_conv_hybrid_topology_params.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    46065 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/single_conv_mppt_power_processor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    45185 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/single_conv_mppt_power_processor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4762 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/single_conv_mppt_topology_params.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4600 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/single_conv_mppt_topology_params.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12990 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sliding_mode_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12719 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sliding_mode_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15935 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/solar_array.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15560 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/solar_array.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9841 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/solar_cell.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9442 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/solar_cell.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    49258 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/solar_panel.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    48053 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/solar_panel.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3436 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sort_values.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3055 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sort_values.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    38549 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/space_target.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    38229 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/space_target.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    71781 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    70880 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    75557 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    74638 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    67434 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_root.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    66513 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_root.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22512 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_update_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22512 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_update_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23021 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_operational_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22661 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_operational_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4757 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/speed_algorithm163.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4676 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/speed_algorithm163.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4583 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/speed_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4583 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/speed_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4753 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/speed_sensors137.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4672 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/speed_sensors137.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4811 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spherical_angles.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4551 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spherical_angles.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41533 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spherical_fuel_tank.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40431 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spherical_fuel_tank.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43035 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spherocylinder_fuel_tank.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41923 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spherocylinder_fuel_tank.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14478 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spontaneous_external_state.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14273 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/spontaneous_external_state.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4769 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/state_vector.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4769 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/state_vector.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10776 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/static_field_of_view_articulation_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10476 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/static_field_of_view_articulation_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6407 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/static_thrust_control_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6119 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/static_thrust_control_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6914 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/study_job.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6914 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/study_job.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11851 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/subsystem.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11604 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/subsystem.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6412 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sun_synchronous_circular_orbit.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     6018 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sun_synchronous_circular_orbit.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    30072 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sun_tracking_surface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    29300 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/sun_tracking_surface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15155 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/surface_material.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14323 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/surface_material.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    43557 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_attitude_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    42695 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_attitude_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17460 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17208 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13395 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_in_fov_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13112 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_in_fov_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23003 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_satellite_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22708 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_satellite_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    24281 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_scalar_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23992 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_scalar_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23404 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_target_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23115 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_target_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13687 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_vector.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13496 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_group_vector.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8151 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_in_fov_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7879 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_in_fov_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3962 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_parameters.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3421 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_parameters.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40729 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_position_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    39867 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_position_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41782 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_range_rate_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40917 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_range_rate_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    41770 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_range_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40914 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_range_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16092 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_to_scalar_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15814 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_to_scalar_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15249 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_to_target_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14971 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_to_target_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13702 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_vector.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13522 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/target_vector.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10893 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/temp_controller_state.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10624 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/temp_controller_state.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4756 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/temperature_base323.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4675 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/temperature_base323.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4492 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_attitude_dynamics.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4281 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_attitude_dynamics.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    24590 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    24176 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    28366 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_model_res.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    27934 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_model_res.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    20243 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_model_root.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    19809 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_model_root.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17002 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_update_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    17002 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_update_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7707 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/thermal_design_layout.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7404 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/thermal_design_layout.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22629 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/thermal_interface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22441 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/thermal_interface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13212 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/thermal_interface_material.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12787 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/thermal_interface_material.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    40833 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/thruster.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    39835 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/thruster.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12881 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/time_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12625 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/time_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3815 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/tle.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     3815 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/tle.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10661 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/tracking_field_of_view_articulation_mode.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10357 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/tracking_field_of_view_articulation_mode.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12536 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/triad_algorithm.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12278 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/triad_algorithm.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    46044 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/two_conv_mppt_power_processor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    45170 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/two_conv_mppt_power_processor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7639 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/two_conv_mppt_topology_params.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7234 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/two_conv_mppt_topology_params.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2855 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/types.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     2612 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/types.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8009 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/validation_error.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8009 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/validation_error.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4725 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/vector.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     4725 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/vector.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     8255 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/vector_in_fov_condition.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     7983 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/vector_in_fov_condition.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    39027 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/vector_sensor.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    38101 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/vector_sensor.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    30743 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/vector_tracking_surface.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    29965 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/vector_tracking_surface.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    24018 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_duration.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23534 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_duration.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    23255 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_speed.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    22777 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_speed.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    21203 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_timestamps.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    20715 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_timestamps.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.712576 sedaro-4.9.19/src/sedaro_base_client/models/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18754 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/models/__init__.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.713186 sedaro-4.9.19/src/sedaro_base_client/paths/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     1821 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/__init__.py
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.715074 sedaro-4.9.19/src/sedaro_base_client/paths/data_id/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      309 2024-01-15 18:05:22.000000 sedaro-4.9.19/src/sedaro_base_client/paths/data_id/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13227 2024-01-15 18:05:22.000000 sedaro-4.9.19/src/sedaro_base_client/paths/data_id/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13116 2024-01-15 18:05:22.000000 sedaro-4.9.19/src/sedaro_base_client/paths/data_id/get.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.719187 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      345 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10272 2024-01-15 18:05:18.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/delete.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10161 2024-01-15 18:05:18.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/delete.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10153 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10042 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/get.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14210 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/patch.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14099 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/patch.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14214 2024-01-15 18:05:18.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/post.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14103 2024-01-15 18:05:18.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/post.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.720695 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_changes_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      363 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_changes_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10314 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_changes_/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10203 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_changes_/get.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.722766 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_commits_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      363 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_commits_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12511 2024-01-15 18:05:18.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_commits_/post.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12400 2024-01-15 18:05:18.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_commits_/post.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.724505 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_committed_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      367 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_committed_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10325 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_committed_/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10214 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_committed_/get.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.726198 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_export_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      361 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_export_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9952 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_export_/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)     9841 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_export_/get.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.727512 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_saved_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      359 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_saved_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10285 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_saved_/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10174 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_saved_/get.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.728713 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      368 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14418 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/post.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14307 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/post.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.731174 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_template/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      363 2024-01-15 18:05:27.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_template/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18207 2024-01-15 18:05:27.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_template/patch.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    18096 2024-01-15 18:05:27.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_template/patch.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.734096 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      411 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16399 2024-01-15 18:05:19.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    16288 2024-01-15 18:05:20.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.735680 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      335 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12039 2024-01-15 18:05:27.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_/post.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    11928 2024-01-15 18:05:27.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_/post.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.737129 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories__import/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      349 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories__import/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12237 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories__import/post.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12126 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories__import/post.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.743133 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      361 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10280 2024-01-15 18:05:27.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/delete.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10169 2024-01-15 18:05:27.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/delete.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10201 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10090 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/get.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14262 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/patch.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14151 2024-01-15 18:05:28.000000 sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/patch.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.745466 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      373 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14785 2024-01-15 18:05:24.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    14586 2024-01-15 18:05:25.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12446 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12335 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.748003 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      385 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10611 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10500 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10530 2024-01-15 18:05:24.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10419 2024-01-15 18:05:24.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.750129 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      385 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13157 2024-01-15 18:05:25.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12958 2024-01-15 18:05:25.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/get.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12413 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/post.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12302 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/post.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.752694 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      397 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10551 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/delete.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10440 2024-01-15 18:05:26.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/delete.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10455 2024-01-15 18:05:25.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    10344 2024-01-15 18:05:25.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/get.pyi
+drwxr-xr-x   0 sebastianwelsh   (501) staff       (20)        0 2024-01-15 19:09:57.755404 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)      427 2024-01-15 18:05:24.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/__init__.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13881 2024-01-15 18:05:23.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/get.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    13770 2024-01-15 18:05:23.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/get.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15793 2024-01-15 18:05:24.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/patch.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    15682 2024-01-15 18:05:24.000000 sedaro-4.9.19/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/patch.pyi
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    12103 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/rest.py
+-rw-r--r--   0 sebastianwelsh   (501) staff       (20)    99090 2024-01-15 18:12:15.000000 sedaro-4.9.19/src/sedaro_base_client/schemas.py
```

### Comparing `sedaro-4.7.9/LICENSE` & `sedaro-4.9.19/LICENSE`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/PKG-INFO` & `sedaro-4.9.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: sedaro
-Version: 4.7.9
+Version: 4.9.19
 Summary: A python client to interact with the Sedaro API.
 Author-email: Sedaro <support@sedarotech.com>
 Project-URL: Homepage, https://github.com/sedaro/sedaro-python
 Project-URL: Bug Tracker, https://github.com/sedaro/sedaro-python/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi>=14.5.14
+Requires-Dist: flatdict~=4.0.1
 Requires-Dist: frozendict~=2.3.4
 Requires-Dist: python-dateutil~=2.7
 Requires-Dist: setuptools>=21.0.0
 Requires-Dist: typing_extensions~=4.3.0
 Requires-Dist: urllib3~=1.26.7
 Requires-Dist: pydash>=5.1.1
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: numpy
+Requires-Dist: orjson
 
 # Sedaro Python Client
 
 A python client for interacting with the Sedaro API using intuitive classes and methods.
 
 This client is intended to be used alongside our [OpenAPI Specification](https://sedaro.github.io/openapi/). Please refer to this documentation for detailed information on the names, attributes, and relationships of each Sedaro Block. See docstrings on classes and their methods for further instructions and explanations.
 
@@ -170,15 +172,15 @@
 solar_cell.update(partNumber="123456789")
 
 solar_cell.delete()
 
 try:
     solar_cell.update(partNumber="987654321")
 except NonexistantBlockError as e:
-    assert str(e) == f'The referenced "SolarCell" (id: {sc_id}) no longer exists.'
+    assert str(e) == f'The referenced Block with ID: {sc_id} no longer exists.'
 ```
 
 ### Multi-Block CRUD
 
 The `crud` method is also available for performing operations on multiple Sedaro blocks and/or root at the same time using kwargs as follows:
 
 - `root`: update fields on the root by passing a dictionary
@@ -285,25 +287,23 @@
     ('foo',),
     ('bar', 'Thermal'),
     ('bar', 'Power')
 ]
 data = sim.results_plain(
   start=65000,
   stop=65001,
-  limit=250,
+  sampleRank=1,
   streams=selected_streams,
-  axisOrder='TIME_MINOR'
 )
 ### alternative:
 data = sim.results_plain(
   start=65000,
   stop=65001,
-  binWidth=0.004,
+  sampleRank=8,
   streams=selected_streams,
-  axisOrder='TIME_MINOR'
 )
 ```
 
 See doc string in the `results_plain` for details on use of the arguments.
 
 ## Bulk Download
 
@@ -375,16 +375,16 @@
 
 ### Deploy (i.e. Initialize)
 
 ```python
 sim_client = sedaro.scenario('NShL7J0Rni63llTcEUp4F').simulation
 
 # Start the simulation
-# Note that when `sim_client.start()` returns, the simulation job has entered your Workspace queue to be built and run. 
-# Passing `wait=True` to start() will wait until the simulation has entered the RUNNING state before returning. 
+# Note that when `sim_client.start()` returns, the simulation job has entered your Workspace queue to be built and run.
+# Passing `wait=True` to start() will wait until the simulation has entered the RUNNING state before returning.
 # At this time, the simulation is ready for external state production/consumption
 simulation_handle = sim_client.start(wait=True)
 ```
 
 ### Consume
 
 ```python
```

### Comparing `sedaro-4.7.9/README.md` & `sedaro-4.9.19/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 solar_cell.update(partNumber="123456789")
 
 solar_cell.delete()
 
 try:
     solar_cell.update(partNumber="987654321")
 except NonexistantBlockError as e:
-    assert str(e) == f'The referenced "SolarCell" (id: {sc_id}) no longer exists.'
+    assert str(e) == f'The referenced Block with ID: {sc_id} no longer exists.'
 ```
 
 ### Multi-Block CRUD
 
 The `crud` method is also available for performing operations on multiple Sedaro blocks and/or root at the same time using kwargs as follows:
 
 - `root`: update fields on the root by passing a dictionary
@@ -261,25 +261,23 @@
     ('foo',),
     ('bar', 'Thermal'),
     ('bar', 'Power')
 ]
 data = sim.results_plain(
   start=65000,
   stop=65001,
-  limit=250,
+  sampleRank=1,
   streams=selected_streams,
-  axisOrder='TIME_MINOR'
 )
 ### alternative:
 data = sim.results_plain(
   start=65000,
   stop=65001,
-  binWidth=0.004,
+  sampleRank=8,
   streams=selected_streams,
-  axisOrder='TIME_MINOR'
 )
 ```
 
 See doc string in the `results_plain` for details on use of the arguments.
 
 ## Bulk Download
 
@@ -351,16 +349,16 @@
 
 ### Deploy (i.e. Initialize)
 
 ```python
 sim_client = sedaro.scenario('NShL7J0Rni63llTcEUp4F').simulation
 
 # Start the simulation
-# Note that when `sim_client.start()` returns, the simulation job has entered your Workspace queue to be built and run. 
-# Passing `wait=True` to start() will wait until the simulation has entered the RUNNING state before returning. 
+# Note that when `sim_client.start()` returns, the simulation job has entered your Workspace queue to be built and run.
+# Passing `wait=True` to start() will wait until the simulation has entered the RUNNING state before returning.
 # At this time, the simulation is ready for external state production/consumption
 simulation_handle = sim_client.start(wait=True)
 ```
 
 ### Consume
 
 ```python
```

### Comparing `sedaro-4.7.9/pyproject.toml` & `sedaro-4.9.19/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sedaro"
-version = "4.7.9"
+version = "4.9.19"
 description = "A python client to interact with the Sedaro API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [ "Programming Language :: Python :: 3.8", "License :: OSI Approved :: GNU General Public License v3 (GPLv3)", "Operating System :: OS Independent", "Topic :: Software Development",]
-dependencies = [ "certifi >= 14.5.14", "frozendict ~= 2.3.4", "python-dateutil ~= 2.7", "setuptools >= 21.0.0", "typing_extensions ~= 4.3.0", "urllib3 ~= 1.26.7", "pydash >= 5.1.1", "scipy >= 1.10.1", "numpy",]
+dependencies = [ "certifi >= 14.5.14", "flatdict ~= 4.0.1", "frozendict ~= 2.3.4", "python-dateutil ~= 2.7", "setuptools >= 21.0.0", "typing_extensions ~= 4.3.0", "urllib3 ~= 1.26.7", "pydash >= 5.1.1", "scipy >= 1.10.1", "numpy", "orjson",]
 [[project.authors]]
 name = "Sedaro"
 email = "support@sedarotech.com"
 
 [project.urls]
 Homepage = "https://github.com/sedaro/sedaro-python"
 "Bug Tracker" = "https://github.com/sedaro/sedaro-python/issues"
```

### Comparing `sedaro-4.7.9/src/sedaro/branches/agent_template_branch.py` & `sedaro-4.9.19/src/sedaro/branches/agent_template_branch.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,224 +12,281 @@
 
 
 class AgentTemplateBranch(Branch):
 
     def __init__(self, body: SchemaFor200ResponseBodyApplicationJson, sedaro: 'SedaroApiClient'):
         super().__init__(body, sedaro)
         if (type_ := self.data['type']) not in VEHICLE_TEMPLATES:
-            raise TypeError(f'Branch must be of type "{VEHICLE_TEMPLATES}" not "{type_}"')
+            raise TypeError(
+                f'Branch must be of type "{VEHICLE_TEMPLATES}" not "{type_}"')
 
     # ==============================================================================================================
     # For intellisense
     # ==============================================================================================================
 
-    # AGENT TEMPLATE
+    # next line used to know where to start auto edit
+    # $AUTO_EDIT_START$
+
     AngularVelocitySensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Antenna: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     AreaTarget: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
-    AttitudeDynamics: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     AveragingAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Battery: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     BatteryCell: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     BatteryPack: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     BodyFrameVector: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     BodyInFovCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     BusRegulator: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     CelestialTarget: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     CelestialVector: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     CircularFieldOfView: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Component: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ComponentToScalarCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     CompoundCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Cooler: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     CooperativeTransmitInterface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     DataBus: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     DataInterface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     DataMode: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     DataStorage: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     DataType: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     DirectionSensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     EkfAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ElapsedTimeCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     FixedSurface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     FuelReservoir: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     FullyRegDetPowerProcessor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     GenericAdAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     GenericOdAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     GpsAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     GroundTarget: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Heater: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     IdealOrbitalAttitudeDynamics: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     InternalDataInterface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     LaserCommModule: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     LoadState: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     LocalVector: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
-    LockPointingMode: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    MagneticHysteresisRod: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Magnetorquer: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     MaxAlignPointingMode: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     MekfAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Modem: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     OpticalAttitudeSensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
-    Orbit: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     OrbitalAttitudeDynamics: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     PassivePointingMode: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     PassiveTransmitInterface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    PermanentDipoleMagnet: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     PhotovoltaicPowerProcessor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     PidAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     PositionSensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     PowerLoad: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     QuasiRegDetPowerProcessor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ReactionWheel: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ReceiveInterface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     RectangularFieldOfView: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ResistanceLoad: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SameTargetMultiCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SatelliteToSatelliteCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SatelliteToScalarCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SatelliteToTargetCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ScanFieldOfViewArticulationMode: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SingleConvHybridPowerProcessor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SingleConvMpptPowerProcessor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SlidingModeAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SolarArray: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SolarCell: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SolarPanel: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
-    SpacecraftOperationalMode: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SpaceTarget: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SphericalFuelTank: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SpherocylinderFuelTank: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     StaticFieldOfViewArticulationMode: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     StaticThrustControlAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Subsystem: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SunTrackingSurface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     SurfaceMaterial: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetAttitudeSensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetGroup: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetGroupInFovCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetGroupToSatelliteCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetGroupToScalarCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetGroupToTargetCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetGroupVector: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetInFovCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetPositionSensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
-    TargetRangeSensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetRangeRateSensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    TargetRangeSensor: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetToScalarCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetToTargetCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TargetVector: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TempControllerState: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ThermalDesignLayout: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ThermalInterface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     ThermalInterfaceMaterial: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     Thruster: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TimeCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TrackingFieldOfViewArticulationMode: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TriadAlgorithm: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     TwoConvMpptPowerProcessor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     VectorInFovCondition: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     VectorSensor: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
     VectorTrackingSurface: BlockType
-    """A Sedaro `Block` class on an `AgentTemplate` branch"""
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    UnresponsiveThrusterFailureMode: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    UnresponsiveSensorFailureMode: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    CombinationalLogic: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    TriadAttitudeInitializer: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    MagneticDetumblingAlgorithm: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    GeoAreaDateTimeGroup: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    CloudFractionGroup: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    UnresponsiveReactionWheelFailureMode: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    SensorFailureMode: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    CloudFractionGroupToScalarCondition: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    FieldOfViewArticulationMode: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    PropagatedOrbitKinematics: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    SpkEphemeris: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    DynamicallyLoadedComponent: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    LockSpinPointingMode: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    FiniteStateMachine: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    RelativeSchedule: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    LogicalConfiguration: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    FixedSchedule: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    ActivePointingMode: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    StkEphemeris: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    StateTransition: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    Sensor: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    PowerProcessor: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    FiniteDifferenceOrbitInitializer: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    UnresponsiveMagnetorquerFailureMode: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    DirectMeasurementAttitudeInitializer: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    Routine: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
+    StaticAttitudeInitializer: BlockType
+    """A Sedaro `Block` class on an `AgentTemplateBranch`"""
```

### Comparing `sedaro-4.7.9/src/sedaro/branches/blocks/block.py` & `sedaro-4.9.19/src/sedaro/branches/blocks/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def __hash__(self):
         # allows a Block instance to be a key in a dictionary
         return hash(self.__class__.__name__ + self.id)
 
     @property
     def type(self) -> str:
         '''Name of the class of the Sedaro Block this `Block` instance is set up to interact with'''
-        return self._block_type.type
+        return self.data[TYPE]
 
     @property
     def data(self) -> Dict:
         '''The properties of the corresponding Sedaro Block as a dictionary'''
         self.enforce_still_exists()
         return self._branch.data[BLOCKS][self.id]
 
@@ -71,15 +71,15 @@
         """Raises and error if the Sedaro Block this `Block` instance references no longer exists.
 
         Raises:
             NonexistantBlockError: indication that the Block no longer exists.
         """
         if not self.check_still_exists():
             raise NonexistantBlockError(
-                f'The referenced "{self.type}" (id: {self.id}) no longer exists.'
+                f'The referenced Block with ID: {self.id} no longer exists.'
             )
 
     def clone(self) -> 'Block':
         """Creates a copy of the Sedaro Block corresponding to the `Block` instance this method is called on.
 
         Note:
         - if there is a name attribute, the name of the created `Block`s will have `'(clone)'` appended to it.
@@ -109,18 +109,20 @@
         Raises:
             SedaroApiException: if there is an error in the response
 
         Returns:
             Block: updated `Block` (Note: the previous `Block` reference is also updated)
         """
         if is_empty(fields):
-            raise ValueError(f'Must provide fields to update on the {self.type}.')
+            raise ValueError(
+                f'Must provide fields to update on the {self.type}.')
 
         if ID in fields and fields[ID] != self.id:
-            raise ValueError(f'Invalid value for "{ID}". Omit or ensure it is the same as this Block\'s {ID}.')
+            raise ValueError(
+                f'Invalid value for "{ID}". Omit or ensure it is the same as this Block\'s {ID}.')
 
         # NOTE: `self.data` calls `self.enforce_still_exists()`, so don't need to call here
         self._branch.crud(blocks=[{**self.data, **fields}])
         return self
 
     def delete(self) -> str:
         """Deletes the associated Sedaro Block
```

### Comparing `sedaro-4.7.9/src/sedaro/branches/blocks/block_type.py` & `sedaro-4.9.19/src/sedaro/branches/blocks/block_type.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/branches/branch.py` & `sedaro-4.9.19/src/sedaro/branches/branch.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/branches/common.py` & `sedaro-4.9.19/src/sedaro/branches/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,18 @@
         if key not in self.data:
             raise make_attr_error(key, self.data[TYPE])
         val = self.data[key]
 
         if not self.is_rel_field(key):
             return val
 
+        # If relationship is undefined, return None
+        if val is None:
+            return None
+
         side_type = self.get_rel_field_type(key)
 
         if side_type == MANY_SIDE:
             return [self._branch.block(id) for id in val]
 
         if side_type == DATA_SIDE:
             return {self._branch.block(id): data for id, data in val.items()}
```

### Comparing `sedaro-4.7.9/src/sedaro/branches/scenario_branch/scenario_branch.py` & `sedaro-4.9.19/src/sedaro/branches/scenario_branch/scenario_branch.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,26 +39,52 @@
         from .study_client import Study
         return Study(self._sedaro, self)
 
     # ==============================================================================================================
     # For intellisense
     # ==============================================================================================================
 
-    # SCENARIO
-    Agent: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
+    # next line used to know where to start auto edit
+    # $AUTO_EDIT_START$
+
     AgentGroup: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
     ClockConfig: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
-    Orbit: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    Menu: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    MenuItem: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
     PerRoundExternalState: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
     SpontaneousExternalState: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
-    WaypointPathWithTimestamps: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
     WaypointPathWithDuration: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
     WaypointPathWithSpeed: BlockType
-    """A Sedaro `Block` class on a `Scenario` branch"""
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    WaypointPathWithTimestamps: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    WidgetSpec: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    PeripheralGroundArea: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    SpkEphemeris: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    PeripheralSpacePoint: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    PropagatedOrbitKinematics: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    EcefStationaryKinematics: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    PeripheralGroundPoint: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    OverrideSet: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    StkEphemeris: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    PeripheralAgent: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    PeripheralCelestialPoint: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
+    TemplatedAgent: BlockType
+    """A Sedaro `Block` class on a `ScenarioBranch`"""
```

### Comparing `sedaro-4.7.9/src/sedaro/branches/scenario_branch/sim_client.py` & `sedaro-4.9.19/src/sedaro/branches/scenario_branch/sim_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import concurrent.futures
 import json
-import math
 import os
 import pathlib
 import tempfile
 import time
-import traceback
 from contextlib import contextmanager
 from threading import Lock
 from typing import (TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple,
                     Union)
 from zipfile import ZIP_DEFLATED, ZipFile
 
 import numpy as np
-from sedaro_base_client.apis.tags import externals_api, jobs_api
-
 from sedaro.results.simulation_result import SimulationResult
+from sedaro_base_client.apis.tags import externals_api, jobs_api
 
 from ...exceptions import (NoSimResultsError, SedaroApiException,
                            SimInitializationError)
 from ...settings import COMMON_API_KWARGS
 from ...utils import body_from_res, parse_urllib_response, progress_bar
 
 if TYPE_CHECKING:
@@ -34,14 +31,87 @@
         return {'ndarray': v.tolist()}
     if type(v) is dict:
         return {k: serdes(v) for k, v in v.items()}
     if type(v) in {list, tuple}:
         return [serdes(v) for v in v]
     return v
 
+def concat_stream_data(main, other, len_main, len_other):
+    assert type(main) == dict and type(other) == dict
+    for k in other:
+        if k not in main:
+            main[k] = [None for _ in range(len_main)]
+        main[k].extend(other[k])
+    for k in main:
+        if k not in other:
+            main[k].extend([None for _ in range(len_other)])
+
+def concat_stream(main, other, stream_id):
+    len_main = len(main[0])
+    len_other = len(other[0])
+    main[0].extend(other[0])
+    stream_id_short = stream_id.split('/')[0]
+    concat_stream_data(main[1][stream_id_short], other[1][stream_id_short], len_main, len_other)
+
+def concat_results(main, other):
+    for stream in other:
+        if stream not in main:
+            main[stream] = other[stream]
+        else: # concat stream parts
+            concat_stream(main[stream], other[stream], stream)
+
+def update_metadata(main, other):
+    for k in other['counts']:
+        if k not in main['counts']:
+            main['counts'][k] = 0
+        main['counts'][k] += other['counts'][k]
+
+def set_numeric_as_list(d):
+    if isinstance(d, dict):
+        if all(key.isdigit() for key in d.keys()):  # Check if all keys are array indexes in string form
+            return [set_numeric_as_list(d[key]) for key in sorted(d.keys(), key=int)]
+        else:
+            return {k: set_numeric_as_list(v) for k, v in d.items()}
+    return d
+
+def __set_nested(results):
+    nested = {}
+    for k in sorted(list(results.keys())):
+        v = results[k]
+        try:
+            ptr = nested
+            tokens = k.split('.')
+            for token in tokens[:-1]:
+                if token not in ptr:
+                    ptr[token] = {}
+                ptr = ptr[token]
+            ptr[tokens[-1]] = v
+        except TypeError:
+            ptr = nested
+            for token in tokens[:-1]:
+                if type(ptr[token]) == list:
+                    del ptr[token]
+                    break
+                else:
+                    ptr = ptr[token]
+            ptr = nested
+            for token in tokens[:-1]:
+                if token not in ptr:
+                    ptr[token] = {}
+                ptr = ptr[token]
+            ptr[tokens[-1]] = v
+    return nested
+
+# TODO: edge case where one page has all nones for a SV, then the next page has a bunch of vectors for it
+def set_nested(results):
+    nested = {}
+    for k in results:
+        kspl = k.split('/')[0]
+        nested[k] = (results[k][0], {kspl: set_numeric_as_list(__set_nested(results[k][1][kspl]))})
+    return nested
 
 class Simulation:
     """A client to interact with the Sedaro API simulation (jobs) routes"""
 
     def __init__(self, sedaro: 'SedaroApiClient', branch: 'ScenarioBranch'):
         """Instantiate a Sedaro `Simulation` instance
 
@@ -77,15 +147,15 @@
             res = jobs.start_simulation(
                 path_params={'branchId': self.__branch_id},
                 **COMMON_API_KWARGS
             )
         handle = SimulationHandle(body_from_res(res), self)
         if not wait:
             return handle
-        
+
         t = 0
         while t < (timeout or float('inf')):
             if (handle := handle.status())['status'] in {'PENDING', 'QUEUED'}:
                 time.sleep(0.1)
                 t += 0.1
             elif handle['status'] in {'FAILED', 'ERROR'}:
                 raise SimInitializationError(handle['message'])
@@ -166,15 +236,17 @@
         *,
         id: str = None,
         start: float = None,
         stop: float = None,
         binWidth: float = None,
         limit: float = None,
         axisOrder: str = None,
-        streams: Optional[List[Tuple[str, ...]]] = None
+        streams: Optional[List[Tuple[str, ...]]] = None,
+        sampleRate: int = None,
+        continuationToken: str = None,
     ):
         """Query latest scenario and return results as a plain dictionary from the Data Service with options to
         customize the response. If an `id` is passed, query for corresponding result rather than latest.
 
         Args:
             id (str, optional): `id` of the data array to fetch (found on `dataArray` attribute on a response from the\
                 `status` or `start` methods)
@@ -194,58 +266,105 @@
                 through the simulation.
 
             binWidth (float, optional): the width of the bins used in downsampling data, as described for `limit`. Note\
                 that `binWidth` and `limit` are not meant to be used together; undefined behavior may occur. If you\
                 would like to downsample data, use either `limit` or `binWidth`, but not both.
 
             streams (list, optional): specify which data streams you would like to fetch data for, according to the\
-                format described in the previous section. If no list is provided, data is fetched for all streams.
+                format described in the docstring for the `results` method below. If no list is provided,\
+                data is fetched for all streams.
 
             axisOrder (enum, optional): the shape of each series in the response. Options: `'TIME_MAJOR'` and\
                 `'TIME_MINOR'`. Default value, if not specified, is `'TIME_MAJOR'`.
 
         Raises:
             NoSimResultsError: if no simulation has been started.
 
         Returns:
             dict: response from the `get` request
         """
+
+        if sampleRate is None and continuationToken is None:
+            sampleRate = 1
+
         if id == None:
             id = self.status()['dataArray']
         url = f'/data/{id}?'
         if start is not None:
             url += f'&start={start}'
         if stop is not None:
             url += f'&stop={stop}'
         if binWidth is not None:
+            print("WARNING: the parameter `binWidth` is deprecated and will be removed in a future release.")
             url += f'&binWidth={binWidth}'
         elif limit is not None:
+            print("WARNING: the parameter `limit` is deprecated and will be removed in a future release.")
             url += f'&limit={limit}'
         streams = streams or []
         if len(streams) > 0:
             encodedStreams = ','.join(['.'.join(x) for x in streams])
             url += f'&streams={encodedStreams}'
         if axisOrder is not None:
             if axisOrder not in {'TIME_MAJOR',  'TIME_MINOR'}:
                 raise ValueError(
                     'axisOrder must be either "TIME_MAJOR" or "TIME_MINOR"')
             url += f'&axisOrder={axisOrder}'
+        if sampleRate is not None:
+            url += f'&sampleRate={sampleRate}'
+        if continuationToken is not None:
+            url += f'&continuationToken={continuationToken}'
         with self.__sedaro.api_client() as api:
-            response = api.call_api(url, 'GET')
+            response = api.call_api(url, 'GET', headers={'Content-Type': 'application/json'})
         _response = None
+        has_nonempty_ctoken = False
         try:
             _response = parse_urllib_response(response)
+            if 'version' in _response['meta'] and _response['meta']['version'] == 3:
+                is_v3 = True
+                if 'continuationToken' in _response['meta'] and _response['meta']['continuationToken'] is not None:
+                    has_nonempty_ctoken = True
+                    ctoken = _response['meta']['continuationToken']
+            else:
+                is_v3 = False
             if response.status != 200:
                 raise Exception()
         except:
             reason = _response['error']['message'] if _response and 'error' in _response else 'An unknown error occurred.'
             raise SedaroApiException(status=response.status, reason=reason)
+        if is_v3: # keep fetching pages until we get an empty continuation token
+            if has_nonempty_ctoken: # need to fetch more pages
+                result = _response
+                while has_nonempty_ctoken:
+                    # fetch page
+                    request_url = f'/data/{id}?&continuationToken={ctoken}'
+                    page = api.call_api(request_url, 'GET', headers={'Content-Type': 'application/json'})
+                    _page = parse_urllib_response(page)
+                    try:
+                        if 'continuationToken' in _page['meta'] and _page['meta']['continuationToken'] is not None:
+                            has_nonempty_ctoken = True
+                            ctoken = _page['meta']['continuationToken']
+                        else:
+                            has_nonempty_ctoken = False
+                        if page.status != 200:
+                            raise Exception()
+                    except Exception:
+                        reason = _page['error']['message'] if _page and 'error' in _page else 'An unknown error occurred.'
+                        raise SedaroApiException(status=page.status, reason=reason)
+                    concat_results(result['series'], _page['series'])
+                    update_metadata(result['meta'], _page['meta'])
+                _response = result
+            _response['series'] = set_nested(_response['series'])
         return _response
 
-    def results(self, job_id: str = None, streams: Optional[List[Tuple[str, ...]]] = None) -> SimulationResult:
+    def results(self,
+                job_id: str = None,
+                start: float = None,
+                stop: float = None,
+                streams: Optional[List[Tuple[str, ...]]] = None,
+                sampleRate: int = None) -> SimulationResult:
         """Query latest scenario result. If a `job_id` is passed, query for corresponding sim results rather than
         latest.
 
         If no argument is provided for `streams`, all data will be fetched. If you pass an argument to `streams`, it
         must be a list of tuples following particular rules:
 
         - Each tuple in the list can contain either 1 or 2 items.
@@ -276,22 +395,23 @@
             SedaroApiException: if no simulation has completed.
 
         Returns:
             SimulationResult: a `SimulationResult` instance to interact with the results of the sim.
         """
         '''Query latest scenario result.'''
         job = self.status(job_id)
-        data = self.results_plain(id=job['dataArray'], streams=streams or [])
+        data = self.results_plain(id=job['dataArray'], start=start, stop=stop, streams=streams or [], sampleRate=sampleRate)
         return SimulationResult(job, data)
 
     def results_poll(
         self,
         job_id: str = None,
         streams: List[Tuple[str, ...]] = None,
-        retry_interval: int = 2
+        sampleRate: int = None,
+        retry_interval: int = 2,
     ) -> SimulationResult:
         """Query latest scenario result and wait for sim to finish if it's running. If a `job_id` is passed, query for
         corresponding sim results rather than latest. See `results` method for details on using the `streams` kwarg.
 
         Args:
             job_id (str, optional): `id` of the data array from which to fetch results. Defaults to `None`.
             streams (List[Tuple[str, ...]], optional): Streams to query for. Defaults to `None`.
@@ -312,15 +432,15 @@
             if job['status'] == 'PENDING':
                 print('Simulation is building...', end='\r')
             else:
                 progress_bar(job['progress']['percentComplete'])
             job = self.status()
             time.sleep(retry_interval)
 
-        return self.results(streams=streams or [])
+        return self.results(streams=streams or [], sampleRate=sampleRate)
 
     def __download(self, p):
         agents, id, dirname, progress, progress_lock = p
         MAX_ATTEMPTS = 3
         for agent in agents:
             attempts = MAX_ATTEMPTS
             while attempts > 0:
@@ -457,15 +577,17 @@
     def results_plain(
         self,
         start: float = None,
         stop: float = None,
         binWidth: float = None,
         limit: float = None,
         axisOrder: str = None,
-        streams: Optional[List[Tuple[str, ...]]] = None
+        streams: Optional[List[Tuple[str, ...]]] = None,
+        sampleRate: int = None,
+        continuationToken: bytes = None,
     ):
         """Query simulation results as a plain dictionary from the Data Service with options to
         customize the response.
 
         Args:
             start (float, optional): the start time of the data to fetch, in MJD format. Defaults to the start of the\
                 simulation.
@@ -500,15 +622,17 @@
         return self.__sim_client.results_plain(
             id=self.__job['dataArray'],
             start=start,
             stop=stop,
             binWidth=binWidth,
             limit=limit,
             axisOrder=axisOrder,
-            streams=streams
+            streams=streams,
+            sampleRate=sampleRate,
+            continuationToken=continuationToken,
         )
 
     def results(self, streams: Optional[List[Tuple[str, ...]]] = None) -> SimulationResult:
         """Query simulaiton results.
 
         If no argument is provided for `streams`, all data will be fetched. If you pass an argument to `streams`, it
         must be a list of tuples following particular rules:
```

### Comparing `sedaro-4.7.9/src/sedaro/branches/scenario_branch/study_client.py` & `sedaro-4.9.19/src/sedaro/branches/scenario_branch/study_client.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/exceptions.py` & `sedaro-4.9.19/src/sedaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/plain_request.py` & `sedaro-4.9.19/src/sedaro/plain_request.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/results/agent.py` & `sedaro-4.9.19/src/sedaro/results/agent.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/results/block.py` & `sedaro-4.9.19/src/sedaro/results/block.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/results/series.py` & `sedaro-4.9.19/src/sedaro/results/series.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/results/simulation_result.py` & `sedaro-4.9.19/src/sedaro/results/simulation_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import datetime as dt
 import gzip
 import json
 from pathlib import Path
 from typing import Dict, List, Union
 
 from .agent import SedaroAgentResult
-from .utils import (HFILL, STATUS_ICON_MAP, _get_agent_id_name_map,
-                    _restructure_data, hfill)
+from .utils import (HFILL, STATUS_ICON_MAP, _block_type_in_supers,
+                    _get_agent_id_name_map, _restructure_data, hfill, to_time_major)
 
 
 class SimulationResult:
 
     def __init__(self, simulation: dict, data: dict):
         '''Initialize a new Simulation Result using methods on the `simulation` property of a `ScenarioBranch`.
 
@@ -26,14 +26,21 @@
         }
         self.__branch = simulation['branch']
         self.__data = data
         self.__meta: Dict = data['meta']
         raw_series = data['series']
         agent_id_name_map = _get_agent_id_name_map(self.__meta)
         self.__simpleseries, self._agent_blocks = _restructure_data(raw_series, agent_id_name_map, self.__meta)
+        try:
+            axis = self.__meta['axis']
+        except KeyError:
+            axis = 'TIME_MAJOR'
+        if axis != 'TIME_MAJOR':
+            assert axis == 'TIME_MINOR'
+            self.__simpleseries = to_time_major(self.__simpleseries)
 
     def __repr__(self) -> str:
         return f'SedaroSimulationResult(branch={self.__branch}, status={self.status})'
 
     @property
     def job_id(self):
         return self.__simulation['id']
@@ -43,23 +50,23 @@
         return self.__meta.get('id', None)
 
     @property
     def templated_agents(self) -> List[str]:
         return tuple([
             entry['name'] for _, entry
             in self.__meta['structure']['scenario']['blocks'].items()
-            if entry['type'] == 'Agent' and not entry['peripheral']
+            if _block_type_in_supers(entry['type'], self.__meta['structure']['scenario']['_supers'], super_type='TemplatedAgent')
         ])
 
     @property
     def peripheral_agents(self) -> List[str]:
         return tuple([
             entry['name'] for id_, entry
             in self.__meta['structure']['scenario']['blocks'].items()
-            if entry['type'] == 'Agent' and entry['peripheral'] and id_ in self._agent_blocks
+            if _block_type_in_supers(entry['type'], self.__meta['structure']['scenario']['_supers'], super_type='PeripheralAgent') and id_ in self._agent_blocks
         ])
 
     @property
     def status(self) -> str:
         return str(self.__simulation['status'])
 
     @property
@@ -81,15 +88,15 @@
     def __assert_success(self) -> None:
         if not self.success:
             raise ValueError(
                 'This operation cannot be completed because the simulation hasn\'t finished or failed early.')
 
     def __agent_id_from_name(self, name: str) -> str:
         for id_, entry in self.__meta['structure']['scenario']['blocks'].items():
-            if entry['type'] == 'Agent' and name == entry['name']:
+            if name == entry.get('name') and _block_type_in_supers(entry['type'], self.__meta['structure']['scenario']['_supers']):
                 if id_ in self._agent_blocks:
                     return id_
         else:
             raise ValueError(f"Agent {name} not found in data set.")
 
     def agent(self, name: str) -> SedaroAgentResult:
         '''Query results for a particular agent by name.'''
```

### Comparing `sedaro-4.7.9/src/sedaro/results/study.py` & `sedaro-4.9.19/src/sedaro/results/study.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/results/utils.py` & `sedaro-4.9.19/src/sedaro/results/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import numpy as np
 
 DEFAULT_HOST = 'https://api.sedaro.com'
 ENGINE_MAP = {
     '0': 'gnc',
     '1': 'cdh',
     '2': 'power',
     '3': 'thermal',
@@ -40,20 +41,32 @@
                         raise ValueError(f"Duplicate ID {id_}")
                     else:
                         out[id_] = value
 
     return out
 
 
+def _block_type_in_supers(block_type: str, meta_supers: dict, super_type: str = 'Agent') -> bool:
+    if block_type == super_type:
+        return True
+    elif block_type in meta_supers:
+        supertypes = meta_supers[block_type]
+        if len(supertypes) == 0:
+            return False
+        return any(_block_type_in_supers(supertype, meta_supers, super_type=super_type) for supertype in supertypes)
+    else:
+        return False
+
+
 def _get_agent_id_name_map(meta):
     '''Get mapping from agent ID to name.'''
     return {
         id_: entry['name']
         for id_, entry in meta['structure']['scenario']['blocks'].items()
-        if entry['type'] == 'Agent'
+        if _block_type_in_supers(entry['type'], meta['structure']['scenario']['_supers'])
     }
 
 
 def _simplify_series(engine_data: dict, blocks: dict) -> dict:
     '''Build a simplified series data structure
 
     Creates a dictionary with the following hierarchy:
@@ -129,7 +142,24 @@
         elif ordered_series[mid] > value:
             return _bsearch(low, mid-1)
         else:
             return _bsearch(mid, high)
     if value < ordered_series[0]:
         return -1
     return _bsearch(0, len(ordered_series) - 1)
+
+
+def to_time_major(series):
+    if type(series) not in [list, dict]:
+        return series
+    elif type(series) == dict:
+        new = {}
+        for k in series:
+            new[k] = to_time_major(series[k])
+        return new
+    else: # type(series) == list
+        np_data = np.array(series)
+        if np_data.ndim > 1:
+            axes = (np_data.ndim - 1,) + tuple(range(np_data.ndim - 1))
+            np_data = np.transpose(np_data, axes=axes)
+        reshaped_data = np_data.tolist()
+        return reshaped_data
```

### Comparing `sedaro-4.7.9/src/sedaro/sedaro_api_client.py` & `sedaro-4.9.19/src/sedaro/sedaro_api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from .utils import body_from_res
 
 
 class SedaroApiClient(ApiClient):
     """A client to interact with the Sedaro API"""
 
     def __init__(self, api_key, host='https://api.sedaro.com'):
+        if host[-1] == '/':
+            host = host[:-1]  # remove trailing forward slash
         self._api_key = api_key
         self._api_host = host
 
     @contextmanager
     def api_client(self) -> Generator[ApiClient, Any, None]:
         """Instantiate ApiClient from sedaro_base_client
```

### Comparing `sedaro-4.7.9/src/sedaro/settings.py` & `sedaro-4.9.19/src/sedaro/settings.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro/utils.py` & `sedaro-4.9.19/src/sedaro/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import importlib
 import inspect
 import json
+import orjson
 from types import ModuleType
 from typing import TYPE_CHECKING, Dict
 
 from sedaro_base_client.api_client import ApiResponse
 from urllib3.response import HTTPResponse
 
 from .exceptions import SedaroApiException
@@ -12,15 +13,18 @@
 
 if TYPE_CHECKING:
     from .branches.branch import Branch
 
 
 def parse_urllib_response(response: HTTPResponse) -> Dict:
     '''Parses the response from urllib3.response.HTTPResponse into a dictionary'''
-    return json.loads(response.data.decode('utf-8'))
+    try:
+        return orjson.loads(response.data)
+    except Exception:
+        return json.loads(response.data.decode('utf-8'))
 
 
 def check_for_res_error(response: ApiResponse):
     """Checks for an 'error' key in the response dictionary and raises that error if present.
 
     Args:
         response (ApiResponse): response from an api request
```

### Comparing `sedaro-4.7.9/src/sedaro.egg-info/PKG-INFO` & `sedaro-4.9.19/src/sedaro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: sedaro
-Version: 4.7.9
+Version: 4.9.19
 Summary: A python client to interact with the Sedaro API.
 Author-email: Sedaro <support@sedarotech.com>
 Project-URL: Homepage, https://github.com/sedaro/sedaro-python
 Project-URL: Bug Tracker, https://github.com/sedaro/sedaro-python/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi>=14.5.14
+Requires-Dist: flatdict~=4.0.1
 Requires-Dist: frozendict~=2.3.4
 Requires-Dist: python-dateutil~=2.7
 Requires-Dist: setuptools>=21.0.0
 Requires-Dist: typing_extensions~=4.3.0
 Requires-Dist: urllib3~=1.26.7
 Requires-Dist: pydash>=5.1.1
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: numpy
+Requires-Dist: orjson
 
 # Sedaro Python Client
 
 A python client for interacting with the Sedaro API using intuitive classes and methods.
 
 This client is intended to be used alongside our [OpenAPI Specification](https://sedaro.github.io/openapi/). Please refer to this documentation for detailed information on the names, attributes, and relationships of each Sedaro Block. See docstrings on classes and their methods for further instructions and explanations.
 
@@ -170,15 +172,15 @@
 solar_cell.update(partNumber="123456789")
 
 solar_cell.delete()
 
 try:
     solar_cell.update(partNumber="987654321")
 except NonexistantBlockError as e:
-    assert str(e) == f'The referenced "SolarCell" (id: {sc_id}) no longer exists.'
+    assert str(e) == f'The referenced Block with ID: {sc_id} no longer exists.'
 ```
 
 ### Multi-Block CRUD
 
 The `crud` method is also available for performing operations on multiple Sedaro blocks and/or root at the same time using kwargs as follows:
 
 - `root`: update fields on the root by passing a dictionary
@@ -285,25 +287,23 @@
     ('foo',),
     ('bar', 'Thermal'),
     ('bar', 'Power')
 ]
 data = sim.results_plain(
   start=65000,
   stop=65001,
-  limit=250,
+  sampleRank=1,
   streams=selected_streams,
-  axisOrder='TIME_MINOR'
 )
 ### alternative:
 data = sim.results_plain(
   start=65000,
   stop=65001,
-  binWidth=0.004,
+  sampleRank=8,
   streams=selected_streams,
-  axisOrder='TIME_MINOR'
 )
 ```
 
 See doc string in the `results_plain` for details on use of the arguments.
 
 ## Bulk Download
 
@@ -375,16 +375,16 @@
 
 ### Deploy (i.e. Initialize)
 
 ```python
 sim_client = sedaro.scenario('NShL7J0Rni63llTcEUp4F').simulation
 
 # Start the simulation
-# Note that when `sim_client.start()` returns, the simulation job has entered your Workspace queue to be built and run. 
-# Passing `wait=True` to start() will wait until the simulation has entered the RUNNING state before returning. 
+# Note that when `sim_client.start()` returns, the simulation job has entered your Workspace queue to be built and run.
+# Passing `wait=True` to start() will wait until the simulation has entered the RUNNING state before returning.
 # At this time, the simulation is ready for external state production/consumption
 simulation_handle = sim_client.start(wait=True)
 ```
 
 ### Consume
 
 ```python
```

### Comparing `sedaro-4.7.9/src/sedaro.egg-info/SOURCES.txt` & `sedaro-4.9.19/src/sedaro.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -63,294 +63,562 @@
 src/sedaro_base_client/apis/tags/data_api.py
 src/sedaro_base_client/apis/tags/externals_api.py
 src/sedaro_base_client/apis/tags/jobs_api.py
 src/sedaro_base_client/apis/tags/meta_models_api.py
 src/sedaro_base_client/apis/tags/repositories_api.py
 src/sedaro_base_client/model/__init__.py
 src/sedaro_base_client/model/agent.py
+src/sedaro_base_client/model/agent.pyi
 src/sedaro_base_client/model/agent_group.py
+src/sedaro_base_client/model/agent_group.pyi
 src/sedaro_base_client/model/agent_parameters.py
+src/sedaro_base_client/model/agent_parameters.pyi
 src/sedaro_base_client/model/angle_algorithm100.py
+src/sedaro_base_client/model/angle_algorithm100.pyi
 src/sedaro_base_client/model/angle_algorithm105.py
+src/sedaro_base_client/model/angle_algorithm105.pyi
 src/sedaro_base_client/model/angle_algorithm95.py
+src/sedaro_base_client/model/angle_algorithm95.pyi
 src/sedaro_base_client/model/angle_base323.py
+src/sedaro_base_client/model/angle_base323.pyi
 src/sedaro_base_client/model/angle_field_of_view141.py
+src/sedaro_base_client/model/angle_field_of_view141.pyi
 src/sedaro_base_client/model/angle_field_of_view146.py
+src/sedaro_base_client/model/angle_field_of_view146.pyi
 src/sedaro_base_client/model/angle_field_of_view147.py
+src/sedaro_base_client/model/angle_field_of_view147.pyi
 src/sedaro_base_client/model/angle_sensors110.py
+src/sedaro_base_client/model/angle_sensors110.pyi
 src/sedaro_base_client/model/angle_sensors115.py
+src/sedaro_base_client/model/angle_sensors115.pyi
 src/sedaro_base_client/model/angle_sensors20.py
+src/sedaro_base_client/model/angle_sensors20.pyi
 src/sedaro_base_client/model/angle_sensors51.py
+src/sedaro_base_client/model/angle_sensors51.pyi
 src/sedaro_base_client/model/angle_sensors56.py
+src/sedaro_base_client/model/angle_sensors56.pyi
 src/sedaro_base_client/model/angular_velocity_algorithm110.py
+src/sedaro_base_client/model/angular_velocity_algorithm110.pyi
 src/sedaro_base_client/model/angular_velocity_attitude14.py
+src/sedaro_base_client/model/angular_velocity_attitude14.pyi
 src/sedaro_base_client/model/angular_velocity_base323.py
+src/sedaro_base_client/model/angular_velocity_base323.pyi
 src/sedaro_base_client/model/angular_velocity_sensor.py
+src/sedaro_base_client/model/angular_velocity_sensor.pyi
 src/sedaro_base_client/model/angular_velocity_sensors84.py
+src/sedaro_base_client/model/angular_velocity_sensors84.pyi
 src/sedaro_base_client/model/antenna.py
+src/sedaro_base_client/model/antenna.pyi
 src/sedaro_base_client/model/area_target.py
+src/sedaro_base_client/model/area_target.pyi
 src/sedaro_base_client/model/averaging_algorithm.py
+src/sedaro_base_client/model/averaging_algorithm.pyi
 src/sedaro_base_client/model/base_dissipations.py
+src/sedaro_base_client/model/base_dissipations.pyi
 src/sedaro_base_client/model/battery.py
+src/sedaro_base_client/model/battery.pyi
 src/sedaro_base_client/model/battery_cell.py
+src/sedaro_base_client/model/battery_cell.pyi
 src/sedaro_base_client/model/battery_pack.py
+src/sedaro_base_client/model/battery_pack.pyi
 src/sedaro_base_client/model/battery_pack_dissipations.py
+src/sedaro_base_client/model/battery_pack_dissipations.pyi
 src/sedaro_base_client/model/body_frame_vector.py
+src/sedaro_base_client/model/body_frame_vector.pyi
 src/sedaro_base_client/model/body_frame_vector_types.py
+src/sedaro_base_client/model/body_frame_vector_types.pyi
 src/sedaro_base_client/model/body_in_fov_condition.py
+src/sedaro_base_client/model/body_in_fov_condition.pyi
 src/sedaro_base_client/model/branch_changes_res.py
+src/sedaro_base_client/model/branch_changes_res.pyi
 src/sedaro_base_client/model/branch_create.py
+src/sedaro_base_client/model/branch_create.pyi
 src/sedaro_base_client/model/branch_merge.py
+src/sedaro_base_client/model/branch_merge.pyi
 src/sedaro_base_client/model/branch_merge_conflicts_res.py
+src/sedaro_base_client/model/branch_merge_conflicts_res.pyi
 src/sedaro_base_client/model/branch_res.py
+src/sedaro_base_client/model/branch_res.pyi
 src/sedaro_base_client/model/branch_scenario_res.py
+src/sedaro_base_client/model/branch_scenario_res.pyi
 src/sedaro_base_client/model/branch_spacecraft_res.py
+src/sedaro_base_client/model/branch_spacecraft_res.pyi
 src/sedaro_base_client/model/branch_terrestrial_vehicle_res.py
+src/sedaro_base_client/model/branch_terrestrial_vehicle_res.pyi
 src/sedaro_base_client/model/branch_update.py
+src/sedaro_base_client/model/branch_update.pyi
 src/sedaro_base_client/model/branch_verify_password.py
+src/sedaro_base_client/model/branch_verify_password.pyi
 src/sedaro_base_client/model/bus_regulator.py
+src/sedaro_base_client/model/bus_regulator.pyi
 src/sedaro_base_client/model/categories.py
+src/sedaro_base_client/model/categories.pyi
 src/sedaro_base_client/model/celestial_pointing_directions.py
+src/sedaro_base_client/model/celestial_pointing_directions.pyi
 src/sedaro_base_client/model/celestial_target.py
+src/sedaro_base_client/model/celestial_target.pyi
 src/sedaro_base_client/model/celestial_vector.py
+src/sedaro_base_client/model/celestial_vector.pyi
 src/sedaro_base_client/model/circular_field_of_view.py
+src/sedaro_base_client/model/circular_field_of_view.pyi
 src/sedaro_base_client/model/classical_orbital_elements.py
+src/sedaro_base_client/model/classical_orbital_elements.pyi
 src/sedaro_base_client/model/clock_config.py
+src/sedaro_base_client/model/clock_config.pyi
 src/sedaro_base_client/model/component.py
+src/sedaro_base_client/model/component.pyi
 src/sedaro_base_client/model/component_dissipations.py
+src/sedaro_base_client/model/component_dissipations.pyi
 src/sedaro_base_client/model/component_parameters.py
+src/sedaro_base_client/model/component_parameters.pyi
 src/sedaro_base_client/model/component_to_scalar_condition.py
+src/sedaro_base_client/model/component_to_scalar_condition.pyi
 src/sedaro_base_client/model/compound_condition.py
+src/sedaro_base_client/model/compound_condition.pyi
 src/sedaro_base_client/model/compound_operators.py
+src/sedaro_base_client/model/compound_operators.pyi
 src/sedaro_base_client/model/condition_relationship.py
+src/sedaro_base_client/model/condition_relationship.pyi
 src/sedaro_base_client/model/configuration_types.py
+src/sedaro_base_client/model/configuration_types.pyi
 src/sedaro_base_client/model/conflicts_obj.py
+src/sedaro_base_client/model/conflicts_obj.pyi
 src/sedaro_base_client/model/constant_power_params.py
+src/sedaro_base_client/model/constant_power_params.pyi
 src/sedaro_base_client/model/constant_resistance_params.py
+src/sedaro_base_client/model/constant_resistance_params.pyi
 src/sedaro_base_client/model/cooler.py
+src/sedaro_base_client/model/cooler.pyi
 src/sedaro_base_client/model/cooperative_transmit_interface.py
+src/sedaro_base_client/model/cooperative_transmit_interface.pyi
 src/sedaro_base_client/model/crud_res.py
+src/sedaro_base_client/model/crud_res.pyi
 src/sedaro_base_client/model/data_bus.py
+src/sedaro_base_client/model/data_bus.pyi
 src/sedaro_base_client/model/data_interface.py
+src/sedaro_base_client/model/data_interface.pyi
 src/sedaro_base_client/model/data_mode.py
+src/sedaro_base_client/model/data_mode.pyi
 src/sedaro_base_client/model/data_service_response.py
+src/sedaro_base_client/model/data_service_response.pyi
 src/sedaro_base_client/model/data_set.py
+src/sedaro_base_client/model/data_set.pyi
 src/sedaro_base_client/model/data_storage.py
+src/sedaro_base_client/model/data_storage.pyi
 src/sedaro_base_client/model/data_type.py
+src/sedaro_base_client/model/data_type.pyi
 src/sedaro_base_client/model/deleted_entity.py
+src/sedaro_base_client/model/deleted_entity.pyi
 src/sedaro_base_client/model/direction_sensor.py
+src/sedaro_base_client/model/direction_sensor.pyi
 src/sedaro_base_client/model/distance_algorithm158.py
+src/sedaro_base_client/model/distance_algorithm158.pyi
 src/sedaro_base_client/model/distance_base323.py
+src/sedaro_base_client/model/distance_base323.pyi
 src/sedaro_base_client/model/distance_sensors126.py
+src/sedaro_base_client/model/distance_sensors126.pyi
 src/sedaro_base_client/model/distance_sensors72.py
+src/sedaro_base_client/model/distance_sensors72.pyi
 src/sedaro_base_client/model/distance_sensors99.py
+src/sedaro_base_client/model/distance_sensors99.pyi
 src/sedaro_base_client/model/duration_base323.py
+src/sedaro_base_client/model/duration_base323.pyi
 src/sedaro_base_client/model/duration_field_of_view61.py
+src/sedaro_base_client/model/duration_field_of_view61.pyi
 src/sedaro_base_client/model/duration_load68.py
+src/sedaro_base_client/model/duration_load68.pyi
 src/sedaro_base_client/model/duration_operational_mode20.py
+src/sedaro_base_client/model/duration_operational_mode20.pyi
 src/sedaro_base_client/model/duration_operational_mode22.py
+src/sedaro_base_client/model/duration_operational_mode22.pyi
 src/sedaro_base_client/model/duration_operational_mode24.py
+src/sedaro_base_client/model/duration_operational_mode24.pyi
 src/sedaro_base_client/model/duration_operational_mode32.py
+src/sedaro_base_client/model/duration_operational_mode32.pyi
 src/sedaro_base_client/model/duration_operational_mode34.py
+src/sedaro_base_client/model/duration_operational_mode34.pyi
 src/sedaro_base_client/model/dynamically_loaded_component.py
+src/sedaro_base_client/model/dynamically_loaded_component.pyi
 src/sedaro_base_client/model/ekf_algorithm.py
+src/sedaro_base_client/model/ekf_algorithm.pyi
 src/sedaro_base_client/model/elapsed_time_condition.py
+src/sedaro_base_client/model/elapsed_time_condition.pyi
 src/sedaro_base_client/model/entity_delete_res.py
+src/sedaro_base_client/model/entity_delete_res.pyi
 src/sedaro_base_client/model/eps_output_types.py
+src/sedaro_base_client/model/eps_output_types.pyi
 src/sedaro_base_client/model/equatorial_circular_reference_orbit.py
+src/sedaro_base_client/model/equatorial_circular_reference_orbit.pyi
 src/sedaro_base_client/model/external_state_set_request.py
+src/sedaro_base_client/model/external_state_set_request.pyi
 src/sedaro_base_client/model/fixed_surface.py
+src/sedaro_base_client/model/fixed_surface.pyi
 src/sedaro_base_client/model/frame_vector_base323.py
+src/sedaro_base_client/model/frame_vector_base323.pyi
 src/sedaro_base_client/model/fuel_reservoir.py
+src/sedaro_base_client/model/fuel_reservoir.pyi
 src/sedaro_base_client/model/fully_reg_det_power_processor.py
+src/sedaro_base_client/model/fully_reg_det_power_processor.pyi
 src/sedaro_base_client/model/fully_reg_det_topology_params.py
+src/sedaro_base_client/model/fully_reg_det_topology_params.pyi
 src/sedaro_base_client/model/generic_ad_algorithm.py
+src/sedaro_base_client/model/generic_ad_algorithm.pyi
 src/sedaro_base_client/model/generic_od_algorithm.py
+src/sedaro_base_client/model/generic_od_algorithm.pyi
 src/sedaro_base_client/model/geostationary_reference_orbit.py
+src/sedaro_base_client/model/geostationary_reference_orbit.pyi
 src/sedaro_base_client/model/geostationary_transfer_reference_orbit.py
+src/sedaro_base_client/model/geostationary_transfer_reference_orbit.pyi
 src/sedaro_base_client/model/gps_algorithm.py
+src/sedaro_base_client/model/gps_algorithm.pyi
 src/sedaro_base_client/model/ground_target.py
+src/sedaro_base_client/model/ground_target.pyi
 src/sedaro_base_client/model/group_rollers.py
+src/sedaro_base_client/model/group_rollers.pyi
 src/sedaro_base_client/model/heater.py
+src/sedaro_base_client/model/heater.pyi
 src/sedaro_base_client/model/http_validation_error.py
+src/sedaro_base_client/model/http_validation_error.pyi
 src/sedaro_base_client/model/ideal_orbital_attitude_dynamics.py
+src/sedaro_base_client/model/ideal_orbital_attitude_dynamics.pyi
 src/sedaro_base_client/model/initial_state_def_type.py
+src/sedaro_base_client/model/initial_state_def_type.pyi
 src/sedaro_base_client/model/input_types.py
+src/sedaro_base_client/model/input_types.pyi
 src/sedaro_base_client/model/internal_data_interface.py
+src/sedaro_base_client/model/internal_data_interface.pyi
 src/sedaro_base_client/model/iss_reference_orbit.py
+src/sedaro_base_client/model/iss_reference_orbit.pyi
 src/sedaro_base_client/model/laser_comm_module.py
+src/sedaro_base_client/model/laser_comm_module.pyi
 src/sedaro_base_client/model/load_state.py
+src/sedaro_base_client/model/load_state.pyi
 src/sedaro_base_client/model/local_pointing_directions.py
+src/sedaro_base_client/model/local_pointing_directions.pyi
 src/sedaro_base_client/model/local_vector.py
+src/sedaro_base_client/model/local_vector.pyi
 src/sedaro_base_client/model/lock_pointing_mode.py
+src/sedaro_base_client/model/lock_pointing_mode.pyi
 src/sedaro_base_client/model/magnetorquer.py
+src/sedaro_base_client/model/magnetorquer.pyi
 src/sedaro_base_client/model/max_align_pointing_mode.py
+src/sedaro_base_client/model/max_align_pointing_mode.pyi
 src/sedaro_base_client/model/mekf_algorithm.py
+src/sedaro_base_client/model/mekf_algorithm.pyi
 src/sedaro_base_client/model/message_res.py
+src/sedaro_base_client/model/message_res.pyi
 src/sedaro_base_client/model/model_crud_res.py
+src/sedaro_base_client/model/model_crud_res.pyi
 src/sedaro_base_client/model/modem.py
+src/sedaro_base_client/model/modem.pyi
 src/sedaro_base_client/model/operational_mode.py
+src/sedaro_base_client/model/operational_mode.pyi
 src/sedaro_base_client/model/optical_attitude_sensor.py
+src/sedaro_base_client/model/optical_attitude_sensor.pyi
 src/sedaro_base_client/model/orbit.py
+src/sedaro_base_client/model/orbit.pyi
 src/sedaro_base_client/model/orbital_attitude_dynamics.py
+src/sedaro_base_client/model/orbital_attitude_dynamics.pyi
 src/sedaro_base_client/model/orbital_elements_data.py
+src/sedaro_base_client/model/orbital_elements_data.pyi
 src/sedaro_base_client/model/orders.py
+src/sedaro_base_client/model/orders.pyi
 src/sedaro_base_client/model/panel_dissipations.py
+src/sedaro_base_client/model/panel_dissipations.pyi
 src/sedaro_base_client/model/passive_pointing_mode.py
+src/sedaro_base_client/model/passive_pointing_mode.pyi
 src/sedaro_base_client/model/passive_transmit_interface.py
+src/sedaro_base_client/model/passive_transmit_interface.pyi
 src/sedaro_base_client/model/per_round_external_state.py
+src/sedaro_base_client/model/per_round_external_state.pyi
 src/sedaro_base_client/model/photovoltaic_power_processor.py
+src/sedaro_base_client/model/photovoltaic_power_processor.pyi
 src/sedaro_base_client/model/pid_algorithm.py
+src/sedaro_base_client/model/pid_algorithm.pyi
 src/sedaro_base_client/model/polar_circular_reference_orbit.py
+src/sedaro_base_client/model/polar_circular_reference_orbit.pyi
 src/sedaro_base_client/model/polynomial_ephemeris_body.py
+src/sedaro_base_client/model/polynomial_ephemeris_body.pyi
 src/sedaro_base_client/model/position_base323.py
+src/sedaro_base_client/model/position_base323.pyi
 src/sedaro_base_client/model/position_sensor.py
+src/sedaro_base_client/model/position_sensor.pyi
 src/sedaro_base_client/model/power_load.py
+src/sedaro_base_client/model/power_load.pyi
 src/sedaro_base_client/model/power_processor.py
+src/sedaro_base_client/model/power_processor.pyi
 src/sedaro_base_client/model/processor_dissipations.py
+src/sedaro_base_client/model/processor_dissipations.pyi
 src/sedaro_base_client/model/quasi_reg_det_power_processor.py
+src/sedaro_base_client/model/quasi_reg_det_power_processor.pyi
 src/sedaro_base_client/model/quasi_reg_det_topology_params.py
+src/sedaro_base_client/model/quasi_reg_det_topology_params.pyi
 src/sedaro_base_client/model/quaternion_base323.py
+src/sedaro_base_client/model/quaternion_base323.pyi
 src/sedaro_base_client/model/range_relationship.py
+src/sedaro_base_client/model/range_relationship.pyi
 src/sedaro_base_client/model/reaction_wheel.py
+src/sedaro_base_client/model/reaction_wheel.pyi
 src/sedaro_base_client/model/receive_interface.py
+src/sedaro_base_client/model/receive_interface.pyi
 src/sedaro_base_client/model/rectangular_field_of_view.py
+src/sedaro_base_client/model/rectangular_field_of_view.pyi
 src/sedaro_base_client/model/repo_create_req.py
+src/sedaro_base_client/model/repo_create_req.pyi
 src/sedaro_base_client/model/repo_import_req.py
+src/sedaro_base_client/model/repo_import_req.pyi
 src/sedaro_base_client/model/repo_res.py
+src/sedaro_base_client/model/repo_res.pyi
 src/sedaro_base_client/model/repo_update_req.py
+src/sedaro_base_client/model/repo_update_req.pyi
 src/sedaro_base_client/model/representation.py
+src/sedaro_base_client/model/representation.pyi
 src/sedaro_base_client/model/resistance_load.py
+src/sedaro_base_client/model/resistance_load.pyi
 src/sedaro_base_client/model/same_target_multi_condition.py
+src/sedaro_base_client/model/same_target_multi_condition.pyi
 src/sedaro_base_client/model/satellite_parameters.py
+src/sedaro_base_client/model/satellite_parameters.pyi
 src/sedaro_base_client/model/satellite_to_satellite_condition.py
+src/sedaro_base_client/model/satellite_to_satellite_condition.pyi
 src/sedaro_base_client/model/satellite_to_scalar_condition.py
+src/sedaro_base_client/model/satellite_to_scalar_condition.pyi
 src/sedaro_base_client/model/satellite_to_target_condition.py
+src/sedaro_base_client/model/satellite_to_target_condition.pyi
 src/sedaro_base_client/model/scan_field_of_view_articulation_mode.py
+src/sedaro_base_client/model/scan_field_of_view_articulation_mode.pyi
 src/sedaro_base_client/model/scenario.py
+src/sedaro_base_client/model/scenario.pyi
 src/sedaro_base_client/model/scenario_model_res.py
+src/sedaro_base_client/model/scenario_model_res.pyi
 src/sedaro_base_client/model/scenario_model_root.py
+src/sedaro_base_client/model/scenario_model_root.pyi
 src/sedaro_base_client/model/scenario_model_update_interface.py
+src/sedaro_base_client/model/scenario_model_update_interface.pyi
 src/sedaro_base_client/model/sensor.py
+src/sedaro_base_client/model/sensor.pyi
 src/sedaro_base_client/model/services_model_spec_models_simulation_job_statuses.py
+src/sedaro_base_client/model/services_model_spec_models_simulation_job_statuses.pyi
 src/sedaro_base_client/model/services_model_spec_models_study_job_statuses.py
+src/sedaro_base_client/model/services_model_spec_models_study_job_statuses.pyi
 src/sedaro_base_client/model/side_categories.py
+src/sedaro_base_client/model/side_categories.pyi
 src/sedaro_base_client/model/simulation_job.py
+src/sedaro_base_client/model/simulation_job.pyi
 src/sedaro_base_client/model/single_conv_hybrid_power_processor.py
+src/sedaro_base_client/model/single_conv_hybrid_power_processor.pyi
 src/sedaro_base_client/model/single_conv_hybrid_topology_params.py
+src/sedaro_base_client/model/single_conv_hybrid_topology_params.pyi
 src/sedaro_base_client/model/single_conv_mppt_power_processor.py
+src/sedaro_base_client/model/single_conv_mppt_power_processor.pyi
 src/sedaro_base_client/model/single_conv_mppt_topology_params.py
+src/sedaro_base_client/model/single_conv_mppt_topology_params.pyi
 src/sedaro_base_client/model/sliding_mode_algorithm.py
+src/sedaro_base_client/model/sliding_mode_algorithm.pyi
 src/sedaro_base_client/model/solar_array.py
+src/sedaro_base_client/model/solar_array.pyi
 src/sedaro_base_client/model/solar_cell.py
+src/sedaro_base_client/model/solar_cell.pyi
 src/sedaro_base_client/model/solar_panel.py
+src/sedaro_base_client/model/solar_panel.pyi
 src/sedaro_base_client/model/sort_values.py
+src/sedaro_base_client/model/sort_values.pyi
 src/sedaro_base_client/model/space_target.py
+src/sedaro_base_client/model/space_target.pyi
 src/sedaro_base_client/model/spacecraft.py
+src/sedaro_base_client/model/spacecraft.pyi
 src/sedaro_base_client/model/spacecraft_model_res.py
+src/sedaro_base_client/model/spacecraft_model_res.pyi
 src/sedaro_base_client/model/spacecraft_model_root.py
+src/sedaro_base_client/model/spacecraft_model_root.pyi
 src/sedaro_base_client/model/spacecraft_model_update_interface.py
+src/sedaro_base_client/model/spacecraft_model_update_interface.pyi
 src/sedaro_base_client/model/spacecraft_operational_mode.py
+src/sedaro_base_client/model/spacecraft_operational_mode.pyi
 src/sedaro_base_client/model/speed_algorithm163.py
+src/sedaro_base_client/model/speed_algorithm163.pyi
 src/sedaro_base_client/model/speed_base323.py
+src/sedaro_base_client/model/speed_base323.pyi
 src/sedaro_base_client/model/speed_sensors137.py
+src/sedaro_base_client/model/speed_sensors137.pyi
 src/sedaro_base_client/model/spherical_angles.py
+src/sedaro_base_client/model/spherical_angles.pyi
 src/sedaro_base_client/model/spherical_fuel_tank.py
+src/sedaro_base_client/model/spherical_fuel_tank.pyi
 src/sedaro_base_client/model/spherocylinder_fuel_tank.py
+src/sedaro_base_client/model/spherocylinder_fuel_tank.pyi
 src/sedaro_base_client/model/spontaneous_external_state.py
+src/sedaro_base_client/model/spontaneous_external_state.pyi
 src/sedaro_base_client/model/state_vector.py
+src/sedaro_base_client/model/state_vector.pyi
 src/sedaro_base_client/model/static_field_of_view_articulation_mode.py
+src/sedaro_base_client/model/static_field_of_view_articulation_mode.pyi
 src/sedaro_base_client/model/static_thrust_control_algorithm.py
+src/sedaro_base_client/model/static_thrust_control_algorithm.pyi
 src/sedaro_base_client/model/study_job.py
+src/sedaro_base_client/model/study_job.pyi
 src/sedaro_base_client/model/subsystem.py
+src/sedaro_base_client/model/subsystem.pyi
 src/sedaro_base_client/model/sun_synchronous_circular_orbit.py
+src/sedaro_base_client/model/sun_synchronous_circular_orbit.pyi
 src/sedaro_base_client/model/sun_tracking_surface.py
+src/sedaro_base_client/model/sun_tracking_surface.pyi
 src/sedaro_base_client/model/surface_material.py
+src/sedaro_base_client/model/surface_material.pyi
 src/sedaro_base_client/model/target_attitude_sensor.py
+src/sedaro_base_client/model/target_attitude_sensor.pyi
 src/sedaro_base_client/model/target_group.py
+src/sedaro_base_client/model/target_group.pyi
 src/sedaro_base_client/model/target_group_in_fov_condition.py
+src/sedaro_base_client/model/target_group_in_fov_condition.pyi
 src/sedaro_base_client/model/target_group_to_satellite_condition.py
+src/sedaro_base_client/model/target_group_to_satellite_condition.pyi
 src/sedaro_base_client/model/target_group_to_scalar_condition.py
+src/sedaro_base_client/model/target_group_to_scalar_condition.pyi
 src/sedaro_base_client/model/target_group_to_target_condition.py
+src/sedaro_base_client/model/target_group_to_target_condition.pyi
 src/sedaro_base_client/model/target_group_vector.py
+src/sedaro_base_client/model/target_group_vector.pyi
 src/sedaro_base_client/model/target_in_fov_condition.py
+src/sedaro_base_client/model/target_in_fov_condition.pyi
 src/sedaro_base_client/model/target_parameters.py
+src/sedaro_base_client/model/target_parameters.pyi
 src/sedaro_base_client/model/target_position_sensor.py
+src/sedaro_base_client/model/target_position_sensor.pyi
 src/sedaro_base_client/model/target_range_rate_sensor.py
+src/sedaro_base_client/model/target_range_rate_sensor.pyi
 src/sedaro_base_client/model/target_range_sensor.py
+src/sedaro_base_client/model/target_range_sensor.pyi
 src/sedaro_base_client/model/target_to_scalar_condition.py
+src/sedaro_base_client/model/target_to_scalar_condition.pyi
 src/sedaro_base_client/model/target_to_target_condition.py
+src/sedaro_base_client/model/target_to_target_condition.pyi
 src/sedaro_base_client/model/target_vector.py
+src/sedaro_base_client/model/target_vector.pyi
 src/sedaro_base_client/model/temp_controller_state.py
+src/sedaro_base_client/model/temp_controller_state.pyi
 src/sedaro_base_client/model/temperature_base323.py
+src/sedaro_base_client/model/temperature_base323.pyi
 src/sedaro_base_client/model/terrestrial_attitude_dynamics.py
+src/sedaro_base_client/model/terrestrial_attitude_dynamics.pyi
 src/sedaro_base_client/model/terrestrial_vehicle.py
+src/sedaro_base_client/model/terrestrial_vehicle.pyi
 src/sedaro_base_client/model/terrestrial_vehicle_model_res.py
+src/sedaro_base_client/model/terrestrial_vehicle_model_res.pyi
 src/sedaro_base_client/model/terrestrial_vehicle_model_root.py
+src/sedaro_base_client/model/terrestrial_vehicle_model_root.pyi
 src/sedaro_base_client/model/terrestrial_vehicle_update_interface.py
+src/sedaro_base_client/model/terrestrial_vehicle_update_interface.pyi
 src/sedaro_base_client/model/thermal_design_layout.py
+src/sedaro_base_client/model/thermal_design_layout.pyi
 src/sedaro_base_client/model/thermal_interface.py
+src/sedaro_base_client/model/thermal_interface.pyi
 src/sedaro_base_client/model/thermal_interface_material.py
+src/sedaro_base_client/model/thermal_interface_material.pyi
 src/sedaro_base_client/model/thruster.py
+src/sedaro_base_client/model/thruster.pyi
 src/sedaro_base_client/model/time_condition.py
+src/sedaro_base_client/model/time_condition.pyi
 src/sedaro_base_client/model/tle.py
+src/sedaro_base_client/model/tle.pyi
 src/sedaro_base_client/model/tracking_field_of_view_articulation_mode.py
+src/sedaro_base_client/model/tracking_field_of_view_articulation_mode.pyi
 src/sedaro_base_client/model/triad_algorithm.py
+src/sedaro_base_client/model/triad_algorithm.pyi
 src/sedaro_base_client/model/two_conv_mppt_power_processor.py
+src/sedaro_base_client/model/two_conv_mppt_power_processor.pyi
 src/sedaro_base_client/model/two_conv_mppt_topology_params.py
+src/sedaro_base_client/model/two_conv_mppt_topology_params.pyi
 src/sedaro_base_client/model/types.py
+src/sedaro_base_client/model/types.pyi
 src/sedaro_base_client/model/validation_error.py
+src/sedaro_base_client/model/validation_error.pyi
 src/sedaro_base_client/model/vector.py
+src/sedaro_base_client/model/vector.pyi
 src/sedaro_base_client/model/vector_in_fov_condition.py
+src/sedaro_base_client/model/vector_in_fov_condition.pyi
 src/sedaro_base_client/model/vector_sensor.py
+src/sedaro_base_client/model/vector_sensor.pyi
 src/sedaro_base_client/model/vector_tracking_surface.py
+src/sedaro_base_client/model/vector_tracking_surface.pyi
 src/sedaro_base_client/model/waypoint_path_with_duration.py
+src/sedaro_base_client/model/waypoint_path_with_duration.pyi
 src/sedaro_base_client/model/waypoint_path_with_speed.py
+src/sedaro_base_client/model/waypoint_path_with_speed.pyi
 src/sedaro_base_client/model/waypoint_path_with_timestamps.py
+src/sedaro_base_client/model/waypoint_path_with_timestamps.pyi
 src/sedaro_base_client/models/__init__.py
 src/sedaro_base_client/paths/__init__.py
 src/sedaro_base_client/paths/data_id/__init__.py
 src/sedaro_base_client/paths/data_id/get.py
+src/sedaro_base_client/paths/data_id/get.pyi
 src/sedaro_base_client/paths/models_branches_branch_id/__init__.py
 src/sedaro_base_client/paths/models_branches_branch_id/delete.py
+src/sedaro_base_client/paths/models_branches_branch_id/delete.pyi
 src/sedaro_base_client/paths/models_branches_branch_id/get.py
+src/sedaro_base_client/paths/models_branches_branch_id/get.pyi
 src/sedaro_base_client/paths/models_branches_branch_id/patch.py
+src/sedaro_base_client/paths/models_branches_branch_id/patch.pyi
 src/sedaro_base_client/paths/models_branches_branch_id/post.py
+src/sedaro_base_client/paths/models_branches_branch_id/post.pyi
 src/sedaro_base_client/paths/models_branches_branch_id_changes_/__init__.py
 src/sedaro_base_client/paths/models_branches_branch_id_changes_/get.py
+src/sedaro_base_client/paths/models_branches_branch_id_changes_/get.pyi
 src/sedaro_base_client/paths/models_branches_branch_id_commits_/__init__.py
 src/sedaro_base_client/paths/models_branches_branch_id_commits_/post.py
+src/sedaro_base_client/paths/models_branches_branch_id_commits_/post.pyi
 src/sedaro_base_client/paths/models_branches_branch_id_committed_/__init__.py
 src/sedaro_base_client/paths/models_branches_branch_id_committed_/get.py
+src/sedaro_base_client/paths/models_branches_branch_id_committed_/get.pyi
 src/sedaro_base_client/paths/models_branches_branch_id_export_/__init__.py
 src/sedaro_base_client/paths/models_branches_branch_id_export_/get.py
+src/sedaro_base_client/paths/models_branches_branch_id_export_/get.pyi
 src/sedaro_base_client/paths/models_branches_branch_id_saved_/__init__.py
 src/sedaro_base_client/paths/models_branches_branch_id_saved_/get.py
+src/sedaro_base_client/paths/models_branches_branch_id_saved_/get.pyi
 src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/__init__.py
 src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/post.py
+src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/post.pyi
 src/sedaro_base_client/paths/models_branches_branch_id_template/__init__.py
 src/sedaro_base_client/paths/models_branches_branch_id_template/patch.py
+src/sedaro_base_client/paths/models_branches_branch_id_template/patch.pyi
 src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/__init__.py
 src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.py
+src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.pyi
 src/sedaro_base_client/paths/models_repositories_/__init__.py
 src/sedaro_base_client/paths/models_repositories_/post.py
+src/sedaro_base_client/paths/models_repositories_/post.pyi
 src/sedaro_base_client/paths/models_repositories__import/__init__.py
 src/sedaro_base_client/paths/models_repositories__import/post.py
+src/sedaro_base_client/paths/models_repositories__import/post.pyi
 src/sedaro_base_client/paths/models_repositories_repository_id/__init__.py
 src/sedaro_base_client/paths/models_repositories_repository_id/delete.py
+src/sedaro_base_client/paths/models_repositories_repository_id/delete.pyi
 src/sedaro_base_client/paths/models_repositories_repository_id/get.py
+src/sedaro_base_client/paths/models_repositories_repository_id/get.pyi
 src/sedaro_base_client/paths/models_repositories_repository_id/patch.py
+src/sedaro_base_client/paths/models_repositories_repository_id/patch.pyi
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_/__init__.py
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.py
+src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.pyi
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.py
+src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.pyi
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/__init__.py
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.py
+src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.pyi
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.py
+src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.pyi
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/__init__.py
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/get.py
+src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/get.pyi
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/post.py
+src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/post.pyi
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/__init__.py
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/delete.py
+src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/delete.pyi
 src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/get.py
+src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/get.pyi
 src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/__init__.py
 src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/get.py
-src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/patch.py
+src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/get.pyi
+src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/patch.py
+src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/patch.pyi
```

### Comparing `sedaro-4.7.9/src/sedaro_base_client/__init__.py` & `sedaro-4.9.19/src/sedaro_base_client/__init__.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/api_client.py` & `sedaro-4.9.19/src/sedaro_base_client/api_client.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/apis/path_to_api.py` & `sedaro-4.9.19/src/sedaro_base_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/apis/tag_to_api.py` & `sedaro-4.9.19/src/sedaro_base_client/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/apis/tags/branches_api.py` & `sedaro-4.9.19/src/sedaro_base_client/apis/tags/branches_api.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/apis/tags/data_api.py` & `sedaro-4.9.19/src/sedaro_base_client/apis/tags/data_api.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/apis/tags/externals_api.py` & `sedaro-4.9.19/src/sedaro_base_client/apis/tags/externals_api.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/apis/tags/jobs_api.py` & `sedaro-4.9.19/src/sedaro_base_client/apis/tags/jobs_api.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/apis/tags/meta_models_api.py` & `sedaro-4.9.19/src/sedaro_base_client/apis/tags/meta_models_api.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/apis/tags/repositories_api.py` & `sedaro-4.9.19/src/sedaro_base_client/apis/tags/repositories_api.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/configuration.py` & `sedaro-4.9.19/src/sedaro_base_client/configuration.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/exceptions.py` & `sedaro-4.9.19/src/sedaro_base_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/agent.py` & `sedaro-4.9.19/src/sedaro_base_client/model/agent.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/agent_group.py` & `sedaro-4.9.19/src/sedaro_base_client/model/agent_group.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/agent_parameters.py` & `sedaro-4.9.19/src/sedaro_base_client/model/agent_parameters.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_algorithm100.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm100.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_algorithm105.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm105.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_algorithm95.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_algorithm95.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_field_of_view141.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view141.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_field_of_view146.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view146.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_field_of_view147.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_field_of_view147.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors110.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors110.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors115.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors115.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors20.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors20.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors51.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors51.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angle_sensors56.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angle_sensors56.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_algorithm110.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_algorithm110.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_attitude14.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_attitude14.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/angular_velocity_sensors84.py` & `sedaro-4.9.19/src/sedaro_base_client/model/angular_velocity_sensors84.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/antenna.py` & `sedaro-4.9.19/src/sedaro_base_client/model/antenna.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/area_target.py` & `sedaro-4.9.19/src/sedaro_base_client/model/area_target.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/averaging_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/averaging_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/base_dissipations.py` & `sedaro-4.9.19/src/sedaro_base_client/model/base_dissipations.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/battery.py` & `sedaro-4.9.19/src/sedaro_base_client/model/battery.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/battery_cell.py` & `sedaro-4.9.19/src/sedaro_base_client/model/battery_cell.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/battery_pack.py` & `sedaro-4.9.19/src/sedaro_base_client/model/battery_pack.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/battery_pack_dissipations.py` & `sedaro-4.9.19/src/sedaro_base_client/model/battery_pack_dissipations.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/body_frame_vector.py` & `sedaro-4.9.19/src/sedaro_base_client/model/body_frame_vector.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/body_frame_vector_types.py` & `sedaro-4.9.19/src/sedaro_base_client/model/body_frame_vector_types.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/body_in_fov_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/body_in_fov_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_changes_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_changes_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_create.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_create.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_merge.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_merge.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_merge_conflicts_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_merge_conflicts_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_scenario_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_scenario_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_spacecraft_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_spacecraft_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_terrestrial_vehicle_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_terrestrial_vehicle_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_update.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_update.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/branch_verify_password.py` & `sedaro-4.9.19/src/sedaro_base_client/model/branch_verify_password.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/bus_regulator.py` & `sedaro-4.9.19/src/sedaro_base_client/model/bus_regulator.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/categories.py` & `sedaro-4.9.19/src/sedaro_base_client/model/categories.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/celestial_pointing_directions.py` & `sedaro-4.9.19/src/sedaro_base_client/model/celestial_pointing_directions.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/celestial_target.py` & `sedaro-4.9.19/src/sedaro_base_client/model/celestial_target.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/celestial_vector.py` & `sedaro-4.9.19/src/sedaro_base_client/model/celestial_vector.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/circular_field_of_view.py` & `sedaro-4.9.19/src/sedaro_base_client/model/circular_field_of_view.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/classical_orbital_elements.py` & `sedaro-4.9.19/src/sedaro_base_client/model/classical_orbital_elements.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/clock_config.py` & `sedaro-4.9.19/src/sedaro_base_client/model/clock_config.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/component.py` & `sedaro-4.9.19/src/sedaro_base_client/model/component.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/component_dissipations.py` & `sedaro-4.9.19/src/sedaro_base_client/model/component_dissipations.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/component_parameters.py` & `sedaro-4.9.19/src/sedaro_base_client/model/component_parameters.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/component_to_scalar_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/component_to_scalar_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/compound_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/compound_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/compound_operators.py` & `sedaro-4.9.19/src/sedaro_base_client/model/compound_operators.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/condition_relationship.py` & `sedaro-4.9.19/src/sedaro_base_client/model/condition_relationship.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/configuration_types.py` & `sedaro-4.9.19/src/sedaro_base_client/model/configuration_types.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/conflicts_obj.py` & `sedaro-4.9.19/src/sedaro_base_client/model/conflicts_obj.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/constant_power_params.py` & `sedaro-4.9.19/src/sedaro_base_client/model/constant_power_params.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/constant_resistance_params.py` & `sedaro-4.9.19/src/sedaro_base_client/model/constant_resistance_params.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/cooler.py` & `sedaro-4.9.19/src/sedaro_base_client/model/cooler.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/cooperative_transmit_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/cooperative_transmit_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/crud_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/crud_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/data_bus.py` & `sedaro-4.9.19/src/sedaro_base_client/model/data_bus.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/data_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/data_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/data_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/data_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/data_service_response.py` & `sedaro-4.9.19/src/sedaro_base_client/model/data_service_response.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/data_set.py` & `sedaro-4.9.19/src/sedaro_base_client/model/data_set.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/data_storage.py` & `sedaro-4.9.19/src/sedaro_base_client/model/data_storage.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/data_type.py` & `sedaro-4.9.19/src/sedaro_base_client/model/data_type.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/deleted_entity.py` & `sedaro-4.9.19/src/sedaro_base_client/model/deleted_entity.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/direction_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/direction_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/distance_algorithm158.py` & `sedaro-4.9.19/src/sedaro_base_client/model/distance_algorithm158.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/distance_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/distance_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/distance_sensors126.py` & `sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors126.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/distance_sensors72.py` & `sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors72.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/distance_sensors99.py` & `sedaro-4.9.19/src/sedaro_base_client/model/distance_sensors99.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/duration_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/duration_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/duration_field_of_view61.py` & `sedaro-4.9.19/src/sedaro_base_client/model/duration_field_of_view61.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/duration_load68.py` & `sedaro-4.9.19/src/sedaro_base_client/model/duration_load68.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode20.py` & `sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode20.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode22.py` & `sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode22.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode24.py` & `sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode24.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode32.py` & `sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode32.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/duration_operational_mode34.py` & `sedaro-4.9.19/src/sedaro_base_client/model/duration_operational_mode34.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/dynamically_loaded_component.py` & `sedaro-4.9.19/src/sedaro_base_client/model/dynamically_loaded_component.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/ekf_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/ekf_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/elapsed_time_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/elapsed_time_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/entity_delete_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/entity_delete_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/eps_output_types.py` & `sedaro-4.9.19/src/sedaro_base_client/model/eps_output_types.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/equatorial_circular_reference_orbit.py` & `sedaro-4.9.19/src/sedaro_base_client/model/equatorial_circular_reference_orbit.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/external_state_set_request.py` & `sedaro-4.9.19/src/sedaro_base_client/model/external_state_set_request.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/fixed_surface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/fixed_surface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/frame_vector_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/frame_vector_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/fuel_reservoir.py` & `sedaro-4.9.19/src/sedaro_base_client/model/fuel_reservoir.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/fully_reg_det_power_processor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/fully_reg_det_power_processor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/fully_reg_det_topology_params.py` & `sedaro-4.9.19/src/sedaro_base_client/model/fully_reg_det_topology_params.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/generic_ad_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/generic_ad_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/generic_od_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/generic_od_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/geostationary_reference_orbit.py` & `sedaro-4.9.19/src/sedaro_base_client/model/geostationary_reference_orbit.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/geostationary_transfer_reference_orbit.py` & `sedaro-4.9.19/src/sedaro_base_client/model/geostationary_transfer_reference_orbit.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/gps_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/gps_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/ground_target.py` & `sedaro-4.9.19/src/sedaro_base_client/model/ground_target.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/group_rollers.py` & `sedaro-4.9.19/src/sedaro_base_client/model/group_rollers.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/heater.py` & `sedaro-4.9.19/src/sedaro_base_client/model/heater.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/http_validation_error.py` & `sedaro-4.9.19/src/sedaro_base_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/ideal_orbital_attitude_dynamics.py` & `sedaro-4.9.19/src/sedaro_base_client/model/ideal_orbital_attitude_dynamics.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/initial_state_def_type.py` & `sedaro-4.9.19/src/sedaro_base_client/model/initial_state_def_type.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/input_types.py` & `sedaro-4.9.19/src/sedaro_base_client/model/input_types.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/internal_data_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/internal_data_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/iss_reference_orbit.py` & `sedaro-4.9.19/src/sedaro_base_client/model/iss_reference_orbit.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/laser_comm_module.py` & `sedaro-4.9.19/src/sedaro_base_client/model/laser_comm_module.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/load_state.py` & `sedaro-4.9.19/src/sedaro_base_client/model/load_state.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/local_pointing_directions.py` & `sedaro-4.9.19/src/sedaro_base_client/model/local_pointing_directions.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/local_vector.py` & `sedaro-4.9.19/src/sedaro_base_client/model/local_vector.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/lock_pointing_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/lock_pointing_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/magnetorquer.py` & `sedaro-4.9.19/src/sedaro_base_client/model/magnetorquer.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/max_align_pointing_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/max_align_pointing_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/mekf_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/mekf_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/message_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/message_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/model_crud_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/model_crud_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/modem.py` & `sedaro-4.9.19/src/sedaro_base_client/model/modem.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/operational_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/operational_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/optical_attitude_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/optical_attitude_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/orbit.py` & `sedaro-4.9.19/src/sedaro_base_client/model/orbit.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/orbital_attitude_dynamics.py` & `sedaro-4.9.19/src/sedaro_base_client/model/orbital_attitude_dynamics.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/orbital_elements_data.py` & `sedaro-4.9.19/src/sedaro_base_client/model/orbital_elements_data.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/orders.py` & `sedaro-4.9.19/src/sedaro_base_client/model/orders.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/panel_dissipations.py` & `sedaro-4.9.19/src/sedaro_base_client/model/panel_dissipations.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/passive_pointing_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/passive_pointing_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/passive_transmit_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/passive_transmit_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/per_round_external_state.py` & `sedaro-4.9.19/src/sedaro_base_client/model/per_round_external_state.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/photovoltaic_power_processor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/photovoltaic_power_processor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/pid_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/pid_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/polar_circular_reference_orbit.py` & `sedaro-4.9.19/src/sedaro_base_client/model/polar_circular_reference_orbit.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/polynomial_ephemeris_body.py` & `sedaro-4.9.19/src/sedaro_base_client/model/polynomial_ephemeris_body.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/position_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/position_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/position_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/position_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/power_load.py` & `sedaro-4.9.19/src/sedaro_base_client/model/power_load.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/power_processor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/power_processor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/processor_dissipations.py` & `sedaro-4.9.19/src/sedaro_base_client/model/processor_dissipations.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/quasi_reg_det_power_processor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/quasi_reg_det_power_processor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/quasi_reg_det_topology_params.py` & `sedaro-4.9.19/src/sedaro_base_client/model/quasi_reg_det_topology_params.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/quaternion_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/quaternion_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/range_relationship.py` & `sedaro-4.9.19/src/sedaro_base_client/model/range_relationship.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/reaction_wheel.py` & `sedaro-4.9.19/src/sedaro_base_client/model/reaction_wheel.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/receive_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/receive_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/rectangular_field_of_view.py` & `sedaro-4.9.19/src/sedaro_base_client/model/rectangular_field_of_view.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/repo_create_req.py` & `sedaro-4.9.19/src/sedaro_base_client/model/repo_create_req.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/repo_import_req.py` & `sedaro-4.9.19/src/sedaro_base_client/model/repo_import_req.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/repo_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/repo_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/repo_update_req.py` & `sedaro-4.9.19/src/sedaro_base_client/model/repo_update_req.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/representation.py` & `sedaro-4.9.19/src/sedaro_base_client/model/representation.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/resistance_load.py` & `sedaro-4.9.19/src/sedaro_base_client/model/resistance_load.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/same_target_multi_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/same_target_multi_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/satellite_parameters.py` & `sedaro-4.9.19/src/sedaro_base_client/model/satellite_parameters.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/satellite_to_satellite_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_satellite_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/satellite_to_scalar_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_scalar_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/satellite_to_target_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/satellite_to_target_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/scan_field_of_view_articulation_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/scan_field_of_view_articulation_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/scenario.py` & `sedaro-4.9.19/src/sedaro_base_client/model/scenario.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/scenario_model_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/scenario_model_root.py` & `sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_root.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/scenario_model_update_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/scenario_model_update_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/services_model_spec_models_simulation_job_statuses.py` & `sedaro-4.9.19/src/sedaro_base_client/model/services_model_spec_models_simulation_job_statuses.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/services_model_spec_models_study_job_statuses.py` & `sedaro-4.9.19/src/sedaro_base_client/model/services_model_spec_models_study_job_statuses.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/side_categories.py` & `sedaro-4.9.19/src/sedaro_base_client/model/side_categories.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/simulation_job.py` & `sedaro-4.9.19/src/sedaro_base_client/model/simulation_job.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/single_conv_hybrid_power_processor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/single_conv_hybrid_power_processor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/single_conv_hybrid_topology_params.py` & `sedaro-4.9.19/src/sedaro_base_client/model/single_conv_hybrid_topology_params.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/single_conv_mppt_power_processor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/single_conv_mppt_power_processor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/single_conv_mppt_topology_params.py` & `sedaro-4.9.19/src/sedaro_base_client/model/single_conv_mppt_topology_params.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/sliding_mode_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/sliding_mode_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/solar_array.py` & `sedaro-4.9.19/src/sedaro_base_client/model/solar_array.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/solar_cell.py` & `sedaro-4.9.19/src/sedaro_base_client/model/solar_cell.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/solar_panel.py` & `sedaro-4.9.19/src/sedaro_base_client/model/solar_panel.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/sort_values.py` & `sedaro-4.9.19/src/sedaro_base_client/model/sort_values.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/space_target.py` & `sedaro-4.9.19/src/sedaro_base_client/model/space_target.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spacecraft.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spacecraft.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spacecraft_model_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spacecraft_model_root.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_root.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spacecraft_model_update_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_model_update_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spacecraft_operational_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spacecraft_operational_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/speed_algorithm163.py` & `sedaro-4.9.19/src/sedaro_base_client/model/speed_algorithm163.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/speed_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/speed_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/speed_sensors137.py` & `sedaro-4.9.19/src/sedaro_base_client/model/speed_sensors137.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spherical_angles.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spherical_angles.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spherical_fuel_tank.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spherical_fuel_tank.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spherocylinder_fuel_tank.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spherocylinder_fuel_tank.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/spontaneous_external_state.py` & `sedaro-4.9.19/src/sedaro_base_client/model/spontaneous_external_state.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/state_vector.py` & `sedaro-4.9.19/src/sedaro_base_client/model/state_vector.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/static_field_of_view_articulation_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/static_field_of_view_articulation_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/static_thrust_control_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/static_thrust_control_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/study_job.py` & `sedaro-4.9.19/src/sedaro_base_client/model/study_job.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/subsystem.py` & `sedaro-4.9.19/src/sedaro_base_client/model/subsystem.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/sun_synchronous_circular_orbit.py` & `sedaro-4.9.19/src/sedaro_base_client/model/sun_synchronous_circular_orbit.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/sun_tracking_surface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/sun_tracking_surface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/surface_material.py` & `sedaro-4.9.19/src/sedaro_base_client/model/surface_material.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_attitude_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_attitude_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_group.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_group.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_group_in_fov_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_group_in_fov_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_group_to_satellite_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_satellite_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_group_to_scalar_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_scalar_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_group_to_target_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_group_to_target_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_group_vector.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_group_vector.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_in_fov_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_in_fov_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_parameters.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_parameters.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_position_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_position_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_range_rate_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_range_rate_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_range_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_range_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_to_scalar_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_to_scalar_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_to_target_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_to_target_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/target_vector.py` & `sedaro-4.9.19/src/sedaro_base_client/model/target_vector.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/temp_controller_state.py` & `sedaro-4.9.19/src/sedaro_base_client/model/temp_controller_state.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/temperature_base323.py` & `sedaro-4.9.19/src/sedaro_base_client/model/temperature_base323.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_attitude_dynamics.py` & `sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_attitude_dynamics.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_vehicle.py` & `sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_vehicle_model_res.py` & `sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_model_res.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_vehicle_model_root.py` & `sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_model_root.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/terrestrial_vehicle_update_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/terrestrial_vehicle_update_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/thermal_design_layout.py` & `sedaro-4.9.19/src/sedaro_base_client/model/thermal_design_layout.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/thermal_interface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/thermal_interface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/thermal_interface_material.py` & `sedaro-4.9.19/src/sedaro_base_client/model/thermal_interface_material.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/thruster.py` & `sedaro-4.9.19/src/sedaro_base_client/model/thruster.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/time_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/time_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/tle.py` & `sedaro-4.9.19/src/sedaro_base_client/model/tle.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/tracking_field_of_view_articulation_mode.py` & `sedaro-4.9.19/src/sedaro_base_client/model/tracking_field_of_view_articulation_mode.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/triad_algorithm.py` & `sedaro-4.9.19/src/sedaro_base_client/model/triad_algorithm.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/two_conv_mppt_power_processor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/two_conv_mppt_power_processor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/two_conv_mppt_topology_params.py` & `sedaro-4.9.19/src/sedaro_base_client/model/two_conv_mppt_topology_params.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/types.py` & `sedaro-4.9.19/src/sedaro_base_client/model/types.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/validation_error.py` & `sedaro-4.9.19/src/sedaro_base_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/vector.py` & `sedaro-4.9.19/src/sedaro_base_client/model/vector.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/vector_in_fov_condition.py` & `sedaro-4.9.19/src/sedaro_base_client/model/vector_in_fov_condition.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/vector_sensor.py` & `sedaro-4.9.19/src/sedaro_base_client/model/vector_sensor.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/vector_tracking_surface.py` & `sedaro-4.9.19/src/sedaro_base_client/model/vector_tracking_surface.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/waypoint_path_with_duration.py` & `sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_duration.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/waypoint_path_with_speed.py` & `sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_speed.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/model/waypoint_path_with_timestamps.py` & `sedaro-4.9.19/src/sedaro_base_client/model/waypoint_path_with_timestamps.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/models/__init__.py` & `sedaro-4.9.19/src/sedaro_base_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/__init__.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/data_id/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/data_id/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/delete.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/delete.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/patch.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/patch.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id/post.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id/post.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_changes_/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_changes_/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_commits_/post.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_commits_/post.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_committed_/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_committed_/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_export_/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_export_/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_saved_/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_saved_/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/post.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_share_auth_/post.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_branch_id_template/patch.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_branch_id_template/patch.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_/post.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_/post.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories__import/post.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories__import/post.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_repository_id/delete.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/delete.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_repository_id/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/models_repositories_repository_id/patch.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/models_repositories_repository_id/patch.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/post.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_/post.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/delete.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/delete.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_branches_branch_id_control_study_job_id/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/get.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/get.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/patch.py` & `sedaro-4.9.19/src/sedaro_base_client/paths/simulations_jobs_job_id_externals_agent_id_external_state_block_id/patch.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/rest.py` & `sedaro-4.9.19/src/sedaro_base_client/rest.py`

 * *Files identical despite different names*

### Comparing `sedaro-4.7.9/src/sedaro_base_client/schemas.py` & `sedaro-4.9.19/src/sedaro_base_client/schemas.py`

 * *Files identical despite different names*

