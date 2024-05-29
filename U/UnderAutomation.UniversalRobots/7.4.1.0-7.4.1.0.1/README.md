# Comparing `tmp/underautomation_universalrobots-7.4.1.0.tar.gz` & `tmp/UnderAutomation.UniversalRobots-7.4.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "underautomation_universalrobots-7.4.1.0.tar", last modified: Wed May 29 19:23:51 2024, max compression
+gzip compressed data, was "UnderAutomation.UniversalRobots-7.4.1.0.1.tar", last modified: Tue May  7 21:31:08 2024, max compression
```

## Comparing `underautomation_universalrobots-7.4.1.0.tar` & `UnderAutomation.UniversalRobots-7.4.1.0.1.tar`

### file list

```diff
@@ -1,260 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.026389 underautomation_universalrobots-7.4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-29 19:23:51.026389 underautomation_universalrobots-7.4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.026389 underautomation_universalrobots-7.4.1.0/UnderAutomation.UniversalRobots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-29 19:23:50.000000 underautomation_universalrobots-7.4.1.0/UnderAutomation.UniversalRobots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15962 2024-05-29 19:23:50.000000 underautomation_universalrobots-7.4.1.0/UnderAutomation.UniversalRobots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:23:50.000000 underautomation_universalrobots-7.4.1.0/UnderAutomation.UniversalRobots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 19:23:50.000000 underautomation_universalrobots-7.4.1.0/UnderAutomation.UniversalRobots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 19:23:50.000000 underautomation_universalrobots-7.4.1.0/UnderAutomation.UniversalRobots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:23:51.026389 underautomation_universalrobots-7.4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.982389 underautomation_universalrobots-7.4.1.0/underautomation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.982389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.990389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/analog_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/cartesian_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/control_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/controller_box_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/dashboard_connect_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/digital_output_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/global_variable_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/global_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/internal_error_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/interpreter_mode_connect_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/joint_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/joints_double_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/joints_int_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/joints_values_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/output_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/pose.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/primary_interface_connect_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/robot_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/robot_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/robot_sub_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/rtde_connect_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/safety_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/socket_communication_connect_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/ssh_connect_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/status_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/tool_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/vector3_d.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/xml_rpc_connect_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/connect_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.990389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/command_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/command_response_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/dashboard_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.990389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/internal/dashboard_client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/internal/dashboard_client_parameters_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/operational_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/polyscope_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/program_save_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/program_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/program_states.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.990389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/files/ur_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/files/ur_installation.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/files/ur_program.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.994389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/dashboard_client_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/interpreter_mode_client_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/primary_interface_client_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/rtde_client_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/sftp_client_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/socket_communication_server_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/ssh_client_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/ur_service_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/xml_rpc_server_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.994389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/command_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/command_response_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.994389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/internal/interpreter_mode_client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/internal/interpreter_mode_client_parameters_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/interpreter_mode_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.998389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/lib/
--rw-r--r--   0 runner    (1001) docker     (127)  1246720 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/lib/UnderAutomation.UniversalRobots.dll
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/lib/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:50.998389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/license/invalid_license_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/license/license_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/license/license_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.006389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/additional_info_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/calibration_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/cartesian_info_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/configuration_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/force_mode_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/global_variables_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/global_variables_firmware_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.006389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/primary_interface_client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/primary_interface_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/primary_interface_parameters_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/primary_interface_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/joint_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/joint_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/joint_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/joint_kinematics_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/key_message_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/kinematics_info_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/masterboard_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/masterboard_digital_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/package_description_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/package_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/popup_message_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/primary_interface_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/program_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/program_threads_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/request_value_message_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/requested_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/robot_mode_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/runtime_exception_message_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/safety_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/singularity_info_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/text_message_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/tool_communication_info_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/tool_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/tool_mode_info_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/version_event_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.010389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.010389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_client_parameters_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_parameters_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_setup_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_setup_item_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_base_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_base_values_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_basic_request_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_bit_registers_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_control_package_setup_inputs_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_control_package_setup_outputs_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_data_description_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_data_package_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_double_registers_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_data_description.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_setup_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_inputs_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_int_registers_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_data_description.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_setup_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_outputs_description.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_protocol_version_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_registers_value_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_text_message_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_value_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.014389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.014389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/internal/socket_communication_parameters_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/internal/socket_communication_server_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_client_connection_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_client_disconnection_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_communication_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_get_var_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_request_event_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.014389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.014389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/internal/sftp_client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/internal/ssh_client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/internal/ssh_parameters_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/sftp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/ssh_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.018389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/authentication_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.018389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/exception_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/object_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/sftp_path_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/sftp_permission_denied_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/shell_data_event_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_authentication_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_connection_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_operation_timeout_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_pass_phrase_null_or_empty_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/terminal_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.018389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/compression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/compression/compression_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/expect_action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.018389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.018389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/connection/global_request_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/service_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.018389 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/messages/transport/disconnect_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/proxy_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/remote_path_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.022390 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/sftp_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/sftp_file_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/sftp_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/sftp_file_sytem_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/shell_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/ssh_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.022390 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:51.022390 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/internal/xml_rpc_parameters_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/internal/xml_rpc_server_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_array_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_boolean_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_double_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_event_arg.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_integer_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_pose_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_string_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_struct_member.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_struct_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_unknown_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-29 19:23:41.000000 underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_value.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.143902 UnderAutomation.UniversalRobots-7.4.1.0.1/
+-rw-rw-rw-   0        0        0      694 2024-05-07 21:31:08.143902 UnderAutomation.UniversalRobots-7.4.1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.143902 UnderAutomation.UniversalRobots-7.4.1.0.1/UnderAutomation.UniversalRobots.egg-info/
+-rw-rw-rw-   0        0        0      694 2024-05-07 21:31:07.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/UnderAutomation.UniversalRobots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14929 2024-05-07 21:31:07.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/UnderAutomation.UniversalRobots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 21:31:07.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/UnderAutomation.UniversalRobots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 21:31:07.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/UnderAutomation.UniversalRobots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-07 21:31:07.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/UnderAutomation.UniversalRobots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 21:31:08.153903 UnderAutomation.UniversalRobots-7.4.1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-07 21:30:46.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.666731 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.676705 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.756705 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/__init__.py
+-rw-rw-rw-   0        0        0       51 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/analog_ranges.py
+-rw-rw-rw-   0        0        0     1422 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/cartesian_coordinates.py
+-rw-rw-rw-   0        0        0       73 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/control_modes.py
+-rw-rw-rw-   0        0        0       70 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/controller_box_types.py
+-rw-rw-rw-   0        0        0      605 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/dashboard_connect_parameters.py
+-rw-rw-rw-   0        0        0       87 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/digital_output_configurations.py
+-rw-rw-rw-   0        0        0      656 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/global_variable.py
+-rw-rw-rw-   0        0        0      117 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/global_variable_types.py
+-rw-rw-rw-   0        0        0     1429 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/global_variable_value.py
+-rw-rw-rw-   0        0        0      811 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/internal_error_event_args.py
+-rw-rw-rw-   0        0        0      268 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/joint_modes.py
+-rw-rw-rw-   0        0        0      528 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/joints_double_values.py
+-rw-rw-rw-   0        0        0      514 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/joints_int_values.py
+-rw-rw-rw-   0        0        0     1430 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/joints_values_1.py
+-rw-rw-rw-   0        0        0       62 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/output_modes.py
+-rw-rw-rw-   0        0        0      605 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/package_event_args.py
+-rw-rw-rw-   0        0        0     1521 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/pose.py
+-rw-rw-rw-   0        0        0      804 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/primary_interface_connect_parameters.py
+-rw-rw-rw-   0        0        0       62 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/robot_models.py
+-rw-rw-rw-   0        0        0      172 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/robot_modes.py
+-rw-rw-rw-   0        0        0       66 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/robot_sub_types.py
+-rw-rw-rw-   0        0        0      704 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/rtde_connect_parameters.py
+-rw-rw-rw-   0        0        0      249 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/safety_status.py
+-rw-rw-rw-   0        0        0      828 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/socket_communication_connect_parameters.py
+-rw-rw-rw-   0        0        0      886 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/ssh_connect_parameters.py
+-rw-rw-rw-   0        0        0      289 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/status_code.py
+-rw-rw-rw-   0        0        0       67 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/tool_modes.py
+-rw-rw-rw-   0        0        0      899 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/vector3_d.py
+-rw-rw-rw-   0        0        0      724 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/xml_rpc_connect_parameters.py
+-rw-rw-rw-   0        0        0     2874 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/connect_parameters.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.793445 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/__init__.py
+-rw-rw-rw-   0        0        0      775 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/command_response.py
+-rw-rw-rw-   0        0        0      793 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/command_response_1.py
+-rw-rw-rw-   0        0        0      604 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/dashboard_client.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.793445 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/internal/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/internal/__init__.py
+-rw-rw-rw-   0        0        0     5657 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/internal/dashboard_client_base.py
+-rw-rw-rw-   0        0        0       67 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/operational_modes.py
+-rw-rw-rw-   0        0        0      948 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/polyscope_version.py
+-rw-rw-rw-   0        0        0      769 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/program_save_state.py
+-rw-rw-rw-   0        0        0      855 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/program_state.py
+-rw-rw-rw-   0        0        0       64 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/program_states.py
+-rw-rw-rw-   0        0        0       91 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/user_roles.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.810110 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/files/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/files/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/files/ur_archive.py
+-rw-rw-rw-   0        0        0      791 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/files/ur_installation.py
+-rw-rw-rw-   0        0        0      756 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/files/ur_program.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.832810 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/dashboard_client_internal.py
+-rw-rw-rw-   0        0        0      805 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/primary_interface_client_internal.py
+-rw-rw-rw-   0        0        0     1003 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/rtde_client_internal.py
+-rw-rw-rw-   0        0        0      635 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/sftp_client_internal.py
+-rw-rw-rw-   0        0        0      657 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/socket_communication_server_internal.py
+-rw-rw-rw-   0        0        0      628 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/ssh_client_internal.py
+-rw-rw-rw-   0        0        0      730 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/ur_service_base.py
+-rw-rw-rw-   0        0        0      553 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/xml_rpc_server_internal.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.841009 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/license/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/license/__init__.py
+-rw-rw-rw-   0        0        0      635 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/license/invalid_license_exception.py
+-rw-rw-rw-   0        0        0     1633 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/license/license_info.py
+-rw-rw-rw-   0        0        0      115 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/license/license_state.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.928586 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/__init__.py
+-rw-rw-rw-   0        0        0     1277 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/additional_info_package_event_args.py
+-rw-rw-rw-   0        0        0     1397 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/calibration_data_package_event_args.py
+-rw-rw-rw-   0        0        0     2436 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/cartesian_info_package_event_args.py
+-rw-rw-rw-   0        0        0     3936 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/configuration_data_package_event_args.py
+-rw-rw-rw-   0        0        0     1555 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/force_mode_data_package_event_args.py
+-rw-rw-rw-   0        0        0     1583 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/global_variables.py
+-rw-rw-rw-   0        0        0      670 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/global_variables_event_args.py
+-rw-rw-rw-   0        0        0       79 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/global_variables_firmware_version.py
+-rw-rw-rw-   0        0        0      147 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/interfaces.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:07.944363 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/internal/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/internal/__init__.py
+-rw-rw-rw-   0        0        0    11506 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/internal/primary_interface_client_base.py
+-rw-rw-rw-   0        0        0      747 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/internal/primary_interface_parameters_base.py
+-rw-rw-rw-   0        0        0      633 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/internal/primary_interface_script.py
+-rw-rw-rw-   0        0        0     1831 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/joint_configuration.py
+-rw-rw-rw-   0        0        0     1684 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/joint_data.py
+-rw-rw-rw-   0        0        0     1671 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/joint_data_package_event_args.py
+-rw-rw-rw-   0        0        0     1188 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/joint_kinematics_info.py
+-rw-rw-rw-   0        0        0     1373 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/key_message_event_args.py
+-rw-rw-rw-   0        0        0     2097 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/kinematics_info_package_event_args.py
+-rw-rw-rw-   0        0        0     5847 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/masterboard_data_package_event_args.py
+-rw-rw-rw-   0        0        0     2000 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/masterboard_digital_io.py
+-rw-rw-rw-   0        0        0      697 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/package_description_attribute.py
+-rw-rw-rw-   0        0        0      194 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/package_unit.py
+-rw-rw-rw-   0        0        0     1904 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/popup_message_event_args.py
+-rw-rw-rw-   0        0        0      792 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/primary_interface_client.py
+-rw-rw-rw-   0        0        0      912 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/program_thread.py
+-rw-rw-rw-   0        0        0      880 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/program_threads_event_args.py
+-rw-rw-rw-   0        0        0     1279 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/request_value_message_event_args.py
+-rw-rw-rw-   0        0        0      144 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/requested_types.py
+-rw-rw-rw-   0        0        0     3387 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/robot_mode_data_package_event_args.py
+-rw-rw-rw-   0        0        0     1277 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/runtime_exception_message_event_args.py
+-rw-rw-rw-   0        0        0      739 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/safety_data_package_event_args.py
+-rw-rw-rw-   0        0        0     1006 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/singularity_info_package_event_args.py
+-rw-rw-rw-   0        0        0      725 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/text_message_event_args.py
+-rw-rw-rw-   0        0        0     1711 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/tool_communication_info_package_event_args.py
+-rw-rw-rw-   0        0        0     2534 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/tool_data_package_event_args.py
+-rw-rw-rw-   0        0        0     1552 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/tool_mode_info_package_event_args.py
+-rw-rw-rw-   0        0        0     1669 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/version_event_args.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.005303 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.011425 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/__init__.py
+-rw-rw-rw-   0        0        0     5032 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_client_base.py
+-rw-rw-rw-   0        0        0      629 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_client_parameters_base.py
+-rw-rw-rw-   0        0        0     1454 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_parameters_base.py
+-rw-rw-rw-   0        0        0      835 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_setup_2.py
+-rw-rw-rw-   0        0        0     1343 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_setup_item_1.py
+-rw-rw-rw-   0        0        0      588 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_base_values.py
+-rw-rw-rw-   0        0        0      655 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_base_values_1.py
+-rw-rw-rw-   0        0        0      719 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_basic_request_event_args.py
+-rw-rw-rw-   0        0        0     9360 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_bit_registers_value.py
+-rw-rw-rw-   0        0        0     1454 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_client.py
+-rw-rw-rw-   0        0        0      430 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_client_parameters.py
+-rw-rw-rw-   0        0        0     1015 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_control_package_setup_inputs_event_args.py
+-rw-rw-rw-   0        0        0     1024 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_control_package_setup_outputs_event_args.py
+-rw-rw-rw-   0        0        0     1054 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_data_description_1.py
+-rw-rw-rw-   0        0        0     1291 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_data_package_event_args.py
+-rw-rw-rw-   0        0        0     7135 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_double_registers_value.py
+-rw-rw-rw-   0        0        0      468 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_data.py
+-rw-rw-rw-   0        0        0      660 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_data_description.py
+-rw-rw-rw-   0        0        0      707 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_setup.py
+-rw-rw-rw-   0        0        0      913 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_setup_item.py
+-rw-rw-rw-   0        0        0     4952 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_values.py
+-rw-rw-rw-   0        0        0     3191 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_inputs_description.py
+-rw-rw-rw-   0        0        0     6929 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_int_registers_value.py
+-rw-rw-rw-   0        0        0     1646 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_data.py
+-rw-rw-rw-   0        0        0      667 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_data_description.py
+-rw-rw-rw-   0        0        0      717 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_setup.py
+-rw-rw-rw-   0        0        0      923 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_setup_item.py
+-rw-rw-rw-   0        0        0    16688 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_values.py
+-rw-rw-rw-   0        0        0    10771 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_outputs_description.py
+-rw-rw-rw-   0        0        0      860 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_protocol_version_event_args.py
+-rw-rw-rw-   0        0        0      827 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_registers_value_1.py
+-rw-rw-rw-   0        0        0       78 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_states.py
+-rw-rw-rw-   0        0        0     1035 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_text_message_event_args.py
+-rw-rw-rw-   0        0        0      237 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_types.py
+-rw-rw-rw-   0        0        0      457 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_value.py
+-rw-rw-rw-   0        0        0      634 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_value_1.py
+-rw-rw-rw-   0        0        0       41 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_versions.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.027117 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.037119 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/internal/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/internal/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/internal/socket_communication_parameters_base.py
+-rw-rw-rw-   0        0        0     2086 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/internal/socket_communication_server_base.py
+-rw-rw-rw-   0        0        0     1396 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_client.py
+-rw-rw-rw-   0        0        0      677 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_client_connection_event_args.py
+-rw-rw-rw-   0        0        0      689 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_client_disconnection_event_args.py
+-rw-rw-rw-   0        0        0      634 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_communication_server.py
+-rw-rw-rw-   0        0        0      857 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_get_var_event_args.py
+-rw-rw-rw-   0        0        0      709 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_request_event_args.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.043653 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.053653 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/internal/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/internal/__init__.py
+-rw-rw-rw-   0        0        0     7603 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/internal/sftp_client_base.py
+-rw-rw-rw-   0        0        0     1917 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/internal/ssh_client_base.py
+-rw-rw-rw-   0        0        0      746 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/internal/ssh_parameters_base.py
+-rw-rw-rw-   0        0        0      609 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/sftp_client.py
+-rw-rw-rw-   0        0        0      602 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/ssh_client.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.060305 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/authentication_result.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.076853 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/__init__.py
+-rw-rw-rw-   0        0        0      559 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/exception_event_args.py
+-rw-rw-rw-   0        0        0      569 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/object_identifier.py
+-rw-rw-rw-   0        0        0      646 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/sftp_path_not_found_exception.py
+-rw-rw-rw-   0        0        0      660 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/sftp_permission_denied_exception.py
+-rw-rw-rw-   0        0        0      617 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/shell_data_event_args.py
+-rw-rw-rw-   0        0        0      646 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_authentication_exception.py
+-rw-rw-rw-   0        0        0      903 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_connection_exception.py
+-rw-rw-rw-   0        0        0      467 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_exception.py
+-rw-rw-rw-   0        0        0      656 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_operation_timeout_exception.py
+-rw-rw-rw-   0        0        0      682 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_pass_phrase_null_or_empty_exception.py
+-rw-rw-rw-   0        0        0      747 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/terminal_modes.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.086861 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/compression/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/compression/__init__.py
+-rw-rw-rw-   0        0        0       58 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/compression/compression_mode.py
+-rw-rw-rw-   0        0        0      611 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/expect_action.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.093447 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.093447 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/connection/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/connection/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/connection/global_request_name.py
+-rw-rw-rw-   0        0        0       64 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/service_name.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.093447 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/transport/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/transport/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/messages/transport/disconnect_reason.py
+-rw-rw-rw-   0        0        0       68 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/proxy_types.py
+-rw-rw-rw-   0        0        0      934 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/remote_path_transformation.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.110487 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/__init__.py
+-rw-rw-rw-   0        0        0     4647 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/sftp_file.py
+-rw-rw-rw-   0        0        0     4310 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/sftp_file_attributes.py
+-rw-rw-rw-   0        0        0     1881 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/sftp_file_stream.py
+-rw-rw-rw-   0        0        0     1434 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/sftp_file_sytem_information.py
+-rw-rw-rw-   0        0        0     1647 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/shell.py
+-rw-rw-rw-   0        0        0     2723 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/shell_stream.py
+-rw-rw-rw-   0        0        0     1510 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/ssh_command.py
+-rw-rw-rw-   0        0        0     2713 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ur.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.126821 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:31:08.136822 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/internal/
+-rw-rw-rw-   0        0        0        0 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/internal/__init__.py
+-rw-rw-rw-   0        0        0      586 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/internal/xml_rpc_parameters_base.py
+-rw-rw-rw-   0        0        0     1016 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/internal/xml_rpc_server_base.py
+-rw-rw-rw-   0        0        0      823 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_array_value.py
+-rw-rw-rw-   0        0        0      896 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_boolean_value.py
+-rw-rw-rw-   0        0        0      895 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_double_value.py
+-rw-rw-rw-   0        0        0     1027 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_event_arg.py
+-rw-rw-rw-   0        0        0      893 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_integer_value.py
+-rw-rw-rw-   0        0        0      928 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_pose_value.py
+-rw-rw-rw-   0        0        0      517 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_server.py
+-rw-rw-rw-   0        0        0      889 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_string_value.py
+-rw-rw-rw-   0        0        0      911 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_struct_member.py
+-rw-rw-rw-   0        0        0      921 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_struct_value.py
+-rw-rw-rw-   0        0        0      120 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_type.py
+-rw-rw-rw-   0        0        0      777 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_unknown_value.py
+-rw-rw-rw-   0        0        0      743 2023-07-14 09:12:41.000000 UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_value.py
```

### Comparing `underautomation_universalrobots-7.4.1.0/UnderAutomation.UniversalRobots.egg-info/SOURCES.txt` & `UnderAutomation.UniversalRobots-7.4.1.0.1/UnderAutomation.UniversalRobots.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 ./underautomation/universal_robots/common/controller_box_types.py
 ./underautomation/universal_robots/common/dashboard_connect_parameters.py
 ./underautomation/universal_robots/common/digital_output_configurations.py
 ./underautomation/universal_robots/common/global_variable.py
 ./underautomation/universal_robots/common/global_variable_types.py
 ./underautomation/universal_robots/common/global_variable_value.py
 ./underautomation/universal_robots/common/internal_error_event_args.py
-./underautomation/universal_robots/common/interpreter_mode_connect_parameters.py
 ./underautomation/universal_robots/common/joint_modes.py
 ./underautomation/universal_robots/common/joints_double_values.py
 ./underautomation/universal_robots/common/joints_int_values.py
 ./underautomation/universal_robots/common/joints_values_1.py
 ./underautomation/universal_robots/common/output_modes.py
 ./underautomation/universal_robots/common/package_event_args.py
 ./underautomation/universal_robots/common/pose.py
@@ -43,38 +42,27 @@
 ./underautomation/universal_robots/dashboard/polyscope_version.py
 ./underautomation/universal_robots/dashboard/program_save_state.py
 ./underautomation/universal_robots/dashboard/program_state.py
 ./underautomation/universal_robots/dashboard/program_states.py
 ./underautomation/universal_robots/dashboard/user_roles.py
 ./underautomation/universal_robots/dashboard/internal/__init__.py
 ./underautomation/universal_robots/dashboard/internal/dashboard_client_base.py
-./underautomation/universal_robots/dashboard/internal/dashboard_client_parameters_base.py
 ./underautomation/universal_robots/files/__init__.py
 ./underautomation/universal_robots/files/ur_archive.py
 ./underautomation/universal_robots/files/ur_installation.py
 ./underautomation/universal_robots/files/ur_program.py
 ./underautomation/universal_robots/internal/__init__.py
 ./underautomation/universal_robots/internal/dashboard_client_internal.py
-./underautomation/universal_robots/internal/interpreter_mode_client_internal.py
 ./underautomation/universal_robots/internal/primary_interface_client_internal.py
 ./underautomation/universal_robots/internal/rtde_client_internal.py
 ./underautomation/universal_robots/internal/sftp_client_internal.py
 ./underautomation/universal_robots/internal/socket_communication_server_internal.py
 ./underautomation/universal_robots/internal/ssh_client_internal.py
 ./underautomation/universal_robots/internal/ur_service_base.py
 ./underautomation/universal_robots/internal/xml_rpc_server_internal.py
-./underautomation/universal_robots/interpreter_mode/__init__.py
-./underautomation/universal_robots/interpreter_mode/command_response.py
-./underautomation/universal_robots/interpreter_mode/command_response_status.py
-./underautomation/universal_robots/interpreter_mode/interpreter_mode_client.py
-./underautomation/universal_robots/interpreter_mode/internal/__init__.py
-./underautomation/universal_robots/interpreter_mode/internal/interpreter_mode_client_base.py
-./underautomation/universal_robots/interpreter_mode/internal/interpreter_mode_client_parameters_base.py
-./underautomation/universal_robots/lib/UnderAutomation.UniversalRobots.dll
-./underautomation/universal_robots/lib/version.txt
 ./underautomation/universal_robots/license/__init__.py
 ./underautomation/universal_robots/license/invalid_license_exception.py
 ./underautomation/universal_robots/license/license_info.py
 ./underautomation/universal_robots/license/license_state.py
 ./underautomation/universal_robots/primary_interface/__init__.py
 ./underautomation/universal_robots/primary_interface/additional_info_package_event_args.py
 ./underautomation/universal_robots/primary_interface/calibration_data_package_event_args.py
@@ -108,15 +96,14 @@
 ./underautomation/universal_robots/primary_interface/text_message_event_args.py
 ./underautomation/universal_robots/primary_interface/tool_communication_info_package_event_args.py
 ./underautomation/universal_robots/primary_interface/tool_data_package_event_args.py
 ./underautomation/universal_robots/primary_interface/tool_mode_info_package_event_args.py
 ./underautomation/universal_robots/primary_interface/version_event_args.py
 ./underautomation/universal_robots/primary_interface/internal/__init__.py
 ./underautomation/universal_robots/primary_interface/internal/primary_interface_client_base.py
-./underautomation/universal_robots/primary_interface/internal/primary_interface_commands.py
 ./underautomation/universal_robots/primary_interface/internal/primary_interface_parameters_base.py
 ./underautomation/universal_robots/primary_interface/internal/primary_interface_script.py
 ./underautomation/universal_robots/rtde/__init__.py
 ./underautomation/universal_robots/rtde/rtde_base_values.py
 ./underautomation/universal_robots/rtde/rtde_base_values_1.py
 ./underautomation/universal_robots/rtde/rtde_basic_request_event_args.py
 ./underautomation/universal_robots/rtde/rtde_bit_registers_value.py
```

### Comparing `underautomation_universalrobots-7.4.1.0/setup.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import setuptools
+from setuptools.dist import Distribution
 import os
 
 with open('README.md', "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version_file = os.path.realpath(os.path.join(os.path.dirname(__file__), "underautomation",  'universal_robots', 'lib', 'version.txt'))
-
-with open(version_file, "r", encoding="utf-8") as fh:
-    version = fh.read()
 
 setuptools.setup(
     name="UnderAutomation.UniversalRobots",
-    version=version,
+    version="7.4.1.0.1",
     author="UnderAutomation",
     author_email="support@underautomation.com",
     description="Quickly create applications that communicate with your Universal Robots cobot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://underautomation.com/universal-robots",
     project_urls={
@@ -27,13 +24,12 @@
     packages=setuptools.find_packages(where="."),
     python_requires=">=3.7",
     install_requires=[
         'pythonnet==3.0.3'
     ],
     include_package_data=True,
     package_data={"": [
-        "universal_robots/lib/*.dll",
-        "universal_robots/lib/*.txt"
+        "universal_robots/lib/*.dll"
     ]}
 )
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/cartesian_coordinates.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/cartesian_coordinates.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/dashboard_connect_parameters.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/dashboard_connect_parameters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import typing
-from underautomation.universal_robots.dashboard.internal.dashboard_client_parameters_base import DashboardClientParametersBase
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
 from UnderAutomation.UniversalRobots.Common import DashboardConnectParameters as dashboard_connect_parameters
 
-class DashboardConnectParameters(DashboardClientParametersBase):
+class DashboardConnectParameters:
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
 			self._instance = dashboard_connect_parameters()
 		else:
 			self._instance = _internal
 	@property
 	def enable(self) -> bool:
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/global_variable.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/global_variable.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/global_variable_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/global_variable_value.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/internal_error_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/internal_error_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/interpreter_mode_connect_parameters.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_value_1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import typing
-from underautomation.universal_robots.interpreter_mode.internal.interpreter_mode_client_parameters_base import InterpreterModeClientParametersBase
+from underautomation.universal_robots.rtde.rtde_value import RtdeValue
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Common import InterpreterModeConnectParameters as interpreter_mode_connect_parameters
+from UnderAutomation.UniversalRobots.Rtde import RtdeValue as rtde_value_1
 
-class InterpreterModeConnectParameters(InterpreterModeClientParametersBase):
+T = typing.TypeVar('T')
+class RtdeValue1(RtdeValue, typing.Generic[T]):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = interpreter_mode_connect_parameters()
+			self._instance = rtde_value_1()
 		else:
 			self._instance = _internal
+	def __repr__(self):
+		return self._instance.ToString()
 	@property
-	def enable(self) -> bool:
-		return self._instance.Enable
-	@enable.setter
-	def enable(self, value: bool):
-		self._instance.Enable = value
+	def value(self) -> T:
+		return self._instance.Value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/joints_double_values.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/joints_double_values.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/joints_int_values.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/joints_int_values.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/joints_values_1.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/joints_values_1.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/pose.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/pose.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,19 +16,14 @@
 	def from_rpy_to_rotation_vector(self) -> 'Pose':
 		return Pose(None, None, None, None, None, None, self._instance.FromRPYToRotationVector())
 	def __repr__(self):
 		return self._instance.ToString()
 	@staticmethod
 	def try_parse(value: str, pose: 'Pose') -> bool:
 		return pose.TryParse(value, pose._instance)
-	def from_rotation_vector_to_quaternion(self, x: float, y: float, z: float, w: float) -> None:
-		self._instance.FromRotationVectorToQuaternion(x, y, z, w)
-	@staticmethod
-	def from_quaternion_to_rotation_vector(x: float, y: float, z: float, w: float) -> 'Pose':
-		return Pose(None, None, None, None, None, None, pose.FromQuaternionToRotationVector(x, y, z, w))
 	@property
 	def rx_degrees(self) -> float:
 		return self._instance.RxDegrees
 	@rx_degrees.setter
 	def rx_degrees(self, value: float):
 		self._instance.RxDegrees = value
 	@property
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/primary_interface_connect_parameters.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/primary_interface_connect_parameters.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/rtde_connect_parameters.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/rtde_connect_parameters.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/socket_communication_connect_parameters.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/socket_communication_connect_parameters.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/ssh_connect_parameters.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/ssh_connect_parameters.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/vector3_d.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/vector3_d.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/common/xml_rpc_connect_parameters.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/common/xml_rpc_connect_parameters.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/connect_parameters.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/connect_parameters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import typing
 from underautomation.universal_robots.common.primary_interface_connect_parameters import PrimaryInterfaceConnectParameters
 from underautomation.universal_robots.common.dashboard_connect_parameters import DashboardConnectParameters
 from underautomation.universal_robots.common.socket_communication_connect_parameters import SocketCommunicationConnectParameters
 from underautomation.universal_robots.common.ssh_connect_parameters import SshConnectParameters
 from underautomation.universal_robots.common.rtde_connect_parameters import RtdeConnectParameters
 from underautomation.universal_robots.common.xml_rpc_connect_parameters import XmlRpcConnectParameters
-from underautomation.universal_robots.common.interpreter_mode_connect_parameters import InterpreterModeConnectParameters
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__),  'lib', 'UnderAutomation.UniversalRobots.dll')))
 from UnderAutomation.UniversalRobots import ConnectParameters as connect_parameters
 
 class ConnectParameters:
 	def __init__(self, ip: str, _internal = 0):
@@ -61,13 +60,7 @@
 		self._instance.Rtde = value
 	@property
 	def xml_rpc(self) -> XmlRpcConnectParameters:
 		return XmlRpcConnectParameters(self._instance.XmlRpc)
 	@xml_rpc.setter
 	def xml_rpc(self, value: XmlRpcConnectParameters):
 		self._instance.XmlRpc = value
-	@property
-	def interpreter_mode(self) -> InterpreterModeConnectParameters:
-		return InterpreterModeConnectParameters(self._instance.InterpreterMode)
-	@interpreter_mode.setter
-	def interpreter_mode(self, value: InterpreterModeConnectParameters):
-		self._instance.InterpreterMode = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/command_response.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/command_response.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/command_response_1.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/command_response_1.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/dashboard_client.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/dashboard_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 class DashboardClient(DashboardClientBase):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
 			self._instance = dashboard_client()
 		else:
 			self._instance = _internal
-	def enable(self, ip: str, port: int=29999) -> None:
-		self._instance.Enable(ip, port)
+	def enable(self, ip: str) -> None:
+		self._instance.Enable(ip)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/internal/dashboard_client_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/internal/dashboard_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,20 +86,14 @@
 		return CommandResponse(self._instance.GetSerialNumber())
 	def get_robot_model(self) -> CommandResponse1[RobotModels]:
 		return CommandResponse1[RobotModels](None, self._instance.GetRobotModel())
 	@property
 	def ip(self) -> str:
 		return self._instance.IP
 	@property
-	def port(self) -> int:
-		return self._instance.Port
-	@port.setter
-	def port(self, value: int):
-		self._instance.Port = value
-	@property
 	def initialized(self) -> bool:
 		return self._instance.Initialized
 	@property
 	def before_shutdown(self) -> typing.Any:
 		return self._instance.BeforeShutdown
 	@before_shutdown.setter
 	def before_shutdown(self, value: typing.Any):
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/internal/dashboard_client_parameters_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/internal/primary_interface_parameters_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import typing
+from underautomation.universal_robots.primary_interface.interfaces import Interfaces
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..", "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Dashboard.Internal import DashboardClientParametersBase as dashboard_client_parameters_base
+from UnderAutomation.UniversalRobots.PrimaryInterface.Internal import PrimaryInterfaceParametersBase as primary_interface_parameters_base
 
-class DashboardClientParametersBase:
+class PrimaryInterfaceParametersBase:
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = dashboard_client_parameters_base()
+			self._instance = primary_interface_parameters_base()
 		else:
 			self._instance = _internal
 	@property
-	def port(self) -> int:
-		return self._instance.Port
+	def port(self) -> Interfaces:
+		return Interfaces(self._instance.Port)
 	@port.setter
-	def port(self, value: int):
+	def port(self, value: Interfaces):
 		self._instance.Port = value
-	@property
-	def defaul_t__port(self) -> int:
-		return self._instance.DEFAULT_PORT
-	@defaul_t__port.setter
-	def defaul_t__port(self, value: int):
-		self._instance.DEFAULT_PORT = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/polyscope_version.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/polyscope_version.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/program_save_state.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/program_save_state.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/dashboard/program_state.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/dashboard/program_state.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/files/ur_archive.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/files/ur_archive.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/files/ur_installation.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/files/ur_installation.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/files/ur_program.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/files/ur_program.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/dashboard_client_internal.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/dashboard_client_internal.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 class DashboardClientInternal(DashboardClientBase):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
 			self._instance = dashboard_client_internal()
 		else:
 			self._instance = _internal
-	def enable(self, port: int=29999) -> None:
-		self._instance.Enable(port)
+	def enable(self) -> None:
+		self._instance.Enable()
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/interpreter_mode_client_internal.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/sftp_client_internal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
-from underautomation.universal_robots.interpreter_mode.internal.interpreter_mode_client_base import InterpreterModeClientBase
+from underautomation.universal_robots.ssh.internal.sftp_client_base import SftpClientBase
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Internal import InterpreterModeClientInternal as interpreter_mode_client_internal
+from UnderAutomation.UniversalRobots.Internal import SftpClientInternal as sftp_client_internal
 
-class InterpreterModeClientInternal(InterpreterModeClientBase):
+class SftpClientInternal(SftpClientBase):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = interpreter_mode_client_internal()
+			self._instance = sftp_client_internal()
 		else:
 			self._instance = _internal
-	def connect(self, port: int=30020) -> None:
-		self._instance.Connect(port)
+	def connect(self, username: str, password: str) -> None:
+		self._instance.Connect(username, password)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/primary_interface_client_internal.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/primary_interface_client_internal.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/rtde_client_internal.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/rtde_client_internal.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 
 class RtdeClientInternal(RtdeClientBase):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
 			self._instance = rtde_client_internal()
 		else:
 			self._instance = _internal
-	def connect(self, outputSetup: RtdeOutputSetup, inputSetup: RtdeInputSetup, version: RtdeVersions, frequency: float, port: int) -> None:
-		self._instance.Connect(outputSetup._instance, inputSetup._instance, version._instance, frequency, port)
+	def connect(self, outputSetup: RtdeOutputSetup, inputSetup: RtdeInputSetup, version: RtdeVersions, frequency: float) -> None:
+		self._instance.Connect(outputSetup._instance, inputSetup._instance, version._instance, frequency)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/sftp_client_internal.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/sftp_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 from underautomation.universal_robots.ssh.internal.sftp_client_base import SftpClientBase
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Internal import SftpClientInternal as sftp_client_internal
+from UnderAutomation.UniversalRobots.Ssh import SftpClient as sftp_client
 
-class SftpClientInternal(SftpClientBase):
+class SftpClient(SftpClientBase):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = sftp_client_internal()
+			self._instance = sftp_client()
 		else:
 			self._instance = _internal
-	def connect(self, port: int, username: str, password: str) -> None:
-		self._instance.Connect(port, username, password)
+	def connect(self, ip: str, username: str, password: str) -> None:
+		self._instance.Connect(ip, username, password)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/socket_communication_server_internal.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/socket_communication_server_internal.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/ssh_client_internal.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/ssh_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 from underautomation.universal_robots.ssh.internal.ssh_client_base import SshClientBase
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Internal import SshClientInternal as ssh_client_internal
+from UnderAutomation.UniversalRobots.Ssh import SshClient as ssh_client
 
-class SshClientInternal(SshClientBase):
+class SshClient(SshClientBase):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = ssh_client_internal()
+			self._instance = ssh_client()
 		else:
 			self._instance = _internal
-	def connect(self, port: int, username: str, password: str) -> None:
-		self._instance.Connect(port, username, password)
+	def connect(self, ip: str, username: str, password: str) -> None:
+		self._instance.Connect(ip, username, password)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/ur_service_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/ur_service_base.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/internal/xml_rpc_server_internal.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/xml_rpc_server_internal.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/command_response.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_data_description_1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import typing
-from underautomation.universal_robots.interpreter_mode.command_response_status import CommandResponseStatus
+from underautomation.universal_robots.rtde.rtde_types import RtdeTypes
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.InterpreterMode import CommandResponse as command_response
+from UnderAutomation.UniversalRobots.Rtde import RtdeDataDescription as rtde_data_description_1
 
-class CommandResponse:
+T = typing.TypeVar('T')
+class RtdeDataDescription1(typing.Generic[T]):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = command_response()
+			self._instance = rtde_data_description_1()
 		else:
 			self._instance = _internal
-	def __repr__(self):
-		return self._instance.ToString()
 	@property
-	def status(self) -> CommandResponseStatus:
-		return CommandResponseStatus(self._instance.Status)
+	def data(self) -> T:
+		return self._instance.Data
 	@property
-	def id(self) -> int:
-		return self._instance.Id
+	def type(self) -> RtdeTypes:
+		return RtdeTypes(self._instance.Type)
 	@property
-	def body(self) -> str:
-		return self._instance.Body
+	def name(self) -> str:
+		return self._instance.Name
 	@property
-	def raw_answer(self) -> str:
-		return self._instance.RawAnswer
+	def description(self) -> str:
+		return self._instance.Description
 	@property
-	def command(self) -> str:
-		return self._instance.Command
+	def lower_index(self) -> int:
+		return self._instance.LowerIndex
+	@property
+	def array_size(self) -> int:
+		return self._instance.ArraySize
+	@property
+	def is_array(self) -> bool:
+		return self._instance.IsArray
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/internal/interpreter_mode_client_parameters_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_client_parameters_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 import typing
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..", "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.InterpreterMode.Internal import InterpreterModeClientParametersBase as interpreter_mode_client_parameters_base
+from UnderAutomation.UniversalRobots.Rtde.Internal import RtdeClientParametersBase as rtde_client_parameters_base
 
-class InterpreterModeClientParametersBase:
+class RtdeClientParametersBase:
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = interpreter_mode_client_parameters_base()
+			self._instance = rtde_client_parameters_base()
 		else:
 			self._instance = _internal
 	@property
-	def port(self) -> int:
-		return self._instance.Port
-	@port.setter
-	def port(self, value: int):
-		self._instance.Port = value
-	@property
-	def defaul_t__port(self) -> int:
-		return self._instance.DEFAULT_PORT
-	@defaul_t__port.setter
-	def defaul_t__port(self, value: int):
-		self._instance.DEFAULT_PORT = value
+	def frequency(self) -> float:
+		return self._instance.Frequency
+	@frequency.setter
+	def frequency(self, value: float):
+		self._instance.Frequency = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/interpreter_mode/interpreter_mode_client.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_request_event_args.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import typing
-from underautomation.universal_robots.interpreter_mode.internal.interpreter_mode_client_base import InterpreterModeClientBase
+from underautomation.universal_robots.socket_communication.socket_client import SocketClient
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.InterpreterMode import InterpreterModeClient as interpreter_mode_client
+from UnderAutomation.UniversalRobots.SocketCommunication import SocketRequestEventArgs as socket_request_event_args
 
-class InterpreterModeClient(InterpreterModeClientBase):
+class SocketRequestEventArgs:
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = interpreter_mode_client()
+			self._instance = socket_request_event_args()
 		else:
 			self._instance = _internal
-	def connect(self, ip: str, port: int=30020) -> None:
-		self._instance.Connect(ip, port)
+	@property
+	def message(self) -> str:
+		return self._instance.Message
+	@property
+	def client(self) -> SocketClient:
+		return SocketClient(self._instance.Client)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/license/invalid_license_exception.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/license/invalid_license_exception.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/license/license_info.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/license/license_info.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/additional_info_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/additional_info_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/calibration_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/calibration_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/cartesian_info_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/cartesian_info_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/configuration_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/configuration_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/force_mode_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/force_mode_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/global_variables.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/global_variables.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/global_variables_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/global_variables_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/primary_interface_client_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/internal/primary_interface_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from underautomation.universal_robots.primary_interface.version_event_args import VersionEventArgs
 from underautomation.universal_robots.primary_interface.key_message_event_args import KeyMessageEventArgs
 from underautomation.universal_robots.primary_interface.popup_message_event_args import PopupMessageEventArgs
 from underautomation.universal_robots.primary_interface.text_message_event_args import TextMessageEventArgs
 from underautomation.universal_robots.primary_interface.runtime_exception_message_event_args import RuntimeExceptionMessageEventArgs
 from underautomation.universal_robots.primary_interface.global_variables import GlobalVariables
 from underautomation.universal_robots.primary_interface.internal.primary_interface_script import PrimaryInterfaceScript
-from underautomation.universal_robots.primary_interface.internal.primary_interface_commands import PrimaryInterfaceCommands
 from underautomation.universal_robots.primary_interface.interfaces import Interfaces
 from underautomation.universal_robots.internal.ur_service_base import URServiceBase
 from underautomation.universal_robots.common.package_event_args import PackageEventArgs
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..", "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
 from UnderAutomation.UniversalRobots.PrimaryInterface.Internal import PrimaryInterfaceClientBase as primary_interface_client_base
@@ -206,17 +205,14 @@
 	@property
 	def global_variables(self) -> GlobalVariables:
 		return GlobalVariables(self._instance.GlobalVariables)
 	@property
 	def script(self) -> PrimaryInterfaceScript:
 		return PrimaryInterfaceScript(self._instance.Script)
 	@property
-	def commands(self) -> PrimaryInterfaceCommands:
-		return PrimaryInterfaceCommands(self._instance.Commands)
-	@property
 	def ip(self) -> str:
 		return self._instance.IP
 	@property
 	def port(self) -> Interfaces:
 		return Interfaces(self._instance.Port)
 	@property
 	def connected(self) -> bool:
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/primary_interface_parameters_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_array_value.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import typing
-from underautomation.universal_robots.primary_interface.interfaces import Interfaces
+from underautomation.universal_robots.xml_rpc.xml_rpc_type import XmlRpcType
+from underautomation.universal_robots.xml_rpc.xml_rpc_value import XmlRpcValue
 import clr
 import os
-clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..", "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.PrimaryInterface.Internal import PrimaryInterfaceParametersBase as primary_interface_parameters_base
+clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
+from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcArrayValue as xml_rpc_array_value
 
-class PrimaryInterfaceParametersBase:
-	def __init__(self, _internal = 0):
+class XmlRpcArrayValue(XmlRpcValue):
+	def __init__(self, value: typing.Any, _internal = 0):
 		if(_internal == 0):
-			self._instance = primary_interface_parameters_base()
+			self._instance = xml_rpc_array_value(value)
 		else:
 			self._instance = _internal
+	def __repr__(self):
+		return self._instance.ToString()
 	@property
-	def port(self) -> Interfaces:
-		return Interfaces(self._instance.Port)
-	@port.setter
-	def port(self, value: Interfaces):
-		self._instance.Port = value
+	def type(self) -> XmlRpcType:
+		return XmlRpcType(self._instance.Type)
+	@property
+	def value(self) -> typing.Any:
+		return self._instance.Value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/internal/primary_interface_script.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/internal/primary_interface_script.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/joint_configuration.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/joint_configuration.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/joint_data.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/joint_data.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/joint_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/joint_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/joint_kinematics_info.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/joint_kinematics_info.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/key_message_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/key_message_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/kinematics_info_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/kinematics_info_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/masterboard_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/masterboard_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/masterboard_digital_io.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/masterboard_digital_io.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/package_description_attribute.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/package_description_attribute.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/popup_message_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/popup_message_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/primary_interface_client.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/primary_interface_client.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/program_thread.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/program_thread.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/program_threads_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/program_threads_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/request_value_message_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/request_value_message_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/robot_mode_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/robot_mode_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/runtime_exception_message_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/runtime_exception_message_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/safety_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/safety_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/singularity_info_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/singularity_info_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/text_message_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/text_message_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/tool_communication_info_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/tool_communication_info_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/tool_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/tool_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/tool_mode_info_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/tool_mode_info_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/primary_interface/version_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/primary_interface/version_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_client_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,12 @@
 	@property
 	def output_recipe_id(self) -> int:
 		return self._instance.OutputRecipeId
 	@property
 	def input_recipe_id(self) -> int:
 		return self._instance.InputRecipeId
 	@property
-	def input_recipe_is_valid(self) -> bool:
-		return self._instance.InputRecipeIsValid
-	@property
 	def measured_frequency(self) -> float:
 		return self._instance.MeasuredFrequency
 	@property
 	def output_data_values(self) -> RtdeOutputValues:
 		return RtdeOutputValues(self._instance.OutputDataValues)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_client_parameters_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/internal/xml_rpc_parameters_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typing
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..", "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Rtde.Internal import RtdeClientParametersBase as rtde_client_parameters_base
+from UnderAutomation.UniversalRobots.XmlRpc.Internal import XmlRpcParametersBase as xml_rpc_parameters_base
 
-class RtdeClientParametersBase:
+class XmlRpcParametersBase:
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = rtde_client_parameters_base()
+			self._instance = xml_rpc_parameters_base()
 		else:
 			self._instance = _internal
 	@property
-	def frequency(self) -> float:
-		return self._instance.Frequency
-	@frequency.setter
-	def frequency(self, value: float):
-		self._instance.Frequency = value
+	def port(self) -> int:
+		return self._instance.Port
+	@port.setter
+	def port(self, value: int):
+		self._instance.Port = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_parameters_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_parameters_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,19 +33,7 @@
 		self._instance.OutputSetup = value
 	@property
 	def input_setup(self) -> RtdeInputSetup:
 		return RtdeInputSetup(self._instance.InputSetup)
 	@input_setup.setter
 	def input_setup(self, value: RtdeInputSetup):
 		self._instance.InputSetup = value
-	@property
-	def port(self) -> int:
-		return self._instance.Port
-	@port.setter
-	def port(self, value: int):
-		self._instance.Port = value
-	@property
-	def defaul_t__port(self) -> int:
-		return self._instance.DEFAULT_PORT
-	@defaul_t__port.setter
-	def defaul_t__port(self, value: int):
-		self._instance.DEFAULT_PORT = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_setup_2.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_setup_2.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/internal/rtde_setup_item_1.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/internal/rtde_setup_item_1.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_base_values.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_base_values.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_base_values_1.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_base_values_1.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_basic_request_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_basic_request_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_bit_registers_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_bit_registers_value.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_client.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class RtdeClient(RtdeClientBase):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
 			self._instance = rtde_client()
 		else:
 			self._instance = _internal
-	def connect(self, ip: str, outputSetup: RtdeOutputSetup, inputSetup: RtdeInputSetup, version: RtdeVersions, frequency: float, port: int=30004) -> None:
-		self._instance.Connect(ip, outputSetup._instance, inputSetup._instance, version._instance, frequency, port)
+	def connect(self, ip: str, outputSetup: RtdeOutputSetup, inputSetup: RtdeInputSetup, version: RtdeVersions, frequency: float) -> None:
+		self._instance.Connect(ip, outputSetup._instance, inputSetup._instance, version._instance, frequency)
 	@property
 	def all_outputs_description(self) -> RtdeOutputsDescription:
 		return RtdeOutputsDescription(self._instance.AllOutputsDescription)
 	@property
 	def all_inputs_description(self) -> RtdeInputsDescription:
 		return RtdeInputsDescription(self._instance.AllInputsDescription)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_control_package_setup_inputs_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_control_package_setup_inputs_event_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,10 +19,7 @@
 		self._instance.InputRecipeId = value
 	@property
 	def variable_types(self) -> typing.List[str]:
 		return self._instance.VariableTypes
 	@variable_types.setter
 	def variable_types(self, value: typing.List[str]):
 		self._instance.VariableTypes = value
-	@property
-	def input_recipe_is_valid(self) -> bool:
-		return self._instance.InputRecipeIsValid
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_control_package_setup_outputs_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_control_package_setup_outputs_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_data_description_1.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_string_value.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 import typing
-from underautomation.universal_robots.rtde.rtde_types import RtdeTypes
+from underautomation.universal_robots.xml_rpc.xml_rpc_type import XmlRpcType
+from underautomation.universal_robots.xml_rpc.xml_rpc_value import XmlRpcValue
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Rtde import RtdeDataDescription as rtde_data_description_1
+from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcStringValue as xml_rpc_string_value
 
-T = typing.TypeVar('T')
-class RtdeDataDescription1(typing.Generic[T]):
-	def __init__(self, _internal = 0):
+class XmlRpcStringValue(XmlRpcValue):
+	def __init__(self, value: str, _internal = 0):
 		if(_internal == 0):
-			self._instance = rtde_data_description_1()
+			self._instance = xml_rpc_string_value(value)
 		else:
 			self._instance = _internal
+	def __repr__(self):
+		return self._instance.ToString()
 	@property
-	def data(self) -> T:
-		return self._instance.Data
+	def type(self) -> XmlRpcType:
+		return XmlRpcType(self._instance.Type)
 	@property
-	def type(self) -> RtdeTypes:
-		return RtdeTypes(self._instance.Type)
-	@property
-	def name(self) -> str:
-		return self._instance.Name
-	@property
-	def description(self) -> str:
-		return self._instance.Description
-	@property
-	def lower_index(self) -> int:
-		return self._instance.LowerIndex
-	@property
-	def array_size(self) -> int:
-		return self._instance.ArraySize
-	@property
-	def is_array(self) -> bool:
-		return self._instance.IsArray
+	def value(self) -> str:
+		return self._instance.Value
+	@value.setter
+	def value(self, value: str):
+		self._instance.Value = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_data_package_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_data_package_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_double_registers_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_double_registers_value.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_data_description.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_data_description.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_setup.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_setup.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_setup_item.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_setup_item.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_input_values.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_input_values.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_inputs_description.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_inputs_description.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_int_registers_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_int_registers_value.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_data_description.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_data_description.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_setup.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_setup.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_setup_item.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_setup_item.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_output_values.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_output_values.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_outputs_description.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_outputs_description.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_protocol_version_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_protocol_version_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_registers_value_1.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_registers_value_1.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_text_message_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/rtde/rtde_text_message_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/rtde/rtde_value_1.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_value.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import typing
-from underautomation.universal_robots.rtde.rtde_value import RtdeValue
+from underautomation.universal_robots.xml_rpc.xml_rpc_type import XmlRpcType
+from underautomation.universal_robots.common.pose import Pose
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Rtde import RtdeValue as rtde_value_1
+from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcValue as xml_rpc_value
 
-T = typing.TypeVar('T')
-class RtdeValue1(RtdeValue, typing.Generic[T]):
+class XmlRpcValue:
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = rtde_value_1()
+			self._instance = xml_rpc_value()
 		else:
 			self._instance = _internal
 	def __repr__(self):
 		return self._instance.ToString()
 	@property
-	def value(self) -> T:
-		return self._instance.Value
+	def type(self) -> XmlRpcType:
+		return XmlRpcType(self._instance.Type)
+	@property
+	def xml(self) -> typing.Any:
+		return self._instance.Xml
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/internal/socket_communication_parameters_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/internal/socket_communication_parameters_base.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/internal/socket_communication_server_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/internal/socket_communication_server_base.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_client.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_client.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_client_connection_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_client_connection_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_client_disconnection_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_client_disconnection_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_communication_server.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_communication_server.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/socket_communication/socket_get_var_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/socket_communication/socket_get_var_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/internal/sftp_client_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/internal/sftp_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 		self._instance.DeleteFile(path)
 	def rename_file(self, oldPath: str, newPath: str, isPosix: bool) -> None:
 		self._instance.RenameFile(oldPath, newPath, isPosix)
 	def symbolic_link(self, path: str, linkPath: str) -> None:
 		self._instance.SymbolicLink(path, linkPath)
 	def list_directory(self, path: str, listCallback: typing.Any=None) -> typing.List[SftpFile]:
 		return [SftpFile(x) for x in self._instance.ListDirectory(path, listCallback)]
-	def enumerate_programs(self) -> typing.List[str]:
-		return self._instance.EnumeratePrograms()
 	def begin_list_directory(self, path: str, asyncCallback: typing.Any, state: typing.Any, listCallback: typing.Any=None) -> typing.Any:
 		return self._instance.BeginListDirectory(path, asyncCallback, state, listCallback)
 	def end_list_directory(self, asyncResult: typing.Any) -> typing.List[SftpFile]:
 		return [SftpFile(x) for x in self._instance.EndListDirectory(asyncResult)]
 	def get(self, path: str) -> SftpFile:
 		return SftpFile(self._instance.Get(path))
 	def exists(self, path: str) -> bool:
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/internal/ssh_client_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/internal/ssh_client_base.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/internal/ssh_parameters_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_struct_member.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 import typing
+from underautomation.universal_robots.xml_rpc.xml_rpc_value import XmlRpcValue
 import clr
 import os
-clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..", "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Ssh.Internal import SshParametersBase as ssh_parameters_base
+clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
+from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcStructMember as xml_rpc_struct_member
 
-class SshParametersBase:
-	def __init__(self, _internal = 0):
+class XmlRpcStructMember:
+	def __init__(self, name: str, value: XmlRpcValue, _internal = 0):
 		if(_internal == 0):
-			self._instance = ssh_parameters_base()
+			self._instance = xml_rpc_struct_member(name, value)
 		else:
 			self._instance = _internal
+	def __repr__(self):
+		return self._instance.ToString()
 	@property
-	def username(self) -> str:
-		return self._instance.Username
-	@username.setter
-	def username(self, value: str):
-		self._instance.Username = value
+	def name(self) -> str:
+		return self._instance.Name
+	@name.setter
+	def name(self, value: str):
+		self._instance.Name = value
 	@property
-	def password(self) -> str:
-		return self._instance.Password
-	@password.setter
-	def password(self, value: str):
-		self._instance.Password = value
-	@property
-	def port(self) -> int:
-		return self._instance.Port
-	@port.setter
-	def port(self, value: int):
-		self._instance.Port = value
-	@property
-	def defaul_t__port(self) -> int:
-		return self._instance.DEFAULT_PORT
-	@defaul_t__port.setter
-	def defaul_t__port(self, value: int):
-		self._instance.DEFAULT_PORT = value
+	def value(self) -> XmlRpcValue:
+		return XmlRpcValue(self._instance.Value)
+	@value.setter
+	def value(self, value: XmlRpcValue):
+		self._instance.Value = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/sftp_client.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/internal/ssh_client_internal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
-from underautomation.universal_robots.ssh.internal.sftp_client_base import SftpClientBase
+from underautomation.universal_robots.ssh.internal.ssh_client_base import SshClientBase
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Ssh import SftpClient as sftp_client
+from UnderAutomation.UniversalRobots.Internal import SshClientInternal as ssh_client_internal
 
-class SftpClient(SftpClientBase):
+class SshClientInternal(SshClientBase):
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = sftp_client()
+			self._instance = ssh_client_internal()
 		else:
 			self._instance = _internal
-	def connect(self, ip: str, username: str, password: str, port: int=22) -> None:
-		self._instance.Connect(ip, username, password, port)
+	def connect(self, username: str, password: str) -> None:
+		self._instance.Connect(username, password)
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/ssh_client.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/expect_action.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import typing
-from underautomation.universal_robots.ssh.internal.ssh_client_base import SshClientBase
 import clr
 import os
-clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.Ssh import SshClient as ssh_client
+clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..", "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
+from UnderAutomation.UniversalRobots.Ssh.Tools import ExpectAction as expect_action
 
-class SshClient(SshClientBase):
-	def __init__(self, _internal = 0):
+class ExpectAction:
+	def __init__(self, expect: typing.Any, action: typing.Any, _internal = 0):
 		if(_internal == 0):
-			self._instance = ssh_client()
+			self._instance = expect_action(expect, action)
 		else:
 			self._instance = _internal
-	def connect(self, ip: str, username: str, password: str, port: int=22) -> None:
-		self._instance.Connect(ip, username, password, port)
+	@property
+	def expect(self) -> typing.Any:
+		return self._instance.Expect
+	@property
+	def action(self) -> typing.Any:
+		return self._instance.Action
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/exception_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/exception_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/object_identifier.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/object_identifier.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/sftp_path_not_found_exception.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/sftp_path_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/sftp_permission_denied_exception.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/sftp_permission_denied_exception.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/shell_data_event_args.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/shell_data_event_args.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_authentication_exception.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_authentication_exception.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_connection_exception.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_connection_exception.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_operation_timeout_exception.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_operation_timeout_exception.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/common/ssh_pass_phrase_null_or_empty_exception.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/common/ssh_pass_phrase_null_or_empty_exception.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/remote_path_transformation.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/remote_path_transformation.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/sftp_file.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/sftp_file.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/sftp_file_attributes.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/sftp_file_attributes.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/sftp_file_stream.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/sftp_file_stream.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/sftp/sftp_file_sytem_information.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/sftp/sftp_file_sytem_information.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/shell.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/shell.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/shell_stream.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/shell_stream.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ssh/tools/ssh_command.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/tools/ssh_command.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/ur.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ur.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from underautomation.universal_robots.internal.primary_interface_client_internal import PrimaryInterfaceClientInternal
 from underautomation.universal_robots.internal.xml_rpc_server_internal import XmlRpcServerInternal
 from underautomation.universal_robots.internal.dashboard_client_internal import DashboardClientInternal
 from underautomation.universal_robots.internal.socket_communication_server_internal import SocketCommunicationServerInternal
 from underautomation.universal_robots.internal.rtde_client_internal import RtdeClientInternal
 from underautomation.universal_robots.internal.ssh_client_internal import SshClientInternal
 from underautomation.universal_robots.internal.sftp_client_internal import SftpClientInternal
-from underautomation.universal_robots.internal.interpreter_mode_client_internal import InterpreterModeClientInternal
 from underautomation.universal_robots.connect_parameters import ConnectParameters
 from underautomation.universal_robots.license.license_info import LicenseInfo
 from underautomation.universal_robots.internal.ur_service_base import URServiceBase
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__),  'lib', 'UnderAutomation.UniversalRobots.dll')))
 from UnderAutomation.UniversalRobots import UR as ur
@@ -46,17 +45,14 @@
 	@property
 	def ssh(self) -> SshClientInternal:
 		return SshClientInternal(self._instance.Ssh)
 	@property
 	def sftp(self) -> SftpClientInternal:
 		return SftpClientInternal(self._instance.Sftp)
 	@property
-	def interpreter_mode(self) -> InterpreterModeClientInternal:
-		return InterpreterModeClientInternal(self._instance.InterpreterMode)
-	@property
 	def ip(self) -> str:
 		return self._instance.IP
 	@property
 	def enabled(self) -> bool:
 		return self._instance.Enabled
 	@property
 	def license_info(self) -> LicenseInfo:
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/internal/xml_rpc_parameters_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/ssh/internal/ssh_parameters_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import typing
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..", "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.XmlRpc.Internal import XmlRpcParametersBase as xml_rpc_parameters_base
+from UnderAutomation.UniversalRobots.Ssh.Internal import SshParametersBase as ssh_parameters_base
 
-class XmlRpcParametersBase:
+class SshParametersBase:
 	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = xml_rpc_parameters_base()
+			self._instance = ssh_parameters_base()
 		else:
 			self._instance = _internal
 	@property
-	def port(self) -> int:
-		return self._instance.Port
-	@port.setter
-	def port(self, value: int):
-		self._instance.Port = value
+	def username(self) -> str:
+		return self._instance.Username
+	@username.setter
+	def username(self, value: str):
+		self._instance.Username = value
+	@property
+	def password(self) -> str:
+		return self._instance.Password
+	@password.setter
+	def password(self, value: str):
+		self._instance.Password = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/internal/xml_rpc_server_base.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/internal/xml_rpc_server_base.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_array_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_double_value.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import typing
 from underautomation.universal_robots.xml_rpc.xml_rpc_type import XmlRpcType
 from underautomation.universal_robots.xml_rpc.xml_rpc_value import XmlRpcValue
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcArrayValue as xml_rpc_array_value
+from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcDoubleValue as xml_rpc_double_value
 
-class XmlRpcArrayValue(XmlRpcValue):
-	def __init__(self, value: typing.Any, _internal = 0):
+class XmlRpcDoubleValue(XmlRpcValue):
+	def __init__(self, value: float, _internal = 0):
 		if(_internal == 0):
-			self._instance = xml_rpc_array_value(value)
+			self._instance = xml_rpc_double_value(value)
 		else:
 			self._instance = _internal
 	def __repr__(self):
 		return self._instance.ToString()
 	@property
 	def type(self) -> XmlRpcType:
 		return XmlRpcType(self._instance.Type)
 	@property
-	def value(self) -> typing.Any:
+	def value(self) -> float:
 		return self._instance.Value
+	@value.setter
+	def value(self, value: float):
+		self._instance.Value = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_boolean_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_boolean_value.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_double_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_struct_value.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import typing
 from underautomation.universal_robots.xml_rpc.xml_rpc_type import XmlRpcType
 from underautomation.universal_robots.xml_rpc.xml_rpc_value import XmlRpcValue
+from underautomation.universal_robots.xml_rpc.xml_rpc_struct_member import XmlRpcStructMember
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcDoubleValue as xml_rpc_double_value
+from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcStructValue as xml_rpc_struct_value
 
-class XmlRpcDoubleValue(XmlRpcValue):
-	def __init__(self, value: float, _internal = 0):
+class XmlRpcStructValue(XmlRpcValue):
+	def __init__(self, value: typing.Any, _internal = 0):
 		if(_internal == 0):
-			self._instance = xml_rpc_double_value(value)
+			self._instance = xml_rpc_struct_value(value)
 		else:
 			self._instance = _internal
 	def __repr__(self):
 		return self._instance.ToString()
 	@property
 	def type(self) -> XmlRpcType:
 		return XmlRpcType(self._instance.Type)
 	@property
-	def value(self) -> float:
+	def value(self) -> typing.Any:
 		return self._instance.Value
-	@value.setter
-	def value(self, value: float):
-		self._instance.Value = value
```

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_event_arg.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_event_arg.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_integer_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_integer_value.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_pose_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_pose_value.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_server.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `underautomation_universalrobots-7.4.1.0/underautomation/universal_robots/xml_rpc/xml_rpc_string_value.py` & `UnderAutomation.UniversalRobots-7.4.1.0.1/underautomation/universal_robots/xml_rpc/xml_rpc_unknown_value.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import typing
 from underautomation.universal_robots.xml_rpc.xml_rpc_type import XmlRpcType
 from underautomation.universal_robots.xml_rpc.xml_rpc_value import XmlRpcValue
 import clr
 import os
 clr.AddReference(os.path.realpath(os.path.join(os.path.dirname(__file__), "..",  'lib', 'UnderAutomation.UniversalRobots.dll')))
-from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcStringValue as xml_rpc_string_value
+from UnderAutomation.UniversalRobots.XmlRpc import XmlRpcUnknownValue as xml_rpc_unknown_value
 
-class XmlRpcStringValue(XmlRpcValue):
-	def __init__(self, value: str, _internal = 0):
+class XmlRpcUnknownValue(XmlRpcValue):
+	def __init__(self, _internal = 0):
 		if(_internal == 0):
-			self._instance = xml_rpc_string_value(value)
+			self._instance = xml_rpc_unknown_value()
 		else:
 			self._instance = _internal
-	def __repr__(self):
-		return self._instance.ToString()
 	@property
 	def type(self) -> XmlRpcType:
 		return XmlRpcType(self._instance.Type)
 	@property
-	def value(self) -> str:
-		return self._instance.Value
-	@value.setter
-	def value(self, value: str):
-		self._instance.Value = value
+	def additional_information(self) -> str:
+		return self._instance.AdditionalInformation
```

