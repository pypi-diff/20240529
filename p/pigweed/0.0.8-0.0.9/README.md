# Comparing `tmp/pigweed-0.0.8.tar.gz` & `tmp/pigweed-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigweed-0.0.8.tar", last modified: Tue May  3 00:18:39 2022, max compression
+gzip compressed data, was "pigweed-0.0.9.tar", last modified: Fri Jul 15 20:26:01 2022, max compression
```

## Comparing `pigweed-0.0.8.tar` & `pigweed-0.0.9.tar`

### file list

```diff
@@ -1,452 +1,471 @@
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.898418 pigweed-0.0.8/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    11358 2022-05-03 00:17:25.000000 pigweed-0.0.8/LICENSE
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1463 2022-05-03 00:18:39.898418 pigweed-0.0.8/PKG-INFO
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      726 2022-05-03 00:17:25.000000 pigweed-0.0.8/README.md
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.854417 pigweed-0.0.8/pigweed.egg-info/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1463 2022-05-03 00:18:39.000000 pigweed-0.0.8/pigweed.egg-info/PKG-INFO
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    11249 2022-05-03 00:18:39.000000 pigweed-0.0.8/pigweed.egg-info/SOURCES.txt
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        1 2022-05-03 00:18:39.000000 pigweed-0.0.8/pigweed.egg-info/dependency_links.txt
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      816 2022-05-03 00:18:39.000000 pigweed-0.0.8/pigweed.egg-info/entry_points.txt
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        1 2022-05-03 00:18:38.000000 pigweed-0.0.8/pigweed.egg-info/not-zip-safe
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      478 2022-05-03 00:18:39.000000 pigweed-0.0.8/pigweed.egg-info/requires.txt
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      671 2022-05-03 00:18:39.000000 pigweed-0.0.8/pigweed.egg-info/top_level.txt
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.854417 pigweed-0.0.8/pw_allocator/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_allocator/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10532 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_allocator/heap_viewer.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_allocator/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.854417 pigweed-0.0.8/pw_arduino_build/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      652 2020-10-19 22:48:42.000000 pigweed-0.0.8/pw_arduino_build/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    24474 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_arduino_build/__main__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    45446 2022-03-14 23:06:10.000000 pigweed-0.0.8/pw_arduino_build/builder.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    16680 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_arduino_build/core_installer.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.846418 pigweed-0.0.8/pw_arduino_build/core_patches/
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.854417 pigweed-0.0.8/pw_arduino_build/core_patches/teensy/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2890 2021-09-29 19:32:40.000000 pigweed-0.0.8/pw_arduino_build/core_patches/teensy/01-teensyduino_1.53-cpp17.diff
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1501 2021-09-29 19:32:40.000000 pigweed-0.0.8/pw_arduino_build/core_patches/teensy/02-teensy4_nonstatic_flash_functions.diff
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     8539 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_arduino_build/file_operations.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1568 2021-09-29 19:32:03.000000 pigweed-0.0.8/pw_arduino_build/log.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_arduino_build/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4430 2021-09-29 19:32:07.000000 pigweed-0.0.8/pw_arduino_build/teensy_detector.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1888 2021-09-29 19:32:03.000000 pigweed-0.0.8/pw_arduino_build/unit_test_client.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    13528 2021-09-29 19:32:40.000000 pigweed-0.0.8/pw_arduino_build/unit_test_runner.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6281 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_arduino_build/unit_test_server.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.854417 pigweed-0.0.8/pw_bloat/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_bloat/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2973 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_bloat/binary_diff.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6949 2022-03-29 20:58:09.000000 pigweed-0.0.8/pw_bloat/bloat.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6923 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_bloat/bloat_output.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    13633 2022-04-14 18:36:12.000000 pigweed-0.0.8/pw_bloat/bloaty_config.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1017 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_bloat/no_bloaty.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1139 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_bloat/no_toolchains.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_bloat/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.858418 pigweed-0.0.8/pw_build/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_build/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1959 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_build/collect_wheels.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5232 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_build/copy_from_cipd.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12490 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_build/create_python_tree.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2737 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_build/error.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5002 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_build/exec.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2680 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_build/file_prefix_map.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6694 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_build/generate_cc_blob_library.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     9453 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_build/generate_modules_lists.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     9361 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_build/generate_python_package.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3555 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_build/generate_python_package_gn.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7538 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_build/generated_tests.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3091 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_build/host_tool.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3843 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_build/mirror_tree.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1161 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_build/nop.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4032 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_build/pip_install_python_deps.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_build/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7614 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_build/python_package.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    22929 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_build/python_runner.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1907 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_build/python_wheels.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5472 2021-09-29 19:32:03.000000 pigweed-0.0.8/pw_build/zip.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.858418 pigweed-0.0.8/pw_build_info/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_build_info/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5763 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_build_info/build_id.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_build_info/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.858418 pigweed-0.0.8/pw_build_mcuxpresso/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      644 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_build_mcuxpresso/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1865 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_build_mcuxpresso/__main__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    15422 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_build_mcuxpresso/components.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.862418 pigweed-0.0.8/pw_cli/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_cli/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1644 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_cli/__main__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1085 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_cli/argument_types.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3128 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_cli/arguments.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2274 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_cli/branding.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2652 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_cli/color.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3072 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_cli/env.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6393 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_cli/envparse.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6315 2022-03-15 19:20:06.000000 pigweed-0.0.8/pw_cli/log.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    15395 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_cli/plugins.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3854 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_cli/process.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2649 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_cli/pw_command_plugins.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_cli/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6008 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_cli/requires.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.866418 pigweed-0.0.8/pw_console/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      706 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4960 2022-04-04 16:54:28.000000 pigweed-0.0.8/pw_console/__main__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    18469 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_console/command_runner.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    37415 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_console/console_app.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10326 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_console/console_prefs.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.866418 pigweed-0.0.8/pw_console/docs/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    32719 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/docs/user_guide.rst
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12302 2022-03-29 20:58:09.000000 pigweed-0.0.8/pw_console/embed.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4418 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_console/filter_toolbar.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      828 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/get_pw_console_app.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12553 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/help_window.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7137 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/key_bindings.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4989 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/log_filter.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3584 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/log_line.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    26098 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/log_pane.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10694 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/log_pane_saveas_dialog.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6802 2022-03-16 00:02:46.000000 pigweed-0.0.8/pw_console/log_pane_selection_dialog.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3298 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/log_pane_toolbars.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    27075 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/log_screen.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     9364 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/log_store.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    31680 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/log_view.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1068 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_console/mouse.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2487 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_console/pigweed_code_style.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6012 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/plugin_mixin.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.866418 pigweed-0.0.8/pw_console/plugins/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      623 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/plugins/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3309 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/plugins/bandwidth_toolbar.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     8555 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/plugins/calc_pane.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    17884 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/plugins/clock_pane.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    18689 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_console/plugins/twenty48_pane.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.866418 pigweed-0.0.8/pw_console/progress_bar/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2370 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_console/progress_bar/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5321 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_console/progress_bar/progress_bar_impl.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4633 2022-01-14 02:07:27.000000 pigweed-0.0.8/pw_console/progress_bar/progress_bar_state.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2490 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_console/progress_bar/progress_bar_task_counter.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12750 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/pw_ptpython_repl.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_console/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4166 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/pyserial_wrapper.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3947 2022-03-26 19:14:52.000000 pigweed-0.0.8/pw_console/python_logging.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5880 2022-04-04 22:22:31.000000 pigweed-0.0.8/pw_console/quit_dialog.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    17447 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/repl_pane.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    16722 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/search_toolbar.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    18974 2022-04-04 22:22:31.000000 pigweed-0.0.8/pw_console/style.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.866418 pigweed-0.0.8/pw_console/templates/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1321 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/templates/keybind_list.jinja
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1146 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/templates/repl_output.jinja
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     8924 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/text_formatting.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.866418 pigweed-0.0.8/pw_console/widgets/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1040 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/widgets/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3873 2022-04-04 22:22:31.000000 pigweed-0.0.8/pw_console/widgets/border.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4829 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/widgets/checkbox.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3758 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_console/widgets/event_count_history.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2069 2022-03-16 00:02:46.000000 pigweed-0.0.8/pw_console/widgets/mouse_handlers.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10956 2022-03-26 19:14:52.000000 pigweed-0.0.8/pw_console/widgets/table.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7297 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/widgets/window_pane.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     9307 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/widgets/window_pane_toolbar.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    21676 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/window_list.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    40473 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/window_manager.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5942 2022-03-23 19:45:05.000000 pigweed-0.0.8/pw_console/yaml_config_loader_mixin.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.866418 pigweed-0.0.8/pw_cpu_exception_cortex_m/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      745 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1941 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m/cfsr_decoder.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    11072 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m/cortex_m_constants.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7840 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m/exception_analyzer.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.870418 pigweed-0.0.8/pw_cpu_exception_cortex_m_protos/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m_protos/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    16111 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m_protos/cpu_state_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5682 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m_protos/cpu_state_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_cpu_exception_cortex_m_protos/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.870418 pigweed-0.0.8/pw_docgen/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_docgen/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6286 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_docgen/docgen.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_docgen/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.870418 pigweed-0.0.8/pw_docgen/sphinx/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_docgen/sphinx/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1466 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_docgen/sphinx/google_analytics.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.870418 pigweed-0.0.8/pw_doctor/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_doctor/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    15242 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_doctor/doctor.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_doctor/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.870418 pigweed-0.0.8/pw_env_setup/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      617 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_env_setup/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2749 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_env_setup/apply_visitor.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4545 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_env_setup/batch_visitor.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.870418 pigweed-0.0.8/pw_env_setup/cipd_setup/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      584 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_env_setup/cipd_setup/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2113 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_env_setup/cipd_setup/luci.json
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4647 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_env_setup/cipd_setup/pigweed.json
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    11860 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_env_setup/cipd_setup/update.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    11913 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_env_setup/cipd_setup/wrapper.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1399 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_env_setup/colors.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    26272 2022-04-19 19:10:00.000000 pigweed-0.0.8/pw_env_setup/env_setup.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    15501 2022-03-16 00:02:46.000000 pigweed-0.0.8/pw_env_setup/environment.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3001 2022-03-16 15:51:05.000000 pigweed-0.0.8/pw_env_setup/gni_visitor.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3147 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_env_setup/json_visitor.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_env_setup/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4424 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_env_setup/python_packages.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6987 2021-12-07 02:31:51.000000 pigweed-0.0.8/pw_env_setup/shell_visitor.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2194 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_env_setup/spinner.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.870418 pigweed-0.0.8/pw_env_setup/virtualenv_setup/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      713 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_env_setup/virtualenv_setup/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2505 2021-09-29 19:32:40.000000 pigweed-0.0.8/pw_env_setup/virtualenv_setup/__main__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    11037 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_env_setup/virtualenv_setup/install.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2955 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_env_setup/windows_env_start.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.874418 pigweed-0.0.8/pw_hdlc/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:40.000000 pigweed-0.0.8/pw_hdlc/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6271 2022-04-14 18:36:12.000000 pigweed-0.0.8/pw_hdlc/decode.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1192 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_hdlc/encode.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2215 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_hdlc/protocol.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:40.000000 pigweed-0.0.8/pw_hdlc/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10365 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_hdlc/rpc.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10282 2022-04-06 15:23:57.000000 pigweed-0.0.8/pw_hdlc/rpc_console.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.874418 pigweed-0.0.8/pw_log/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_log/__init__.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.874418 pigweed-0.0.8/pw_log/proto/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_log/proto/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    27996 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_log/proto/log_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    15841 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_log/proto/log_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_log/proto/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_log/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.874418 pigweed-0.0.8/pw_log_tokenized/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2722 2022-03-26 19:14:52.000000 pigweed-0.0.8/pw_log_tokenized/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_log_tokenized/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.874418 pigweed-0.0.8/pw_module/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2020-10-19 22:49:42.000000 pigweed-0.0.8/pw_module/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7107 2020-10-19 22:49:42.000000 pigweed-0.0.8/pw_module/check.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_module/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.874418 pigweed-0.0.8/pw_package/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_package/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5020 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/git_repo.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6156 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/package_manager.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.878418 pigweed-0.0.8/pw_package/packages/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      584 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_package/packages/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5318 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/packages/arduino_core.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2720 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/packages/boringssl.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5808 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/packages/chromium_verifier.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3104 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_package/packages/crlset.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1439 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_package/packages/freertos.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1444 2022-04-04 22:22:31.000000 pigweed-0.0.8/pw_package/packages/googletest.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1558 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/packages/mbedtls.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1599 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/packages/micro_ecc.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1377 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/packages/nanopb.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1456 2022-04-04 22:22:31.000000 pigweed-0.0.8/pw_package/packages/pico_sdk.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1443 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/packages/protobuf.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1476 2022-04-06 15:23:57.000000 pigweed-0.0.8/pw_package/packages/smartfusion_mss.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4795 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_package/packages/stm32cube.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1875 2022-04-06 15:23:57.000000 pigweed-0.0.8/pw_package/pigweed_packages.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:07.000000 pigweed-0.0.8/pw_package/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.878418 pigweed-0.0.8/pw_presubmit/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      745 2020-10-19 22:49:42.000000 pigweed-0.0.8/pw_presubmit/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12263 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_presubmit/build.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7487 2022-03-16 15:51:05.000000 pigweed-0.0.8/pw_presubmit/cli.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1989 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_presubmit/cpp_checks.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    18594 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_presubmit/format_code.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    11610 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_presubmit/git_repo.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5168 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_presubmit/inclusive_language.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3771 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_presubmit/install_hook.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    30122 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_presubmit/pigweed_presubmit.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    23134 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_presubmit/presubmit.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_presubmit/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6025 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_presubmit/python_checks.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6182 2021-09-29 19:32:08.000000 pigweed-0.0.8/pw_presubmit/tools.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.878418 pigweed-0.0.8/pw_protobuf/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2020-10-19 22:49:42.000000 pigweed-0.0.8/pw_protobuf/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    76335 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_protobuf/codegen_pwpb.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2801 2022-04-06 15:23:57.000000 pigweed-0.0.8/pw_protobuf/options.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2288 2020-10-19 22:49:42.000000 pigweed-0.0.8/pw_protobuf/output_file.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3506 2022-04-06 15:23:57.000000 pigweed-0.0.8/pw_protobuf/plugin.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    20386 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_protobuf/proto_tree.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_protobuf/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.882418 pigweed-0.0.8/pw_protobuf_codegen_protos/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_codegen_protos/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3907 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_codegen_protos/options_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1562 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_codegen_protos/options_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_codegen_protos/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.882418 pigweed-0.0.8/pw_protobuf_compiler/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2020-10-19 22:49:42.000000 pigweed-0.0.8/pw_protobuf_compiler/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6934 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_protobuf_compiler/generate_protos.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2163 2021-09-29 19:32:06.000000 pigweed-0.0.8/pw_protobuf_compiler/proto_target_invalid.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_protobuf_compiler/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    13783 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_protobuf_compiler/python_protos.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.882418 pigweed-0.0.8/pw_protobuf_compiler_protos/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/__init__.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.882418 pigweed-0.0.8/pw_protobuf_compiler_protos/nested/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/nested/__init__.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.882418 pigweed-0.0.8/pw_protobuf_compiler_protos/nested/more_nesting/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/nested/more_nesting/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/nested/more_nesting/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2219 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/nested/more_nesting/test_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      635 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/nested/more_nesting/test_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/nested/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1811 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/test_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      639 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_compiler_protos/test_pb2.pyi
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.882418 pigweed-0.0.8/pw_protobuf_protos/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_protos/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1583 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_protos/common_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      378 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_protos/common_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_protos/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5385 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_protos/status_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1798 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_protobuf_protos/status_pb2.pyi
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.886418 pigweed-0.0.8/pw_rpc/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      863 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_rpc/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3092 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/benchmark_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      649 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/benchmark_pb2.pyi
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.886418 pigweed-0.0.8/pw_rpc/callback_client/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4106 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/callback_client/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12055 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/callback_client/call.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1489 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/callback_client/errors.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    18013 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/callback_client/impl.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/callback_client/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    21158 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_rpc/client.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    17802 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_rpc/codegen.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10059 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_rpc/codegen_nanopb.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     9579 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_rpc/codegen_pwpb.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6869 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_rpc/codegen_raw.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.886418 pigweed-0.0.8/pw_rpc/console_tools/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      969 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/console_tools/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12026 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/console_tools/console.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3033 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/console_tools/functions.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/console_tools/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3059 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_rpc/console_tools/watchdog.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    14830 2022-04-04 22:22:31.000000 pigweed-0.0.8/pw_rpc/descriptors.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2880 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/echo_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      649 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/echo_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1238 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/ids.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.886418 pigweed-0.0.8/pw_rpc/internal/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/internal/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7701 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/internal/packet_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4686 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/internal/packet_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/internal/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     8781 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_rpc/lossy_channel.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3568 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_rpc/packets.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2781 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_rpc/plugin.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      798 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/plugin_nanopb.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      801 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_rpc/plugin_pwpb.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      792 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_rpc/plugin_raw.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_rpc/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3759 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_rpc/testing.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.886418 pigweed-0.0.8/pw_snapshot/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_snapshot/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7359 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_snapshot/processor.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_snapshot/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.886418 pigweed-0.0.8/pw_snapshot_metadata/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_snapshot_metadata/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5012 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_snapshot_metadata/metadata.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_snapshot_metadata/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.886418 pigweed-0.0.8/pw_snapshot_metadata_proto/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_snapshot_metadata_proto/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_snapshot_metadata_proto/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12212 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_snapshot_metadata_proto/snapshot_metadata_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5771 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_snapshot_metadata_proto/snapshot_metadata_pb2.pyi
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.886418 pigweed-0.0.8/pw_snapshot_protos/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_snapshot_protos/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_snapshot_protos/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     8431 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_snapshot_protos/snapshot_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4912 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_snapshot_protos/snapshot_pb2.pyi
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.890418 pigweed-0.0.8/pw_software_update/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      609 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_software_update/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    20910 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_software_update/bundled_update_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    11809 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_software_update/bundled_update_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3726 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_software_update/dev_sign.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    19253 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_software_update/generate_test_bundle.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5899 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_software_update/keys.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2713 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_software_update/metadata.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_software_update/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    17211 2022-04-15 22:03:46.000000 pigweed-0.0.8/pw_software_update/remote_sign.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3744 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_software_update/root_metadata.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    43932 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_software_update/tuf_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    26207 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_software_update/tuf_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     8734 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_software_update/update_bundle.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    15472 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_software_update/update_bundle_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     8946 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_software_update/update_bundle_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    15429 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_software_update/verify.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.890418 pigweed-0.0.8/pw_status/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1093 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_status/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_status/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.890418 pigweed-0.0.8/pw_stm32cube_build/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      647 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_stm32cube_build/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3464 2022-04-06 15:23:57.000000 pigweed-0.0.8/pw_stm32cube_build/__main__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10711 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_stm32cube_build/find_files.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1971 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_stm32cube_build/gen_file_list.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7382 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_stm32cube_build/icf_to_ld.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2300 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_stm32cube_build/inject_init.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_stm32cube_build/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.890418 pigweed-0.0.8/pw_symbolizer/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      784 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_symbolizer/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5768 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_symbolizer/llvm_symbolizer.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:22.000000 pigweed-0.0.8/pw_symbolizer/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3389 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_symbolizer/symbolizer.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.890418 pigweed-0.0.8/pw_system/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      584 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_system/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10439 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_system/console.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7233 2022-04-04 22:22:31.000000 pigweed-0.0.8/pw_system/device.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.894418 pigweed-0.0.8/pw_thread/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_thread/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_thread/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10305 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_thread/thread_analyzer.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.894418 pigweed-0.0.8/pw_thread_protos/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_thread_protos/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_thread_protos/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    13749 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_thread_protos/thread_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10137 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_thread_protos/thread_pb2.pyi
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.894418 pigweed-0.0.8/pw_tls_client/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_tls_client/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     9332 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_tls_client/generate_test_data.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.894418 pigweed-0.0.8/pw_tokenizer/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      721 2020-10-19 22:49:56.000000 pigweed-0.0.8/pw_tokenizer/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      687 2020-10-19 22:49:56.000000 pigweed-0.0.8/pw_tokenizer/__main__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    22632 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_tokenizer/database.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    15325 2022-04-06 15:23:57.000000 pigweed-0.0.8/pw_tokenizer/decode.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    20468 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_tokenizer/detokenize.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    14212 2021-09-29 19:32:08.000000 pigweed-0.0.8/pw_tokenizer/elf_reader.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3105 2021-11-12 01:04:18.000000 pigweed-0.0.8/pw_tokenizer/encode.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5956 2022-04-11 21:01:25.000000 pigweed-0.0.8/pw_tokenizer/parse_message.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.894418 pigweed-0.0.8/pw_tokenizer/proto/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3341 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_tokenizer/proto/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2533 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_tokenizer/proto/options_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1408 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_tokenizer/proto/options_pb2.pyi
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_tokenizer/proto/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_tokenizer/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     3040 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_tokenizer/serial_detokenizer.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    16759 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_tokenizer/tokens.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.894418 pigweed-0.0.8/pw_toolchain/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_toolchain/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     2712 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_toolchain/bad_toolchain.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6681 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_toolchain/clang_arm_toolchain.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6204 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_toolchain/clang_tidy.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     1503 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_toolchain/copy_with_metadata.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_toolchain/py.typed
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.894418 pigweed-0.0.8/pw_trace/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      620 2020-10-19 22:49:56.000000 pigweed-0.0.8/pw_trace/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_trace/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5137 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_trace/trace.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.898418 pigweed-0.0.8/pw_trace_tokenized/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2020-10-19 22:48:37.000000 pigweed-0.0.8/pw_trace_tokenized/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     5942 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_trace_tokenized/get_trace.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_trace_tokenized/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     8017 2022-05-03 00:06:00.000000 pigweed-0.0.8/pw_trace_tokenized/trace_tokenized.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.898418 pigweed-0.0.8/pw_transfer/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      770 2021-12-06 21:17:15.000000 pigweed-0.0.8/pw_transfer/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    14153 2022-04-15 22:03:46.000000 pigweed-0.0.8/pw_transfer/client.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:56.000000 pigweed-0.0.8/pw_transfer/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    19199 2022-04-15 22:03:46.000000 pigweed-0.0.8/pw_transfer/transfer.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12328 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_transfer/transfer_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    10549 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_transfer/transfer_pb2.pyi
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.898418 pigweed-0.0.8/pw_unit_test/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      705 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_unit_test/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_unit_test/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7056 2021-11-10 14:58:28.000000 pigweed-0.0.8/pw_unit_test/rpc.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    12043 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_unit_test/test_runner.py
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.898418 pigweed-0.0.8/pw_unit_test_proto/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_unit_test_proto/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_unit_test_proto/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    18737 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_unit_test_proto/unit_test_pb2.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     7301 2022-05-03 00:15:55.000000 pigweed-0.0.8/pw_unit_test_proto/unit_test_pb2.pyi
-drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-05-03 00:18:39.898418 pigweed-0.0.8/pw_watch/
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2020-10-19 22:49:56.000000 pigweed-0.0.8/pw_watch/__init__.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     6986 2022-03-14 20:54:20.000000 pigweed-0.0.8/pw_watch/debounce.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-09-29 19:32:05.000000 pigweed-0.0.8/pw_watch/py.typed
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    37412 2022-04-04 22:22:31.000000 pigweed-0.0.8/pw_watch/watch.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)    14302 2022-04-19 19:09:55.000000 pigweed-0.0.8/pw_watch/watch_app.py
--rw-r-----   0 tonymd   (372438) primarygroup (89939)      673 2022-05-03 00:17:25.000000 pigweed-0.0.8/pyproject.toml
--rw-r-----   0 tonymd   (372438) primarygroup (89939)     4321 2022-05-03 00:18:39.902418 pigweed-0.0.8/setup.cfg
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.475847 pigweed-0.0.9/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    11358 2022-07-15 20:24:55.000000 pigweed-0.0.9/LICENSE
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1569 2022-07-15 20:26:01.475847 pigweed-0.0.9/PKG-INFO
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      727 2022-07-15 20:24:55.000000 pigweed-0.0.9/README.md
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.435847 pigweed-0.0.9/pigweed.egg-info/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1569 2022-07-15 20:26:01.000000 pigweed-0.0.9/pigweed.egg-info/PKG-INFO
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    11720 2022-07-15 20:26:01.000000 pigweed-0.0.9/pigweed.egg-info/SOURCES.txt
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        1 2022-07-15 20:26:01.000000 pigweed-0.0.9/pigweed.egg-info/dependency_links.txt
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      816 2022-07-15 20:26:01.000000 pigweed-0.0.9/pigweed.egg-info/entry_points.txt
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        1 2022-07-15 20:26:01.000000 pigweed-0.0.9/pigweed.egg-info/not-zip-safe
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      466 2022-07-15 20:26:01.000000 pigweed-0.0.9/pigweed.egg-info/requires.txt
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      707 2022-07-15 20:26:01.000000 pigweed-0.0.9/pigweed.egg-info/top_level.txt
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.435847 pigweed-0.0.9/pw_allocator/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_allocator/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10534 2022-06-30 17:37:54.000000 pigweed-0.0.9/pw_allocator/heap_viewer.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_allocator/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.435847 pigweed-0.0.9/pw_arduino_build/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      652 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    24474 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/__main__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    45446 2021-07-26 18:53:53.000000 pigweed-0.0.9/pw_arduino_build/builder.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    16680 2021-07-26 18:53:53.000000 pigweed-0.0.9/pw_arduino_build/core_installer.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.431847 pigweed-0.0.9/pw_arduino_build/core_patches/
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.439847 pigweed-0.0.9/pw_arduino_build/core_patches/teensy/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2890 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/core_patches/teensy/01-teensyduino_1.53-cpp17.diff
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1501 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/core_patches/teensy/02-teensy4_nonstatic_flash_functions.diff
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     8539 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/file_operations.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1568 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/log.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4430 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/teensy_detector.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1888 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/unit_test_client.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    13528 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_arduino_build/unit_test_runner.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6281 2021-10-06 21:02:26.000000 pigweed-0.0.9/pw_arduino_build/unit_test_server.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.439847 pigweed-0.0.9/pw_bloat/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_bloat/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2973 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_bloat/binary_diff.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6949 2022-04-05 15:22:10.000000 pigweed-0.0.9/pw_bloat/bloat.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6923 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_bloat/bloat_output.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    13633 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_bloat/bloaty_config.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1017 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_bloat/no_bloaty.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1139 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_bloat/no_toolchains.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_bloat/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.439847 pigweed-0.0.9/pw_build/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_build/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6069 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_build/check_python_install_requires.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1959 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_build/collect_wheels.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5129 2022-07-12 20:08:24.000000 pigweed-0.0.9/pw_build/copy_from_cipd.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12490 2022-07-15 20:10:39.000000 pigweed-0.0.9/pw_build/create_python_tree.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2737 2021-03-16 20:40:07.000000 pigweed-0.0.9/pw_build/error.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5002 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_build/exec.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2680 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_build/file_prefix_map.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6756 2022-07-12 20:08:24.000000 pigweed-0.0.9/pw_build/generate_cc_blob_library.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9453 2022-04-25 19:08:54.000000 pigweed-0.0.9/pw_build/generate_modules_lists.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9361 2022-07-15 20:00:23.000000 pigweed-0.0.9/pw_build/generate_python_package.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3555 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_build/generate_python_package_gn.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7538 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_build/generated_tests.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3091 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_build/host_tool.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3843 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_build/mirror_tree.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1161 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_build/nop.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4032 2022-05-02 19:58:49.000000 pigweed-0.0.9/pw_build/pip_install_python_deps.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_build/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7614 2022-07-15 20:00:23.000000 pigweed-0.0.9/pw_build/python_package.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    23153 2022-07-15 20:00:23.000000 pigweed-0.0.9/pw_build/python_runner.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1907 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_build/python_wheels.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5472 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_build/zip.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.439847 pigweed-0.0.9/pw_build_info/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_build_info/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5763 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_build_info/build_id.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_build_info/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.439847 pigweed-0.0.9/pw_build_mcuxpresso/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      644 2021-10-28 18:56:12.000000 pigweed-0.0.9/pw_build_mcuxpresso/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1865 2021-10-28 18:56:12.000000 pigweed-0.0.9/pw_build_mcuxpresso/__main__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    15422 2021-10-28 18:56:12.000000 pigweed-0.0.9/pw_build_mcuxpresso/components.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.443847 pigweed-0.0.9/pw_chrono/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_chrono/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9310 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_chrono/chrono_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7198 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_chrono/chrono_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_chrono/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.443847 pigweed-0.0.9/pw_cli/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_cli/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1644 2021-04-18 15:00:58.000000 pigweed-0.0.9/pw_cli/__main__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1085 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_cli/argument_types.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3128 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_cli/arguments.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2274 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_cli/branding.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2652 2021-10-06 21:02:26.000000 pigweed-0.0.9/pw_cli/color.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3125 2022-05-25 16:52:23.000000 pigweed-0.0.9/pw_cli/env.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6393 2021-09-01 17:26:16.000000 pigweed-0.0.9/pw_cli/envparse.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6315 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_cli/log.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    15395 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_cli/plugins.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3854 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_cli/process.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2649 2021-09-13 19:22:32.000000 pigweed-0.0.9/pw_cli/pw_command_plugins.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_cli/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6288 2022-05-13 19:22:52.000000 pigweed-0.0.9/pw_cli/requires.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.447847 pigweed-0.0.9/pw_console/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      706 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_console/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4960 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_console/__main__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    18469 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_console/command_runner.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    37415 2022-07-15 20:09:33.000000 pigweed-0.0.9/pw_console/console_app.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10326 2022-05-02 19:58:49.000000 pigweed-0.0.9/pw_console/console_prefs.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.447847 pigweed-0.0.9/pw_console/docs/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    32719 2022-05-19 21:29:30.000000 pigweed-0.0.9/pw_console/docs/user_guide.rst
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12302 2022-07-15 20:09:33.000000 pigweed-0.0.9/pw_console/embed.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4418 2021-10-06 21:02:26.000000 pigweed-0.0.9/pw_console/filter_toolbar.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      828 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_console/get_pw_console_app.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12553 2022-07-15 20:09:33.000000 pigweed-0.0.9/pw_console/help_window.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7137 2022-03-16 22:28:00.000000 pigweed-0.0.9/pw_console/key_bindings.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4989 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_console/log_filter.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3584 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_console/log_line.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    26098 2022-03-16 22:28:00.000000 pigweed-0.0.9/pw_console/log_pane.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10694 2022-03-16 22:28:00.000000 pigweed-0.0.9/pw_console/log_pane_saveas_dialog.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6802 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_console/log_pane_selection_dialog.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3298 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_console/log_pane_toolbars.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    27075 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_console/log_screen.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9366 2022-07-15 20:09:33.000000 pigweed-0.0.9/pw_console/log_store.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    31791 2022-05-25 16:52:23.000000 pigweed-0.0.9/pw_console/log_view.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1068 2021-07-26 18:53:53.000000 pigweed-0.0.9/pw_console/mouse.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2487 2022-07-01 22:28:14.000000 pigweed-0.0.9/pw_console/pigweed_code_style.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6012 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_console/plugin_mixin.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.447847 pigweed-0.0.9/pw_console/plugins/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      623 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_console/plugins/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3309 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_console/plugins/bandwidth_toolbar.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     8555 2022-05-19 21:29:30.000000 pigweed-0.0.9/pw_console/plugins/calc_pane.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    17884 2022-05-19 21:29:30.000000 pigweed-0.0.9/pw_console/plugins/clock_pane.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    18689 2022-05-19 21:29:30.000000 pigweed-0.0.9/pw_console/plugins/twenty48_pane.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.447847 pigweed-0.0.9/pw_console/progress_bar/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2370 2021-10-06 21:02:26.000000 pigweed-0.0.9/pw_console/progress_bar/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5321 2021-10-06 21:02:26.000000 pigweed-0.0.9/pw_console/progress_bar/progress_bar_impl.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4633 2021-10-06 21:02:26.000000 pigweed-0.0.9/pw_console/progress_bar/progress_bar_state.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2490 2021-10-06 21:02:26.000000 pigweed-0.0.9/pw_console/progress_bar/progress_bar_task_counter.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12750 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_console/pw_ptpython_repl.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_console/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4166 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_console/pyserial_wrapper.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3947 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_console/python_logging.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5880 2022-04-05 15:22:10.000000 pigweed-0.0.9/pw_console/quit_dialog.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    17447 2022-03-16 22:28:00.000000 pigweed-0.0.9/pw_console/repl_pane.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    16722 2022-03-16 22:28:00.000000 pigweed-0.0.9/pw_console/search_toolbar.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    18974 2022-04-05 15:22:10.000000 pigweed-0.0.9/pw_console/style.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.447847 pigweed-0.0.9/pw_console/templates/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1321 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_console/templates/keybind_list.jinja
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1146 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_console/templates/repl_output.jinja
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     8924 2022-02-10 18:16:11.000000 pigweed-0.0.9/pw_console/text_formatting.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.447847 pigweed-0.0.9/pw_console/widgets/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1040 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_console/widgets/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3873 2022-04-05 15:22:10.000000 pigweed-0.0.9/pw_console/widgets/border.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4829 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_console/widgets/checkbox.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3758 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_console/widgets/event_count_history.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2069 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_console/widgets/mouse_handlers.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10956 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_console/widgets/table.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7297 2022-03-16 21:11:07.000000 pigweed-0.0.9/pw_console/widgets/window_pane.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9307 2022-03-16 21:11:07.000000 pigweed-0.0.9/pw_console/widgets/window_pane_toolbar.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    21676 2022-03-16 21:11:07.000000 pigweed-0.0.9/pw_console/window_list.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    40473 2022-03-16 22:28:00.000000 pigweed-0.0.9/pw_console/window_manager.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5942 2022-03-16 22:28:00.000000 pigweed-0.0.9/pw_console/yaml_config_loader_mixin.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.451847 pigweed-0.0.9/pw_cpu_exception_cortex_m/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      745 2021-08-13 23:33:50.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1941 2021-04-18 15:00:58.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m/cfsr_decoder.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    11072 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m/cortex_m_constants.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7840 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m/exception_analyzer.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.451847 pigweed-0.0.9/pw_cpu_exception_cortex_m_protos/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m_protos/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    16111 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m_protos/cpu_state_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5682 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m_protos/cpu_state_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_cpu_exception_cortex_m_protos/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.451847 pigweed-0.0.9/pw_docgen/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_docgen/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6288 2022-07-01 21:44:56.000000 pigweed-0.0.9/pw_docgen/docgen.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_docgen/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.451847 pigweed-0.0.9/pw_docgen/sphinx/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_docgen/sphinx/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1466 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_docgen/sphinx/google_analytics.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.451847 pigweed-0.0.9/pw_doctor/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_doctor/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    15383 2022-07-01 17:16:49.000000 pigweed-0.0.9/pw_doctor/doctor.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_doctor/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.451847 pigweed-0.0.9/pw_env_setup/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      617 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_env_setup/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2749 2021-03-16 20:40:07.000000 pigweed-0.0.9/pw_env_setup/apply_visitor.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4545 2021-03-16 20:40:07.000000 pigweed-0.0.9/pw_env_setup/batch_visitor.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.451847 pigweed-0.0.9/pw_env_setup/cipd_setup/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      584 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_env_setup/cipd_setup/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2113 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_env_setup/cipd_setup/luci.json
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4919 2022-07-12 20:08:24.000000 pigweed-0.0.9/pw_env_setup/cipd_setup/pigweed.json
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12172 2022-05-25 16:52:23.000000 pigweed-0.0.9/pw_env_setup/cipd_setup/update.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    11917 2022-05-25 16:52:23.000000 pigweed-0.0.9/pw_env_setup/cipd_setup/wrapper.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1399 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_env_setup/colors.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    27271 2022-07-12 20:08:06.000000 pigweed-0.0.9/pw_env_setup/env_setup.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    15501 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_env_setup/environment.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3001 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_env_setup/gni_visitor.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3147 2021-03-16 20:40:07.000000 pigweed-0.0.9/pw_env_setup/json_visitor.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_env_setup/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9623 2022-07-12 20:08:06.000000 pigweed-0.0.9/pw_env_setup/python_packages.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6987 2021-07-26 18:53:53.000000 pigweed-0.0.9/pw_env_setup/shell_visitor.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2194 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_env_setup/spinner.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.451847 pigweed-0.0.9/pw_env_setup/virtualenv_setup/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      713 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_env_setup/virtualenv_setup/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2505 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_env_setup/virtualenv_setup/__main__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12469 2022-07-12 20:08:06.000000 pigweed-0.0.9/pw_env_setup/virtualenv_setup/install.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1909 2022-07-12 19:42:43.000000 pigweed-0.0.9/pw_env_setup/virtualenv_setup/requirements.txt
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2955 2021-03-16 20:40:07.000000 pigweed-0.0.9/pw_env_setup/windows_env_start.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_hdlc/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_hdlc/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6271 2022-05-19 21:29:30.000000 pigweed-0.0.9/pw_hdlc/decode.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1192 2022-05-19 21:29:30.000000 pigweed-0.0.9/pw_hdlc/encode.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2215 2021-04-18 15:00:58.000000 pigweed-0.0.9/pw_hdlc/protocol.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_hdlc/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10365 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_hdlc/rpc.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10282 2022-07-15 20:10:39.000000 pigweed-0.0.9/pw_hdlc/rpc_console.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_log/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_log/__init__.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_log/proto/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_log/proto/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    25536 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_log/proto/log_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    14212 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_log/proto/log_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_log/proto/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_log/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_log_tokenized/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2722 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_log_tokenized/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-03-16 20:40:07.000000 pigweed-0.0.9/pw_log_tokenized/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_metric/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      584 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_metric/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2830 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_metric/metric_parser.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_metric/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_metric_proto/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_metric_proto/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7602 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_metric_proto/metric_service_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4270 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_metric_proto/metric_service_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_metric_proto/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_module/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_module/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7107 2021-08-14 18:01:36.000000 pigweed-0.0.9/pw_module/check.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_module/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_package/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_package/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5020 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_package/git_repo.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6156 2021-05-05 01:25:46.000000 pigweed-0.0.9/pw_package/package_manager.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.455847 pigweed-0.0.9/pw_package/packages/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      584 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_package/packages/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5318 2021-05-05 01:25:46.000000 pigweed-0.0.9/pw_package/packages/arduino_core.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2720 2021-07-26 18:53:53.000000 pigweed-0.0.9/pw_package/packages/boringssl.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5808 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_package/packages/chromium_verifier.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3104 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_package/packages/crlset.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1439 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_package/packages/freertos.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1444 2022-04-05 15:22:10.000000 pigweed-0.0.9/pw_package/packages/googletest.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1558 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_package/packages/mbedtls.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1599 2021-09-01 17:26:16.000000 pigweed-0.0.9/pw_package/packages/micro_ecc.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1377 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_package/packages/nanopb.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1456 2022-04-05 15:22:10.000000 pigweed-0.0.9/pw_package/packages/pico_sdk.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1443 2021-09-27 20:02:53.000000 pigweed-0.0.9/pw_package/packages/protobuf.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1476 2022-05-25 16:52:23.000000 pigweed-0.0.9/pw_package/packages/smartfusion_mss.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4795 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_package/packages/stm32cube.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1875 2022-04-07 18:33:10.000000 pigweed-0.0.9/pw_package/pigweed_packages.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_package/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.459847 pigweed-0.0.9/pw_presubmit/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      745 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_presubmit/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12382 2022-07-01 17:16:49.000000 pigweed-0.0.9/pw_presubmit/build.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7487 2022-05-19 21:29:30.000000 pigweed-0.0.9/pw_presubmit/cli.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1989 2021-12-08 01:19:16.000000 pigweed-0.0.9/pw_presubmit/cpp_checks.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    18594 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_presubmit/format_code.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    11610 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_presubmit/git_repo.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5168 2021-10-28 18:56:12.000000 pigweed-0.0.9/pw_presubmit/inclusive_language.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6055 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_presubmit/install_hook.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      885 2022-07-12 20:08:24.000000 pigweed-0.0.9/pw_presubmit/npm_presubmit.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    29909 2022-07-12 20:08:24.000000 pigweed-0.0.9/pw_presubmit/pigweed_presubmit.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    23281 2022-07-15 20:10:39.000000 pigweed-0.0.9/pw_presubmit/presubmit.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_presubmit/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6025 2022-07-06 20:25:30.000000 pigweed-0.0.9/pw_presubmit/python_checks.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1252 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_presubmit/shell_checks.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6182 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_presubmit/tools.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.459847 pigweed-0.0.9/pw_protobuf/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_protobuf/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    76756 2022-06-30 17:37:54.000000 pigweed-0.0.9/pw_protobuf/codegen_pwpb.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2801 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_protobuf/options.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2288 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_protobuf/output_file.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3506 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_protobuf/plugin.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    20903 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_protobuf/proto_tree.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_protobuf/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12923 2022-07-06 19:01:24.000000 pigweed-0.0.9/pw_protobuf/symbol_name_mapping.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.459847 pigweed-0.0.9/pw_protobuf_codegen_protos/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_codegen_protos/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3907 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_codegen_protos/options_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1562 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_codegen_protos/options_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_codegen_protos/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.459847 pigweed-0.0.9/pw_protobuf_compiler/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_protobuf_compiler/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6934 2022-04-28 18:27:47.000000 pigweed-0.0.9/pw_protobuf_compiler/generate_protos.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2163 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_protobuf_compiler/proto_target_invalid.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_protobuf_compiler/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    15359 2022-07-01 20:59:32.000000 pigweed-0.0.9/pw_protobuf_compiler/python_protos.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.459847 pigweed-0.0.9/pw_protobuf_compiler_protos/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/__init__.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.459847 pigweed-0.0.9/pw_protobuf_compiler_protos/nested/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/nested/__init__.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.459847 pigweed-0.0.9/pw_protobuf_compiler_protos/nested/more_nesting/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/nested/more_nesting/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/nested/more_nesting/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2219 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/nested/more_nesting/test_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      635 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/nested/more_nesting/test_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/nested/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1811 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/test_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      639 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_compiler_protos/test_pb2.pyi
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.463847 pigweed-0.0.9/pw_protobuf_protos/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_protos/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1583 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_protos/common_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      378 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_protos/common_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_protos/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5385 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_protos/status_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1798 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_protobuf_protos/status_pb2.pyi
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.463847 pigweed-0.0.9/pw_rpc/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      863 2022-05-02 19:58:49.000000 pigweed-0.0.9/pw_rpc/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3092 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/benchmark_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      649 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/benchmark_pb2.pyi
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.463847 pigweed-0.0.9/pw_rpc/callback_client/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4106 2021-08-16 23:22:22.000000 pigweed-0.0.9/pw_rpc/callback_client/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12055 2021-09-13 19:22:32.000000 pigweed-0.0.9/pw_rpc/callback_client/call.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1489 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_rpc/callback_client/errors.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    18013 2021-09-13 19:22:32.000000 pigweed-0.0.9/pw_rpc/callback_client/impl.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/callback_client/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    21158 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_rpc/client.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    17802 2022-04-29 17:32:33.000000 pigweed-0.0.9/pw_rpc/codegen.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10059 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_rpc/codegen_nanopb.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9579 2022-04-28 18:27:47.000000 pigweed-0.0.9/pw_rpc/codegen_pwpb.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7508 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_rpc/codegen_raw.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.463847 pigweed-0.0.9/pw_rpc/console_tools/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      969 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_rpc/console_tools/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12026 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_rpc/console_tools/console.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3033 2021-04-18 15:00:58.000000 pigweed-0.0.9/pw_rpc/console_tools/functions.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/console_tools/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3059 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_rpc/console_tools/watchdog.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    14830 2022-04-07 18:33:10.000000 pigweed-0.0.9/pw_rpc/descriptors.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2880 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/echo_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      649 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/echo_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1238 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_rpc/ids.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.463847 pigweed-0.0.9/pw_rpc/internal/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/internal/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7701 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/internal/packet_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4694 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/internal/packet_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/internal/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     8781 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_rpc/lossy_channel.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3568 2021-10-28 18:56:12.000000 pigweed-0.0.9/pw_rpc/packets.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2781 2022-04-28 18:27:47.000000 pigweed-0.0.9/pw_rpc/plugin.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      798 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_rpc/plugin_nanopb.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      801 2022-04-28 18:27:47.000000 pigweed-0.0.9/pw_rpc/plugin_pwpb.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      792 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_rpc/plugin_raw.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_rpc/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3761 2022-07-01 17:16:49.000000 pigweed-0.0.9/pw_rpc/testing.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.467847 pigweed-0.0.9/pw_snapshot/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-07-26 18:53:53.000000 pigweed-0.0.9/pw_snapshot/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7359 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_snapshot/processor.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.467847 pigweed-0.0.9/pw_snapshot_metadata/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-07-26 18:53:53.000000 pigweed-0.0.9/pw_snapshot_metadata/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5012 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_snapshot_metadata/metadata.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_metadata/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.467847 pigweed-0.0.9/pw_snapshot_metadata_proto/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_metadata_proto/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_metadata_proto/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12212 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_metadata_proto/snapshot_metadata_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6052 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_metadata_proto/snapshot_metadata_pb2.pyi
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.467847 pigweed-0.0.9/pw_snapshot_protos/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_protos/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_protos/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9134 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_protos/snapshot_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5425 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_snapshot_protos/snapshot_pb2.pyi
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.467847 pigweed-0.0.9/pw_software_update/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      609 2021-09-21 18:33:47.000000 pigweed-0.0.9/pw_software_update/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    20910 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_software_update/bundled_update_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    11809 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_software_update/bundled_update_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3726 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_software_update/dev_sign.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    19257 2022-06-30 17:37:54.000000 pigweed-0.0.9/pw_software_update/generate_test_bundle.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5899 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_software_update/keys.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2713 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_software_update/metadata.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_software_update/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    17211 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_software_update/remote_sign.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3744 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_software_update/root_metadata.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    43932 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_software_update/tuf_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    26207 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_software_update/tuf_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     8734 2022-02-07 18:07:34.000000 pigweed-0.0.9/pw_software_update/update_bundle.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    15472 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_software_update/update_bundle_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     8946 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_software_update/update_bundle_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    15429 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_software_update/verify.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.467847 pigweed-0.0.9/pw_status/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1093 2021-08-19 14:35:30.000000 pigweed-0.0.9/pw_status/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_status/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.467847 pigweed-0.0.9/pw_stm32cube_build/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      647 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_stm32cube_build/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3464 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_stm32cube_build/__main__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10711 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_stm32cube_build/find_files.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1971 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_stm32cube_build/gen_file_list.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7382 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_stm32cube_build/icf_to_ld.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2300 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_stm32cube_build/inject_init.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_stm32cube_build/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_symbolizer/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      784 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_symbolizer/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5768 2021-12-01 21:42:56.000000 pigweed-0.0.9/pw_symbolizer/llvm_symbolizer.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:31.000000 pigweed-0.0.9/pw_symbolizer/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3389 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_symbolizer/symbolizer.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_system/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      584 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_system/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    11688 2022-07-15 20:10:39.000000 pigweed-0.0.9/pw_system/console.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     8226 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_system/device.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_thread/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_thread/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_thread/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10305 2022-03-16 18:45:01.000000 pigweed-0.0.9/pw_thread/thread_analyzer.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_thread_protos/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_thread_protos/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_thread_protos/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    13749 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_thread_protos/thread_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    10137 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_thread_protos/thread_pb2.pyi
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_tls_client/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-07-27 23:39:16.000000 pigweed-0.0.9/pw_tls_client/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     9330 2022-06-30 17:37:54.000000 pigweed-0.0.9/pw_tls_client/generate_test_data.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_tokenizer/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      721 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_tokenizer/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      687 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_tokenizer/__main__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    22632 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_tokenizer/database.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    15325 2022-04-07 18:33:10.000000 pigweed-0.0.9/pw_tokenizer/decode.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    20468 2022-04-29 00:06:10.000000 pigweed-0.0.9/pw_tokenizer/detokenize.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    14212 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_tokenizer/elf_reader.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5035 2022-07-12 20:08:24.000000 pigweed-0.0.9/pw_tokenizer/encode.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5956 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_tokenizer/parse_message.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_tokenizer/proto/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3341 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_tokenizer/proto/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2533 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_tokenizer/proto/options_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1410 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_tokenizer/proto/options_pb2.pyi
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_tokenizer/proto/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_tokenizer/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     3040 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_tokenizer/serial_detokenizer.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    16759 2022-01-21 01:23:21.000000 pigweed-0.0.9/pw_tokenizer/tokens.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_toolchain/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_toolchain/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     2712 2021-03-16 20:40:07.000000 pigweed-0.0.9/pw_toolchain/bad_toolchain.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6681 2021-06-21 16:53:22.000000 pigweed-0.0.9/pw_toolchain/clang_arm_toolchain.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6294 2022-06-30 17:37:54.000000 pigweed-0.0.9/pw_toolchain/clang_tidy.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     1503 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_toolchain/copy_with_metadata.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_toolchain/py.typed
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_trace/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      620 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_trace/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_trace/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5137 2021-07-26 18:53:53.000000 pigweed-0.0.9/pw_trace/trace.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.471847 pigweed-0.0.9/pw_trace_tokenized/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_trace_tokenized/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     5942 2022-07-15 20:10:39.000000 pigweed-0.0.9/pw_trace_tokenized/get_trace.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_trace_tokenized/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     8017 2022-04-28 18:26:58.000000 pigweed-0.0.9/pw_trace_tokenized/trace_tokenized.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.475847 pigweed-0.0.9/pw_transfer/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      770 2021-10-28 18:56:12.000000 pigweed-0.0.9/pw_transfer/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    14574 2022-07-01 20:59:32.000000 pigweed-0.0.9/pw_transfer/client.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_transfer/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    19978 2022-06-23 18:48:08.000000 pigweed-0.0.9/pw_transfer/transfer.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    14022 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_transfer/transfer_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12813 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_transfer/transfer_pb2.pyi
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.475847 pigweed-0.0.9/pw_unit_test/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      705 2021-08-13 20:13:24.000000 pigweed-0.0.9/pw_unit_test/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_unit_test/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7056 2021-08-16 15:58:52.000000 pigweed-0.0.9/pw_unit_test/rpc.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    12043 2022-02-04 21:46:50.000000 pigweed-0.0.9/pw_unit_test/test_runner.py
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.475847 pigweed-0.0.9/pw_unit_test_proto/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)       91 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_unit_test_proto/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_unit_test_proto/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    18737 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_unit_test_proto/unit_test_pb2.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     7301 2022-07-15 20:24:53.000000 pigweed-0.0.9/pw_unit_test_proto/unit_test_pb2.pyi
+drwxr-x---   0 tonymd   (372438) primarygroup (89939)        0 2022-07-15 20:26:01.475847 pigweed-0.0.9/pw_watch/
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_watch/__init__.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     6986 2022-03-16 18:45:07.000000 pigweed-0.0.9/pw_watch/debounce.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)        0 2021-02-02 19:12:39.000000 pigweed-0.0.9/pw_watch/py.typed
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    37878 2022-07-01 20:59:32.000000 pigweed-0.0.9/pw_watch/watch.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)    14302 2022-04-15 22:05:45.000000 pigweed-0.0.9/pw_watch/watch_app.py
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)      673 2022-07-15 20:24:55.000000 pigweed-0.0.9/pyproject.toml
+-rw-r-----   0 tonymd   (372438) primarygroup (89939)     4532 2022-07-15 20:26:01.475847 pigweed-0.0.9/setup.cfg
```

### Comparing `pigweed-0.0.8/LICENSE` & `pigweed-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/PKG-INFO` & `pigweed-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pigweed
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pigweed Python modules
 Home-page: https://pigweed.dev
 Author: Pigweed Authors
 Author-email: pigweed-developers@googlegroups.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://bugs.chromium.org/p/pigweed/issues/list
-Project-URL: Code Search, https://cs.opensource.google/pigweed/pigweed
-Project-URL: Gerrit, https://pigweed-review.googlesource.com
-Platform: UNKNOWN
+Project-URL: Documentation, https://pigweed.dev
+Project-URL: Source Code, https://cs.opensource.google/pigweed/pigweed
+Project-URL: Code Reviews, https://pigweed-review.googlesource.com
+Project-URL: Mailing List, https://groups.google.com/g/pigweed
+Project-URL: Issue Tracker, https://bugs.pigweed.dev
+Project-URL: Chat, https://discord.gg/M9NSeTA
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,20 +23,18 @@
 
 Pigweed is an open source collection of embedded-targeted libraries–or as we
 like to call them, modules. These modules are building blocks and infrastructure
 that enable faster and more reliable development on small-footprint MMU-less
 32-bit microcontrollers like the STMicroelectronics STM32L452 or the Nordic
 nRF52832.
 
-For more information please see our website: https://pigweed.dev/
+For more information please see our website: https://pigweed.dev/.
 
 ## Links
 
 - [Documentation](https://pigweed.dev/)
 - [Source Code](https://cs.opensource.google/pigweed/pigweed)
 - [Code Reviews](https://pigweed-review.googlesource.com)
 - [Mailing List](https://groups.google.com/forum/#!forum/pigweed)
 - [Chat Room](https://discord.gg/M9NSeTA)
 - [Issue Tracker](https://bugs.pigweed.dev/)
 
-
-
```

### Comparing `pigweed-0.0.8/README.md` & `pigweed-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Pigweed is an open source collection of embedded-targeted libraries–or as we
 like to call them, modules. These modules are building blocks and infrastructure
 that enable faster and more reliable development on small-footprint MMU-less
 32-bit microcontrollers like the STMicroelectronics STM32L452 or the Nordic
 nRF52832.
 
-For more information please see our website: https://pigweed.dev/
+For more information please see our website: https://pigweed.dev/.
 
 ## Links
 
 - [Documentation](https://pigweed.dev/)
 - [Source Code](https://cs.opensource.google/pigweed/pigweed)
 - [Code Reviews](https://pigweed-review.googlesource.com)
 - [Mailing List](https://groups.google.com/forum/#!forum/pigweed)
```

### Comparing `pigweed-0.0.8/pigweed.egg-info/PKG-INFO` & `pigweed-0.0.9/pigweed.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pigweed
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pigweed Python modules
 Home-page: https://pigweed.dev
 Author: Pigweed Authors
 Author-email: pigweed-developers@googlegroups.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://bugs.chromium.org/p/pigweed/issues/list
-Project-URL: Code Search, https://cs.opensource.google/pigweed/pigweed
-Project-URL: Gerrit, https://pigweed-review.googlesource.com
-Platform: UNKNOWN
+Project-URL: Documentation, https://pigweed.dev
+Project-URL: Source Code, https://cs.opensource.google/pigweed/pigweed
+Project-URL: Code Reviews, https://pigweed-review.googlesource.com
+Project-URL: Mailing List, https://groups.google.com/g/pigweed
+Project-URL: Issue Tracker, https://bugs.pigweed.dev
+Project-URL: Chat, https://discord.gg/M9NSeTA
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,20 +23,18 @@
 
 Pigweed is an open source collection of embedded-targeted libraries–or as we
 like to call them, modules. These modules are building blocks and infrastructure
 that enable faster and more reliable development on small-footprint MMU-less
 32-bit microcontrollers like the STMicroelectronics STM32L452 or the Nordic
 nRF52832.
 
-For more information please see our website: https://pigweed.dev/
+For more information please see our website: https://pigweed.dev/.
 
 ## Links
 
 - [Documentation](https://pigweed.dev/)
 - [Source Code](https://cs.opensource.google/pigweed/pigweed)
 - [Code Reviews](https://pigweed-review.googlesource.com)
 - [Mailing List](https://groups.google.com/forum/#!forum/pigweed)
 - [Chat Room](https://discord.gg/M9NSeTA)
 - [Issue Tracker](https://bugs.pigweed.dev/)
 
-
-
```

### Comparing `pigweed-0.0.8/pigweed.egg-info/SOURCES.txt` & `pigweed-0.0.9/pigweed.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 pw_bloat/bloat.py
 pw_bloat/bloat_output.py
 pw_bloat/bloaty_config.py
 pw_bloat/no_bloaty.py
 pw_bloat/no_toolchains.py
 pw_bloat/py.typed
 pw_build/__init__.py
+pw_build/check_python_install_requires.py
 pw_build/collect_wheels.py
 pw_build/copy_from_cipd.py
 pw_build/create_python_tree.py
 pw_build/error.py
 pw_build/exec.py
 pw_build/file_prefix_map.py
 pw_build/generate_cc_blob_library.py
@@ -56,14 +57,18 @@
 pw_build/zip.py
 pw_build_info/__init__.py
 pw_build_info/build_id.py
 pw_build_info/py.typed
 pw_build_mcuxpresso/__init__.py
 pw_build_mcuxpresso/__main__.py
 pw_build_mcuxpresso/components.py
+pw_chrono/__init__.py
+pw_chrono/chrono_pb2.py
+pw_chrono/chrono_pb2.pyi
+pw_chrono/py.typed
 pw_cli/__init__.py
 pw_cli/__main__.py
 pw_cli/argument_types.py
 pw_cli/arguments.py
 pw_cli/branding.py
 pw_cli/color.py
 pw_cli/env.py
@@ -162,14 +167,15 @@
 pw_env_setup/cipd_setup/luci.json
 pw_env_setup/cipd_setup/pigweed.json
 pw_env_setup/cipd_setup/update.py
 pw_env_setup/cipd_setup/wrapper.py
 pw_env_setup/virtualenv_setup/__init__.py
 pw_env_setup/virtualenv_setup/__main__.py
 pw_env_setup/virtualenv_setup/install.py
+pw_env_setup/virtualenv_setup/requirements.txt
 pw_hdlc/__init__.py
 pw_hdlc/decode.py
 pw_hdlc/encode.py
 pw_hdlc/protocol.py
 pw_hdlc/py.typed
 pw_hdlc/rpc.py
 pw_hdlc/rpc_console.py
@@ -177,14 +183,21 @@
 pw_log/py.typed
 pw_log/proto/__init__.py
 pw_log/proto/log_pb2.py
 pw_log/proto/log_pb2.pyi
 pw_log/proto/py.typed
 pw_log_tokenized/__init__.py
 pw_log_tokenized/py.typed
+pw_metric/__init__.py
+pw_metric/metric_parser.py
+pw_metric/py.typed
+pw_metric_proto/__init__.py
+pw_metric_proto/metric_service_pb2.py
+pw_metric_proto/metric_service_pb2.pyi
+pw_metric_proto/py.typed
 pw_module/__init__.py
 pw_module/check.py
 pw_module/py.typed
 pw_package/__init__.py
 pw_package/git_repo.py
 pw_package/package_manager.py
 pw_package/pigweed_packages.py
@@ -207,26 +220,29 @@
 pw_presubmit/build.py
 pw_presubmit/cli.py
 pw_presubmit/cpp_checks.py
 pw_presubmit/format_code.py
 pw_presubmit/git_repo.py
 pw_presubmit/inclusive_language.py
 pw_presubmit/install_hook.py
+pw_presubmit/npm_presubmit.py
 pw_presubmit/pigweed_presubmit.py
 pw_presubmit/presubmit.py
 pw_presubmit/py.typed
 pw_presubmit/python_checks.py
+pw_presubmit/shell_checks.py
 pw_presubmit/tools.py
 pw_protobuf/__init__.py
 pw_protobuf/codegen_pwpb.py
 pw_protobuf/options.py
 pw_protobuf/output_file.py
 pw_protobuf/plugin.py
 pw_protobuf/proto_tree.py
 pw_protobuf/py.typed
+pw_protobuf/symbol_name_mapping.py
 pw_protobuf_codegen_protos/__init__.py
 pw_protobuf_codegen_protos/options_pb2.py
 pw_protobuf_codegen_protos/options_pb2.pyi
 pw_protobuf_codegen_protos/py.typed
 pw_protobuf_compiler/__init__.py
 pw_protobuf_compiler/generate_protos.py
 pw_protobuf_compiler/proto_target_invalid.py
```

### Comparing `pigweed-0.0.8/pigweed.egg-info/entry_points.txt` & `pigweed-0.0.9/pigweed.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pigweed.egg-info/top_level.txt` & `pigweed-0.0.9/pigweed.egg-info/top_level.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 pw_allocator
 pw_arduino_build
 pw_bloat
 pw_build
 pw_build_info
 pw_build_mcuxpresso
+pw_chrono
 pw_cli
 pw_console
 pw_cpu_exception_cortex_m
 pw_cpu_exception_cortex_m_protos
 pw_docgen
 pw_doctor
 pw_env_setup
 pw_hdlc
 pw_log
 pw_log_tokenized
+pw_metric
+pw_metric_proto
 pw_module
 pw_package
 pw_presubmit
 pw_protobuf
 pw_protobuf_codegen_protos
 pw_protobuf_compiler
 pw_protobuf_compiler_protos
```

### Comparing `pigweed-0.0.8/pw_allocator/heap_viewer.py` & `pigweed-0.0.9/pw_allocator/heap_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,16 @@
 
 def visualize(dump_file=None,
               heap_low_address=None,
               heap_high_address=None,
               poison_enabled=False,
               pointer_size=4):
     """Visualization of heap usage."""
-    # TODO(pwbug/236): Add standarized mechanisms to produce dump file and read
-    # heap information from dump file.
+    # TODO(b/235282507): Add standarized mechanisms to produce dump file and
+    # read heap information from dump file.
     aligned_bytes = pointer_size
     header_size = pointer_size * 2
 
     try:
         if heap_high_address < heap_low_address:
             _exit_due_to_bad_heap_info()
         heap_size = heap_high_address - heap_low_address
```

### Comparing `pigweed-0.0.8/pw_arduino_build/__init__.py` & `pigweed-0.0.9/pw_arduino_build/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/__main__.py` & `pigweed-0.0.9/pw_arduino_build/__main__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/builder.py` & `pigweed-0.0.9/pw_arduino_build/builder.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/core_installer.py` & `pigweed-0.0.9/pw_arduino_build/core_installer.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/core_patches/teensy/01-teensyduino_1.53-cpp17.diff` & `pigweed-0.0.9/pw_arduino_build/core_patches/teensy/01-teensyduino_1.53-cpp17.diff`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/core_patches/teensy/02-teensy4_nonstatic_flash_functions.diff` & `pigweed-0.0.9/pw_arduino_build/core_patches/teensy/02-teensy4_nonstatic_flash_functions.diff`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/file_operations.py` & `pigweed-0.0.9/pw_arduino_build/file_operations.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/log.py` & `pigweed-0.0.9/pw_arduino_build/log.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/teensy_detector.py` & `pigweed-0.0.9/pw_arduino_build/teensy_detector.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/unit_test_client.py` & `pigweed-0.0.9/pw_arduino_build/unit_test_client.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/unit_test_runner.py` & `pigweed-0.0.9/pw_arduino_build/unit_test_runner.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_arduino_build/unit_test_server.py` & `pigweed-0.0.9/pw_arduino_build/unit_test_server.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_bloat/binary_diff.py` & `pigweed-0.0.9/pw_bloat/binary_diff.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_bloat/bloat.py` & `pigweed-0.0.9/pw_bloat/bloat.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_bloat/bloat_output.py` & `pigweed-0.0.9/pw_bloat/bloat_output.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_bloat/bloaty_config.py` & `pigweed-0.0.9/pw_bloat/bloaty_config.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_bloat/no_bloaty.py` & `pigweed-0.0.9/pw_bloat/no_bloaty.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_bloat/no_toolchains.py` & `pigweed-0.0.9/pw_bloat/no_toolchains.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/collect_wheels.py` & `pigweed-0.0.9/pw_build/collect_wheels.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/copy_from_cipd.py` & `pigweed-0.0.9/pw_build/copy_from_cipd.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,18 +88,15 @@
     base_package_name = os.path.basename(package_name)
     instance_id_path = os.path.join(cipd_path, '.versions',
                                     f'{base_package_name}.cipd_version')
     with open(instance_id_path, 'r') as ins:
         instance_id = json.load(ins)['instance_id']
 
     with open(manifest, 'r') as ins:
-        data = json.load(ins)
-    # TODO(pwbug/599) Always assume this is a dict.
-    if isinstance(data, dict):
-        data = data['packages']
+        data = json.load(ins)['packages']
 
     path = None
     expected_version = None
     for entry in data:
         if package_name in entry['path']:
             path = entry['path']
             expected_version = entry['tags'][0]
```

### Comparing `pigweed-0.0.8/pw_build/create_python_tree.py` & `pigweed-0.0.9/pw_build/create_python_tree.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/error.py` & `pigweed-0.0.9/pw_build/error.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/exec.py` & `pigweed-0.0.9/pw_build/exec.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/file_prefix_map.py` & `pigweed-0.0.9/pw_build/file_prefix_map.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/generate_cc_blob_library.py` & `pigweed-0.0.9/pw_build/generate_cc_blob_library.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,87 +15,103 @@
 
 import argparse
 import itertools
 import json
 from pathlib import Path
 from string import Template
 import textwrap
-from typing import Any, Generator, Iterable, NamedTuple, Optional, Tuple
+from typing import (Any, Generator, Iterable, NamedTuple, Optional, Sequence,
+                    Tuple)
 
-HEADER_PREFIX = textwrap.dedent("""\
-    // This file is auto-generated; Do not hand-modify!
-    // See https://pigweed.dev/pw_build/#pw-cc-blob-library for details.
+COMMENT = f"""\
+// This file was generated by {Path(__file__).name}.
+//
+// DO NOT EDIT!
+//
+// This file contains declarations for byte arrays created from files during the
+// build. The byte arrays are constant initialized and are safe to access at any
+// time, including before main().
+//
+// See https://pigweed.dev/pw_build/#pw-cc-blob-library for details.
+"""
 
+HEADER_PREFIX = COMMENT + textwrap.dedent("""\
     #pragma once
 
     #include <array>
     #include <cstddef>
+
     """)
 
-SOURCE_PREFIX_TEMPLATE = Template(
-    textwrap.dedent("""\
-        // This file is auto-generated; Do not hand-modify!
-        // See https://pigweed.dev/pw_build/#pw-cc-blob-library for details.
+SOURCE_PREFIX_TEMPLATE = Template(COMMENT + textwrap.dedent("""\
 
         #include "$header_path"
 
         #include <array>
         #include <cstddef>
 
         #include "pw_preprocessor/compiler.h"
+
         """))
 
 NAMESPACE_OPEN_TEMPLATE = Template('namespace ${namespace} {\n')
 
-NAMESPACE_CLOSE_TEMPLATE = Template('}  // namespace ${namespace}\n')
+NAMESPACE_CLOSE_TEMPLATE = Template('\n}  // namespace ${namespace}\n')
 
 BLOB_DECLARATION_TEMPLATE = Template(
-    'extern const std::array<std::byte, ${size_bytes}> ${symbol_name};')
-
-LINKER_SECTION_TEMPLATE = Template('PW_PLACE_IN_SECTION("${linker_section}")')
+    '\nextern const std::array<std::byte, ${size_bytes}> ${symbol_name};\n')
 
-BLOB_DEFINITION_SINGLE_LINE = Template(
-    'const std::array<std::byte, ${size_bytes}> ${symbol_name}'
-    ' = { $bytes };')
+LINKER_SECTION_TEMPLATE = Template(
+    'PW_PLACE_IN_SECTION("${linker_section}")\n')
 
 BLOB_DEFINITION_MULTI_LINE = Template(
-    'const std::array<std::byte, ${size_bytes}> ${symbol_name}'
-    ' = {\n${bytes_lines}\n};')
+    '\n${section_attr}'
+    '${alignas}constexpr std::array<std::byte, ${size_bytes}> ${symbol_name}'
+    ' = {\n${bytes_lines}\n};\n')
 
 BYTES_PER_LINE = 4
 
 
 class Blob(NamedTuple):
     symbol_name: str
     file_path: Path
     linker_section: Optional[str]
+    alignas: Optional[str] = None
 
+    @staticmethod
+    def from_dict(blob_dict: dict) -> 'Blob':
+        return Blob(blob_dict['symbol_name'], Path(blob_dict['file_path']),
+                    blob_dict.get('linker_section'), blob_dict.get('alignas'))
 
-def parse_args():
+
+def parse_args() -> dict:
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument('--blob-file',
                         type=Path,
                         required=True,
                         help=('Path to json file containing the list of blobs '
                               'to generate.'))
+    parser.add_argument('--header-include',
+                        required=True,
+                        help='Path to use in #includes for the header')
     parser.add_argument('--out-source',
                         type=Path,
                         required=True,
                         help='Path at which to write .cpp file')
     parser.add_argument('--out-header',
                         type=Path,
                         required=True,
                         help='Path at which to write .h file')
     parser.add_argument('--namespace',
                         type=str,
                         required=False,
                         help=('Optional namespace that blobs will be scoped'
                               'within.'))
 
-    return parser.parse_args()
+    return vars(parser.parse_args())
 
 
 def split_into_chunks(
         data: Iterable[Any],
         chunk_size: int) -> Generator[Tuple[Any, ...], None, None]:
     """Splits an iterable into chunks of a given size."""
     data_iterator = iter(data)
@@ -112,79 +128,73 @@
     if namespace:
         lines.append(NAMESPACE_OPEN_TEMPLATE.substitute(namespace=namespace))
     for blob in blobs:
         data = blob.file_path.read_bytes()
         lines.append(
             BLOB_DECLARATION_TEMPLATE.substitute(symbol_name=blob.symbol_name,
                                                  size_bytes=len(data)))
-        lines.append('')
     if namespace:
         lines.append(NAMESPACE_CLOSE_TEMPLATE.substitute(namespace=namespace))
 
-    return '\n'.join(lines)
+    return ''.join(lines)
 
 
-def array_def_from_blob_data(symbol_name: str, blob_data: bytes) -> str:
+def array_def_from_blob_data(blob: Blob, blob_data: bytes) -> str:
     """Generates an array definition for the given blob data."""
-    byte_strs = ['std::byte{{0x{:02X}}}'.format(b) for b in blob_data]
+    if blob.linker_section:
+        section_attr = LINKER_SECTION_TEMPLATE.substitute(
+            linker_section=blob.linker_section)
+    else:
+        section_attr = ''
 
-    # Try to fit the blob definition on a single line first.
-    single_line_def = BLOB_DEFINITION_SINGLE_LINE.substitute(
-        symbol_name=symbol_name,
-        size_bytes=len(blob_data),
-        bytes=', '.join(byte_strs))
-    if len(single_line_def) <= 80:
-        return single_line_def
+    byte_strs = ['std::byte{{0x{:02X}}}'.format(b) for b in blob_data]
 
-    # Blob definition didn't fit on a single line; do multi-line.
     lines = []
     for byte_strs_for_line in split_into_chunks(byte_strs, BYTES_PER_LINE):
         bytes_segment = ', '.join(byte_strs_for_line)
-        lines.append(f'  {bytes_segment},')
-    # Removing the trailing comma from the final line of bytes.
-    lines[-1] = lines[-1].rstrip(',')
-
-    return BLOB_DEFINITION_MULTI_LINE.substitute(symbol_name=symbol_name,
-                                                 size_bytes=len(blob_data),
-                                                 bytes_lines='\n'.join(lines))
+        lines.append(f'    {bytes_segment},')
+
+    return BLOB_DEFINITION_MULTI_LINE.substitute(
+        section_attr=section_attr,
+        alignas=f'alignas({blob.alignas}) ' if blob.alignas else '',
+        symbol_name=blob.symbol_name,
+        size_bytes=len(blob_data),
+        bytes_lines='\n'.join(lines))
 
 
 def source_from_blobs(blobs: Iterable[Blob],
-                      header_path: Path,
+                      header_path: str,
                       namespace: Optional[str] = None) -> str:
     """Generate the contents of a C++ source file from blobs."""
     lines = [SOURCE_PREFIX_TEMPLATE.substitute(header_path=header_path)]
     if namespace:
         lines.append(NAMESPACE_OPEN_TEMPLATE.substitute(namespace=namespace))
     for blob in blobs:
-        if blob.linker_section:
-            lines.append(
-                LINKER_SECTION_TEMPLATE.substitute(
-                    linker_section=blob.linker_section))
         data = blob.file_path.read_bytes()
-        lines.append(array_def_from_blob_data(blob.symbol_name, data))
-        lines.append('')
+        lines.append(array_def_from_blob_data(blob, data))
     if namespace:
         lines.append(NAMESPACE_CLOSE_TEMPLATE.substitute(namespace=namespace))
 
-    return '\n'.join(lines)
+    return ''.join(lines)
 
 
-def load_blobs(blob_file: Path) -> Iterable[Blob]:
+def load_blobs(blob_file: Path) -> Sequence[Blob]:
     with blob_file.open() as blob_fp:
-        return [
-            Blob(b["symbol_name"], Path(b["file_path"]),
-                 b.get("linker_section")) for b in json.load(blob_fp)
-        ]
+        return [Blob.from_dict(blob) for blob in json.load(blob_fp)]
 
 
 def main(blob_file: Path,
+         header_include: str,
          out_source: Path,
          out_header: Path,
          namespace: Optional[str] = None) -> None:
     blobs = load_blobs(blob_file)
+
+    out_header.parent.mkdir(parents=True, exist_ok=True)
     out_header.write_text(header_from_blobs(blobs, namespace))
-    out_source.write_text(source_from_blobs(blobs, out_header, namespace))
+
+    out_source.parent.mkdir(parents=True, exist_ok=True)
+    out_source.write_text(source_from_blobs(blobs, header_include, namespace))
 
 
 if __name__ == '__main__':
-    main(**vars(parse_args()))
+    main(**parse_args())
```

### Comparing `pigweed-0.0.8/pw_build/generate_modules_lists.py` & `pigweed-0.0.9/pw_build/generate_modules_lists.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/generate_python_package.py` & `pigweed-0.0.9/pw_build/generate_python_package.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/generate_python_package_gn.py` & `pigweed-0.0.9/pw_build/generate_python_package_gn.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/generated_tests.py` & `pigweed-0.0.9/pw_build/generated_tests.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/host_tool.py` & `pigweed-0.0.9/pw_build/host_tool.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/mirror_tree.py` & `pigweed-0.0.9/pw_build/mirror_tree.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/nop.py` & `pigweed-0.0.9/pw_build/nop.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/pip_install_python_deps.py` & `pigweed-0.0.9/pw_build/pip_install_python_deps.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/python_package.py` & `pigweed-0.0.9/pw_build/python_package.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/python_runner.py` & `pigweed-0.0.9/pw_build/python_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,15 +425,15 @@
     if not target.generated:
         raise ExpressionError(f'Target {target} has not been generated by GN!')
 
     for obj in target.object_files:
         yield _ArgAction.EMIT_NEW, str(obj)
 
 
-# TODO(pwbug/347): Replace expressions with native GN features when possible.
+# TODO(b/234886742): Replace expressions with native GN features when possible.
 _FUNCTIONS: Dict['str', Callable[[GnPaths, _Expression], _Actions]] = {
     'TARGET_FILE': _target_file,
     'TARGET_FILE_IF_EXISTS': _target_file_if_exists,
     'TARGET_OBJECTS': _target_objects,
 }
 
 _START_EXPRESSION = re.compile(fr'<({"|".join(_FUNCTIONS)})\(')
@@ -561,15 +561,20 @@
 
         for pkg in py_packages:
             top_level_source_dir = pkg.package_dir
             if not top_level_source_dir:
                 raise MissingPythonDependency(
                     'Unable to find top level source dir for the Python '
                     f'package "{pkg}"')
+            # Don't add this dir to the PYTHONPATH if no __init__.py exists.
+            init_py_files = top_level_source_dir.parent.glob('*/__init__.py')
+            if not any(init_py_files):
+                continue
             python_paths_list.append(top_level_source_dir.parent.resolve())
+
         # Sort the PYTHONPATH list, it will be in a different order each build.
         python_paths_list = sorted(python_paths_list)
 
     if not original_cmd or original_cmd[0] != '--':
         _LOG.error('%s requires a command to run', sys.argv[0])
         return 1
 
@@ -653,16 +658,16 @@
     except ExpressionError as err:
         _LOG.error('%s: %s', sys.argv[0], err)
         return 1
 
     if working_directory:
         run_args['cwd'] = working_directory
 
-    # TODO(pwbug/666): Deprecate the --lockfile option as part of the Python GN
-    # template refactor.
+    # TODO(b/235239674): Deprecate the --lockfile option as part of the Python
+    # GN template refactor.
     if lockfile:
         try:
             acquire_lock(lockfile, is_pip_command)
         except LockAcquisitionTimeoutError as exception:
             _LOG.error('%s', exception)
             return 1
```

### Comparing `pigweed-0.0.8/pw_build/python_wheels.py` & `pigweed-0.0.9/pw_build/python_wheels.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build/zip.py` & `pigweed-0.0.9/pw_build/zip.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build_info/build_id.py` & `pigweed-0.0.9/pw_build_info/build_id.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build_mcuxpresso/__init__.py` & `pigweed-0.0.9/pw_build_mcuxpresso/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build_mcuxpresso/__main__.py` & `pigweed-0.0.9/pw_build_mcuxpresso/__main__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_build_mcuxpresso/components.py` & `pigweed-0.0.9/pw_build_mcuxpresso/components.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/__main__.py` & `pigweed-0.0.9/pw_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/argument_types.py` & `pigweed-0.0.9/pw_cli/argument_types.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/arguments.py` & `pigweed-0.0.9/pw_cli/arguments.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/branding.py` & `pigweed-0.0.9/pw_cli/branding.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/color.py` & `pigweed-0.0.9/pw_cli/color.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/env.py` & `pigweed-0.0.9/pw_cli/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 def pigweed_environment_parser() -> envparse.EnvironmentParser:
     """Defines Pigweed's environment variables on an EnvironmentParser."""
     parser = envparse.EnvironmentParser(prefix='PW_')
 
     parser.add_var('PW_BOOTSTRAP_PYTHON')
-    parser.add_var('PW_BOOTSTRAP_USE_ROSETTA')
     parser.add_var('PW_ENABLE_PRESUBMIT_HOOK_WARNING', default=False)
     parser.add_var('PW_EMOJI', type=envparse.strict_bool, default=False)
     parser.add_var('PW_ENVSETUP')
     parser.add_var('PW_ENVSETUP_FULL')
     parser.add_var('PW_ENVSETUP_NO_BANNER',
                    type=envparse.strict_bool,
                    default=False)
@@ -58,14 +57,17 @@
 
     parser.add_var('PW_PRESUBMIT_DISABLE_SUBPROCESS_CAPTURE',
                    type=envparse.strict_bool)
 
     parser.add_var('PW_CONSOLE_CONFIG_FILE')
     parser.add_var('PW_ENVIRONMENT_NO_ERROR_ON_UNRECOGNIZED')
 
+    # TODO(b/231998579) Remove after a week or two.
+    parser.add_var('PW_BOOTSTRAP_USE_ROSETTA')
+
     return parser
 
 
 # Internal: memoize environment parsing to avoid unnecessary computation in
 # multiple calls to pigweed_environment().
 _memoized_environment: Optional[envparse.EnvNamespace] = None
```

### Comparing `pigweed-0.0.8/pw_cli/envparse.py` & `pigweed-0.0.9/pw_cli/envparse.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/log.py` & `pigweed-0.0.9/pw_cli/log.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/plugins.py` & `pigweed-0.0.9/pw_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/process.py` & `pigweed-0.0.9/pw_cli/process.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/pw_command_plugins.py` & `pigweed-0.0.9/pw_cli/pw_command_plugins.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cli/requires.py` & `pigweed-0.0.9/pw_cli/requires.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 references internal-project:1234 so the current commit effectively has a
 requirement on internal-project:1234.
 
 For more see http://go/pigweed-ci-cq-intro.
 """
 
 import argparse
+import json
 import logging
 from pathlib import Path
 import re
 import subprocess
 import sys
 import tempfile
 import uuid
@@ -96,25 +97,32 @@
 
 def clone(requires_dir: Path) -> None:
     _LOG.info('cloning helper repository into %s', requires_dir)
     _run_command(['git', 'clone', HELPER_REPO, '.'], cwd=requires_dir)
 
 
 def create_commit(requires_dir: Path, requirements) -> None:
+    """Create a commit in the local tree with the given requirements."""
     change_id = str(uuid.uuid4()).replace('-', '00')
     _LOG.debug('change_id %s', change_id)
-    path = requires_dir / change_id
+
+    reqs = []
+    for req in requirements:
+        gerrit_name, number = req.split(':', 1)
+        reqs.append({'gerrit_name': gerrit_name, 'number': number})
+
+    path = requires_dir / 'patches.json'
     _LOG.debug('path %s', path)
-    with open(path, 'w'):
-        pass
+    with open(path, 'w') as outs:
+        json.dump(reqs, outs)
 
     _run_command(['git', 'add', path], cwd=requires_dir)
 
     commit_message = [
-        f'{_DNS} {change_id[0:10]}',
+        f'{_DNS} {change_id[0:10]}\n\n',
         '',
         f'Change-Id: I{change_id}',
     ]
     for req in requirements:
         commit_message.append(f'Requires: {req}')
 
     _LOG.debug('message %s', commit_message)
```

### Comparing `pigweed-0.0.8/pw_console/__init__.py` & `pigweed-0.0.9/pw_console/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/__main__.py` & `pigweed-0.0.9/pw_console/__main__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/command_runner.py` & `pigweed-0.0.9/pw_console/command_runner.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/console_app.py` & `pigweed-0.0.9/pw_console/console_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 # Fake logger for --test-mode
 FAKE_DEVICE_LOGGER_NAME = 'pw_console_fake_device'
 _FAKE_DEVICE_LOG = logging.getLogger(FAKE_DEVICE_LOGGER_NAME)
 # Don't send fake_device logs to the root Python logger.
 _FAKE_DEVICE_LOG.propagate = False
 
-MAX_FPS = 15
+MAX_FPS = 30
 MIN_REDRAW_INTERVAL = (60.0 / MAX_FPS) / 60.0
 
 
 class FloatingMessageBar(ConditionalContainer):
     """Floating message bar for showing status messages."""
     def __init__(self, application):
         super().__init__(
```

### Comparing `pigweed-0.0.8/pw_console/console_prefs.py` & `pigweed-0.0.9/pw_console/console_prefs.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/docs/user_guide.rst` & `pigweed-0.0.9/pw_console/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/embed.py` & `pigweed-0.0.9/pw_console/embed.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/filter_toolbar.py` & `pigweed-0.0.9/pw_console/filter_toolbar.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/get_pw_console_app.py` & `pigweed-0.0.9/pw_console/get_pw_console_app.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/help_window.py` & `pigweed-0.0.9/pw_console/help_window.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/key_bindings.py` & `pigweed-0.0.9/pw_console/key_bindings.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/log_filter.py` & `pigweed-0.0.9/pw_console/log_filter.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/log_line.py` & `pigweed-0.0.9/pw_console/log_line.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/log_pane.py` & `pigweed-0.0.9/pw_console/log_pane.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/log_pane_saveas_dialog.py` & `pigweed-0.0.9/pw_console/log_pane_saveas_dialog.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/log_pane_selection_dialog.py` & `pigweed-0.0.9/pw_console/log_pane_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/log_pane_toolbars.py` & `pigweed-0.0.9/pw_console/log_pane_toolbars.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/log_screen.py` & `pigweed-0.0.9/pw_console/log_screen.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/log_store.py` & `pigweed-0.0.9/pw_console/log_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,16 +212,16 @@
             LogLine(record=record,
                     formatted_log=formatted_log,
                     ansi_stripped_log=ansi_stripped_log))
         # Increment this logger count
         self.channel_counts[record.name] = self.channel_counts.get(
             record.name, 0) + 1
 
-        # TODO(pwbug/614): Revisit calculating prefix widths automatically when
-        # line wrapping indentation is supported.
+        # TODO(b/235271486): Revisit calculating prefix widths automatically
+        # when line wrapping indentation is supported.
         # Set the prefix width to 0
         self.channel_formatted_prefix_widths[record.name] = 0
 
         # Parse metadata fields
         self.logs[-1].update_metadata()
 
         # Check for bigger column widths.
```

### Comparing `pigweed-0.0.8/pw_console/log_view.py` & `pigweed-0.0.9/pw_console/log_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,17 @@
         self.follow: bool = True
 
         self.visual_select_mode: bool = False
 
         # Cache of formatted text tuples used in the last UI render.
         self._line_fragment_cache: List[StyleAndTextTuples] = []
 
+        # Check if any logs are already in the log_store and update the view.
+        self.new_logs_arrived()
+
     def view_mode_changed(self) -> None:
         self._reset_log_screen_on_next_render = True
 
     @property
     def log_index(self):
         if self.filtering_on:
             return self._filtered_log_index
```

### Comparing `pigweed-0.0.8/pw_console/mouse.py` & `pigweed-0.0.9/pw_console/mouse.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/pigweed_code_style.py` & `pigweed-0.0.9/pw_console/pigweed_code_style.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/plugin_mixin.py` & `pigweed-0.0.9/pw_console/plugin_mixin.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/plugins/__init__.py` & `pigweed-0.0.9/pw_console/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/plugins/bandwidth_toolbar.py` & `pigweed-0.0.9/pw_console/plugins/bandwidth_toolbar.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/plugins/calc_pane.py` & `pigweed-0.0.9/pw_console/plugins/calc_pane.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/plugins/clock_pane.py` & `pigweed-0.0.9/pw_console/plugins/clock_pane.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/plugins/twenty48_pane.py` & `pigweed-0.0.9/pw_console/plugins/twenty48_pane.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/progress_bar/__init__.py` & `pigweed-0.0.9/pw_console/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/progress_bar/progress_bar_impl.py` & `pigweed-0.0.9/pw_console/progress_bar/progress_bar_impl.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/progress_bar/progress_bar_state.py` & `pigweed-0.0.9/pw_console/progress_bar/progress_bar_state.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/progress_bar/progress_bar_task_counter.py` & `pigweed-0.0.9/pw_console/progress_bar/progress_bar_task_counter.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/pw_ptpython_repl.py` & `pigweed-0.0.9/pw_console/pw_ptpython_repl.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/pyserial_wrapper.py` & `pigweed-0.0.9/pw_console/pyserial_wrapper.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/python_logging.py` & `pigweed-0.0.9/pw_console/python_logging.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/quit_dialog.py` & `pigweed-0.0.9/pw_console/quit_dialog.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/repl_pane.py` & `pigweed-0.0.9/pw_console/repl_pane.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/search_toolbar.py` & `pigweed-0.0.9/pw_console/search_toolbar.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/style.py` & `pigweed-0.0.9/pw_console/style.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/templates/keybind_list.jinja` & `pigweed-0.0.9/pw_console/templates/keybind_list.jinja`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/templates/repl_output.jinja` & `pigweed-0.0.9/pw_console/templates/repl_output.jinja`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/text_formatting.py` & `pigweed-0.0.9/pw_console/text_formatting.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/widgets/__init__.py` & `pigweed-0.0.9/pw_console/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/widgets/border.py` & `pigweed-0.0.9/pw_console/widgets/border.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/widgets/checkbox.py` & `pigweed-0.0.9/pw_console/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/widgets/event_count_history.py` & `pigweed-0.0.9/pw_console/widgets/event_count_history.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/widgets/mouse_handlers.py` & `pigweed-0.0.9/pw_console/widgets/mouse_handlers.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/widgets/table.py` & `pigweed-0.0.9/pw_console/widgets/table.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/widgets/window_pane.py` & `pigweed-0.0.9/pw_console/widgets/window_pane.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/widgets/window_pane_toolbar.py` & `pigweed-0.0.9/pw_console/widgets/window_pane_toolbar.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/window_list.py` & `pigweed-0.0.9/pw_console/window_list.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/window_manager.py` & `pigweed-0.0.9/pw_console/window_manager.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_console/yaml_config_loader_mixin.py` & `pigweed-0.0.9/pw_console/yaml_config_loader_mixin.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cpu_exception_cortex_m/__init__.py` & `pigweed-0.0.9/pw_cpu_exception_cortex_m/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cpu_exception_cortex_m/cfsr_decoder.py` & `pigweed-0.0.9/pw_cpu_exception_cortex_m/cfsr_decoder.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cpu_exception_cortex_m/cortex_m_constants.py` & `pigweed-0.0.9/pw_cpu_exception_cortex_m/cortex_m_constants.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cpu_exception_cortex_m/exception_analyzer.py` & `pigweed-0.0.9/pw_cpu_exception_cortex_m/exception_analyzer.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cpu_exception_cortex_m_protos/cpu_state_pb2.py` & `pigweed-0.0.9/pw_cpu_exception_cortex_m_protos/cpu_state_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_cpu_exception_cortex_m_protos/cpu_state_pb2.pyi` & `pigweed-0.0.9/pw_cpu_exception_cortex_m_protos/cpu_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_docgen/docgen.py` & `pigweed-0.0.9/pw_docgen/docgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
     args = parse_args()
 
     # Clear out any existing docs for the target.
     if os.path.exists(args.sphinx_build_dir):
         shutil.rmtree(args.sphinx_build_dir)
 
-    # TODO(pwbug/164): Printing the header causes unicode problems on Windows.
+    # TODO(b/235349854): Printing the header causes unicode problems on Windows.
     # Disabled for now; re-enable once the root issue is fixed.
     # print(SCRIPT_HEADER)
     copy_doc_tree(args)
 
     # Flush all script output before running Sphinx.
     print('-' * 80, flush=True)
```

### Comparing `pigweed-0.0.8/pw_docgen/sphinx/google_analytics.py` & `pigweed-0.0.9/pw_docgen/sphinx/google_analytics.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_doctor/doctor.py` & `pigweed-0.0.9/pw_doctor/doctor.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,17 +210,15 @@
 
 
 @register_into(CHECKS)
 def python_version(ctx: DoctorContext):
     """Check the Python version is correct."""
     actual = sys.version_info
     expected = (3, 8)
-    latest = (3, 9)
-    if (actual[0:2] < expected or actual[0] != expected[0]
-            or actual[0:2] > latest):
+    if actual[0:2] < expected or actual[0] != expected[0]:
         # If we get the wrong version but it still came from CIPD print a
         # warning but give it a pass.
         if 'chromium' in sys.version:
             ctx.warning('Python %d.%d.x expected, got Python %d.%d.%d',
                         *expected, *actual[0:3])
         else:
             ctx.error('Python %d.%d.x required, got Python %d.%d.%d',
@@ -373,14 +371,20 @@
 
             else:
                 ctx.debug('CIPD package %s in %s is current',
                           installed['package_name'], install_path)
 
     for json_path in json_paths:
         ctx.debug(f'Checking packages in {json_path}')
+        if not json_path.exists():
+            ctx.error(
+                'CIPD package file %s may have been deleted, please '
+                'rerun bootstrap', json_path)
+            continue
+
         install_path = pathlib.Path(
             cipd_update.package_installation_path(cipd_dir, json_path))
         for package in json.loads(json_path.read_text()).get('packages', ()):
             ctx.submit(check_cipd, package, install_path)
 
 
 @register_into(CHECKS)
@@ -422,15 +426,15 @@
 
     if doctor.failures:
         doctor.log.info('Failed checks: %s', ', '.join(doctor.failures))
         doctor.log.info(
             "Your environment setup has completed, but something isn't right "
             'and some things may not work correctly. You may continue with '
             'development, but please seek support at '
-            'https://bugs.pigweed.dev/ or by reaching out to your team.')
+            'https://bugs.pigweed.dev/new or by reaching out to your team.')
     else:
         doctor.log.info('Environment passes all checks!')
     return len(doctor.failures)
 
 
 def main() -> int:
     """Check that the environment is set up correctly for Pigweed."""
```

### Comparing `pigweed-0.0.8/pw_env_setup/__init__.py` & `pigweed-0.0.9/pw_env_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/apply_visitor.py` & `pigweed-0.0.9/pw_env_setup/apply_visitor.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/batch_visitor.py` & `pigweed-0.0.9/pw_env_setup/batch_visitor.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/cipd_setup/__init__.py` & `pigweed-0.0.9/pw_env_setup/cipd_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/cipd_setup/luci.json` & `pigweed-0.0.9/pw_env_setup/cipd_setup/luci.json`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/cipd_setup/pigweed.json` & `pigweed-0.0.9/pw_env_setup/cipd_setup/pigweed.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9451754385964912%*

 * *Differences: {"'packages'": "{0: {'tags': ['git_revision:03ce92df5f9875bd9929b564be4b612713569aa9']}, 1: "*

 * *               "{'tags': ['version:2@1.11.0.chromium.4']}, 3: {'tags': "*

 * *               "['version:3.24.20220709-g6734c2a']}, 8: {'tags': ['version:2@1.18.3']}, 12: "*

 * *               "{'tags': ['git_revision:0c7cba1e230563ac772cac1bad1782ce973b0021']}, 13: "*

 * *               "{'platforms': {insert: [(1, 'mac-amd64'), (2, 'mac-arm64')]}, 'tags': "*

 * *               "['re_client_version:0.58.0.d457d5a']}, 14: {'tags': ['ve […]*

```diff
@@ -6,41 +6,54 @@
                 "linux-amd64",
                 "linux-arm64",
                 "mac-amd64",
                 "mac-arm64",
                 "windows-amd64"
             ],
             "tags": [
-                "git_revision:48b013c9d9debc0f5fc1dd71a257b3c38c5acb43"
+                "git_revision:03ce92df5f9875bd9929b564be4b612713569aa9"
             ],
             "version_file": ".versions/gn.cipd_version"
         },
         {
             "path": "infra/3pp/tools/ninja/${platform}",
             "platforms": [
                 "linux-amd64",
                 "linux-arm64",
                 "mac-amd64",
                 "mac-arm64",
                 "windows-amd64"
             ],
             "tags": [
-                "version:2@1.10.2"
+                "version:2@1.11.0.chromium.4"
+            ]
+        },
+        {
+            "path": "infra/3pp/tools/nodejs/${platform}",
+            "platforms": [
+                "linux-amd64",
+                "linux-arm64",
+                "mac-amd64",
+                "mac-arm64",
+                "windows-amd64"
+            ],
+            "tags": [
+                "version:2@18.4.0"
             ]
         },
         {
             "path": "fuchsia/third_party/cmake/${platform}",
             "platforms": [
                 "mac-amd64",
                 "linux-amd64",
                 "linux-arm64",
                 "windows-amd64"
             ],
             "tags": [
-                "version:3.23.20220430-g833e952"
+                "version:3.24.20220709-g6734c2a"
             ],
             "version_file": ".versions/cmake.cipd_version"
         },
         {
             "path": "pigweed/third_party/bloaty-embedded/${platform}",
             "platforms": [
                 "linux-amd64",
@@ -92,15 +105,15 @@
                 "linux-amd64",
                 "linux-arm64",
                 "mac-amd64",
                 "mac-arm64",
                 "windows-amd64"
             ],
             "tags": [
-                "version:2@1.18.1"
+                "version:2@1.18.3"
             ]
         },
         {
             "path": "pigweed/third_party/protoc-gen-go/${platform}",
             "platforms": [
                 "linux-amd64",
                 "mac-amd64",
@@ -136,37 +149,39 @@
             "path": "pigweed/host_tools/${platform}",
             "platforms": [
                 "linux-amd64",
                 "mac-amd64",
                 "windows-amd64"
             ],
             "tags": [
-                "git_revision:3a1b296bc3d0d0a9b663a714f2373d6e9483b4d9"
+                "git_revision:0c7cba1e230563ac772cac1bad1782ce973b0021"
             ],
             "version_file": ".versions/host_tools.cipd_version"
         },
         {
             "path": "infra/rbe/client/${platform}",
             "platforms": [
                 "linux-amd64",
+                "mac-amd64",
+                "mac-arm64",
                 "windows-amd64"
             ],
             "tags": [
-                "re_client_version:0.41.4.3f0d8bb"
+                "re_client_version:0.58.0.d457d5a"
             ]
         },
         {
             "path": "fuchsia/third_party/qemu/${platform}",
             "platforms": [
                 "linux-amd64",
                 "linux-arm64",
                 "mac-amd64"
             ],
             "tags": [
-                "git_revision:44f28df24767cf9dca1ddc9b23157737c4cbb645"
+                "version:v6.2.0"
             ],
             "version_file": ".versions/qemu.cipd_version"
         },
         {
             "path": "fuchsia/third_party/kythe",
             "platforms": [
                 "linux-amd64"
```

### Comparing `pigweed-0.0.8/pw_env_setup/cipd_setup/update.py` & `pigweed-0.0.9/pw_env_setup/cipd_setup/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,21 @@
             stderr('  {}'.format(path))
         stderr('=' * 60)
         return False
 
     return True
 
 
-def platform():
+def platform(rosetta=None):
+    """Return the CIPD platform string of the current system."""
+    # If running inside a bootstrapped environment we can use the env var.
+    # Otherwise, require rosetta be set.
+    if rosetta is None:
+        rosetta = os.environ['_PW_ROSETTA']
+
     osname = {
         'darwin': 'mac',
         'linux': 'linux',
         'windows': 'windows',
     }[platform_module.system().lower()]
 
     if platform_module.machine().startswith(('aarch64', 'armv8')):
@@ -133,16 +139,15 @@
         arch = 'i386'
     else:
         arch = platform_module.machine()
 
     platform_arch = '{}-{}'.format(osname, arch).lower()
 
     # Support `mac-arm64` through Rosetta until `mac-arm64` binaries are ready
-    if platform_arch == 'mac-arm64' and os.getenv(
-            'PW_BOOTSTRAP_USE_ROSETTA', 'false').lower() in ('true', 't', '1'):
+    if platform_arch == 'mac-arm64' and rosetta:
         return 'mac-amd64'
 
     return platform_arch
 
 
 def all_package_files(env_vars, package_files):
     """Recursively retrieve all package files."""
@@ -175,15 +180,15 @@
 
             if entry not in result and entry not in to_process:
                 to_process.append(entry)
 
     return result
 
 
-def write_ensure_file(package_files, ensure_file):
+def write_ensure_file(package_files, ensure_file, platform):  # pylint: disable=redefined-outer-name
     packages = []
 
     for package_file in package_files:
         name = package_file_name(package_file)
         with open(package_file, 'r') as ins:
             file_packages = json.load(ins).get('packages', ())
             for package in file_packages:
@@ -197,15 +202,15 @@
         outs.write('$VerifiedPlatform linux-amd64\n'
                    '$VerifiedPlatform mac-amd64\n'
                    '$ParanoidMode CheckPresence\n')
 
         for pkg in packages:
             # If this is a new-style package manifest platform handling must
             # be done here instead of by the cipd executable.
-            if 'platforms' in pkg and platform() not in pkg['platforms']:
+            if 'platforms' in pkg and platform not in pkg['platforms']:
                 continue
 
             outs.write('@Subdir {}\n'.format(pkg.get('subdir', '')))
             outs.write('{} {}\n'.format(pkg['path'], ' '.join(pkg['tags'])))
 
 
 def package_file_name(package_file):
@@ -219,19 +224,20 @@
       root_install_dir: The CIPD installation directory.
       package_file: The path to the .json package definition file.
     """
     return os.path.join(root_install_dir, 'packages',
                         package_file_name(package_file))
 
 
-def update(
+def update(  # pylint: disable=too-many-locals
     cipd,
     package_files,
     root_install_dir,
     cache_dir,
+    rosetta=False,
     env_vars=None,
     spin=None,
     trust_hash=False,
 ):
     """Grab the tools listed in ensure_files."""
 
     package_files = all_package_files(env_vars, package_files)
@@ -255,16 +261,18 @@
     pw_root = None
 
     if env_vars:
         pw_root = env_vars.get('PW_ROOT', None)
     if not pw_root:
         pw_root = os.environ['PW_ROOT']
 
+    plat = platform(rosetta)
+
     ensure_file = os.path.join(root_install_dir, 'packages.ensure')
-    write_ensure_file(package_files, ensure_file)
+    write_ensure_file(package_files, ensure_file, plat)
 
     install_dir = os.path.join(root_install_dir, 'packages')
 
     cmd = [
         cipd,
         'ensure',
         '-ensure-file', ensure_file,
@@ -324,15 +332,15 @@
             file_install_dir = os.path.join(install_dir, name)
             # Some executables get installed at top-level and some get
             # installed under 'bin'. A small number of old packages prefix the
             # entire tree with the platform (e.g., chromium/third_party/tcl).
             for bin_dir in (
                     file_install_dir,
                     os.path.join(file_install_dir, 'bin'),
-                    os.path.join(file_install_dir, platform(), 'bin'),
+                    os.path.join(file_install_dir, plat, 'bin'),
             ):
                 if os.path.isdir(bin_dir):
                     env_vars.prepend('PATH', bin_dir)
             env_vars.set('PW_{}_CIPD_INSTALL_DIR'.format(name.upper()),
                          file_install_dir)
 
             # Windows has its own special toolchain.
```

### Comparing `pigweed-0.0.8/pw_env_setup/cipd_setup/wrapper.py` & `pigweed-0.0.9/pw_env_setup/cipd_setup/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,39 +113,34 @@
             'darwin': 'mac',
             'windows': 'windows',
         }[os_name]
     except KeyError:
         raise Exception('unrecognized os: {}'.format(os_name))
 
 
-def arch_normalized():
+def arch_normalized(rosetta=False):
     """Normalize arch into format expected in CIPD paths."""
 
     machine = platform.machine()
+    if platform_normalized() == 'mac' and rosetta:
+        return 'amd64'
     if machine.startswith(('arm', 'aarch')):
         machine = machine.replace('aarch', 'arm')
         if machine == 'arm64':
             return machine
         return 'armv6l'
     if machine.endswith('64'):
         return 'amd64'
     if machine.endswith('86'):
         return '386'
     raise Exception('unrecognized arch: {}'.format(machine))
 
 
-def platform_arch_normalized():
-    platform_arch = '{}-{}'.format(platform_normalized(), arch_normalized())
-
-    # Support `mac-arm64` through Rosetta until `mac-arm64` binaries are ready
-    if platform_arch == 'mac-arm64' and os.getenv(
-            'PW_BOOTSTRAP_USE_ROSETTA', 'false').lower() in ('true', 't', '1'):
-        platform_arch = 'mac-amd64'
-
-    return platform_arch
+def platform_arch_normalized(rosetta=False):
+    return '{}-{}'.format(platform_normalized(), arch_normalized(rosetta))
 
 
 def user_agent():
     """Generate a user-agent based on the project name and current hash."""
 
     try:
         rev = subprocess.check_output(
@@ -164,18 +159,18 @@
 
     hasher = hashlib.sha256()
     with open(path, 'rb') as ins:
         hasher.update(ins.read())
     return hasher.hexdigest()
 
 
-def expected_hash():
+def expected_hash(rosetta=False):
     """Pulls expected hash from digests file."""
 
-    expected_plat = platform_arch_normalized()
+    expected_plat = platform_arch_normalized(rosetta)
 
     with open(DIGESTS_FILE, 'r') as ins:
         for line in ins:
             line = line.strip()
             if line.startswith('#') or not line:
                 continue
             plat, hashtype, hashval = line.split()
@@ -204,15 +199,15 @@
                 base64.b64encode(auth.encode()).decode())
         else:
             headers['Proxy-Authorization'] = 'Basic ' + base64.b64encode(auth)
     conn.set_tunnel(target_url, 443, headers)
     return conn
 
 
-def client_bytes():
+def client_bytes(rosetta=False):
     """Pull down the CIPD client and return it as a bytes object.
 
     Often CIPD_HOST returns a 302 FOUND with a pointer to
     storage.googleapis.com, so this needs to handle redirects, but it
     shouldn't require the initial response to be a redirect either.
     """
 
@@ -230,15 +225,15 @@
 
 brew install openssl  # Probably already installed, but good to confirm.
 brew uninstall python && brew install python
 '''.strip())
         print('=' * 70)
         raise
 
-    full_platform = platform_arch_normalized()
+    full_platform = platform_arch_normalized(rosetta)
     if full_platform not in SUPPORTED_PLATFORMS:
         raise UnsupportedPlatform(full_platform)
 
     path = '/client?platform={}&version={}'.format(full_platform, version)
 
     for _ in range(10):
         try:
@@ -292,30 +287,34 @@
         else:
             break
 
     raise Exception('failed to download client from https://{}{}'.format(
         CIPD_HOST, path))
 
 
-def bootstrap(client, silent=('PW_ENVSETUP_QUIET' in os.environ)):
+def bootstrap(
+        client,
+        silent=('PW_ENVSETUP_QUIET' in os.environ),
+        rosetta=False,
+):
     """Bootstrap cipd client installation."""
 
     client_dir = os.path.dirname(client)
     if not os.path.isdir(client_dir):
         os.makedirs(client_dir)
 
     if not silent:
         print('Bootstrapping cipd client for {}'.format(
-            platform_arch_normalized()))
+            platform_arch_normalized(rosetta)))
 
     tmp_path = client + '.tmp'
     with open(tmp_path, 'wb') as tmp:
-        tmp.write(client_bytes())
+        tmp.write(client_bytes(rosetta))
 
-    expected = expected_hash()
+    expected = expected_hash(rosetta=rosetta)
     actual = actual_hash(tmp_path)
 
     if expected != actual:
         raise Exception('digest of downloaded CIPD client is incorrect, '
                         'check that digests file is current')
 
     os.chmod(tmp_path, 0o755)
@@ -337,31 +336,36 @@
 def _default_client(install_dir):
     client = os.path.join(install_dir, 'cipd')
     if os.name == 'nt':
         client += '.exe'
     return client
 
 
-def init(install_dir=DEFAULT_INSTALL_DIR, silent=False, client=None):
+def init(
+    install_dir=DEFAULT_INSTALL_DIR,
+    silent=False,
+    client=None,
+    rosetta=False,
+):
     """Install/update cipd client."""
 
     if not client:
         client = _default_client(install_dir)
 
     os.environ['CIPD_HTTP_USER_AGENT_PREFIX'] = user_agent()
 
     if not os.path.isfile(client):
-        bootstrap(client, silent)
+        bootstrap(client, silent, rosetta=rosetta)
 
     try:
         selfupdate(client)
     except subprocess.CalledProcessError:
         print('CIPD selfupdate failed. Bootstrapping then retrying...',
               file=sys.stderr)
-        bootstrap(client)
+        bootstrap(client, rosetta=rosetta)
         selfupdate(client)
 
     return client
 
 
 def main(install_dir=DEFAULT_INSTALL_DIR, silent=False):
     """Install/update cipd client."""
```

### Comparing `pigweed-0.0.8/pw_env_setup/colors.py` & `pigweed-0.0.9/pw_env_setup/colors.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/env_setup.py` & `pigweed-0.0.9/pw_env_setup/env_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,14 +194,15 @@
             os.unlink(shell_file)
 
         if isinstance(self._pw_root, bytes) and bytes != str:
             self._pw_root = self._pw_root.decode()
 
         self._cipd_package_file = []
         self._virtualenv_requirements = []
+        self._virtualenv_constraints = []
         self._virtualenv_gn_targets = []
         self._virtualenv_gn_args = []
         self._use_pinned_pip_packages = use_pinned_pip_packages
         self._optional_submodules = []
         self._required_submodules = []
         self._virtualenv_system_packages = False
         self._pw_packages = []
@@ -257,14 +258,20 @@
         return files, warnings
 
     def _parse_config_file(self, config_file):
         config = json.load(config_file)
 
         self._root_variable = config.pop('root_variable', None)
 
+        rosetta = config.pop('rosetta', 'allow')
+        if rosetta not in ('never', 'allow', 'force'):
+            raise ValueError(rosetta)
+        self._rosetta = rosetta in ('allow', 'force')
+        self._env.set('_PW_ROSETTA', str(int(self._rosetta)))
+
         if 'json_file' in config:
             self._json_file = config.pop('json_file')
 
         self._gni_file = config.pop('gni_file', None)
 
         self._optional_submodules.extend(config.pop('optional_submodules', ()))
         self._required_submodules.extend(config.pop('required_submodules', ()))
@@ -294,14 +301,22 @@
                 virtualenv_setup.GnTarget('{}#{}'.format(root, target)))
 
         self._virtualenv_gn_args = virtualenv.pop('gn_args', ())
 
         self._virtualenv_system_packages = virtualenv.pop(
             'system_packages', False)
 
+        for req_txt in virtualenv.pop('requirements', ()):
+            self._virtualenv_requirements.append(
+                os.path.join(self._project_root, req_txt))
+
+        for constraint_txt in virtualenv.pop('constraints', ()):
+            self._virtualenv_constraints.append(
+                os.path.join(self._project_root, constraint_txt))
+
         if virtualenv:
             raise ConfigFileError(
                 'unrecognized option in {}: "virtualenv.{}"'.format(
                     self._config_file_name, next(iter(virtualenv))))
 
         if config:
             raise ConfigFileError('unrecognized option in {}: "{}"'.format(
@@ -335,15 +350,15 @@
         if missing:
             print(
                 'Not all submodules are initialized. Please run the '
                 'following commands.',
                 file=sys.stderr)
             print('', file=sys.stderr)
 
-            for miss in missing:
+            for miss in sorted(missing):
                 print('    git submodule update --init {}'.format(miss),
                       file=sys.stderr)
             print('', file=sys.stderr)
 
             if self._required_submodules:
                 print(
                     'If these submodules are not required, remove them from '
@@ -524,15 +539,19 @@
         # flag is set, but this flag should only be set in LUCI builds which
         # will always have CIPD.
         if self._use_existing_cipd:
             cipd_client = 'cipd'
 
         else:
             try:
-                cipd_client = cipd_wrapper.init(install_dir, silent=True)
+                cipd_client = cipd_wrapper.init(
+                    install_dir,
+                    silent=True,
+                    rosetta=self._rosetta,
+                )
             except cipd_wrapper.UnsupportedPlatform as exc:
                 return result_func(('    {!r}'.format(exc), ))(
                     _Result.Status.SKIPPED,
                     '    abandoning CIPD setup',
                 )
 
         package_files, glob_warnings = self._process_globs(
@@ -543,26 +562,31 @@
             return result(_Result.Status.SKIPPED)
 
         if not cipd_update.update(cipd=cipd_client,
                                   root_install_dir=install_dir,
                                   package_files=package_files,
                                   cache_dir=self._cipd_cache_dir,
                                   env_vars=self._env,
+                                  rosetta=self._rosetta,
                                   spin=spin,
                                   trust_hash=self._trust_cipd_hash):
             return result(_Result.Status.FAILED)
 
         return result(_Result.Status.DONE)
 
     def virtualenv(self, unused_spin):
         """Setup virtualenv."""
 
         requirements, req_glob_warnings = self._process_globs(
             self._virtualenv_requirements)
-        result = result_func(req_glob_warnings)
+
+        constraints, constraint_glob_warnings = self._process_globs(
+            self._virtualenv_constraints)
+
+        result = result_func(req_glob_warnings + constraint_glob_warnings)
 
         orig_python3 = _which('python3')
         with self._env():
             new_python3 = _which('python3')
 
         # There is an issue with the virtualenv module on Windows where it
         # expects sys.executable to be called "python.exe" or it fails to
@@ -579,14 +603,15 @@
         if not requirements and not self._virtualenv_gn_targets:
             return result(_Result.Status.SKIPPED)
 
         if not virtualenv_setup.install(
                 project_root=self._project_root,
                 venv_path=self._virtualenv_root,
                 requirements=requirements,
+                constraints=constraints,
                 gn_args=self._virtualenv_gn_args,
                 gn_targets=self._virtualenv_gn_targets,
                 gn_out_dir=self._virtualenv_gn_out_dir,
                 python=new_python3,
                 env=self._env,
                 system_packages=self._virtualenv_system_packages,
                 use_pinned_pip_packages=self._use_pinned_pip_packages,
```

### Comparing `pigweed-0.0.8/pw_env_setup/environment.py` & `pigweed-0.0.9/pw_env_setup/environment.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/gni_visitor.py` & `pigweed-0.0.9/pw_env_setup/gni_visitor.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/json_visitor.py` & `pigweed-0.0.9/pw_env_setup/json_visitor.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/shell_visitor.py` & `pigweed-0.0.9/pw_env_setup/shell_visitor.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/spinner.py` & `pigweed-0.0.9/pw_env_setup/spinner.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/virtualenv_setup/__init__.py` & `pigweed-0.0.9/pw_env_setup/virtualenv_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/virtualenv_setup/__main__.py` & `pigweed-0.0.9/pw_env_setup/virtualenv_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_env_setup/virtualenv_setup/install.py` & `pigweed-0.0.9/pw_env_setup/virtualenv_setup/install.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import glob
 import os
 import platform
 import re
 import shutil
 import subprocess
 import sys
+import stat
 import tempfile
 
 # Grabbing datetime string once so it will always be the same for all GnTarget
 # objects.
 _DATETIME_STRING = datetime.datetime.now().strftime('%Y%m%d-%H%M%S')
 
 
@@ -126,34 +127,57 @@
         home = pyvenv_values.get('home')
         if pydir != home and not pydir.startswith(venv_path):
             shutil.rmtree(venv_path)
         elif pyvenv_values.get('version') not in version:
             shutil.rmtree(venv_path)
 
 
-def install(  # pylint: disable=too-many-arguments
+def _check_python_install_permissions(python):
+    # These pickle files are not included on windows.
+    # The path on windows is environment/cipd/packages/python/bin/Lib/lib2to3/
+    if platform.system().lower() == 'windows':
+        return
+
+    # Make any existing lib2to3 pickle files read+write. This is needed for
+    # importing yapf.
+    lib2to3_path = os.path.join(os.path.dirname(os.path.dirname(python)),
+                                'lib', 'python3.9', 'lib2to3')
+    pickle_file_paths = []
+    if os.path.isdir(lib2to3_path):
+        pickle_file_paths.extend(file_path
+                                 for file_path in os.listdir(lib2to3_path)
+                                 if '.pickle' in file_path)
+    try:
+        for pickle_file in pickle_file_paths:
+            pickle_full_path = os.path.join(lib2to3_path, pickle_file)
+            os.chmod(pickle_full_path,
+                     stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP)
+    except PermissionError:
+        pass
+
+
+def install(  # pylint: disable=too-many-arguments,too-many-locals
     project_root,
     venv_path,
     full_envsetup=True,
-    requirements=(),
+    requirements=None,
+    constraints=None,
     gn_args=(),
     gn_targets=(),
     gn_out_dir=None,
     python=sys.executable,
     env=None,
     system_packages=False,
     use_pinned_pip_packages=True,
 ):
     """Creates a venv and installs all packages in this Git repo."""
 
     version = subprocess.check_output(
         (python, '--version'), stderr=subprocess.STDOUT).strip().decode()
-    # We expect Python 3.8, but if it came from CIPD let it pass anyway.
-    if ('3.8' not in version and '3.9' not in version
-            and 'chromium' not in version):
+    if ' 3.' not in version:
         print('=' * 60, file=sys.stderr)
         print('Unexpected Python version:', version, file=sys.stderr)
         print('=' * 60, file=sys.stderr)
         return False
 
     # The bin/ directory is called Scripts/ on Windows. Don't ask.
     venv_bin = os.path.join(venv_path, 'Scripts' if os.name == 'nt' else 'bin')
@@ -171,14 +195,15 @@
     if os.path.isdir(venv_bin):
         for entry in os.listdir(venv_bin):
             if entry.lower().startswith('activate'):
                 os.unlink(os.path.join(venv_bin, entry))
 
     pyvenv_cfg = os.path.join(venv_path, 'pyvenv.cfg')
 
+    _check_python_install_permissions(python)
     _check_venv(python, version, venv_path, pyvenv_cfg)
 
     if full_envsetup or not os.path.exists(pyvenv_cfg):
         # On Mac sometimes the CIPD Python has __PYVENV_LAUNCHER__ set to
         # point to the system Python, which causes CIPD Python to create
         # virtualenvs that reference the system Python instead of the CIPD
         # Python. Clearing __PYVENV_LAUNCHER__ fixes that. See also pwbug/59.
@@ -213,30 +238,42 @@
         os.unlink(egg_link)
 
     def pip_install(*args):
         with env():
             cmd = [venv_python, '-m', 'pip', 'install'] + list(args)
             return _check_call(cmd)
 
+    constraint_args = []
+    if constraints:
+        constraint_args.extend('--constraint={}'.format(constraint)
+                               for constraint in constraints)
+
     pip_install(
         '--log',
         os.path.join(venv_path, 'pip-upgrade.log'),
         '--upgrade',
         'pip',
         'setuptools',
         'toml',  # Needed for pyproject.toml package installs.
         # Include wheel so pip installs can be done without build
         # isolation.
-        'wheel')
+        'wheel',
+        *constraint_args)
+
+    # TODO(tonymd): Remove this when projects have defined requirements.
+    if (not requirements) and constraints:
+        requirements = constraints
 
     if requirements:
-        requirement_args = tuple('--requirement={}'.format(req)
-                                 for req in requirements)
+        requirement_args = ['--no-build-isolation']
+        requirement_args.extend('--requirement={}'.format(req)
+                                for req in requirements)
+        combined_requirement_args = requirement_args + constraint_args
         pip_install('--log', os.path.join(venv_path, 'pip-requirements.log'),
-                    *requirement_args)
+                    *combined_requirement_args)
 
     def install_packages(gn_target):
         if gn_out_dir is None:
             build_dir = os.path.join(venv_path, 'gn-install-dir')
         else:
             build_dir = gn_out_dir
```

### Comparing `pigweed-0.0.8/pw_env_setup/windows_env_start.py` & `pigweed-0.0.9/pw_env_setup/windows_env_start.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_hdlc/decode.py` & `pigweed-0.0.9/pw_hdlc/decode.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_hdlc/encode.py` & `pigweed-0.0.9/pw_hdlc/encode.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_hdlc/protocol.py` & `pigweed-0.0.9/pw_hdlc/protocol.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_hdlc/rpc.py` & `pigweed-0.0.9/pw_hdlc/rpc.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_hdlc/rpc_console.py` & `pigweed-0.0.9/pw_hdlc/rpc_console.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_log/proto/log_pb2.py` & `pigweed-0.0.9/pw_log/proto/log_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='pw_log/proto/log.proto',
   package='pw.log',
   syntax='proto3',
   serialized_options=b'B\003Log',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x16pw_log/proto/log.proto\x12\x06pw.log\x1a\x1fpw_protobuf_protos/common.proto\x1a pw_tokenizer/proto/options.proto\"\xc6\x02\n\x08LogEntry\x12\x1a\n\x07message\x18\x01 \x01(\x0c\x42\x04\x80\xaf&\x00H\x01\x88\x01\x01\x12\x17\n\nline_level\x18\x02 \x01(\rH\x02\x88\x01\x01\x12\x12\n\x05\x66lags\x18\x03 \x01(\rH\x03\x88\x01\x01\x12\x13\n\ttimestamp\x18\x04 \x01(\x03H\x00\x12\x1f\n\x15time_since_last_entry\x18\x05 \x01(\x03H\x00\x12\x14\n\x07\x64ropped\x18\x06 \x01(\rH\x04\x88\x01\x01\x12\x19\n\x06module\x18\x07 \x01(\x0c\x42\x04\x80\xaf&\x00H\x05\x88\x01\x01\x12\x17\n\x04\x66ile\x18\x08 \x01(\x0c\x42\x04\x80\xaf&\x00H\x06\x88\x01\x01\x12\x19\n\x06thread\x18\t \x01(\x0c\x42\x04\x80\xaf&\x00H\x07\x88\x01\x01\x42\x06\n\x04timeB\n\n\x08_messageB\r\n\x0b_line_levelB\x08\n\x06_flagsB\n\n\x08_droppedB\t\n\x07_moduleB\x07\n\x05_fileB\t\n\x07_thread\"\x0c\n\nLogRequest\"q\n\nLogEntries\x12!\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x10.pw.log.LogEntry\x12$\n\x17\x66irst_entry_sequence_id\x18\x02 \x01(\rH\x00\x88\x01\x01\x42\x1a\n\x18_first_entry_sequence_id\"\xd5\x02\n\nFilterRule\x12=\n\x1blevel_greater_than_or_equal\x18\x01 \x01(\x0e\x32\x18.pw.log.FilterRule.Level\x12\x1b\n\rmodule_equals\x18\x02 \x01(\x0c\x42\x04\x80\xaf&\x00\x12\x15\n\rany_flags_set\x18\x03 \x01(\r\x12)\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x19.pw.log.FilterRule.Action\"}\n\x05Level\x12\r\n\tANY_LEVEL\x10\x00\x12\x0f\n\x0b\x44\x45\x42UG_LEVEL\x10\x01\x12\x0e\n\nINFO_LEVEL\x10\x02\x12\x0e\n\nWARN_LEVEL\x10\x03\x12\x0f\n\x0b\x45RROR_LEVEL\x10\x04\x12\x12\n\x0e\x43RITICAL_LEVEL\x10\x05\x12\x0f\n\x0b\x46\x41TAL_LEVEL\x10\x07\"*\n\x06\x41\x63tion\x12\x0c\n\x08INACTIVE\x10\x00\x12\x08\n\x04KEEP\x10\x01\x12\x08\n\x04\x44ROP\x10\x02\"*\n\x06\x46ilter\x12 \n\x04rule\x18\x01 \x03(\x0b\x32\x12.pw.log.FilterRule\"K\n\x10SetFilterRequest\x12\x17\n\tfilter_id\x18\x01 \x01(\x0c\x42\x04\x80\xaf&\x00\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.pw.log.Filter\"+\n\x10GetFilterRequest\x12\x17\n\tfilter_id\x18\x01 \x01(\x0c\x42\x04\x80\xaf&\x00\"\x15\n\x13\x46ilterIdListRequest\"/\n\x14\x46ilterIdListResponse\x12\x17\n\tfilter_id\x18\x01 \x03(\x0c\x42\x04\x80\xaf&\x00\x32:\n\x04Logs\x12\x32\n\x06Listen\x12\x12.pw.log.LogRequest\x1a\x12.pw.log.LogEntries0\x01\x32\xc7\x01\n\x07\x46ilters\x12\x39\n\tSetFilter\x12\x18.pw.log.SetFilterRequest\x1a\x12.pw.protobuf.Empty\x12\x35\n\tGetFilter\x12\x18.pw.log.GetFilterRequest\x1a\x0e.pw.log.Filter\x12J\n\rListFilterIds\x12\x1b.pw.log.FilterIdListRequest\x1a\x1c.pw.log.FilterIdListResponseB\x05\x42\x03Logb\x06proto3'
+  serialized_pb=b'\n\x16pw_log/proto/log.proto\x12\x06pw.log\x1a\x1fpw_protobuf_protos/common.proto\x1a pw_tokenizer/proto/options.proto\"\xe4\x01\n\x08LogEntry\x12\x1a\n\x07message\x18\x01 \x01(\x0c\x42\x04\x80\xaf&\x00H\x01\x88\x01\x01\x12\x12\n\nline_level\x18\x02 \x01(\r\x12\r\n\x05\x66lags\x18\x03 \x01(\r\x12\x13\n\ttimestamp\x18\x04 \x01(\x03H\x00\x12\x1f\n\x15time_since_last_entry\x18\x05 \x01(\x03H\x00\x12\x0f\n\x07\x64ropped\x18\x06 \x01(\r\x12\x14\n\x06module\x18\x07 \x01(\x0c\x42\x04\x80\xaf&\x00\x12\x12\n\x04\x66ile\x18\x08 \x01(\x0c\x42\x04\x80\xaf&\x00\x12\x14\n\x06thread\x18\t \x01(\x0c\x42\x04\x80\xaf&\x00\x42\x06\n\x04timeB\n\n\x08_message\"\x0c\n\nLogRequest\"P\n\nLogEntries\x12!\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x10.pw.log.LogEntry\x12\x1f\n\x17\x66irst_entry_sequence_id\x18\x02 \x01(\r\"\xf2\x02\n\nFilterRule\x12=\n\x1blevel_greater_than_or_equal\x18\x01 \x01(\x0e\x32\x18.pw.log.FilterRule.Level\x12\x1b\n\rmodule_equals\x18\x02 \x01(\x0c\x42\x04\x80\xaf&\x00\x12\x15\n\rany_flags_set\x18\x03 \x01(\r\x12)\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x19.pw.log.FilterRule.Action\x12\x1b\n\rthread_equals\x18\x05 \x01(\x0c\x42\x04\x80\xaf&\x00\"}\n\x05Level\x12\r\n\tANY_LEVEL\x10\x00\x12\x0f\n\x0b\x44\x45\x42UG_LEVEL\x10\x01\x12\x0e\n\nINFO_LEVEL\x10\x02\x12\x0e\n\nWARN_LEVEL\x10\x03\x12\x0f\n\x0b\x45RROR_LEVEL\x10\x04\x12\x12\n\x0e\x43RITICAL_LEVEL\x10\x05\x12\x0f\n\x0b\x46\x41TAL_LEVEL\x10\x07\"*\n\x06\x41\x63tion\x12\x0c\n\x08INACTIVE\x10\x00\x12\x08\n\x04KEEP\x10\x01\x12\x08\n\x04\x44ROP\x10\x02\"*\n\x06\x46ilter\x12 \n\x04rule\x18\x01 \x03(\x0b\x32\x12.pw.log.FilterRule\"K\n\x10SetFilterRequest\x12\x17\n\tfilter_id\x18\x01 \x01(\x0c\x42\x04\x80\xaf&\x00\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.pw.log.Filter\"+\n\x10GetFilterRequest\x12\x17\n\tfilter_id\x18\x01 \x01(\x0c\x42\x04\x80\xaf&\x00\"\x15\n\x13\x46ilterIdListRequest\"/\n\x14\x46ilterIdListResponse\x12\x17\n\tfilter_id\x18\x01 \x03(\x0c\x42\x04\x80\xaf&\x00\x32:\n\x04Logs\x12\x32\n\x06Listen\x12\x12.pw.log.LogRequest\x1a\x12.pw.log.LogEntries0\x01\x32\xc7\x01\n\x07\x46ilters\x12\x39\n\tSetFilter\x12\x18.pw.log.SetFilterRequest\x1a\x12.pw.protobuf.Empty\x12\x35\n\tGetFilter\x12\x18.pw.log.GetFilterRequest\x1a\x0e.pw.log.Filter\x12J\n\rListFilterIds\x12\x1b.pw.log.FilterIdListRequest\x1a\x1c.pw.log.FilterIdListResponseB\x05\x42\x03Logb\x06proto3'
   ,
   dependencies=[pw__protobuf__protos_dot_common__pb2.DESCRIPTOR,pw__tokenizer_dot_proto_dot_options__pb2.DESCRIPTOR,])
 
 
 
 _FILTERRULE_LEVEL = _descriptor.EnumDescriptor(
   name='Level',
@@ -68,16 +68,16 @@
       name='FATAL_LEVEL', index=6, number=7,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=732,
-  serialized_end=857,
+  serialized_start=630,
+  serialized_end=755,
 )
 _sym_db.RegisterEnumDescriptor(_FILTERRULE_LEVEL)
 
 _FILTERRULE_ACTION = _descriptor.EnumDescriptor(
   name='Action',
   full_name='pw.log.FilterRule.Action',
   filename=None,
@@ -98,16 +98,16 @@
       name='DROP', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=859,
-  serialized_end=901,
+  serialized_start=757,
+  serialized_end=799,
 )
 _sym_db.RegisterEnumDescriptor(_FILTERRULE_ACTION)
 
 
 _LOGENTRY = _descriptor.Descriptor(
   name='LogEntry',
   full_name='pw.log.LogEntry',
@@ -196,47 +196,17 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_message', full_name='pw.log.LogEntry._message',
       index=1, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
-    _descriptor.OneofDescriptor(
-      name='_line_level', full_name='pw.log.LogEntry._line_level',
-      index=2, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-    _descriptor.OneofDescriptor(
-      name='_flags', full_name='pw.log.LogEntry._flags',
-      index=3, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-    _descriptor.OneofDescriptor(
-      name='_dropped', full_name='pw.log.LogEntry._dropped',
-      index=4, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-    _descriptor.OneofDescriptor(
-      name='_module', full_name='pw.log.LogEntry._module',
-      index=5, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-    _descriptor.OneofDescriptor(
-      name='_file', full_name='pw.log.LogEntry._file',
-      index=6, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-    _descriptor.OneofDescriptor(
-      name='_thread', full_name='pw.log.LogEntry._thread',
-      index=7, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
   ],
   serialized_start=102,
-  serialized_end=428,
+  serialized_end=330,
 )
 
 
 _LOGREQUEST = _descriptor.Descriptor(
   name='LogRequest',
   full_name='pw.log.LogRequest',
   filename=None,
@@ -252,16 +222,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=430,
-  serialized_end=442,
+  serialized_start=332,
+  serialized_end=344,
 )
 
 
 _LOGENTRIES = _descriptor.Descriptor(
   name='LogEntries',
   full_name='pw.log.LogEntries',
   filename=None,
@@ -290,22 +260,17 @@
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
-    _descriptor.OneofDescriptor(
-      name='_first_entry_sequence_id', full_name='pw.log.LogEntries._first_entry_sequence_id',
-      index=0, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
   ],
-  serialized_start=444,
-  serialized_end=557,
+  serialized_start=346,
+  serialized_end=426,
 )
 
 
 _FILTERRULE = _descriptor.Descriptor(
   name='FilterRule',
   full_name='pw.log.FilterRule',
   filename=None,
@@ -337,30 +302,37 @@
     _descriptor.FieldDescriptor(
       name='action', full_name='pw.log.FilterRule.action', index=3,
       number=4, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='thread_equals', full_name='pw.log.FilterRule.thread_equals', index=4,
+      number=5, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=b'\200\257&\000', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
     _FILTERRULE_LEVEL,
     _FILTERRULE_ACTION,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=560,
-  serialized_end=901,
+  serialized_start=429,
+  serialized_end=799,
 )
 
 
 _FILTER = _descriptor.Descriptor(
   name='Filter',
   full_name='pw.log.Filter',
   filename=None,
@@ -383,16 +355,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=903,
-  serialized_end=945,
+  serialized_start=801,
+  serialized_end=843,
 )
 
 
 _SETFILTERREQUEST = _descriptor.Descriptor(
   name='SetFilterRequest',
   full_name='pw.log.SetFilterRequest',
   filename=None,
@@ -422,16 +394,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=947,
-  serialized_end=1022,
+  serialized_start=845,
+  serialized_end=920,
 )
 
 
 _GETFILTERREQUEST = _descriptor.Descriptor(
   name='GetFilterRequest',
   full_name='pw.log.GetFilterRequest',
   filename=None,
@@ -454,16 +426,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1024,
-  serialized_end=1067,
+  serialized_start=922,
+  serialized_end=965,
 )
 
 
 _FILTERIDLISTREQUEST = _descriptor.Descriptor(
   name='FilterIdListRequest',
   full_name='pw.log.FilterIdListRequest',
   filename=None,
@@ -479,16 +451,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1069,
-  serialized_end=1090,
+  serialized_start=967,
+  serialized_end=988,
 )
 
 
 _FILTERIDLISTRESPONSE = _descriptor.Descriptor(
   name='FilterIdListResponse',
   full_name='pw.log.FilterIdListResponse',
   filename=None,
@@ -511,49 +483,28 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1092,
-  serialized_end=1139,
+  serialized_start=990,
+  serialized_end=1037,
 )
 
 _LOGENTRY.oneofs_by_name['time'].fields.append(
   _LOGENTRY.fields_by_name['timestamp'])
 _LOGENTRY.fields_by_name['timestamp'].containing_oneof = _LOGENTRY.oneofs_by_name['time']
 _LOGENTRY.oneofs_by_name['time'].fields.append(
   _LOGENTRY.fields_by_name['time_since_last_entry'])
 _LOGENTRY.fields_by_name['time_since_last_entry'].containing_oneof = _LOGENTRY.oneofs_by_name['time']
 _LOGENTRY.oneofs_by_name['_message'].fields.append(
   _LOGENTRY.fields_by_name['message'])
 _LOGENTRY.fields_by_name['message'].containing_oneof = _LOGENTRY.oneofs_by_name['_message']
-_LOGENTRY.oneofs_by_name['_line_level'].fields.append(
-  _LOGENTRY.fields_by_name['line_level'])
-_LOGENTRY.fields_by_name['line_level'].containing_oneof = _LOGENTRY.oneofs_by_name['_line_level']
-_LOGENTRY.oneofs_by_name['_flags'].fields.append(
-  _LOGENTRY.fields_by_name['flags'])
-_LOGENTRY.fields_by_name['flags'].containing_oneof = _LOGENTRY.oneofs_by_name['_flags']
-_LOGENTRY.oneofs_by_name['_dropped'].fields.append(
-  _LOGENTRY.fields_by_name['dropped'])
-_LOGENTRY.fields_by_name['dropped'].containing_oneof = _LOGENTRY.oneofs_by_name['_dropped']
-_LOGENTRY.oneofs_by_name['_module'].fields.append(
-  _LOGENTRY.fields_by_name['module'])
-_LOGENTRY.fields_by_name['module'].containing_oneof = _LOGENTRY.oneofs_by_name['_module']
-_LOGENTRY.oneofs_by_name['_file'].fields.append(
-  _LOGENTRY.fields_by_name['file'])
-_LOGENTRY.fields_by_name['file'].containing_oneof = _LOGENTRY.oneofs_by_name['_file']
-_LOGENTRY.oneofs_by_name['_thread'].fields.append(
-  _LOGENTRY.fields_by_name['thread'])
-_LOGENTRY.fields_by_name['thread'].containing_oneof = _LOGENTRY.oneofs_by_name['_thread']
 _LOGENTRIES.fields_by_name['entries'].message_type = _LOGENTRY
-_LOGENTRIES.oneofs_by_name['_first_entry_sequence_id'].fields.append(
-  _LOGENTRIES.fields_by_name['first_entry_sequence_id'])
-_LOGENTRIES.fields_by_name['first_entry_sequence_id'].containing_oneof = _LOGENTRIES.oneofs_by_name['_first_entry_sequence_id']
 _FILTERRULE.fields_by_name['level_greater_than_or_equal'].enum_type = _FILTERRULE_LEVEL
 _FILTERRULE.fields_by_name['action'].enum_type = _FILTERRULE_ACTION
 _FILTERRULE_LEVEL.containing_type = _FILTERRULE
 _FILTERRULE_ACTION.containing_type = _FILTERRULE
 _FILTER.fields_by_name['rule'].message_type = _FILTERRULE
 _SETFILTERREQUEST.fields_by_name['filter'].message_type = _FILTER
 DESCRIPTOR.message_types_by_name['LogEntry'] = _LOGENTRY
@@ -633,27 +584,28 @@
 
 DESCRIPTOR._options = None
 _LOGENTRY.fields_by_name['message']._options = None
 _LOGENTRY.fields_by_name['module']._options = None
 _LOGENTRY.fields_by_name['file']._options = None
 _LOGENTRY.fields_by_name['thread']._options = None
 _FILTERRULE.fields_by_name['module_equals']._options = None
+_FILTERRULE.fields_by_name['thread_equals']._options = None
 _SETFILTERREQUEST.fields_by_name['filter_id']._options = None
 _GETFILTERREQUEST.fields_by_name['filter_id']._options = None
 _FILTERIDLISTRESPONSE.fields_by_name['filter_id']._options = None
 
 _LOGS = _descriptor.ServiceDescriptor(
   name='Logs',
   full_name='pw.log.Logs',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=1141,
-  serialized_end=1199,
+  serialized_start=1039,
+  serialized_end=1097,
   methods=[
   _descriptor.MethodDescriptor(
     name='Listen',
     full_name='pw.log.Logs.Listen',
     index=0,
     containing_service=None,
     input_type=_LOGREQUEST,
@@ -670,16 +622,16 @@
 _FILTERS = _descriptor.ServiceDescriptor(
   name='Filters',
   full_name='pw.log.Filters',
   file=DESCRIPTOR,
   index=1,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=1202,
-  serialized_end=1401,
+  serialized_start=1100,
+  serialized_end=1299,
   methods=[
   _descriptor.MethodDescriptor(
     name='SetFilter',
     full_name='pw.log.Filters.SetFilter',
     index=0,
     containing_service=None,
     input_type=_SETFILTERREQUEST,
```

### Comparing `pigweed-0.0.8/pw_log/proto/log_pb2.pyi` & `pigweed-0.0.9/pw_log/proto/log_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -138,31 +138,19 @@
         timestamp : builtins.int = ...,
         time_since_last_entry : builtins.int = ...,
         dropped : builtins.int = ...,
         module : builtins.bytes = ...,
         file : builtins.bytes = ...,
         thread : builtins.bytes = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"_dropped",b"_dropped",u"_file",b"_file",u"_flags",b"_flags",u"_line_level",b"_line_level",u"_message",b"_message",u"_module",b"_module",u"_thread",b"_thread",u"dropped",b"dropped",u"file",b"file",u"flags",b"flags",u"line_level",b"line_level",u"message",b"message",u"module",b"module",u"thread",b"thread",u"time",b"time",u"time_since_last_entry",b"time_since_last_entry",u"timestamp",b"timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"_dropped",b"_dropped",u"_file",b"_file",u"_flags",b"_flags",u"_line_level",b"_line_level",u"_message",b"_message",u"_module",b"_module",u"_thread",b"_thread",u"dropped",b"dropped",u"file",b"file",u"flags",b"flags",u"line_level",b"line_level",u"message",b"message",u"module",b"module",u"thread",b"thread",u"time",b"time",u"time_since_last_entry",b"time_since_last_entry",u"timestamp",b"timestamp"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_dropped",b"_dropped"]) -> typing.Optional[typing_extensions.Literal["dropped"]]: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_file",b"_file"]) -> typing.Optional[typing_extensions.Literal["file"]]: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_flags",b"_flags"]) -> typing.Optional[typing_extensions.Literal["flags"]]: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_line_level",b"_line_level"]) -> typing.Optional[typing_extensions.Literal["line_level"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal[u"_message",b"_message",u"message",b"message",u"time",b"time",u"time_since_last_entry",b"time_since_last_entry",u"timestamp",b"timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"_message",b"_message",u"dropped",b"dropped",u"file",b"file",u"flags",b"flags",u"line_level",b"line_level",u"message",b"message",u"module",b"module",u"thread",b"thread",u"time",b"time",u"time_since_last_entry",b"time_since_last_entry",u"timestamp",b"timestamp"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_message",b"_message"]) -> typing.Optional[typing_extensions.Literal["message"]]: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_module",b"_module"]) -> typing.Optional[typing_extensions.Literal["module"]]: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_thread",b"_thread"]) -> typing.Optional[typing_extensions.Literal["thread"]]: ...
-    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal[u"time",b"time"]) -> typing.Optional[typing_extensions.Literal["timestamp","time_since_last_entry"]]: ...
 global___LogEntry = LogEntry
 
 class LogRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     def __init__(self,
         ) -> None: ...
@@ -176,17 +164,15 @@
     def entries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LogEntry]: ...
     first_entry_sequence_id: builtins.int = ...
     def __init__(self,
         *,
         entries : typing.Optional[typing.Iterable[global___LogEntry]] = ...,
         first_entry_sequence_id : builtins.int = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"_first_entry_sequence_id",b"_first_entry_sequence_id",u"first_entry_sequence_id",b"first_entry_sequence_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"_first_entry_sequence_id",b"_first_entry_sequence_id",u"entries",b"entries",u"first_entry_sequence_id",b"first_entry_sequence_id"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_first_entry_sequence_id",b"_first_entry_sequence_id"]) -> typing.Optional[typing_extensions.Literal["first_entry_sequence_id"]]: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"entries",b"entries",u"first_entry_sequence_id",b"first_entry_sequence_id"]) -> None: ...
 global___LogEntries = LogEntries
 
 class FilterRule(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     # Log level values match pw_log/levels.h. Enum names avoid collissions with
     # possible macros.
     class Level(_Level, metaclass=_LevelEnumTypeWrapper):
@@ -232,29 +218,33 @@
     # Drop the log entry if all conditions are met
     DROP = FilterRule.Action.V(2)
 
     LEVEL_GREATER_THAN_OR_EQUAL_FIELD_NUMBER: builtins.int
     MODULE_EQUALS_FIELD_NUMBER: builtins.int
     ANY_FLAGS_SET_FIELD_NUMBER: builtins.int
     ACTION_FIELD_NUMBER: builtins.int
+    THREAD_EQUALS_FIELD_NUMBER: builtins.int
     # Condition 1: log.level >= level_greater_than_or_equal.
     level_greater_than_or_equal: global___FilterRule.Level.V = ...
     # Condition 2: (module_equals.size() == 0) || (log.module == module_equals);
     module_equals: builtins.bytes = ...
     # Condition 3: (any_flags_set == 0) || (log.flags & any_flags_set) != 0))
     any_flags_set: builtins.int = ...
     action: global___FilterRule.Action.V = ...
+    # Condition 4: (thread_equals.size() == 0 || log.thread == thread_equals).
+    thread_equals: builtins.bytes = ...
     def __init__(self,
         *,
         level_greater_than_or_equal : global___FilterRule.Level.V = ...,
         module_equals : builtins.bytes = ...,
         any_flags_set : builtins.int = ...,
         action : global___FilterRule.Action.V = ...,
+        thread_equals : builtins.bytes = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"action",b"action",u"any_flags_set",b"any_flags_set",u"level_greater_than_or_equal",b"level_greater_than_or_equal",u"module_equals",b"module_equals"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"action",b"action",u"any_flags_set",b"any_flags_set",u"level_greater_than_or_equal",b"level_greater_than_or_equal",u"module_equals",b"module_equals",u"thread_equals",b"thread_equals"]) -> None: ...
 global___FilterRule = FilterRule
 
 # A filter is a series of rules. First matching rule wins.
 class Filter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     RULE_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `pigweed-0.0.8/pw_log_tokenized/__init__.py` & `pigweed-0.0.9/pw_log_tokenized/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_module/check.py` & `pigweed-0.0.9/pw_module/check.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/git_repo.py` & `pigweed-0.0.9/pw_package/git_repo.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/package_manager.py` & `pigweed-0.0.9/pw_package/package_manager.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/__init__.py` & `pigweed-0.0.9/pw_package/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/arduino_core.py` & `pigweed-0.0.9/pw_package/packages/arduino_core.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/boringssl.py` & `pigweed-0.0.9/pw_package/packages/boringssl.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/chromium_verifier.py` & `pigweed-0.0.9/pw_package/packages/chromium_verifier.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/crlset.py` & `pigweed-0.0.9/pw_package/packages/crlset.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/freertos.py` & `pigweed-0.0.9/pw_package/packages/freertos.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/googletest.py` & `pigweed-0.0.9/pw_package/packages/googletest.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/mbedtls.py` & `pigweed-0.0.9/pw_package/packages/mbedtls.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/micro_ecc.py` & `pigweed-0.0.9/pw_package/packages/micro_ecc.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/nanopb.py` & `pigweed-0.0.9/pw_package/packages/nanopb.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/pico_sdk.py` & `pigweed-0.0.9/pw_package/packages/pico_sdk.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/protobuf.py` & `pigweed-0.0.9/pw_package/packages/protobuf.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/packages/stm32cube.py` & `pigweed-0.0.9/pw_package/packages/stm32cube.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_package/pigweed_packages.py` & `pigweed-0.0.9/pw_package/pigweed_packages.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_presubmit/__init__.py` & `pigweed-0.0.9/pw_presubmit/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_presubmit/build.py` & `pigweed-0.0.9/pw_presubmit/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,37 +100,39 @@
 
 def gn_gen(gn_source_dir: Path,
            gn_output_dir: Path,
            *args: str,
            gn_check: bool = True,
            gn_fail_on_unused: bool = True,
            export_compile_commands: Union[bool, str] = True,
+           preserve_args_gn: bool = False,
            **gn_arguments) -> None:
     """Runs gn gen in the specified directory with optional GN args."""
     args_option = gn_args(**gn_arguments)
 
-    # Delete args.gn to ensure this is a clean build.
-    args_gn = gn_output_dir / 'args.gn'
-    if args_gn.is_file():
-        args_gn.unlink()
+    if not preserve_args_gn:
+        # Delete args.gn to ensure this is a clean build.
+        args_gn = gn_output_dir / 'args.gn'
+        if args_gn.is_file():
+            args_gn.unlink()
 
     export_commands_arg = ''
     if export_compile_commands:
         export_commands_arg = '--export-compile-commands'
         if isinstance(export_compile_commands, str):
             export_commands_arg += f'={export_compile_commands}'
 
     call('gn',
          'gen',
          gn_output_dir,
          '--color=always',
          *(['--fail-on-unused-args'] if gn_fail_on_unused else []),
          *([export_commands_arg] if export_commands_arg else []),
          *args,
-         args_option,
+         *([args_option] if gn_arguments else []),
          cwd=gn_source_dir)
 
     if gn_check:
         call('gn',
              'check',
              gn_output_dir,
              '--check-generated',
@@ -309,15 +311,15 @@
 
     missing: Dict[str, List[Path]] = collections.defaultdict(list)
 
     if bazel_dirs:
         for path in (p for p in files
                      if p.suffix in bazel_extensions_to_check):
             if path not in bazel_builds:
-                # TODO(pwbug/176) Replace this workaround for fuzzers.
+                # TODO(b/234883555) Replace this workaround for fuzzers.
                 if 'fuzz' not in str(path):
                     missing['Bazel'].append(path)
 
     if gn_dirs or gn_build_files:
         for path in (p for p in files if p.suffix in gn_extensions_to_check):
             if path not in gn_builds:
                 missing['GN'].append(path)
```

### Comparing `pigweed-0.0.8/pw_presubmit/cli.py` & `pigweed-0.0.9/pw_presubmit/cli.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_presubmit/cpp_checks.py` & `pigweed-0.0.9/pw_presubmit/cpp_checks.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_presubmit/format_code.py` & `pigweed-0.0.9/pw_presubmit/format_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,17 +279,17 @@
     language: str
     extensions: Collection[str]
     exclude: Collection[str]
     check: Callable[[Iterable], Dict[Path, str]]
     fix: Callable[[Iterable], Dict[Path, str]]
 
 
-CPP_HEADER_EXTS = frozenset(
-    ('.h', '.hpp', '.hxx', '.h++', '.hh', '.H', '.inc', '.inl'))
-CPP_SOURCE_EXTS = frozenset(('.c', '.cpp', '.cxx', '.c++', '.cc', '.C'))
+CPP_HEADER_EXTS = frozenset(('.h', '.hpp', '.hxx', '.h++', '.hh', '.H'))
+CPP_SOURCE_EXTS = frozenset(
+    ('.c', '.cpp', '.cxx', '.c++', '.cc', '.C', '.inc', '.inl'))
 CPP_EXTS = CPP_HEADER_EXTS.union(CPP_SOURCE_EXTS)
 
 C_FORMAT: CodeFormat = CodeFormat('C and C++', CPP_EXTS,
                                   (r'\.pb\.h$', r'\.pb\.c$'),
                                   clang_format_check, clang_format_fix)
 
 PROTO_FORMAT: CodeFormat = CodeFormat('Protocol buffer', ('.proto', ), (),
```

### Comparing `pigweed-0.0.8/pw_presubmit/git_repo.py` & `pigweed-0.0.9/pw_presubmit/git_repo.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_presubmit/inclusive_language.py` & `pigweed-0.0.9/pw_presubmit/inclusive_language.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_presubmit/pigweed_presubmit.py` & `pigweed-0.0.9/pw_presubmit/pigweed_presubmit.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import argparse
 import json
 import logging
 import os
 from pathlib import Path
 import re
+import shutil
 import subprocess
 import sys
 from typing import Sequence, IO, Tuple, Optional, Callable, List
 
 try:
     import pw_presubmit
 except ImportError:
@@ -46,16 +47,18 @@
     filter_paths,
     inclusive_language,
     plural,
     PresubmitContext,
     PresubmitFailure,
     Programs,
     python_checks,
+    shell_checks,
+    npm_presubmit,
 )
-from pw_presubmit.install_hook import install_hook
+from pw_presubmit.install_hook import install_git_hook
 
 _LOG = logging.getLogger(__name__)
 
 pw_package.pigweed_packages.initialize()
 
 # Trigger builds if files with these extensions change.
 _BUILD_EXTENSIONS = ('.py', '.rst', '.gn', '.gni',
@@ -95,30 +98,41 @@
 @filter_paths(endswith=_BUILD_EXTENSIONS)
 def gn_quick_build_check(ctx: PresubmitContext):
     """Checks the state of the GN build by running gn gen and gn check."""
     build.gn_gen(ctx.root, ctx.output_dir)
 
 
 @filter_paths(endswith=_BUILD_EXTENSIONS)
-def gn_full_build_check(ctx: PresubmitContext):
+def gn_full_build_check(ctx: PresubmitContext) -> None:
+    build_targets = [
+        *_at_all_optimization_levels('stm32f429i'),
+        *_at_all_optimization_levels(f'host_{_HOST_COMPILER}'),
+        'python.tests',
+        'python.lint',
+        'docs',
+        'fuzzers',
+        'pw_env_setup:build_pigweed_python_source_tree',
+    ]
+
+    # TODO(b/234645359): Re-enable on Windows when compatibility tests build.
+    if sys.platform != 'win32':
+        build_targets.append('cpp14_compatibility')
+        build_targets.append('cpp20_compatibility')
+
     build.gn_gen(ctx.root, ctx.output_dir)
-    build.ninja(ctx.output_dir, *_at_all_optimization_levels('stm32f429i'),
-                *_at_all_optimization_levels(f'host_{_HOST_COMPILER}'),
-                'python.tests', 'python.lint', 'docs', 'fuzzers',
-                'pw_env_setup:build_pigweed_python_source_tree')
+    build.ninja(ctx.output_dir, *build_targets)
 
 
 @filter_paths(endswith=_BUILD_EXTENSIONS)
 def gn_full_qemu_check(ctx: PresubmitContext):
     build.gn_gen(ctx.root, ctx.output_dir)
     build.ninja(
         ctx.output_dir,
         *_at_all_optimization_levels('qemu_gcc'),
-        # TODO(pwbug/321) Re-enable clang.
-        # *_at_all_optimization_levels('qemu_clang'),
+        *_at_all_optimization_levels('qemu_clang'),
     )
 
 
 @filter_paths(endswith=_BUILD_EXTENSIONS)
 def gn_arm_build(ctx: PresubmitContext):
     build.gn_gen(ctx.root, ctx.output_dir)
     build.ninja(ctx.output_dir, *_at_all_optimization_levels('stm32f429i'))
@@ -316,129 +330,108 @@
 @filter_paths(endswith=(*format_code.C_FORMAT.extensions, '.cmake',
                         'CMakeLists.txt'))
 def cmake_gcc(ctx: PresubmitContext):
     _run_cmake(ctx, toolchain='host_gcc')
     build.ninja(ctx.output_dir, 'pw_apps', 'pw_run_tests.modules')
 
 
-# TODO(pwbug/180): Slowly add modules here that work with bazel until all
-# modules are added. Then replace with //...
-_MODULES_THAT_BUILD_WITH_BAZEL = [
-    '//pw_allocator/...',
-    '//pw_analog/...',
-    '//pw_assert/...',
-    '//pw_assert_basic/...',
-    '//pw_assert_log/...',
-    '//pw_base64/...',
-    '//pw_bloat/...',
-    '//pw_build/...',
-    '//pw_checksum/...',
-    '//pw_chrono_embos/...',
-    '//pw_chrono_freertos/...',
-    '//pw_chrono_stl/...',
-    '//pw_chrono_threadx/...',
-    '//pw_cli/...',
-    '//pw_containers/...',
-    '//pw_cpu_exception/...',
-    '//pw_docgen/...',
-    '//pw_doctor/...',
-    '//pw_env_setup/...',
-    '//pw_fuzzer/...',
-    '//pw_hdlc/java/...',
-    '//pw_hex_dump/...',
-    '//pw_i2c/...',
-    '//pw_interrupt/...',
-    '//pw_interrupt_cortex_m/...',
-    '//pw_libc/...',
-    '//pw_log/...',
-    '//pw_log_basic/...',
-    '//pw_malloc/...',
-    '//pw_malloc_freelist/...',
-    '//pw_multisink/...',
-    '//pw_polyfill/...',
-    '//pw_preprocessor/...',
-    '//pw_protobuf/...',
-    '//pw_protobuf_compiler/...',
-    '//pw_random/...',
-    '//pw_result/...',
-    '//pw_rpc/...',
-    '//pw_span/...',
-    '//pw_status/...',
-    '//pw_stream/...',
-    '//pw_string/...',
-    '//pw_sync_baremetal/...',
-    '//pw_sync_embos/...',
-    '//pw_sync_freertos/...',
-    '//pw_sync_stl/...',
-    '//pw_sync_threadx/...',
-    '//pw_sys_io/...',
-    '//pw_sys_io_baremetal_lm3s6965evb/...',
-    '//pw_sys_io_baremetal_stm32f429/...',
-    '//pw_sys_io_stdio/...',
-    '//pw_thread/...',
-    '//pw_thread_stl/...',
-    '//pw_tokenizer/ts/...',
-    '//pw_tool/...',
-    '//pw_toolchain/...',
-    '//pw_transfer/...',
-    '//pw_unit_test/...',
-    '//pw_varint/...',
-    '//pw_web_ui/...',
-]
-
-# TODO(pwbug/180): Slowly add modules here that work with bazel until all
-# modules are added. Then replace with //...
-_MODULES_THAT_TEST_WITH_BAZEL = [
-    '//pw_allocator/...',
-    '//pw_analog/...',
-    '//pw_assert/...',
-    '//pw_base64/...',
-    '//pw_checksum/...',
-    '//pw_cli/...',
-    '//pw_containers/...',
-    '//pw_hdlc/java/...',
-    '//pw_hex_dump/...',
-    '//pw_i2c/...',
-    '//pw_libc/...',
-    '//pw_log/...',
-    '//pw_multisink/...',
-    '//pw_polyfill/...',
-    '//pw_preprocessor/...',
-    '//pw_protobuf/...',
-    '//pw_protobuf_compiler/...',
-    '//pw_random/...',
-    '//pw_result/...',
-    '//pw_rpc/...',
-    '//pw_span/...',
-    '//pw_status/...',
-    '//pw_stream/...',
-    '//pw_string/...',
-    '//pw_thread/...',
-    '//pw_thread_stl/...',
-    '//pw_tokenizer/ts/...',
-    '//pw_transfer/...',
-    '//pw_unit_test/...',
-    '//pw_varint/...',
-    '//:buildifier_test',
-]
+# TODO(b/235882003): Slowly remove modules from here that work with bazel until
+# no modules remain.
+_MODULES_THAT_DO_NOT_BUILD_WITH_BAZEL = (
+    'docker',
+    'pw_android_toolchain',
+    'pw_arduino_build',
+    'pw_assert_tokenized',
+    'pw_assert_zephyr',
+    'pw_blob_store',
+    'pw_boot',
+    'pw_build_mcuxpresso',
+    'pw_bytes',
+    'pw_chrono_zephyr',
+    'pw_console',
+    'pw_cpu_exception_cortex_m',
+    'pw_crypto',
+    'pw_file',
+    'pw_function',
+    'pw_hdlc',
+    'pw_i2c_mcuxpresso',
+    'pw_interrupt_zephyr',
+    'pw_kvs',
+    'pw_log_android',
+    'pw_log_null',
+    'pw_log_rpc',
+    'pw_log_string',
+    'pw_log_tokenized',
+    'pw_log_zephyr',
+    'pw_metric',
+    'pw_minimal_cpp_stdlib',
+    'pw_module',
+    'pw_package',
+    'pw_persistent_ram',
+    'pw_presubmit',
+    'pw_ring_buffer',
+    'pw_software_update',
+    'pw_spi',
+    'pw_stm32cube_build',
+    'pw_sync_zephyr',
+    'pw_sys_io_arduino',
+    'pw_sys_io_mcuxpresso',
+    'pw_sys_io_stm32cube',
+    'pw_sys_io_zephyr',
+    'pw_system',
+    'pw_target_runner',
+    'pw_thread_embos',
+    'pw_thread_freertos',
+    'pw_thread_threadx',
+    'pw_tls_client',
+    'pw_tls_client_boringssl',
+    'pw_tls_client_mbedtls',
+    'pw_trace',
+    'pw_trace_tokenized',
+    'pw_watch',
+    'pw_web_ui',
+    'pw_work_queue',
+)
+
+# TODO(b/235882003): Slowly remove modules from here that work with bazel until
+# no modules remain.
+_MODULES_THAT_DO_NOT_TEST_WITH_BAZEL = _MODULES_THAT_DO_NOT_BUILD_WITH_BAZEL + (
+    'pw_malloc_freelist', )
+
+
+def all_modules():
+    return Path(os.environ['PW_ROOT'],
+                'PIGWEED_MODULES').read_text().splitlines()
 
 
 @filter_paths(endswith=(*format_code.C_FORMAT.extensions, '.bazel', '.bzl',
                         'BUILD'))
 def bazel_test(ctx: PresubmitContext) -> None:
     """Runs bazel test on each bazel compatible module"""
-    build.bazel(ctx, 'test', *_MODULES_THAT_TEST_WITH_BAZEL,
-                '--test_output=errors')
+    # TODO(b/231256840): Instead of relying on PIGWEED_MODULES it would be nicer
+    # to do something like `bazel build //... -//pw_boot -//pw_system`. This
+    # doesn't quite work; see bug.
+    modules = list()
+    for module in all_modules():
+        if module in _MODULES_THAT_DO_NOT_TEST_WITH_BAZEL:
+            continue
+        modules.append(f'//{module}/...:all')
+    build.bazel(ctx, 'test', *modules, '--test_output=errors')
 
 
 @filter_paths(endswith=(*format_code.C_FORMAT.extensions, '.bazel', '.bzl',
                         'BUILD'))
 def bazel_build(ctx: PresubmitContext) -> None:
     """Runs Bazel build on each Bazel compatible module."""
-    build.bazel(ctx, 'build', *_MODULES_THAT_BUILD_WITH_BAZEL)
+    modules = list()
+    for module in all_modules():
+        if module in _MODULES_THAT_DO_NOT_BUILD_WITH_BAZEL:
+            continue
+        modules.append(f'//{module}/...:all')
+    build.bazel(ctx, 'build', *modules)
 
 
 def pw_transfer_integration_test(ctx: PresubmitContext) -> None:
     """Runs the pw_transfer cross-language integration test only.
 
     This test is not part of the regular bazel build because it's slow and
     intended to run in CI only.
@@ -544,14 +537,15 @@
     r'\bOWNERS$',
     r'\bPIGWEED_MODULES$',
     r'\brequirements.txt$',
     r'\bgo.(mod|sum)$',
     r'\bpackage.json$',
     r'\byarn.lock$',
     # Data files
+    r'\.bin$',
     r'\.elf$',
     r'\.gif$',
     r'\.jpg$',
     r'\.json$',
     r'\.png$',
     r'\.svg$',
     r'\.xml$',
@@ -789,15 +783,15 @@
 #
 
 OTHER_CHECKS = (
     cpp_checks.all_sanitizers(),
     # Build that attempts to duplicate the build OSS-Fuzz does. Currently
     # failing.
     oss_fuzz_build,
-    # TODO(pwbug/346): Enable all Bazel tests when they're fixed.
+    # TODO(b/235277910): Enable all Bazel tests when they're fixed.
     bazel_test,
     cmake_clang,
     cmake_gcc,
     gn_boringssl_build,
     build.gn_gen_check,
     gn_nanopb_build,
     gn_crypto_mbedtls_build,
@@ -809,37 +803,39 @@
     gn_clang_build,
     gn_gcc_build,
     gn_pw_system_demo_build,
     pw_transfer_integration_test,
     renode_check,
     static_analysis,
     stm32f429i,
+    npm_presubmit.npm_test,
 )
 
 _LINTFORMAT = (
     commit_message_format,
     copyright_notice,
     format_code.presubmit_checks(),
     inclusive_language.inclusive_language.with_filter(
         exclude=(r'\byarn.lock$', )),
     cpp_checks.pragma_once,
     build.bazel_lint,
     source_is_in_build_files,
+    shell_checks.shellcheck if shutil.which('shellcheck') else (),
 )
 
 LINTFORMAT = (
     _LINTFORMAT,
     pw_presubmit.python_checks.check_python_versions,
     pw_presubmit.python_checks.gn_python_lint,
 )
 
 QUICK = (
     _LINTFORMAT,
     gn_quick_build_check,
-    # TODO(pwbug/141): Re-enable CMake and Bazel for Mac after we have fixed the
+    # TODO(b/34884583): Re-enable CMake and Bazel for Mac after we have fixed
     # the clang issues. The problem is that all clang++ invocations need the
     # two extra flags: "-nostdc++" and "${clang_prefix}/../lib/libc++.a".
     cmake_clang if sys.platform != 'darwin' else (),
 )
 
 FULL = (
     _LINTFORMAT,
@@ -886,19 +882,18 @@
     return parser.parse_args()
 
 
 def run(install: bool, **presubmit_args) -> int:
     """Entry point for presubmit."""
 
     if install:
-        # TODO(pwbug/209, pwbug/386) inclusive-language: disable
-        install_hook(__file__, 'pre-push',
-                     ['--base', 'origin/master..HEAD', '--program', 'quick'],
-                     Path.cwd())
-        # TODO(pwbug/209, pwbug/386) inclusive-language: enable
+        install_git_hook('pre-push', [
+            'python', '-m', 'pw_presubmit.pigweed_presubmit', '--base',
+            'origin/main..HEAD', '--program', 'quick'
+        ])
         return 0
 
     return cli.run(**presubmit_args)
 
 
 def main() -> int:
     """Run the presubmit for the Pigweed repository."""
```

### Comparing `pigweed-0.0.8/pw_presubmit/presubmit.py` & `pigweed-0.0.9/pw_presubmit/presubmit.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,18 +425,23 @@
         keep_going: whether to continue running checks if an error occurs
 
     Returns:
         True if all presubmit checks succeeded
     """
     repos = [repo.resolve() for repo in repos]
 
+    non_empty_repos = []
     for repo in repos:
-        if git_repo.root(repo) != repo:
-            raise ValueError(f'{repo} is not the root of a Git repo; '
-                             'presubmit checks must be run from a Git repo')
+        if list(repo.iterdir()):
+            non_empty_repos.append(repo)
+            if git_repo.root(repo) != repo:
+                raise ValueError(
+                    f'{repo} is not the root of a Git repo; '
+                    'presubmit checks must be run from a Git repo')
+    repos = non_empty_repos
 
     pathspecs_by_repo = _process_pathspecs(repos, paths)
 
     files: List[Path] = []
 
     for repo, pathspecs in pathspecs_by_repo.items():
         files += tools.exclude_paths(
```

### Comparing `pigweed-0.0.8/pw_presubmit/python_checks.py` & `pigweed-0.0.9/pw_presubmit/python_checks.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_presubmit/tools.py` & `pigweed-0.0.9/pw_presubmit/tools.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf/codegen_pwpb.py` & `pigweed-0.0.9/pw_protobuf/codegen_pwpb.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 """This module defines the generated code for pw_protobuf C++ classes."""
 
 import abc
-from datetime import datetime
 import enum
 # Type ignore here for graphlib-backport on Python 3.8
 from graphlib import CycleError, TopologicalSorter  # type: ignore
 from itertools import takewhile
 import os
 import sys
 from typing import Dict, Iterable, List, Optional, Tuple
@@ -253,15 +252,15 @@
         return '::pw::Result<{}>'.format(self._result_type())
 
     def _result_type(self) -> str:
         """The type returned by the deoder function.
 
         Defined in subclasses.
 
-        e.g. 'uint32_t', 'std::span<std::byte>', etc.
+        e.g. 'uint32_t', 'pw::span<std::byte>', etc.
         """
         raise NotImplementedError()
 
     def body(self) -> List[str]:
         lines: List[str] = []
         lines += ['::pw::Result<uint32_t> field_number = FieldNumber();']
         lines += ['PW_ASSERT(field_number.ok());']
@@ -303,15 +302,15 @@
     def should_appear(self) -> bool:
         return self._field.is_repeated()
 
     def return_type(self, from_root: bool = False) -> str:
         return '::pw::StatusWithSize'
 
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<{}>'.format(self._result_type()), 'out')]
+        return [('pw::span<{}>'.format(self._result_type()), 'out')]
 
 
 class PackedReadVectorMethod(ReadMethod):
     """A method for a reading a packed repeated field.
 
     An alternative to ReadMethod for repeated fields that appends values into
     a pw::Vector.
@@ -325,15 +324,15 @@
     def params(self) -> List[Tuple[str, str]]:
         return [('::pw::Vector<{}>&'.format(self._result_type()), 'out')]
 
 
 class MessageProperty(ProtoMember):
     """Base class for a C++ property for a field in a protobuf message."""
     def name(self) -> str:
-        return self._field.enum_name().lower()
+        return self._field.field_name()
 
     def should_appear(self) -> bool:
         return True
 
     @abc.abstractmethod
     def type_name(self, from_root: bool = False) -> str:
         """Returns the type of the property, e.g. uint32_t."""
@@ -352,14 +351,19 @@
     def use_callback(self) -> bool:  # pylint: disable=no-self-use
         """Returns whether the decoder should use a callback."""
         options = self._field.options()
         assert options is not None
         return options.use_callback or (self._field.is_repeated()
                                         and self.max_size() == 0)
 
+    def is_optional(self) -> bool:
+        """Returns whether the decoder should use std::optional."""
+        return (self._field.is_optional() and self.max_size() == 0
+                and self.wire_type() != 'kDelimited')
+
     def max_size(self) -> int:
         """Returns the maximum size of the field."""
         if self._field.is_repeated():
             options = self._field.options()
             assert options is not None
             return options.max_count
 
@@ -379,14 +383,19 @@
 
     def struct_member(self, from_root: bool = False) -> Tuple[str, str]:
         """Returns the structure member."""
         if self.use_callback():
             return (f'{PROTOBUF_NAMESPACE}::Callback'
                     '<StreamEncoder, StreamDecoder>', self.name())
 
+        # Optional fields are wrapped in std::optional
+        if self.is_optional():
+            return ('std::optional<{}>'.format(self.type_name(from_root)),
+                    self.name())
+
         # Non-repeated fields have a member of just the type name.
         max_size = self.max_size()
         if max_size == 0:
             return (self.type_name(from_root), self.name())
 
         # Fixed size fields use std::array.
         if self.fixed_size():
@@ -415,14 +424,15 @@
         return [
             self.field_cast(),
             self._wire_type_table_entry(),
             self._elem_size_table_entry(),
             self._varint_type_table_entry(),
             'true' if self.fixed_size() else 'false',
             'true' if self._field.is_repeated() else 'false',
+            'true' if self.is_optional() else 'false',
             'true' if self.use_callback() else 'false',
             'offsetof(Message, {})'.format(self.name()),
             'sizeof(Message::{})'.format(self.name()),
             self.sub_table(),
         ]
 
     @abc.abstractmethod
@@ -583,15 +593,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteDouble'
 
 
 class PackedDoubleWriteMethod(PackedWriteMethod):
     """Method which writes a packed list of doubles."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const double>', 'values')]
+        return [('pw::span<const double>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedDouble'
 
 
 class PackedDoubleWriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of doubles."""
@@ -649,15 +659,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteFloat'
 
 
 class PackedFloatWriteMethod(PackedWriteMethod):
     """Method which writes a packed list of floats."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const float>', 'values')]
+        return [('pw::span<const float>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedFloat'
 
 
 class PackedFloatWriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of floats."""
@@ -715,15 +725,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteInt32'
 
 
 class PackedInt32WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of int32."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const int32_t>', 'values')]
+        return [('pw::span<const int32_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedInt32'
 
 
 class PackedInt32WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of int32."""
@@ -784,15 +794,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteSint32'
 
 
 class PackedSint32WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of sint32."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const int32_t>', 'values')]
+        return [('pw::span<const int32_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedSint32'
 
 
 class PackedSint32WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of sint32."""
@@ -853,15 +863,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteSfixed32'
 
 
 class PackedSfixed32WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of sfixed32."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const int32_t>', 'values')]
+        return [('pw::span<const int32_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedSfixed32'
 
 
 class PackedSfixed32WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of sfixed32."""
@@ -919,15 +929,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteInt64'
 
 
 class PackedInt64WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of int64."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const int64_t>', 'values')]
+        return [('pw::span<const int64_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedInt64'
 
 
 class PackedInt64WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of int64."""
@@ -988,15 +998,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteSint64'
 
 
 class PackedSint64WriteMethod(PackedWriteMethod):
     """Method which writes a packst list of sint64."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const int64_t>', 'values')]
+        return [('pw::span<const int64_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedSint64'
 
 
 class PackedSint64WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of sint64."""
@@ -1057,15 +1067,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteSfixed64'
 
 
 class PackedSfixed64WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of sfixed64."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const int64_t>', 'values')]
+        return [('pw::span<const int64_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedSfixed4'
 
 
 class PackedSfixed64WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of sfixed64."""
@@ -1123,15 +1133,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteUint32'
 
 
 class PackedUint32WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of uint32."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const uint32_t>', 'values')]
+        return [('pw::span<const uint32_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedUint32'
 
 
 class PackedUint32WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of uint32."""
@@ -1192,15 +1202,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteFixed32'
 
 
 class PackedFixed32WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of fixed32."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const uint32_t>', 'values')]
+        return [('pw::span<const uint32_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedFixed32'
 
 
 class PackedFixed32WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of fixed32."""
@@ -1258,15 +1268,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteUint64'
 
 
 class PackedUint64WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of uint64."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const uint64_t>', 'values')]
+        return [('pw::span<const uint64_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedUint64'
 
 
 class PackedUint64WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of uint64."""
@@ -1327,15 +1337,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteFixed64'
 
 
 class PackedFixed64WriteMethod(PackedWriteMethod):
     """Method which writes a packed list of fixed64."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const uint64_t>', 'values')]
+        return [('pw::span<const uint64_t>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedFixed64'
 
 
 class PackedFixed64WriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed list of fixed64."""
@@ -1393,15 +1403,15 @@
     def _encoder_fn(self) -> str:
         return 'WriteBool'
 
 
 class PackedBoolWriteMethod(PackedWriteMethod):
     """Method which writes a packed list of bools."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const bool>', 'values')]
+        return [('pw::span<const bool>', 'values')]
 
     def _encoder_fn(self) -> str:
         return 'WritePackedBool'
 
 
 class PackedBoolWriteVectorMethod(PackedWriteMethod):
     """Method which writes a packed vector of bools."""
@@ -1444,27 +1454,27 @@
     def _size_fn(self) -> str:
         return 'SizeOfFieldBool'
 
 
 class BytesWriteMethod(WriteMethod):
     """Method which writes a proto bytes value."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const std::byte>', 'value')]
+        return [('pw::span<const std::byte>', 'value')]
 
     def _encoder_fn(self) -> str:
         return 'WriteBytes'
 
 
 class BytesReadMethod(ReadMethod):
     """Method which reads a proto bytes value."""
     def return_type(self, from_root: bool = False) -> str:
         return '::pw::StatusWithSize'
 
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<std::byte>', 'out')]
+        return [('pw::span<std::byte>', 'out')]
 
     def _decoder_fn(self) -> str:
         return 'ReadBytes'
 
 
 class BytesProperty(MessageProperty):
     """Property which holds a proto bytes value."""
@@ -1525,15 +1535,15 @@
 
 class StringReadMethod(ReadMethod):
     """Method which reads a proto string value."""
     def return_type(self, from_root: bool = False) -> str:
         return '::pw::StatusWithSize'
 
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<char>', 'out')]
+        return [('pw::span<char>', 'out')]
 
     def _decoder_fn(self) -> str:
         return 'ReadString'
 
 
 class StringProperty(MessageProperty):
     """Property which holds a proto string value."""
@@ -1586,22 +1596,22 @@
     def _encoder_fn(self) -> str:
         raise NotImplementedError()
 
 
 class PackedEnumWriteMethod(PackedWriteMethod):
     """Method which writes a packed list of enum."""
     def params(self) -> List[Tuple[str, str]]:
-        return [('std::span<const {}>'.format(self._relative_type_namespace()),
+        return [('pw::span<const {}>'.format(self._relative_type_namespace()),
                  'values')]
 
     def body(self) -> List[str]:
         value_param = self.params()[0][1]
         line = (
             f'return {self._base_class}::WritePackedUint32('
-            f'{self.field_cast()}, std::span(reinterpret_cast<const uint32_t*>('
+            f'{self.field_cast()}, pw::span(reinterpret_cast<const uint32_t*>('
             f'{value_param}.data()), {value_param}.size()));')
         return [line]
 
     def in_class_definition(self) -> bool:
         return True
 
     def _encoder_fn(self) -> str:
@@ -1638,15 +1648,15 @@
     def _result_type(self):
         return self._relative_type_namespace()
 
     def _decoder_body(self) -> List[str]:
         value_param = self.params()[0][1]
         return [
             f'return ReadPackedUint32('
-            f'std::span(reinterpret_cast<uint32_t*>({value_param}.data()), '
+            f'pw::span(reinterpret_cast<uint32_t*>({value_param}.data()), '
             f'{value_param}.size()));'
         ]
 
 
 class PackedEnumReadVectorMethod(PackedReadVectorMethod):
     """Method which reads packed enum values."""
     def _result_type(self):
@@ -1857,25 +1867,25 @@
         # Generate entry for message table read or write methods.
         if class_type == ClassType.STREAMING_DECODER:
             output.write_line()
             output.write_line('::pw::Status Read(Message& message) {')
             with output.indent():
                 output.write_line(
                     f'return {base_class}::Read('
-                    'std::as_writable_bytes(std::span(&message, 1)), '
+                    'pw::as_writable_bytes(pw::span(&message, 1)), '
                     'kMessageFields);')
             output.write_line('}')
         elif class_type in (ClassType.STREAMING_ENCODER,
                             ClassType.MEMORY_ENCODER):
             output.write_line()
             output.write_line('::pw::Status Write(const Message& message) {')
             with output.indent():
                 output.write_line(
                     f'return {base_class}::Write('
-                    'std::as_bytes(std::span(&message, 1)), kMessageFields);')
+                    'pw::as_bytes(pw::span(&message, 1)), kMessageFields);')
             output.write_line('}')
 
         # Generate methods for each of the message's fields.
         for field in message.fields():
             for method_class in proto_field_methods(class_type, field.type()):
                 method = method_class(field, message, root, base_class)
                 if not method.should_appear():
@@ -2110,17 +2120,18 @@
         for prop in properties:
             table = ', '.join(prop.table_entry())
             output.write_line(f'{{{table}}},')
 
     output.write_line('};')
     output.write_line('PW_MODIFY_DIAGNOSTICS_POP();')
 
-    output.write_line('inline constexpr std::span<const {}::MessageField> '
-                      'kMessageFields = {{ _kMessageFields, {} }};'.format(
-                          PROTOBUF_NAMESPACE, len(properties)))
+    output.write_line(
+        'inline constexpr pw::span<const {}::MessageField> '
+        'kMessageFields = {{ _kMessageFields, size_t({}) }};'.format(
+            PROTOBUF_NAMESPACE, len(properties)))
 
     output.write_line(f'}}  // namespace {namespace}')
 
 
 def generate_sizes_for_message(message: ProtoMessage, root: ProtoNode,
                                output: OutputFile) -> None:
     """Creates C++ constants for the encoded sizes of a protobuf message."""
@@ -2204,21 +2215,21 @@
                               output: OutputFile) -> None:
     """Generates code for a single .pb.h file corresponding to a .proto file."""
 
     assert package.type() == ProtoNode.Type.PACKAGE
 
     output.write_line(f'// {os.path.basename(output.name())} automatically '
                       f'generated by {PLUGIN_NAME} {PLUGIN_VERSION}')
-    output.write_line(f'// on {datetime.now()}')
     output.write_line('#pragma once\n')
     output.write_line('#include <algorithm>')
     output.write_line('#include <array>')
     output.write_line('#include <cstddef>')
     output.write_line('#include <cstdint>')
-    output.write_line('#include <span>')
+    output.write_line('#include <optional>')
+    output.write_line('#include "pw_span/span.h"')
     output.write_line('#include <string_view>\n')
     output.write_line('#include "pw_assert/assert.h"')
     output.write_line('#include "pw_containers/vector.h"')
     output.write_line('#include "pw_preprocessor/compiler.h"')
     output.write_line('#include "pw_protobuf/encoder.h"')
     output.write_line('#include "pw_protobuf/internal/codegen.h"')
     output.write_line('#include "pw_protobuf/serialized_size.h"')
@@ -2287,14 +2298,14 @@
 def process_proto_file(proto_file, proto_options) -> Iterable[OutputFile]:
     """Generates code for a single .proto file."""
 
     # Two passes are made through the file. The first builds the tree of all
     # message/enum nodes, then the second creates the fields in each. This is
     # done as non-primitive fields need pointers to their types, which requires
     # the entire tree to have been parsed into memory.
-    _, package_root = build_node_tree(proto_file, proto_options)
+    _, package_root = build_node_tree(proto_file, proto_options=proto_options)
 
     output_filename = _proto_filename_to_generated_header(proto_file.name)
     output_file = OutputFile(output_filename)
     generate_code_for_package(proto_file, package_root, output_file)
 
     return [output_file]
```

### Comparing `pigweed-0.0.8/pw_protobuf/options.py` & `pigweed-0.0.9/pw_protobuf/options.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf/output_file.py` & `pigweed-0.0.9/pw_protobuf/output_file.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf/plugin.py` & `pigweed-0.0.9/pw_protobuf/plugin.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf/proto_tree.py` & `pigweed-0.0.9/pw_protobuf/proto_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import enum
 
 from typing import Callable, Dict, Iterator, List, Optional, Tuple, TypeVar
 from typing import cast
 
 from google.protobuf import descriptor_pb2
 
-from pw_protobuf import options
+from pw_protobuf import options, symbol_name_mapping
 from pw_protobuf_codegen_protos.options_pb2 import Options
 
 T = TypeVar('T')  # pylint: disable=invalid-name
 
 
 class ProtoNode(abc.ABC):
     """A ProtoNode represents a C++ scope mapping of an entity in a .proto file.
@@ -62,15 +62,16 @@
         return list(self._children.values())
 
     def name(self) -> str:
         return self._name
 
     def cpp_name(self) -> str:
         """The name of this node in generated C++ code."""
-        return self._name.replace('.', '::')
+        return symbol_name_mapping.fix_cc_identifier(self._name).replace(
+            '.', '::')
 
     def cpp_namespace(self, root: Optional['ProtoNode'] = None) -> str:
         """C++ namespace of the node, up to the specified root."""
         return '::'.join(name for name in self._attr_hierarchy(
             lambda node: node.cpp_name(), root) if name)
 
     def proto_path(self) -> str:
@@ -156,15 +157,19 @@
             del child._parent._children[child.name()]
 
         child._parent = self
         self._children[child.name()] = child
         # pylint: enable=protected-access
 
     def find(self, path: str) -> Optional['ProtoNode']:
-        """Finds a node within this node's subtree."""
+        """Finds a node within this node's subtree.
+
+        Args:
+          path: The path to the sought node.
+        """
         node = self
 
         # pylint: disable=protected-access
         for section in path.split('.'):
             child = node._children.get(section)
             if child is None:
                 return None
@@ -225,15 +230,19 @@
     def type(self) -> ProtoNode.Type:
         return ProtoNode.Type.ENUM
 
     def values(self) -> List[Tuple[str, int]]:
         return list(self._values)
 
     def add_value(self, name: str, value: int) -> None:
-        self._values.append((ProtoMessageField.upper_snake_case(name), value))
+        self._values.append((
+            ProtoMessageField.upper_snake_case(
+                symbol_name_mapping.fix_cc_enum_value_name(name)),
+            value,
+        ))
 
     def _supports_child(self, child: ProtoNode) -> bool:
         # Enums cannot have nested children.
         return False
 
 
 class ProtoMessage(ProtoNode):
@@ -322,51 +331,58 @@
 class ProtoMessageField:
     """Representation of a field within a protobuf message."""
     def __init__(self,
                  field_name: str,
                  field_number: int,
                  field_type: int,
                  type_node: Optional[ProtoNode] = None,
+                 optional: bool = False,
                  repeated: bool = False,
                  field_options: Optional[Options] = None):
-        self._field_name = field_name
+        self._field_name = symbol_name_mapping.fix_cc_identifier(field_name)
         self._number: int = field_number
         self._type: int = field_type
         self._type_node: Optional[ProtoNode] = type_node
+        self._optional: bool = optional
         self._repeated: bool = repeated
         self._options: Optional[Options] = field_options
 
     def name(self) -> str:
         return self.upper_camel_case(self._field_name)
 
+    def field_name(self) -> str:
+        return self._field_name
+
     def enum_name(self) -> str:
-        return self.upper_snake_case(self._field_name)
+        return self.upper_snake_case(
+            symbol_name_mapping.fix_cc_enum_value_name(self._field_name))
 
     def number(self) -> int:
         return self._number
 
     def type(self) -> int:
         return self._type
 
     def type_node(self) -> Optional[ProtoNode]:
         return self._type_node
 
+    def is_optional(self) -> bool:
+        return self._optional
+
     def is_repeated(self) -> bool:
         return self._repeated
 
     def options(self) -> Optional[Options]:
         return self._options
 
     @staticmethod
     def upper_camel_case(field_name: str) -> str:
         """Converts a field name to UpperCamelCase."""
         name_components = field_name.split('_')
-        for i, _ in enumerate(name_components):
-            name_components[i] = name_components[i].lower().capitalize()
-        return ''.join(name_components)
+        return ''.join([word.lower().capitalize() for word in name_components])
 
     @staticmethod
     def upper_snake_case(field_name: str) -> str:
         """Converts a field name to UPPER_SNAKE_CASE."""
         return field_name.upper()
 
 
@@ -474,22 +490,23 @@
             # field's type object, for example ".pw.protobuf.test.KeyValuePair".
             # Try to find the node for this object within the current context.
             type_node = _find_or_create_node(global_root, package_root,
                                              field.type_name)
         else:
             type_node = None
 
+        optional = field.proto3_optional
         repeated = \
             field.label == descriptor_pb2.FieldDescriptorProto.LABEL_REPEATED
         field_options = options.match_options(
             '.'.join((message.proto_path(), field.name)),
             proto_options) if proto_options is not None else None
         message.add_field(
             ProtoMessageField(field.name, field.number, field.type, type_node,
-                              repeated, field_options))
+                              optional, repeated, field_options))
 
 
 def _add_service_methods(global_root: ProtoNode, package_root: ProtoNode,
                          service: ProtoNode, proto_service) -> None:
     assert service.type() == ProtoNode.Type.SERVICE
     service = cast(ProtoService, service)
```

### Comparing `pigweed-0.0.8/pw_protobuf_codegen_protos/options_pb2.py` & `pigweed-0.0.9/pw_protobuf_codegen_protos/options_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_codegen_protos/options_pb2.pyi` & `pigweed-0.0.9/pw_protobuf_codegen_protos/options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_compiler/generate_protos.py` & `pigweed-0.0.9/pw_protobuf_compiler/generate_protos.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_compiler/proto_target_invalid.py` & `pigweed-0.0.9/pw_protobuf_compiler/proto_target_invalid.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_compiler/python_protos.py` & `pigweed-0.0.9/pw_protobuf_compiler/python_protos.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,38 @@
 import subprocess
 import shlex
 import tempfile
 from types import ModuleType
 from typing import (Dict, Generic, Iterable, Iterator, List, NamedTuple, Set,
                     Tuple, TypeVar, Union)
 
+# Temporarily set the root logger level to critical while importing yapf.
+# This silences INFO level messages from
+# .environment/cipd/packages/python/lib/python3.9/lib2to3/driver.py
+# when it writes Grammar3.*.pickle and PatternGrammar3.*.pickle files.
+_original_level = 0
+for handler in logging.getLogger().handlers:
+    if type(handler) == logging.StreamHandler:  # pylint: disable=unidiomatic-typecheck
+        if handler.level > _original_level:
+            _original_level = handler.level
+        handler.level = logging.CRITICAL
+
+try:
+    from yapf.yapflib import yapf_api  # type: ignore[import] # pylint: disable=wrong-import-position
+except ImportError:
+    yapf_api = None
+
+# Restore the original stderr/out log handler level.
+for handler in logging.getLogger().handlers:
+    # Must use type() check here since isinstance returns True for FileHandlers
+    # and StreamHandler: isinstance(logging.FileHandler, logging.StreamHandler)
+    if type(handler) == logging.StreamHandler:  # pylint: disable=unidiomatic-typecheck
+        handler.level = _original_level
+del _original_level
+
 _LOG = logging.getLogger(__name__)
 
 PathOrStr = Union[Path, str]
 
 
 def compile_protos(
     output_dir: PathOrStr,
@@ -390,10 +414,25 @@
             else:
                 values = ', '.join(_field_repr(field, v) for v in value)
                 yield f'{field.name}=[{values}]'
         else:
             yield f'{field.name}={_field_repr(field, value)}'
 
 
-def proto_repr(message) -> str:
-    """Creates a repr-like string for a protobuf."""
-    return f'{message.DESCRIPTOR.full_name}({", ".join(_proto_repr(message))})'
+def proto_repr(message, *, wrap: bool = True) -> str:
+    """Creates a repr-like string for a protobuf.
+
+    In an interactive console that imports proto objects into the namespace, the
+    output of proto_repr() can be used as Python source to create a proto
+    object.
+
+    Args:
+      message: The protobuf message to format
+      wrap: If true and YAPF is available, the output is wrapped according to
+          PEP8 using YAPF.
+    """
+    raw = f'{message.DESCRIPTOR.full_name}({", ".join(_proto_repr(message))})'
+
+    if wrap and yapf_api is not None:
+        return yapf_api.FormatCode(raw, style_config='PEP8')[0].rstrip()
+
+    return raw
```

### Comparing `pigweed-0.0.8/pw_protobuf_compiler_protos/nested/more_nesting/test_pb2.py` & `pigweed-0.0.9/pw_protobuf_compiler_protos/nested/more_nesting/test_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_compiler_protos/nested/more_nesting/test_pb2.pyi` & `pigweed-0.0.9/pw_protobuf_compiler_protos/nested/more_nesting/test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_compiler_protos/test_pb2.py` & `pigweed-0.0.9/pw_protobuf_compiler_protos/test_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_compiler_protos/test_pb2.pyi` & `pigweed-0.0.9/pw_protobuf_compiler_protos/test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_protos/common_pb2.py` & `pigweed-0.0.9/pw_protobuf_protos/common_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_protos/status_pb2.py` & `pigweed-0.0.9/pw_protobuf_protos/status_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_protobuf_protos/status_pb2.pyi` & `pigweed-0.0.9/pw_protobuf_protos/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/__init__.py` & `pigweed-0.0.9/pw_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/benchmark_pb2.py` & `pigweed-0.0.9/pw_rpc/benchmark_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/benchmark_pb2.pyi` & `pigweed-0.0.9/pw_rpc/benchmark_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/callback_client/__init__.py` & `pigweed-0.0.9/pw_rpc/callback_client/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/callback_client/call.py` & `pigweed-0.0.9/pw_rpc/callback_client/call.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/callback_client/errors.py` & `pigweed-0.0.9/pw_rpc/callback_client/errors.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/callback_client/impl.py` & `pigweed-0.0.9/pw_rpc/callback_client/impl.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/client.py` & `pigweed-0.0.9/pw_rpc/client.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/codegen.py` & `pigweed-0.0.9/pw_rpc/codegen.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/codegen_nanopb.py` & `pigweed-0.0.9/pw_rpc/codegen_nanopb.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/codegen_pwpb.py` & `pigweed-0.0.9/pw_rpc/codegen_pwpb.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/codegen_raw.py` & `pigweed-0.0.9/pw_rpc/codegen_raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,14 +129,27 @@
             self.indented_list(*args,
                                'std::move(on_completed)',
                                'std::move(on_error)',
                                end=');')
 
         self.line('}')
 
+    def method_info_specialization(self, method: ProtoServiceMethod) -> None:
+        self.line()
+        # We have Request/Response as voids to mark raw as a special case.
+        # Raw operates in ConstByteSpans, which won't be copied by copying the
+        # span itself and without special treatment will lead to dangling
+        # pointers.
+        #
+        # Helpers/traits that want to use Request/Response and should support
+        # raw are required to do a special implementation for them instead that
+        # will copy the actual data.
+        self.line('using Request = void;')
+        self.line('using Response = void;')
+
 
 class StubGenerator(codegen.StubGenerator):
     def unary_signature(self, method: ProtoServiceMethod, prefix: str) -> str:
         return (f'void {prefix}{method.name()}(pw::ConstByteSpan request, '
                 'pw::rpc::RawUnaryResponder& responder)')
 
     def unary_stub(self, method: ProtoServiceMethod,
```

### Comparing `pigweed-0.0.8/pw_rpc/console_tools/__init__.py` & `pigweed-0.0.9/pw_rpc/console_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/console_tools/console.py` & `pigweed-0.0.9/pw_rpc/console_tools/console.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/console_tools/functions.py` & `pigweed-0.0.9/pw_rpc/console_tools/functions.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/console_tools/watchdog.py` & `pigweed-0.0.9/pw_rpc/console_tools/watchdog.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/descriptors.py` & `pigweed-0.0.9/pw_rpc/descriptors.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/echo_pb2.py` & `pigweed-0.0.9/pw_rpc/echo_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/echo_pb2.pyi` & `pigweed-0.0.9/pw_rpc/echo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/ids.py` & `pigweed-0.0.9/pw_rpc/ids.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/internal/packet_pb2.py` & `pigweed-0.0.9/pw_rpc/internal/packet_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/internal/packet_pb2.pyi` & `pigweed-0.0.9/pw_rpc/internal/packet_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     REQUEST = PacketType.V(0)
     # A message in a client stream. Always sent after a REQUEST and before a
     # CLIENT_STREAM_END.
     CLIENT_STREAM = PacketType.V(2)
     # The client received a packet for an RPC it did not request.
     CLIENT_ERROR = PacketType.V(4)
     # Deprecated, do not use. Send a CLIENT_ERROR with status CANCELLED instead.
-    # TODO(pwbug/512): Remove this packet type.
+    # TODO(b/234879973): Remove this packet type.
     DEPRECATED_CANCEL = PacketType.V(6)
     # A client stream has completed.
     CLIENT_STREAM_END = PacketType.V(8)
     # Server-to-client packets
 
     # The RPC has finished.
     RESPONSE = PacketType.V(1)
     # Deprecated, do not use. Formerly was used as the last packet in a server
     # stream.
-    # TODO(pwbug/512): Remove this packet type.
+    # TODO(b/234879973): Remove this packet type.
     DEPRECATED_SERVER_STREAM_END = PacketType.V(3)
     # The server was unable to process a request.
     SERVER_ERROR = PacketType.V(5)
     # A message in a server stream.
     SERVER_STREAM = PacketType.V(7)
 
 # Client-to-server packets
@@ -52,25 +52,25 @@
 REQUEST = PacketType.V(0)
 # A message in a client stream. Always sent after a REQUEST and before a
 # CLIENT_STREAM_END.
 CLIENT_STREAM = PacketType.V(2)
 # The client received a packet for an RPC it did not request.
 CLIENT_ERROR = PacketType.V(4)
 # Deprecated, do not use. Send a CLIENT_ERROR with status CANCELLED instead.
-# TODO(pwbug/512): Remove this packet type.
+# TODO(b/234879973): Remove this packet type.
 DEPRECATED_CANCEL = PacketType.V(6)
 # A client stream has completed.
 CLIENT_STREAM_END = PacketType.V(8)
 # Server-to-client packets
 
 # The RPC has finished.
 RESPONSE = PacketType.V(1)
 # Deprecated, do not use. Formerly was used as the last packet in a server
 # stream.
-# TODO(pwbug/512): Remove this packet type.
+# TODO(b/234879973): Remove this packet type.
 DEPRECATED_SERVER_STREAM_END = PacketType.V(3)
 # The server was unable to process a request.
 SERVER_ERROR = PacketType.V(5)
 # A message in a server stream.
 SERVER_STREAM = PacketType.V(7)
 global___PacketType = PacketType
```

### Comparing `pigweed-0.0.8/pw_rpc/lossy_channel.py` & `pigweed-0.0.9/pw_rpc/lossy_channel.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/packets.py` & `pigweed-0.0.9/pw_rpc/packets.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/plugin.py` & `pigweed-0.0.9/pw_rpc/plugin.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/plugin_nanopb.py` & `pigweed-0.0.9/pw_rpc/plugin_nanopb.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/plugin_pwpb.py` & `pigweed-0.0.9/pw_rpc/plugin_pwpb.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/plugin_raw.py` & `pigweed-0.0.9/pw_rpc/plugin_raw.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_rpc/testing.py` & `pigweed-0.0.9/pw_rpc/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         temp_dir = tempfile.TemporaryDirectory(prefix='pw_rpc_test_')
         common_args = [
             temp_dir.name if a == TEMP_DIR_MARKER else a for a in common_args
         ]
 
     try:
         server_process = subprocess.Popen([server, *common_args])
-        # TODO(pwbug/508): Replace this delay with some sort of IPC.
+        # TODO(b/234879791): Replace this delay with some sort of IPC.
         time.sleep(setup_time_s)
 
         result = subprocess.run([client, *common_args]).returncode
 
         server_process.terminate()
         server_process.communicate()
     finally:
```

### Comparing `pigweed-0.0.8/pw_snapshot/processor.py` & `pigweed-0.0.9/pw_snapshot/processor.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_snapshot_metadata/metadata.py` & `pigweed-0.0.9/pw_snapshot_metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_snapshot_metadata_proto/snapshot_metadata_pb2.py` & `pigweed-0.0.9/pw_snapshot_metadata_proto/snapshot_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_snapshot_metadata_proto/snapshot_metadata_pb2.pyi` & `pigweed-0.0.9/pw_snapshot_metadata_proto/snapshot_metadata_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -55,16 +55,19 @@
     reason: builtins.bytes = ...
     # Whether or not the snapshot was captured due to a crash of some kind.
     fatal: builtins.bool = ...
     # Project name to assist in identifying where to redirect this snapshot. A
     # single project might have multiple devices that can produce snapshots.
     project_name: builtins.bytes = ...
     # Version characters must be alphanumeric, punctuation, and space. This
-    # string is case-sensitive. This should either be human readable text, or
-    # tokenized data.
+    # string is case-sensitive. This should always be human readable text, and
+    # does not support tokenization by design. If this field was tokenized, it's
+    # possible that the token could be lost (e.g. generated by a local developer
+    # build and not uploaded anywhere) and a firmware version running on a device
+    # in the field would be left entirely unidentifiable.
     #
     # Examples:
     #   "codename-local-[build_id]"
     #   "codename-release-193"
     software_version: typing.Text = ...
     # UUID associated with the build for the software version.
     software_build_uuid: builtins.bytes = ...
```

### Comparing `pigweed-0.0.8/pw_snapshot_protos/snapshot_pb2.py` & `pigweed-0.0.9/pw_snapshot_protos/snapshot_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from pw_chrono import chrono_pb2 as pw__chrono_dot_chrono__pb2
 from pw_cpu_exception_cortex_m_protos import cpu_state_pb2 as pw__cpu__exception__cortex__m__protos_dot_cpu__state__pb2
 from pw_log.proto import log_pb2 as pw__log_dot_proto_dot_log__pb2
 from pw_thread_protos import thread_pb2 as pw__thread__protos_dot_thread__pb2
 from pw_snapshot_metadata_proto import snapshot_metadata_pb2 as pw__snapshot__metadata__proto_dot_snapshot__metadata__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='pw_snapshot_protos/snapshot.proto',
   package='pw.snapshot',
   syntax='proto3',
   serialized_options=b'\n\021pw.snapshot.protoB\010Snapshot',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n!pw_snapshot_protos/snapshot.proto\x12\x0bpw.snapshot\x1a\x30pw_cpu_exception_cortex_m_protos/cpu_state.proto\x1a\x16pw_log/proto/log.proto\x1a\x1dpw_thread_protos/thread.proto\x1a\x32pw_snapshot_metadata_proto/snapshot_metadata.proto\"\xfc\x02\n\x08Snapshot\x12\x1e\n\x04logs\x18\x01 \x03(\x0b\x32\x10.pw.log.LogEntry\x12\'\n\x08metadata\x18\x10 \x01(\x0b\x32\x15.pw.snapshot.Metadata\x12-\n\x04tags\x18\x11 \x03(\x0b\x32\x1f.pw.snapshot.Snapshot.TagsEntry\x12\"\n\x07threads\x18\x12 \x03(\x0b\x32\x11.pw.thread.Thread\x12\x30\n\x11related_snapshots\x18\x13 \x03(\x0b\x32\x15.pw.snapshot.Snapshot\x12\x43\n\x10\x61rmv7m_cpu_state\x18\x14 \x01(\x0b\x32).pw.cpu_exception.cortex_m.ArmV7mCpuState\x12\x12\n\ntrace_data\x18\x15 \x01(\x0c\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01J\x04\x08\x02\x10\x08J\x04\x08\x08\x10\x10J\x05\x08\x16\x10\x88\x08J\t\x08\x88\x08\x10\x80\x80\x80\x80\x02\x42\x1d\n\x11pw.snapshot.protoB\x08Snapshotb\x06proto3'
+  serialized_pb=b'\n!pw_snapshot_protos/snapshot.proto\x12\x0bpw.snapshot\x1a\x16pw_chrono/chrono.proto\x1a\x30pw_cpu_exception_cortex_m_protos/cpu_state.proto\x1a\x16pw_log/proto/log.proto\x1a\x1dpw_thread_protos/thread.proto\x1a\x32pw_snapshot_metadata_proto/snapshot_metadata.proto\"\xa6\x03\n\x08Snapshot\x12\x1e\n\x04logs\x18\x01 \x03(\x0b\x32\x10.pw.log.LogEntry\x12\'\n\x08metadata\x18\x10 \x01(\x0b\x32\x15.pw.snapshot.Metadata\x12-\n\x04tags\x18\x11 \x03(\x0b\x32\x1f.pw.snapshot.Snapshot.TagsEntry\x12\"\n\x07threads\x18\x12 \x03(\x0b\x32\x11.pw.thread.Thread\x12\x30\n\x11related_snapshots\x18\x13 \x03(\x0b\x32\x15.pw.snapshot.Snapshot\x12\x43\n\x10\x61rmv7m_cpu_state\x18\x14 \x01(\x0b\x32).pw.cpu_exception.cortex_m.ArmV7mCpuState\x12\x12\n\ntrace_data\x18\x15 \x01(\x0c\x12(\n\ntimestamps\x18\x16 \x03(\x0b\x32\x14.pw.chrono.TimePoint\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01J\x04\x08\x02\x10\x08J\x04\x08\x08\x10\x10J\x05\x08\x17\x10\x88\x08J\t\x08\x88\x08\x10\x80\x80\x80\x80\x02\x42\x1d\n\x11pw.snapshot.protoB\x08Snapshotb\x06proto3'
   ,
-  dependencies=[pw__cpu__exception__cortex__m__protos_dot_cpu__state__pb2.DESCRIPTOR,pw__log_dot_proto_dot_log__pb2.DESCRIPTOR,pw__thread__protos_dot_thread__pb2.DESCRIPTOR,pw__snapshot__metadata__proto_dot_snapshot__metadata__pb2.DESCRIPTOR,])
+  dependencies=[pw__chrono_dot_chrono__pb2.DESCRIPTOR,pw__cpu__exception__cortex__m__protos_dot_cpu__state__pb2.DESCRIPTOR,pw__log_dot_proto_dot_log__pb2.DESCRIPTOR,pw__thread__protos_dot_thread__pb2.DESCRIPTOR,pw__snapshot__metadata__proto_dot_snapshot__metadata__pb2.DESCRIPTOR,])
 
 
 
 
 _SNAPSHOT_TAGSENTRY = _descriptor.Descriptor(
   name='TagsEntry',
   full_name='pw.snapshot.Snapshot.TagsEntry',
@@ -60,16 +61,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=515,
-  serialized_end=558,
+  serialized_start=581,
+  serialized_end=624,
 )
 
 _SNAPSHOT = _descriptor.Descriptor(
   name='Snapshot',
   full_name='pw.snapshot.Snapshot',
   filename=None,
   file=DESCRIPTOR,
@@ -121,37 +122,45 @@
     _descriptor.FieldDescriptor(
       name='trace_data', full_name='pw.snapshot.Snapshot.trace_data', index=6,
       number=21, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='timestamps', full_name='pw.snapshot.Snapshot.timestamps', index=7,
+      number=22, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[_SNAPSHOT_TAGSENTRY, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=208,
-  serialized_end=588,
+  serialized_start=232,
+  serialized_end=654,
 )
 
 _SNAPSHOT_TAGSENTRY.containing_type = _SNAPSHOT
 _SNAPSHOT.fields_by_name['logs'].message_type = pw__log_dot_proto_dot_log__pb2._LOGENTRY
 _SNAPSHOT.fields_by_name['metadata'].message_type = pw__snapshot__metadata__proto_dot_snapshot__metadata__pb2._METADATA
 _SNAPSHOT.fields_by_name['tags'].message_type = _SNAPSHOT_TAGSENTRY
 _SNAPSHOT.fields_by_name['threads'].message_type = pw__thread__protos_dot_thread__pb2._THREAD
 _SNAPSHOT.fields_by_name['related_snapshots'].message_type = _SNAPSHOT
 _SNAPSHOT.fields_by_name['armv7m_cpu_state'].message_type = pw__cpu__exception__cortex__m__protos_dot_cpu__state__pb2._ARMV7MCPUSTATE
+_SNAPSHOT.fields_by_name['timestamps'].message_type = pw__chrono_dot_chrono__pb2._TIMEPOINT
 DESCRIPTOR.message_types_by_name['Snapshot'] = _SNAPSHOT
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Snapshot = _reflection.GeneratedProtocolMessageType('Snapshot', (_message.Message,), {
 
   'TagsEntry' : _reflection.GeneratedProtocolMessageType('TagsEntry', (_message.Message,), {
     'DESCRIPTOR' : _SNAPSHOT_TAGSENTRY,
```

### Comparing `pigweed-0.0.8/pw_snapshot_protos/snapshot_pb2.pyi` & `pigweed-0.0.9/pw_snapshot_protos/snapshot_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
+import pw_chrono.chrono_pb2
 import pw_cpu_exception_cortex_m_protos.cpu_state_pb2
 import pw_log.proto.log_pb2
 import pw_snapshot_metadata_proto.snapshot_metadata_pb2
 import pw_thread_protos.thread_pb2
 import typing
 import typing_extensions
 
@@ -55,14 +56,15 @@
     LOGS_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     TAGS_FIELD_NUMBER: builtins.int
     THREADS_FIELD_NUMBER: builtins.int
     RELATED_SNAPSHOTS_FIELD_NUMBER: builtins.int
     ARMV7M_CPU_STATE_FIELD_NUMBER: builtins.int
     TRACE_DATA_FIELD_NUMBER: builtins.int
+    TIMESTAMPS_FIELD_NUMBER: builtins.int
     @property
     def logs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[pw_log.proto.log_pb2.LogEntry]: ...
     # Note: Proto tags 16-2047 encode with two bytes of overhead.
     @property
     def metadata(self) -> pw_snapshot_metadata_proto.snapshot_metadata_pb2.Metadata: ...
     # Other data that should be highlighted in this crash. This field may have
     # entries added to it during a decode.
@@ -77,20 +79,26 @@
     @property
     def related_snapshots(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Snapshot]: ...
     @property
     def armv7m_cpu_state(self) -> pw_cpu_exception_cortex_m_protos.cpu_state_pb2.ArmV7mCpuState: ...
     # Platform-specific binary trace data region. Binary trace data is using
     # pw_trace_tokenized buffer format for stored data.
     trace_data: builtins.bytes = ...
+    # Timestamps that mark when this snapshot occurred. This field is repeated
+    # to accommodate wall-clock time, time since boot, and/or the raw system
+    # clock value.
+    @property
+    def timestamps(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[pw_chrono.chrono_pb2.TimePoint]: ...
     def __init__(self,
         *,
         logs : typing.Optional[typing.Iterable[pw_log.proto.log_pb2.LogEntry]] = ...,
         metadata : typing.Optional[pw_snapshot_metadata_proto.snapshot_metadata_pb2.Metadata] = ...,
         tags : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         threads : typing.Optional[typing.Iterable[pw_thread_protos.thread_pb2.Thread]] = ...,
         related_snapshots : typing.Optional[typing.Iterable[global___Snapshot]] = ...,
         armv7m_cpu_state : typing.Optional[pw_cpu_exception_cortex_m_protos.cpu_state_pb2.ArmV7mCpuState] = ...,
         trace_data : builtins.bytes = ...,
+        timestamps : typing.Optional[typing.Iterable[pw_chrono.chrono_pb2.TimePoint]] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal[u"armv7m_cpu_state",b"armv7m_cpu_state",u"metadata",b"metadata"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"armv7m_cpu_state",b"armv7m_cpu_state",u"logs",b"logs",u"metadata",b"metadata",u"related_snapshots",b"related_snapshots",u"tags",b"tags",u"threads",b"threads",u"trace_data",b"trace_data"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"armv7m_cpu_state",b"armv7m_cpu_state",u"logs",b"logs",u"metadata",b"metadata",u"related_snapshots",b"related_snapshots",u"tags",b"tags",u"threads",b"threads",u"timestamps",b"timestamps",u"trace_data",b"trace_data"]) -> None: ...
 global___Snapshot = Snapshot
```

### Comparing `pigweed-0.0.8/pw_software_update/__init__.py` & `pigweed-0.0.9/pw_software_update/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/bundled_update_pb2.py` & `pigweed-0.0.9/pw_software_update/bundled_update_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/bundled_update_pb2.pyi` & `pigweed-0.0.9/pw_software_update/bundled_update_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/dev_sign.py` & `pigweed-0.0.9/pw_software_update/dev_sign.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/generate_test_bundle.py` & `pigweed-0.0.9/pw_software_update/generate_test_bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     parser.add_argument("output_header",
                         help="output path of the generated C header")
     return parser.parse_args()
 
 
 def main() -> int:
     """Main"""
-    # TODO(pwbug/456): Refactor the code so that each test bundle generation
+    # TODO(b/237580538): Refactor the code so that each test bundle generation
     # is done in a separate function or script.
     # pylint: disable=too-many-locals
     args = parse_args()
 
     test_bundle = Bundle()
 
     dev_signed_root = test_bundle.generate_dev_signed_root_metadata()
@@ -427,15 +427,15 @@
                     personalized_out_bundle,
                     f'kTestBundlePersonalizedOutFile{idx}'))
     subprocess.run([
         'clang-format',
         '-i',
         args.output_header,
     ], check=True)
-    # TODO(pwbug/456): Refactor the code so that each test bundle generation
+    # TODO(b/237580538): Refactor the code so that each test bundle generation
     # is done in a separate function or script.
     # pylint: enable=too-many-locals
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pigweed-0.0.8/pw_software_update/keys.py` & `pigweed-0.0.9/pw_software_update/keys.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/metadata.py` & `pigweed-0.0.9/pw_software_update/metadata.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/remote_sign.py` & `pigweed-0.0.9/pw_software_update/remote_sign.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/root_metadata.py` & `pigweed-0.0.9/pw_software_update/root_metadata.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/tuf_pb2.py` & `pigweed-0.0.9/pw_software_update/tuf_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/tuf_pb2.pyi` & `pigweed-0.0.9/pw_software_update/tuf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/update_bundle.py` & `pigweed-0.0.9/pw_software_update/update_bundle.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/update_bundle_pb2.py` & `pigweed-0.0.9/pw_software_update/update_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/update_bundle_pb2.pyi` & `pigweed-0.0.9/pw_software_update/update_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_software_update/verify.py` & `pigweed-0.0.9/pw_software_update/verify.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_status/__init__.py` & `pigweed-0.0.9/pw_status/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_stm32cube_build/__init__.py` & `pigweed-0.0.9/pw_stm32cube_build/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_stm32cube_build/__main__.py` & `pigweed-0.0.9/pw_stm32cube_build/__main__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_stm32cube_build/find_files.py` & `pigweed-0.0.9/pw_stm32cube_build/find_files.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_stm32cube_build/gen_file_list.py` & `pigweed-0.0.9/pw_stm32cube_build/gen_file_list.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_stm32cube_build/icf_to_ld.py` & `pigweed-0.0.9/pw_stm32cube_build/icf_to_ld.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_stm32cube_build/inject_init.py` & `pigweed-0.0.9/pw_stm32cube_build/inject_init.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_symbolizer/__init__.py` & `pigweed-0.0.9/pw_symbolizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_symbolizer/llvm_symbolizer.py` & `pigweed-0.0.9/pw_symbolizer/llvm_symbolizer.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_symbolizer/symbolizer.py` & `pigweed-0.0.9/pw_symbolizer/symbolizer.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_system/__init__.py` & `pigweed-0.0.9/pw_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_system/console.py` & `pigweed-0.0.9/pw_system/console.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 import logging
 from pathlib import Path
 import sys
 from types import ModuleType
 from typing import (
     Any,
     Collection,
+    Dict,
     Iterable,
     Iterator,
     List,
     Optional,
     Union,
 )
 import socket
@@ -53,22 +54,27 @@
 import serial  # type: ignore
 
 import pw_cli.log
 import pw_console.python_logging
 from pw_console import PwConsoleEmbed
 from pw_console.pyserial_wrapper import SerialWithLogging
 from pw_console.plugins.bandwidth_toolbar import BandwidthToolbar
-
+from pw_console.log_store import LogStore
 from pw_log.proto import log_pb2
+from pw_metric_proto import metric_service_pb2
 from pw_rpc.console_tools.console import flattened_rpc_completions
-from pw_system.device import Device
 from pw_tokenizer.detokenize import AutoUpdatingDetokenizer
+from pw_unit_test_proto import unit_test_pb2
+
+from pw_system.device import Device
 
 _LOG = logging.getLogger('tools')
 _DEVICE_LOG = logging.getLogger('rpc_device')
+_SERIAL_DEBUG = logging.getLogger('pw_console.serial_debug_logger')
+_ROOT_LOG = logging.getLogger()
 
 PW_RPC_MAX_PACKET_SIZE = 256
 SOCKET_SERVER = 'localhost'
 SOCKET_PORT = 33000
 MKFIFO_MODE = 0o666
 
 
@@ -106,31 +112,38 @@
                         type=Path,
                         help="Path to tokenizer database csv file(s).")
     parser.add_argument('--config-file',
                         type=Path,
                         help='Path to a pw_console yaml config file.')
     parser.add_argument('--proto-globs',
                         nargs='+',
+                        default=[],
                         help='glob pattern for .proto files')
     parser.add_argument('-v',
                         '--verbose',
                         action='store_true',
                         help='Enables debug logging when set')
     return parser.parse_args()
 
 
 def _expand_globs(globs: Iterable[str]) -> Iterator[Path]:
     for pattern in globs:
         for file in glob.glob(pattern, recursive=True):
             yield Path(file)
 
 
-def _start_ipython_terminal(device: Device,
-                            serial_debug: bool = False,
-                            config_file_path: Optional[Path] = None) -> None:
+def _start_ipython_terminal(
+    device: Device,
+    device_log_store: LogStore,
+    root_log_store: LogStore,
+    serial_debug_log_store: LogStore,
+    log_file: str,
+    serial_debug: bool = False,
+    config_file_path: Optional[Path] = None,
+) -> None:
     """Starts an interactive IPython terminal with preset variables."""
     local_variables = dict(
         client=device.client,
         device=device,
         rpcs=device.rpcs,
         protos=device.client.protos.packages,
         # Include the active pane logger for creating logs in the repl.
@@ -150,41 +163,39 @@
           LOG.warning('Message appears in Host Logs window.')
           DEVICE_LOG.warning('Message appears in Device Logs window.')
     """)
 
     client_info = device.info()
     completions = flattened_rpc_completions([client_info])
 
-    log_windows = {
-        'Device Logs': [_DEVICE_LOG],
-        'Host Logs': [logging.getLogger()],
+    log_windows: Dict[str, Union[List[logging.Logger], LogStore]] = {
+        'Device Logs': device_log_store,
+        'Host Logs': root_log_store,
     }
     if serial_debug:
-        log_windows['Serial Debug'] = [
-            logging.getLogger('pw_console.serial_debug_logger')
-        ]
+        log_windows['Serial Debug'] = serial_debug_log_store
 
     interactive_console = PwConsoleEmbed(
         global_vars=local_variables,
         local_vars=None,
         loggers=log_windows,
         repl_startup_message=welcome_message,
         help_text=__doc__,
         config_file_path=config_file_path,
     )
-    interactive_console.hide_windows('Host Logs')
     interactive_console.add_sentence_completer(completions)
     if serial_debug:
         interactive_console.add_bottom_toolbar(BandwidthToolbar())
 
     # Setup Python logger propagation
-    interactive_console.setup_python_logging()
-
-    # Don't send device logs to the root logger.
-    _DEVICE_LOG.propagate = False
+    interactive_console.setup_python_logging(
+        # Send any unhandled log messages to the external file.
+        last_resort_filename=log_file,
+        # Don't change propagation for these loggers.
+        loggers_with_no_propagation=[_DEVICE_LOG])
 
     interactive_console.embed()
 
 
 class SocketClientImpl:
     def __init__(self, config: str):
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
@@ -219,42 +230,57 @@
             verbose: bool = False,
             compiled_protos: Optional[List[ModuleType]] = None) -> int:
     """Starts an interactive RPC console for HDLC."""
     # argparse.FileType doesn't correctly handle '-' for binary files.
     if output is sys.stdout:
         output = sys.stdout.buffer
 
+    # Don't send device logs to the root logger.
+    _DEVICE_LOG.propagate = False
+    # Create pw_console LogStore handlers. These are the data source for log
+    # messages to be displayed in the UI.
+    device_log_store = LogStore()
+    root_log_store = LogStore()
+    serial_debug_log_store = LogStore()
+    # Attach the LogStores as handlers for each log window we want to show.
+    # This should be done before device initialization to capture early
+    # messages.
+    _DEVICE_LOG.addHandler(device_log_store)
+    _ROOT_LOG.addHandler(root_log_store)
+    _SERIAL_DEBUG.addHandler(serial_debug_log_store)
+
     if not logfile:
         # Create a temp logfile to prevent logs from appearing over stdout. This
         # would corrupt the prompt toolkit UI.
         logfile = pw_console.python_logging.create_temp_log_file()
 
     log_level = logging.DEBUG if verbose else logging.INFO
     pw_cli.log.install(log_level, True, False, logfile)
-    _DEVICE_LOG.setLevel(log_level)
     _LOG.setLevel(log_level)
+    _DEVICE_LOG.setLevel(log_level)
+    _ROOT_LOG.setLevel(log_level)
+    _SERIAL_DEBUG.setLevel(log_level)
 
     detokenizer = None
     if token_databases:
         detokenizer = AutoUpdatingDetokenizer(*token_databases)
         detokenizer.show_errors = True
 
-    if not proto_globs:
-        proto_globs = ['**/*.proto']
-
     protos: List[Union[ModuleType, Path]] = list(_expand_globs(proto_globs))
 
     if compiled_protos is None:
         compiled_protos = []
 
     # Append compiled log.proto library to avoid include errors when manually
     # provided, and shadowing errors due to ordering when the default global
     # search path is used.
     compiled_protos.append(log_pb2)
+    compiled_protos.append(unit_test_pb2)
     protos.extend(compiled_protos)
+    protos.append(metric_service_pb2)
 
     if not protos:
         _LOG.critical('No .proto files were found with %s',
                       ', '.join(proto_globs))
         _LOG.critical('At least one .proto file is required')
         return 1
 
@@ -294,15 +320,17 @@
                            read,
                            write,
                            protos,
                            detokenizer,
                            timestamp_decoder=timestamp_decoder,
                            rpc_timeout_s=5)
 
-    _start_ipython_terminal(device_client, serial_debug, config_file)
+    _start_ipython_terminal(device_client, device_log_store, root_log_store,
+                            serial_debug_log_store, logfile, serial_debug,
+                            config_file)
     return 0
 
 
 def main() -> int:
     return console(**vars(_parse_args()))
```

### Comparing `pigweed-0.0.8/pw_system/device.py` & `pigweed-0.0.9/pw_system/device.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 import logging
 from pathlib import Path
 from types import ModuleType
 from typing import Any, Callable, List, Union, Optional
 
 from pw_hdlc.rpc import HdlcRpcClient, default_channels
 import pw_log_tokenized
-
 from pw_log.proto import log_pb2
+from pw_metric import metric_parser
 from pw_rpc import callback_client, console_tools
 from pw_status import Status
-from pw_tokenizer.detokenize import Detokenizer
+from pw_tokenizer import detokenize
 from pw_tokenizer.proto import decode_optionally_tokenized
+import pw_unit_test.rpc
 
 # Internal log for troubleshooting this tool (the console).
 _LOG = logging.getLogger('tools')
 DEFAULT_DEVICE_LOGGER = logging.getLogger('rpc_device')
 
 
 class Device:
@@ -40,28 +41,29 @@
     Note: use this class as a base for specialized device representations.
     """
     def __init__(self,
                  channel_id: int,
                  read,
                  write,
                  proto_library: List[Union[ModuleType, Path]],
-                 detokenizer: Optional[Detokenizer],
+                 detokenizer: Optional[detokenize.Detokenizer],
                  timestamp_decoder: Optional[Callable[[int], str]],
                  rpc_timeout_s=5):
         self.channel_id = channel_id
         self.protos = proto_library
         self.detokenizer = detokenizer
+        self.rpc_timeout_s = rpc_timeout_s
 
         self.logger = DEFAULT_DEVICE_LOGGER
         self.logger.setLevel(logging.DEBUG)  # Allow all device logs through.
         self.timestamp_decoder = timestamp_decoder
         self._expected_log_sequence_id = 0
 
         callback_client_impl = callback_client.Impl(
-            default_unary_timeout_s=rpc_timeout_s,
+            default_unary_timeout_s=self.rpc_timeout_s,
             default_stream_timeout_s=None,
         )
         self.client = HdlcRpcClient(
             read,
             self.protos,
             default_channels(write),
             lambda data: self.logger.info("%s", str(data)),
@@ -75,14 +77,18 @@
                                         self.client.client)
 
     @property
     def rpcs(self) -> Any:
         """Returns an object for accessing services on the specified channel."""
         return next(iter(self.client.client.channels())).rpcs
 
+    def run_tests(self, timeout_s: Optional[float] = 5) -> bool:
+        """Runs the unit tests on this device."""
+        return pw_unit_test.rpc.run_tests(self.rpcs, timeout_s=timeout_s)
+
     def listen_to_log_stream(self):
         """Opens a log RPC for the device's unrequested log stream.
 
         The RPCs remain open until the server cancels or closes them, either
         with a response or error packet.
         """
         self.rpcs.pw.log.Logs.Listen.open(
@@ -164,7 +170,23 @@
 
         Defaults to interpreting the input timestamp as nanoseconds since boot.
         Devices can override this to match their timestamp units.
         """
         if self.timestamp_decoder:
             return self.timestamp_decoder(timestamp)
         return str(datetime.timedelta(seconds=timestamp / 1e9))[:-3]
+
+    def get_and_log_metrics(self) -> dict:
+        """Retrieves the parsed metrics and logs them to the console."""
+        metrics = metric_parser.parse_metrics(self.rpcs, self.detokenizer,
+                                              self.rpc_timeout_s)
+
+        def print_metrics(metrics, path):
+            """Traverses dictionaries, until a non-dict value is reached."""
+            for path_name, metric in metrics.items():
+                if isinstance(metric, dict):
+                    print_metrics(metric, path + '/' + path_name)
+                else:
+                    _LOG.info('%s/%s: %s', path, path_name, str(metric))
+
+        print_metrics(metrics, '')
+        return metrics
```

### Comparing `pigweed-0.0.8/pw_thread/thread_analyzer.py` & `pigweed-0.0.9/pw_thread/thread_analyzer.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_thread_protos/thread_pb2.py` & `pigweed-0.0.9/pw_thread_protos/thread_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_thread_protos/thread_pb2.pyi` & `pigweed-0.0.9/pw_thread_protos/thread_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tls_client/generate_test_data.py` & `pigweed-0.0.9/pw_tls_client/generate_test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     body = ''.join([f'\\x{b:02x}' for b in data])
     return f'{{\"{body}\", {len(data)}}}'
 
 
 def byte_array_declaration(data: bytes, name: str) -> str:
     """Generates a ConstByteSpan declaration for a byte array"""
     type_name = '[[maybe_unused]] const pw::ConstByteSpan'
-    array_body = f'std::as_bytes(std::span{c_escaped_string(data)})'
+    array_body = f'pw::as_bytes(pw::span{c_escaped_string(data)})'
     return f'{type_name} {name} = {array_body};'
 
 
 class Codegen:
     """Base helper class for code generation"""
     def generate_code(self) -> str:
         """Generates C++ code for this object"""
```

### Comparing `pigweed-0.0.8/pw_tokenizer/__init__.py` & `pigweed-0.0.9/pw_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/__main__.py` & `pigweed-0.0.9/pw_tokenizer/__main__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/database.py` & `pigweed-0.0.9/pw_tokenizer/database.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/decode.py` & `pigweed-0.0.9/pw_tokenizer/decode.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/detokenize.py` & `pigweed-0.0.9/pw_tokenizer/detokenize.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/elf_reader.py` & `pigweed-0.0.9/pw_tokenizer/elf_reader.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/parse_message.py` & `pigweed-0.0.9/pw_tokenizer/parse_message.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/proto/__init__.py` & `pigweed-0.0.9/pw_tokenizer/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/proto/options_pb2.py` & `pigweed-0.0.9/pw_tokenizer/proto/options_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/proto/options_pb2.pyi` & `pigweed-0.0.9/pw_tokenizer/proto/options_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 # prefixed Base64).
 TOKENIZATION_OPTIONAL = Tokenization.V(0)
 global___Tokenization = Tokenization
 
 
 # The field number was randomly selected from the reserved, internal use
 # field numbers (50000-99999).
-# TODO(pwbug/393): Register with the Protobuf Global Extension Registry:
+# TODO(b/234886465): Register with the Protobuf Global Extension Registry:
 #     https://github.com/protocolbuffers/protobuf/blob/HEAD/docs/options.md
 format: google.protobuf.internal.extension_dict._ExtensionFieldDescriptor[google.protobuf.descriptor_pb2.FieldOptions, global___Tokenization.V] = ...
```

### Comparing `pigweed-0.0.8/pw_tokenizer/serial_detokenizer.py` & `pigweed-0.0.9/pw_tokenizer/serial_detokenizer.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_tokenizer/tokens.py` & `pigweed-0.0.9/pw_tokenizer/tokens.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_toolchain/bad_toolchain.py` & `pigweed-0.0.9/pw_toolchain/bad_toolchain.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_toolchain/clang_arm_toolchain.py` & `pigweed-0.0.9/pw_toolchain/clang_arm_toolchain.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_toolchain/clang_tidy.py` & `pigweed-0.0.9/pw_toolchain/clang_tidy.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,14 @@
                         nargs=argparse.REMAINDER,
                         help=argparse.SUPPRESS)
 
     parsed_args = parser.parse_args()
 
     if parsed_args.extra_args[0] != '--':
         parser.error('arguments not correctly split')
-
     parsed_args.extra_args = parsed_args.extra_args[1:]
     return parsed_args
 
 
 def _filter_include_paths(args: Iterable[str],
                           skip_include_paths: Iterable[str]) -> Iterable[str]:
     filters = [f.rstrip('/') for f in skip_include_paths]
@@ -122,26 +121,28 @@
 
     if not verbose:
         command.append('--quiet')
 
     if export_fixes is not None:
         command.extend(['--export-fixes', export_fixes])
 
-    # Append extra compilation flags. extra_args[0] is skipped as it contains
-    # the compiler binary name.
+    # Append extra compilation flags.  Extra args up to
+    # END_OF_INVOKER are skipped.
     command.append('--')
-    command.extend(_filter_include_paths(extra_args[1:], skip_include_path))
+    end_of_invoker = extra_args.index('END_OF_INVOKER')
+    command.extend(
+        _filter_include_paths(extra_args[end_of_invoker + 1:],
+                              skip_include_path))
 
     process = subprocess.run(
         command,
         stdout=subprocess.PIPE,
         # clang-tidy prints regular information on
         # stderr, even with the option --quiet.
         stderr=subprocess.PIPE)
-
     if process.returncode != 0:
         _LOG.warning('%s', ' '.join(shlex.quote(str(arg)) for arg in command))
 
     if process.stdout:
         _LOG.warning(process.stdout.decode().strip())
 
     if process.stderr and process.returncode != 0:
```

### Comparing `pigweed-0.0.8/pw_toolchain/copy_with_metadata.py` & `pigweed-0.0.9/pw_toolchain/copy_with_metadata.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_trace/__init__.py` & `pigweed-0.0.9/pw_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_trace/trace.py` & `pigweed-0.0.9/pw_trace/trace.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_trace_tokenized/get_trace.py` & `pigweed-0.0.9/pw_trace_tokenized/get_trace.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_trace_tokenized/trace_tokenized.py` & `pigweed-0.0.9/pw_trace_tokenized/trace_tokenized.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_transfer/__init__.py` & `pigweed-0.0.9/pw_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_transfer/client.py` & `pigweed-0.0.9/pw_transfer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 from typing import Any, Dict, Optional, Union
 
 from pw_rpc.callback_client import BidirectionalStreamingCall
 from pw_status import Status
 
 from pw_transfer.transfer import (ProgressCallback, ReadTransfer, Transfer,
                                   WriteTransfer)
-from pw_transfer.transfer_pb2 import Chunk
+try:
+    from pw_transfer import transfer_pb2
+except ImportError:
+    # For the bazel build, which puts generated protos in a different location.
+    from pigweed.pw_transfer import transfer_pb2  # type: ignore
 
 _LOG = logging.getLogger(__package__)
 
 _TransferDict = Dict[int, Transfer]
 
 
 class Manager:  # pylint: disable=too-many-instance-attributes
@@ -66,14 +70,17 @@
 
         # RPC streams for read and write transfers. These are shareable by
         # multiple transfers of the same type.
         self._read_stream: Optional[BidirectionalStreamingCall] = None
         self._write_stream: Optional[BidirectionalStreamingCall] = None
 
         self._loop = asyncio.new_event_loop()
+        # If constructed from non-main thread, set the event loop.
+        if threading.current_thread() is not threading.main_thread():
+            asyncio.set_event_loop(self._loop)
 
         # Queues are used for communication between the Manager context and the
         # dedicated asyncio transfer thread.
         self._new_transfer_queue: asyncio.Queue = asyncio.Queue()
         self._read_chunk_queue: asyncio.Queue = asyncio.Queue()
         self._write_chunk_queue: asyncio.Queue = asyncio.Queue()
         self._quit_event = asyncio.Event()
@@ -152,19 +159,19 @@
         self._start_write_transfer(transfer)
 
         transfer.done.wait()
 
         if not transfer.status.ok():
             raise Error(transfer.id, transfer.status)
 
-    def _send_read_chunk(self, chunk: Chunk) -> None:
+    def _send_read_chunk(self, chunk: transfer_pb2.Chunk) -> None:
         assert self._read_stream is not None
         self._read_stream.send(chunk)
 
-    def _send_write_chunk(self, chunk: Chunk) -> None:
+    def _send_write_chunk(self, chunk: transfer_pb2.Chunk) -> None:
         assert self._write_stream is not None
         self._write_stream.send(chunk)
 
     def _start_event_loop_thread(self):
         """Entry point for event loop thread that starts an asyncio context."""
         asyncio.set_event_loop(self._loop)
 
@@ -212,28 +219,29 @@
                                        write_chunk.result()))
                 write_chunk = self._loop.create_task(
                     self._write_chunk_queue.get())
 
         self._loop.stop()
 
     @staticmethod
-    async def _handle_chunk(transfers: _TransferDict, chunk: Chunk) -> None:
+    async def _handle_chunk(transfers: _TransferDict,
+                            chunk: transfer_pb2.Chunk) -> None:
         """Processes an incoming chunk from a stream.
 
         The chunk is dispatched to an active transfer based on its ID. If the
         transfer indicates that it is complete, the provided completion callback
         is invoked.
         """
 
         try:
-            transfer = transfers[chunk.session_id]
+            transfer = transfers[chunk.transfer_id]
         except KeyError:
             _LOG.error(
                 'TransferManager received chunk for unknown transfer %d',
-                chunk.session_id)
+                chunk.transfer_id)
             # TODO(frolv): What should be done here, if anything?
             return
 
         await transfer.handle_chunk(chunk)
 
     def _open_read_stream(self) -> None:
         self._read_stream = self._service.Read.invoke(
```

### Comparing `pigweed-0.0.8/pw_transfer/transfer.py` & `pigweed-0.0.9/pw_transfer/transfer.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 from dataclasses import dataclass
 import logging
 import math
 import threading
 from typing import Any, Callable, Optional
 
 from pw_status import Status
-from pw_transfer.transfer_pb2 import Chunk
+try:
+    from pw_transfer import transfer_pb2
+except ImportError:
+    # For the bazel build, which puts generated protos in a different location.
+    from pigweed.pw_transfer import transfer_pb2  # type: ignore
 
 _LOG = logging.getLogger(__package__)
 
 
 @dataclass(frozen=True)
 class ProgressStats:
     bytes_sent: int
@@ -84,15 +88,15 @@
 
     Subclasses are responsible for implementing all of the logic for their type
     of transfer, receiving messages from the server and sending the appropriate
     messages in response.
     """
     def __init__(self,
                  session_id: int,
-                 send_chunk: Callable[[Chunk], None],
+                 send_chunk: Callable[[transfer_pb2.Chunk], None],
                  end_transfer: Callable[['Transfer'], None],
                  response_timeout_s: float,
                  initial_response_timeout_s: float,
                  max_retries: int,
                  progress_callback: ProgressCallback = None):
         self.id = session_id
         self.status = Status.OK
@@ -115,18 +119,18 @@
 
     @property
     @abc.abstractmethod
     def data(self) -> bytes:
         """Returns the data read or written in this transfer."""
 
     @abc.abstractmethod
-    def _initial_chunk(self) -> Chunk:
+    def _initial_chunk(self) -> transfer_pb2.Chunk:
         """Returns the initial chunk to notify the sever of the transfer."""
 
-    async def handle_chunk(self, chunk: Chunk) -> None:
+    async def handle_chunk(self, chunk: transfer_pb2.Chunk) -> None:
         """Processes an incoming chunk from the server.
 
         Handles terminating chunks (i.e. those with a status) and forwards
         non-terminating chunks to handle_data_chunk.
         """
         self._response_timer.stop()
         self._retries = 0  # Received data from service, so reset the retries.
@@ -141,15 +145,15 @@
 
         await self._handle_data_chunk(chunk)
 
         # Start the timeout for the server to send a chunk in response.
         self._response_timer.start()
 
     @abc.abstractmethod
-    async def _handle_data_chunk(self, chunk: Chunk) -> None:
+    async def _handle_data_chunk(self, chunk: transfer_pb2.Chunk) -> None:
         """Handles a chunk that contains or requests data."""
 
     @abc.abstractmethod
     def _retry_after_timeout(self) -> None:
         """Retries after a timeout occurs."""
 
     def _on_timeout(self) -> None:
@@ -193,27 +197,27 @@
 
         if self._progress_callback:
             self._progress_callback(stats)
 
     def _send_error(self, error: Status) -> None:
         """Sends an error chunk to the server and finishes the transfer."""
         self._send_chunk(
-            Chunk(session_id=self.id,
-                  status=error.value,
-                  type=Chunk.Type.TRANSFER_COMPLETION))
+            transfer_pb2.Chunk(transfer_id=self.id,
+                               status=error.value,
+                               type=transfer_pb2.Chunk.Type.COMPLETION))
         self.finish(error)
 
 
 class WriteTransfer(Transfer):
     """A client -> server write transfer."""
     def __init__(
         self,
         session_id: int,
         data: bytes,
-        send_chunk: Callable[[Chunk], None],
+        send_chunk: Callable[[transfer_pb2.Chunk], None],
         end_transfer: Callable[[Transfer], None],
         response_timeout_s: float,
         initial_response_timeout_s: float,
         max_retries: int,
         progress_callback: ProgressCallback = None,
     ):
         super().__init__(session_id, send_chunk, end_transfer,
@@ -234,22 +238,22 @@
 
         self._last_chunk = self._initial_chunk()
 
     @property
     def data(self) -> bytes:
         return self._data
 
-    def _initial_chunk(self) -> Chunk:
+    def _initial_chunk(self) -> transfer_pb2.Chunk:
         # TODO(frolv): session_id should not be set here, but assigned by the
         # server during an initial handshake.
-        return Chunk(session_id=self.id,
-                     resource_id=self.id,
-                     type=Chunk.Type.TRANSFER_START)
+        return transfer_pb2.Chunk(transfer_id=self.id,
+                                  resource_id=self.id,
+                                  type=transfer_pb2.Chunk.Type.START)
 
-    async def _handle_data_chunk(self, chunk: Chunk) -> None:
+    async def _handle_data_chunk(self, chunk: transfer_pb2.Chunk) -> None:
         """Processes an incoming chunk from the server.
 
         In a write transfer, the server only sends transfer parameter updates
         to the client. When a message is received, update local parameters and
         send data accordingly.
         """
 
@@ -284,21 +288,22 @@
                                   len(self.data))
 
             if sent_requested_bytes:
                 break
 
         self._last_chunk = write_chunk
 
-    def _handle_parameters_update(self, chunk: Chunk) -> bool:
+    def _handle_parameters_update(self, chunk: transfer_pb2.Chunk) -> bool:
         """Updates transfer state based on a transfer parameters update."""
 
         retransmit = True
         if chunk.HasField('type'):
-            retransmit = (chunk.type == Chunk.Type.PARAMETERS_RETRANSMIT
-                          or chunk.type == Chunk.Type.TRANSFER_START)
+            retransmit = (chunk.type
+                          == transfer_pb2.Chunk.Type.PARAMETERS_RETRANSMIT
+                          or chunk.type == transfer_pb2.Chunk.Type.START)
 
         if chunk.offset > len(self.data):
             # Bad offset; terminate the transfer.
             _LOG.error(
                 'Transfer %d: server requested invalid offset %d (size %d)',
                 self.id, chunk.offset, len(self.data))
 
@@ -324,15 +329,15 @@
             # Retransmit is the default behavior for older versions of the
             # transfer protocol. The window_end_offset field is not guaranteed
             # to be set in these version, so it must be calculated.
             max_bytes_to_send = min(chunk.pending_bytes,
                                     len(self.data) - self._offset)
             self._window_end_offset = self._offset + max_bytes_to_send
         else:
-            assert chunk.type == Chunk.Type.PARAMETERS_CONTINUE
+            assert chunk.type == transfer_pb2.Chunk.Type.PARAMETERS_CONTINUE
 
             # Extend the window to the new end offset specified by the server.
             self._window_end_offset = min(chunk.window_end_offset,
                                           len(self.data))
 
         if chunk.HasField('max_chunk_size_bytes'):
             self._max_chunk_size = chunk.max_chunk_size_bytes
@@ -341,19 +346,19 @@
             self._chunk_delay_us = chunk.min_delay_microseconds
 
         return True
 
     def _retry_after_timeout(self) -> None:
         self._send_chunk(self._last_chunk)
 
-    def _next_chunk(self) -> Chunk:
+    def _next_chunk(self) -> transfer_pb2.Chunk:
         """Returns the next Chunk message to send in the data transfer."""
-        chunk = Chunk(session_id=self.id,
-                      offset=self._offset,
-                      type=Chunk.Type.TRANSFER_DATA)
+        chunk = transfer_pb2.Chunk(transfer_id=self.id,
+                                   offset=self._offset,
+                                   type=transfer_pb2.Chunk.Type.DATA)
         max_bytes_in_chunk = min(self._max_chunk_size,
                                  self._window_end_offset - self._offset)
 
         chunk.data = self.data[self._offset:self._offset + max_bytes_in_chunk]
 
         # Mark the final chunk of the transfer.
         if len(self.data) - self._offset <= max_bytes_in_chunk:
@@ -378,15 +383,15 @@
     # requested data has been received, a divisor of three will extend at a
     # third of the window, and so on.
     EXTEND_WINDOW_DIVISOR = 2
 
     def __init__(  # pylint: disable=too-many-arguments
             self,
             session_id: int,
-            send_chunk: Callable[[Chunk], None],
+            send_chunk: Callable[[transfer_pb2.Chunk], None],
             end_transfer: Callable[[Transfer], None],
             response_timeout_s: float,
             initial_response_timeout_s: float,
             max_retries: int,
             max_bytes_to_receive: int = 8192,
             max_chunk_size: int = 1024,
             chunk_delay_us: int = None,
@@ -405,43 +410,45 @@
         self._window_end_offset = max_bytes_to_receive
 
     @property
     def data(self) -> bytes:
         """Returns an immutable copy of the data that has been read."""
         return bytes(self._data)
 
-    def _initial_chunk(self) -> Chunk:
-        return self._transfer_parameters(Chunk.Type.TRANSFER_START)
+    def _initial_chunk(self) -> transfer_pb2.Chunk:
+        return self._transfer_parameters(transfer_pb2.Chunk.Type.START)
 
-    async def _handle_data_chunk(self, chunk: Chunk) -> None:
+    async def _handle_data_chunk(self, chunk: transfer_pb2.Chunk) -> None:
         """Processes an incoming chunk from the server.
 
         In a read transfer, the client receives data chunks from the server.
         Once all pending data is received, the transfer parameters are updated.
         """
 
         if chunk.offset != self._offset:
             # Initially, the transfer service only supports in-order transfers.
             # If data is received out of order, request that the server
             # retransmit from the previous offset.
             self._send_chunk(
-                self._transfer_parameters(Chunk.Type.PARAMETERS_RETRANSMIT))
+                self._transfer_parameters(
+                    transfer_pb2.Chunk.Type.PARAMETERS_RETRANSMIT))
             return
 
         self._data += chunk.data
         self._pending_bytes -= len(chunk.data)
         self._offset += len(chunk.data)
 
         if chunk.HasField('remaining_bytes'):
             if chunk.remaining_bytes == 0:
                 # No more data to read. Acknowledge receipt and finish.
                 self._send_chunk(
-                    Chunk(session_id=self.id,
-                          status=Status.OK.value,
-                          type=Chunk.Type.TRANSFER_COMPLETION))
+                    transfer_pb2.Chunk(
+                        transfer_id=self.id,
+                        status=Status.OK.value,
+                        type=transfer_pb2.Chunk.Type.COMPLETION))
                 self.finish(Status.OK)
                 return
 
             # The server may indicate if the amount of remaining data is known.
             self._remaining_transfer_size = chunk.remaining_bytes
         elif self._remaining_transfer_size is not None:
             # Update the remaining transfer size, if it is known.
@@ -479,33 +486,36 @@
         extend_window = (remaining_window_size <= self._max_bytes_to_receive /
                          ReadTransfer.EXTEND_WINDOW_DIVISOR)
 
         if self._pending_bytes == 0:
             # All pending data was received. Send out a new parameters chunk for
             # the next block.
             self._send_chunk(
-                self._transfer_parameters(Chunk.Type.PARAMETERS_RETRANSMIT))
+                self._transfer_parameters(
+                    transfer_pb2.Chunk.Type.PARAMETERS_RETRANSMIT))
         elif extend_window:
             self._send_chunk(
-                self._transfer_parameters(Chunk.Type.PARAMETERS_CONTINUE))
+                self._transfer_parameters(
+                    transfer_pb2.Chunk.Type.PARAMETERS_CONTINUE))
 
     def _retry_after_timeout(self) -> None:
         self._send_chunk(
-            self._transfer_parameters(Chunk.Type.PARAMETERS_RETRANSMIT))
+            self._transfer_parameters(
+                transfer_pb2.Chunk.Type.PARAMETERS_RETRANSMIT))
 
-    def _transfer_parameters(self, chunk_type: Any) -> Chunk:
+    def _transfer_parameters(self, chunk_type: Any) -> transfer_pb2.Chunk:
         """Sends an updated transfer parameters chunk to the server."""
 
         self._pending_bytes = self._max_bytes_to_receive
         self._window_end_offset = self._offset + self._max_bytes_to_receive
 
-        chunk = Chunk(session_id=self.id,
-                      pending_bytes=self._pending_bytes,
-                      window_end_offset=self._window_end_offset,
-                      max_chunk_size_bytes=self._max_chunk_size,
-                      offset=self._offset,
-                      type=chunk_type)
+        chunk = transfer_pb2.Chunk(transfer_id=self.id,
+                                   pending_bytes=self._pending_bytes,
+                                   window_end_offset=self._window_end_offset,
+                                   max_chunk_size_bytes=self._max_chunk_size,
+                                   offset=self._offset,
+                                   type=chunk_type)
 
         if self._chunk_delay_us:
             chunk.min_delay_microseconds = self._chunk_delay_us
 
         return chunk
```

### Comparing `pigweed-0.0.8/pw_transfer/transfer_pb2.py` & `pigweed-0.0.9/pw_transfer/transfer_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,75 +15,85 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='pw_transfer/transfer.proto',
   package='pw.transfer',
   syntax='proto3',
   serialized_options=b'\n\027dev.pigweed.pw_transferP\001',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1apw_transfer/transfer.proto\x12\x0bpw.transfer\"\xb4\x04\n\x05\x43hunk\x12\x12\n\nsession_id\x18\x01 \x01(\r\x12\x1a\n\rpending_bytes\x18\x02 \x01(\rH\x00\x88\x01\x01\x12!\n\x14max_chunk_size_bytes\x18\x03 \x01(\rH\x01\x88\x01\x01\x12#\n\x16min_delay_microseconds\x18\x04 \x01(\rH\x02\x88\x01\x01\x12\x0e\n\x06offset\x18\x05 \x01(\x04\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x1c\n\x0fremaining_bytes\x18\x07 \x01(\x04H\x03\x88\x01\x01\x12\x13\n\x06status\x18\x08 \x01(\rH\x04\x88\x01\x01\x12\x19\n\x11window_end_offset\x18\t \x01(\r\x12*\n\x04type\x18\n \x01(\x0e\x32\x17.pw.transfer.Chunk.TypeH\x05\x88\x01\x01\x12\x13\n\x0bresource_id\x18\x0b \x01(\r\"\x97\x01\n\x04Type\x12\x11\n\rTRANSFER_DATA\x10\x00\x12\x12\n\x0eTRANSFER_START\x10\x01\x12\x19\n\x15PARAMETERS_RETRANSMIT\x10\x02\x12\x17\n\x13PARAMETERS_CONTINUE\x10\x03\x12\x17\n\x13TRANSFER_COMPLETION\x10\x04\x12\x1b\n\x17TRANSFER_COMPLETION_ACK\x10\x05\x42\x10\n\x0e_pending_bytesB\x17\n\x15_max_chunk_size_bytesB\x19\n\x17_min_delay_microsecondsB\x12\n\x10_remaining_bytesB\t\n\x07_statusB\x07\n\x05_type2s\n\x08Transfer\x12\x32\n\x04Read\x12\x12.pw.transfer.Chunk\x1a\x12.pw.transfer.Chunk(\x01\x30\x01\x12\x33\n\x05Write\x12\x12.pw.transfer.Chunk\x1a\x12.pw.transfer.Chunk(\x01\x30\x01\x42\x1b\n\x17\x64\x65v.pigweed.pw_transferP\x01\x62\x06proto3'
+  serialized_pb=b'\n\x1apw_transfer/transfer.proto\x12\x0bpw.transfer\"\xf9\x04\n\x05\x43hunk\x12\x13\n\x0btransfer_id\x18\x01 \x01(\r\x12\x1a\n\rpending_bytes\x18\x02 \x01(\rH\x00\x88\x01\x01\x12!\n\x14max_chunk_size_bytes\x18\x03 \x01(\rH\x01\x88\x01\x01\x12#\n\x16min_delay_microseconds\x18\x04 \x01(\rH\x02\x88\x01\x01\x12\x0e\n\x06offset\x18\x05 \x01(\x04\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x1c\n\x0fremaining_bytes\x18\x07 \x01(\x04H\x03\x88\x01\x01\x12\x13\n\x06status\x18\x08 \x01(\rH\x04\x88\x01\x01\x12\x19\n\x11window_end_offset\x18\t \x01(\r\x12*\n\x04type\x18\n \x01(\x0e\x32\x17.pw.transfer.Chunk.TypeH\x05\x88\x01\x01\x12\x18\n\x0bresource_id\x18\x0b \x01(\rH\x06\x88\x01\x01\x12\x17\n\nsession_id\x18\x0c \x01(\rH\x07\x88\x01\x01\"\x9e\x01\n\x04Type\x12\x08\n\x04\x44\x41TA\x10\x00\x12\t\n\x05START\x10\x01\x12\x19\n\x15PARAMETERS_RETRANSMIT\x10\x02\x12\x17\n\x13PARAMETERS_CONTINUE\x10\x03\x12\x0e\n\nCOMPLETION\x10\x04\x12\x12\n\x0e\x43OMPLETION_ACK\x10\x05\x12\r\n\tSTART_ACK\x10\x06\x12\x1a\n\x16START_ACK_CONFIRMATION\x10\x07\x42\x10\n\x0e_pending_bytesB\x17\n\x15_max_chunk_size_bytesB\x19\n\x17_min_delay_microsecondsB\x12\n\x10_remaining_bytesB\t\n\x07_statusB\x07\n\x05_typeB\x0e\n\x0c_resource_idB\r\n\x0b_session_id2s\n\x08Transfer\x12\x32\n\x04Read\x12\x12.pw.transfer.Chunk\x1a\x12.pw.transfer.Chunk(\x01\x30\x01\x12\x33\n\x05Write\x12\x12.pw.transfer.Chunk\x1a\x12.pw.transfer.Chunk(\x01\x30\x01\x42\x1b\n\x17\x64\x65v.pigweed.pw_transferP\x01\x62\x06proto3'
 )
 
 
 
 _CHUNK_TYPE = _descriptor.EnumDescriptor(
   name='Type',
   full_name='pw.transfer.Chunk.Type',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='TRANSFER_DATA', index=0, number=0,
+      name='DATA', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='TRANSFER_START', index=1, number=1,
+      name='START', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='PARAMETERS_RETRANSMIT', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='PARAMETERS_CONTINUE', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='TRANSFER_COMPLETION', index=4, number=4,
+      name='COMPLETION', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='TRANSFER_COMPLETION_ACK', index=5, number=5,
+      name='COMPLETION_ACK', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='START_ACK', index=6, number=6,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='START_ACK_CONFIRMATION', index=7, number=7,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=347,
-  serialized_end=498,
+  serialized_start=378,
+  serialized_end=536,
 )
 _sym_db.RegisterEnumDescriptor(_CHUNK_TYPE)
 
 
 _CHUNK = _descriptor.Descriptor(
   name='Chunk',
   full_name='pw.transfer.Chunk',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='session_id', full_name='pw.transfer.Chunk.session_id', index=0,
+      name='transfer_id', full_name='pw.transfer.Chunk.transfer_id', index=0,
       number=1, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='pending_bytes', full_name='pw.transfer.Chunk.pending_bytes', index=1,
@@ -151,14 +161,21 @@
     _descriptor.FieldDescriptor(
       name='resource_id', full_name='pw.transfer.Chunk.resource_id', index=10,
       number=11, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='session_id', full_name='pw.transfer.Chunk.session_id', index=11,
+      number=12, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
     _CHUNK_TYPE,
   ],
@@ -193,17 +210,27 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_type', full_name='pw.transfer.Chunk._type',
       index=5, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_resource_id', full_name='pw.transfer.Chunk._resource_id',
+      index=6, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_session_id', full_name='pw.transfer.Chunk._session_id',
+      index=7, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
   serialized_start=44,
-  serialized_end=608,
+  serialized_end=677,
 )
 
 _CHUNK.fields_by_name['type'].enum_type = _CHUNK_TYPE
 _CHUNK_TYPE.containing_type = _CHUNK
 _CHUNK.oneofs_by_name['_pending_bytes'].fields.append(
   _CHUNK.fields_by_name['pending_bytes'])
 _CHUNK.fields_by_name['pending_bytes'].containing_oneof = _CHUNK.oneofs_by_name['_pending_bytes']
@@ -218,14 +245,20 @@
 _CHUNK.fields_by_name['remaining_bytes'].containing_oneof = _CHUNK.oneofs_by_name['_remaining_bytes']
 _CHUNK.oneofs_by_name['_status'].fields.append(
   _CHUNK.fields_by_name['status'])
 _CHUNK.fields_by_name['status'].containing_oneof = _CHUNK.oneofs_by_name['_status']
 _CHUNK.oneofs_by_name['_type'].fields.append(
   _CHUNK.fields_by_name['type'])
 _CHUNK.fields_by_name['type'].containing_oneof = _CHUNK.oneofs_by_name['_type']
+_CHUNK.oneofs_by_name['_resource_id'].fields.append(
+  _CHUNK.fields_by_name['resource_id'])
+_CHUNK.fields_by_name['resource_id'].containing_oneof = _CHUNK.oneofs_by_name['_resource_id']
+_CHUNK.oneofs_by_name['_session_id'].fields.append(
+  _CHUNK.fields_by_name['session_id'])
+_CHUNK.fields_by_name['session_id'].containing_oneof = _CHUNK.oneofs_by_name['_session_id']
 DESCRIPTOR.message_types_by_name['Chunk'] = _CHUNK
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Chunk = _reflection.GeneratedProtocolMessageType('Chunk', (_message.Message,), {
   'DESCRIPTOR' : _CHUNK,
   '__module__' : 'pw_transfer.transfer_pb2'
   # @@protoc_insertion_point(class_scope:pw.transfer.Chunk)
@@ -238,16 +271,16 @@
 _TRANSFER = _descriptor.ServiceDescriptor(
   name='Transfer',
   full_name='pw.transfer.Transfer',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=610,
-  serialized_end=725,
+  serialized_start=679,
+  serialized_end=794,
   methods=[
   _descriptor.MethodDescriptor(
     name='Read',
     full_name='pw.transfer.Transfer.Read',
     index=0,
     containing_service=None,
     input_type=_CHUNK,
```

### Comparing `pigweed-0.0.8/pw_transfer/transfer_pb2.pyi` & `pigweed-0.0.9/pw_transfer/transfer_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -22,67 +22,86 @@
     class Type(_Type, metaclass=_TypeEnumTypeWrapper):
         pass
     class _Type:
         V = typing.NewType('V', builtins.int)
     class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Type.V], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
         # Chunk containing transfer data.
-        TRANSFER_DATA = Chunk.Type.V(0)
+        DATA = Chunk.Type.V(0)
         # First chunk of a transfer (only sent by the client).
-        TRANSFER_START = Chunk.Type.V(1)
+        START = Chunk.Type.V(1)
         # Transfer parameters indicating that the transmitter should retransmit
         # from the specified offset.
         PARAMETERS_RETRANSMIT = Chunk.Type.V(2)
         # Transfer parameters telling the transmitter to continue sending up to
         # index `offset + pending_bytes` of data. If the transmitter is already
         # beyond `offset`, it does not have to rewind.
         PARAMETERS_CONTINUE = Chunk.Type.V(3)
         # Sender of the chunk is terminating the transfer.
-        TRANSFER_COMPLETION = Chunk.Type.V(4)
+        COMPLETION = Chunk.Type.V(4)
         # Acknowledge the completion of a transfer. Currently unused.
         # TODO(konkers): Implement this behavior.
-        TRANSFER_COMPLETION_ACK = Chunk.Type.V(5)
+        COMPLETION_ACK = Chunk.Type.V(5)
+        # Acknowledges a transfer start request, assigning a session ID for the
+        # transfer and optionally negotiating the protocol version. Sent from
+        # server to client.
+        START_ACK = Chunk.Type.V(6)
+        # Confirmation of a START_ACK's assigned session ID and negotiated
+        # parameters, sent by the client to the server. Initiates the data transfer
+        # proper.
+        START_ACK_CONFIRMATION = Chunk.Type.V(7)
 
     # Chunk containing transfer data.
-    TRANSFER_DATA = Chunk.Type.V(0)
+    DATA = Chunk.Type.V(0)
     # First chunk of a transfer (only sent by the client).
-    TRANSFER_START = Chunk.Type.V(1)
+    START = Chunk.Type.V(1)
     # Transfer parameters indicating that the transmitter should retransmit
     # from the specified offset.
     PARAMETERS_RETRANSMIT = Chunk.Type.V(2)
     # Transfer parameters telling the transmitter to continue sending up to
     # index `offset + pending_bytes` of data. If the transmitter is already
     # beyond `offset`, it does not have to rewind.
     PARAMETERS_CONTINUE = Chunk.Type.V(3)
     # Sender of the chunk is terminating the transfer.
-    TRANSFER_COMPLETION = Chunk.Type.V(4)
+    COMPLETION = Chunk.Type.V(4)
     # Acknowledge the completion of a transfer. Currently unused.
     # TODO(konkers): Implement this behavior.
-    TRANSFER_COMPLETION_ACK = Chunk.Type.V(5)
+    COMPLETION_ACK = Chunk.Type.V(5)
+    # Acknowledges a transfer start request, assigning a session ID for the
+    # transfer and optionally negotiating the protocol version. Sent from
+    # server to client.
+    START_ACK = Chunk.Type.V(6)
+    # Confirmation of a START_ACK's assigned session ID and negotiated
+    # parameters, sent by the client to the server. Initiates the data transfer
+    # proper.
+    START_ACK_CONFIRMATION = Chunk.Type.V(7)
 
-    SESSION_ID_FIELD_NUMBER: builtins.int
+    TRANSFER_ID_FIELD_NUMBER: builtins.int
     PENDING_BYTES_FIELD_NUMBER: builtins.int
     MAX_CHUNK_SIZE_BYTES_FIELD_NUMBER: builtins.int
     MIN_DELAY_MICROSECONDS_FIELD_NUMBER: builtins.int
     OFFSET_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     REMAINING_BYTES_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     WINDOW_END_OFFSET_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     RESOURCE_ID_FIELD_NUMBER: builtins.int
+    SESSION_ID_FIELD_NUMBER: builtins.int
     # Represents the source or destination of the data. May be ephemeral or
     # stable depending on the implementation. Sent in every request to identify
     # the transfer target.
     #
+    # LEGACY FIELD ONLY. Split into resource_id and session_id in transfer v2.
+    #
     #  Read → ID of transfer
     #  Read ← ID of transfer
     # Write → ID of transfer
     # Write ← ID of transfer
-    session_id: builtins.int = ...
+    transfer_id: builtins.int = ...
     # Used by the receiver to indicate how many bytes it can accept. The
     # transmitter sends this much data, divided into chunks no larger than
     # max_chunk_size_bytes. The receiver then starts another window by sending
     # request_bytes again with a new offset.
     #
     #  Read → The client requests this many bytes to be sent.
     #  Read ← N/A
@@ -168,38 +187,59 @@
     # semantics from this field.
     #
     #  Read → Chunk type (start/parameters).
     #  Read ← Chunk type (data).
     # Write → Chunk type (data).
     # Write ← Chunk type (start/parameters).
     type: global___Chunk.Type.V = ...
-    # Not currently used. Will inherit session_id's behavior in the future.
+    # Unique identifier for the source or destination of transfer data. May be
+    # stable or ephemeral depending on the implementation. Only sent during the
+    # initial handshake phase of a version 2 or higher transfer.
+    #
+    #  Read → ID of transferable resource
+    #  Read ← ID of transferable resource
+    # Write → ID of transferable resource
+    # Write ← ID of transferable resource
     resource_id: builtins.int = ...
+    # Unique identifier for a specific transfer session. Assigned by a transfer
+    # service during the initial handshake phase, and persists for the remainder
+    # of that transfer operation.
+    #
+    #  Read → ID of transfer session
+    #  Read ← ID of transfer session
+    # Write → ID of transfer session
+    # Write ← ID of transfer session
+    session_id: builtins.int = ...
     def __init__(self,
         *,
-        session_id : builtins.int = ...,
+        transfer_id : builtins.int = ...,
         pending_bytes : builtins.int = ...,
         max_chunk_size_bytes : builtins.int = ...,
         min_delay_microseconds : builtins.int = ...,
         offset : builtins.int = ...,
         data : builtins.bytes = ...,
         remaining_bytes : builtins.int = ...,
         status : builtins.int = ...,
         window_end_offset : builtins.int = ...,
         type : global___Chunk.Type.V = ...,
         resource_id : builtins.int = ...,
+        session_id : builtins.int = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"_max_chunk_size_bytes",b"_max_chunk_size_bytes",u"_min_delay_microseconds",b"_min_delay_microseconds",u"_pending_bytes",b"_pending_bytes",u"_remaining_bytes",b"_remaining_bytes",u"_status",b"_status",u"_type",b"_type",u"max_chunk_size_bytes",b"max_chunk_size_bytes",u"min_delay_microseconds",b"min_delay_microseconds",u"pending_bytes",b"pending_bytes",u"remaining_bytes",b"remaining_bytes",u"status",b"status",u"type",b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"_max_chunk_size_bytes",b"_max_chunk_size_bytes",u"_min_delay_microseconds",b"_min_delay_microseconds",u"_pending_bytes",b"_pending_bytes",u"_remaining_bytes",b"_remaining_bytes",u"_status",b"_status",u"_type",b"_type",u"data",b"data",u"max_chunk_size_bytes",b"max_chunk_size_bytes",u"min_delay_microseconds",b"min_delay_microseconds",u"offset",b"offset",u"pending_bytes",b"pending_bytes",u"remaining_bytes",b"remaining_bytes",u"resource_id",b"resource_id",u"session_id",b"session_id",u"status",b"status",u"type",b"type",u"window_end_offset",b"window_end_offset"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal[u"_max_chunk_size_bytes",b"_max_chunk_size_bytes",u"_min_delay_microseconds",b"_min_delay_microseconds",u"_pending_bytes",b"_pending_bytes",u"_remaining_bytes",b"_remaining_bytes",u"_resource_id",b"_resource_id",u"_session_id",b"_session_id",u"_status",b"_status",u"_type",b"_type",u"max_chunk_size_bytes",b"max_chunk_size_bytes",u"min_delay_microseconds",b"min_delay_microseconds",u"pending_bytes",b"pending_bytes",u"remaining_bytes",b"remaining_bytes",u"resource_id",b"resource_id",u"session_id",b"session_id",u"status",b"status",u"type",b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"_max_chunk_size_bytes",b"_max_chunk_size_bytes",u"_min_delay_microseconds",b"_min_delay_microseconds",u"_pending_bytes",b"_pending_bytes",u"_remaining_bytes",b"_remaining_bytes",u"_resource_id",b"_resource_id",u"_session_id",b"_session_id",u"_status",b"_status",u"_type",b"_type",u"data",b"data",u"max_chunk_size_bytes",b"max_chunk_size_bytes",u"min_delay_microseconds",b"min_delay_microseconds",u"offset",b"offset",u"pending_bytes",b"pending_bytes",u"remaining_bytes",b"remaining_bytes",u"resource_id",b"resource_id",u"session_id",b"session_id",u"status",b"status",u"transfer_id",b"transfer_id",u"type",b"type",u"window_end_offset",b"window_end_offset"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_max_chunk_size_bytes",b"_max_chunk_size_bytes"]) -> typing.Optional[typing_extensions.Literal["max_chunk_size_bytes"]]: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_min_delay_microseconds",b"_min_delay_microseconds"]) -> typing.Optional[typing_extensions.Literal["min_delay_microseconds"]]: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_pending_bytes",b"_pending_bytes"]) -> typing.Optional[typing_extensions.Literal["pending_bytes"]]: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_remaining_bytes",b"_remaining_bytes"]) -> typing.Optional[typing_extensions.Literal["remaining_bytes"]]: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_resource_id",b"_resource_id"]) -> typing.Optional[typing_extensions.Literal["resource_id"]]: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_session_id",b"_session_id"]) -> typing.Optional[typing_extensions.Literal["session_id"]]: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_status",b"_status"]) -> typing.Optional[typing_extensions.Literal["status"]]: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal[u"_type",b"_type"]) -> typing.Optional[typing_extensions.Literal["type"]]: ...
 global___Chunk = Chunk
```

### Comparing `pigweed-0.0.8/pw_unit_test/__init__.py` & `pigweed-0.0.9/pw_unit_test/__init__.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_unit_test/rpc.py` & `pigweed-0.0.9/pw_unit_test/rpc.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_unit_test/test_runner.py` & `pigweed-0.0.9/pw_unit_test/test_runner.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_unit_test_proto/unit_test_pb2.py` & `pigweed-0.0.9/pw_unit_test_proto/unit_test_pb2.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_unit_test_proto/unit_test_pb2.pyi` & `pigweed-0.0.9/pw_unit_test_proto/unit_test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_watch/debounce.py` & `pigweed-0.0.9/pw_watch/debounce.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pw_watch/watch.py` & `pigweed-0.0.9/pw_watch/watch.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,18 @@
     NamedTuple,
     NoReturn,
     Optional,
     Sequence,
     Tuple,
 )
 
-import httpwatcher  # type: ignore
+try:
+    import httpwatcher  # type: ignore[import]
+except ImportError:
+    httpwatcher = None
 
 from watchdog.events import FileSystemEventHandler  # type: ignore[import]
 from watchdog.observers import Observer  # type: ignore[import]
 
 from prompt_toolkit.formatted_text.base import OneStyleAndTextTuple
 from prompt_toolkit.formatted_text import StyleAndTextTuples
 
@@ -182,14 +185,15 @@
         patterns: Sequence[str] = (),
         ignore_patterns: Sequence[str] = (),
         charset: WatchCharset = _ASCII_CHARSET,
         restart: bool = True,
         jobs: int = None,
         fullscreen: bool = False,
         banners: bool = True,
+        keep_going: bool = False,
     ):
         super().__init__()
 
         self.banners = banners
         self.status_message: Optional[OneStyleAndTextTuple] = None
         self.result_message: Optional[StyleAndTextTuples] = None
         self.current_stdout = ''
@@ -203,14 +207,16 @@
 
         self.restart_on_changes = restart
         self.fullscreen_enabled = fullscreen
         self.watch_app: Optional[WatchApp] = None
         self._current_build: subprocess.Popen
 
         self._extra_ninja_args = [] if jobs is None else [f'-j{jobs}']
+        if keep_going:
+            self._extra_ninja_args.extend(['-k', '0'])
 
         self.debouncer = Debouncer(self)
 
         # Track state of a build. These need to be members instead of locals
         # due to the split between dispatch(), run(), and on_complete().
         self.matching_path: Optional[Path] = None
         self.builds_succeeded: List[bool] = []
@@ -569,14 +575,19 @@
                         type=Path,
                         help='directories to ignore during pw watch',
                         default=[])
     parser.add_argument('--no-restart',
                         dest='restart',
                         action='store_false',
                         help='do not restart ongoing builds if files change')
+    parser.add_argument('-k',
+                        '--keep-going',
+                        action='store_true',
+                        help=('Keep building past the first failure. This is'
+                              'equivalent to passing "-k 0" to ninja.'))
     parser.add_argument(
         'default_build_targets',
         nargs='*',
         metavar='target',
         default=[],
         help=('Automatically locate a build directory and build these '
               'targets. For example, `host docs` searches for a Ninja '
@@ -595,31 +606,31 @@
               'build. `pw watch -C out tgt` is equivalent to `ninja '
               '-C out tgt`'))
     parser.add_argument(
         '--serve-docs',
         dest='serve_docs',
         action='store_true',
         default=False,
-        help='Start a webserver for docs on localhost. The port for this '
-        ' webserver can be set with the --serve-docs-port option. '
-        ' Defaults to http://127.0.0.1:8000')
+        help=('Start a webserver for docs on localhost. The port for this '
+              'webserver can be set with the --serve-docs-port option. '
+              'Defaults to http://127.0.0.1:8000. This option requires '
+              'the httpwatcher package to be installed.'))
     parser.add_argument(
         '--serve-docs-port',
         dest='serve_docs_port',
         type=int,
         default=8000,
         help='Set the port for the docs webserver. Default to 8000.')
-
     parser.add_argument(
         '--serve-docs-path',
         dest='serve_docs_path',
         type=Path,
         default="docs/gen/docs",
-        help='Set the path for the docs to serve. Default to docs/gen/docs'
-        ' in the build directory.')
+        help=('Set the path for the docs to serve. Default to docs/gen/docs'
+              ' in the build directory.'))
     parser.add_argument(
         '-j',
         '--jobs',
         type=int,
         help="Number of cores to use; defaults to Ninja's default")
     parser.add_argument('-f',
                         '--fullscreen',
@@ -776,27 +787,49 @@
     if found_legacy:
         _LOG.warning('Found legacy environment directory(s); these '
                      'should be deleted')
 
     return exclude_list
 
 
+def _serve_docs(build_dir: Path, serve_docs_port: int,
+                serve_docs_path: Path) -> None:
+    if httpwatcher is None:
+        _LOG.warning(
+            '--serve-docs was specified, but httpwatcher is not available')
+        _LOG.info('Install httpwatcher to use --serve-docs')
+        return
+
+    def httpwatcher_thread():
+        # Disable logs from httpwatcher and deps
+        logging.getLogger('httpwatcher').setLevel(logging.CRITICAL)
+        logging.getLogger('tornado').setLevel(logging.CRITICAL)
+
+        docs_path = build_dir.joinpath(serve_docs_path.joinpath('html'))
+        httpwatcher.watch(docs_path, host='127.0.0.1', port=serve_docs_port)
+
+    # Spin up an httpwatcher in a new thread since it blocks
+    threading.Thread(None, httpwatcher_thread, 'httpwatcher').start()
+
+
 def watch_setup(
     default_build_targets: List[str],
     build_directories: List[str],
     patterns: str,
     ignore_patterns_string: str,
     exclude_list: List[Path],
     restart: bool,
     jobs: Optional[int],
     serve_docs: bool,
     serve_docs_port: int,
     serve_docs_path: Path,
     fullscreen: bool,
     banners: bool,
+    keep_going: bool,
+    debug_logging: bool,  # pylint: disable=unused-argument
     # pylint: disable=too-many-arguments
 ) -> Tuple[str, PigweedBuildWatcher, List[Path]]:
     """Watches files and runs Ninja commands when they change."""
     _LOG.info('Starting Pigweed build watcher')
 
     # Get pigweed directory information from environment variable PW_ROOT.
     if os.environ['PW_ROOT'] is None:
@@ -832,28 +865,16 @@
         else:
             _LOG.info('Will build [%d/%d]: %s', i, len(build_commands),
                       build_target)
 
     _LOG.debug('Patterns: %s', patterns)
 
     if serve_docs:
-
-        def _serve_docs():
-            # Disable logs from httpwatcher and deps
-            logging.getLogger('httpwatcher').setLevel(logging.CRITICAL)
-            logging.getLogger('tornado').setLevel(logging.CRITICAL)
-
-            docs_path = build_commands[0].build_dir.joinpath(
-                serve_docs_path.joinpath('html'))
-            httpwatcher.watch(docs_path,
-                              host="127.0.0.1",
-                              port=serve_docs_port)
-
-        # Spin up an httpwatcher in a new thread since it blocks
-        threading.Thread(None, _serve_docs, "httpwatcher").start()
+        _serve_docs(build_commands[0].build_dir, serve_docs_port,
+                    serve_docs_path)
 
     # Try to make a short display path for the watched directory that has
     # "$HOME" instead of the full home directory. This is nice for users
     # who have deeply nested home directories.
     path_to_log = str(Path().resolve()).replace(str(Path.home()), '$HOME')
 
     # Ignore the user-specified patterns.
@@ -871,14 +892,15 @@
         patterns=patterns.split(_WATCH_PATTERN_DELIMITER),
         ignore_patterns=ignore_patterns,
         charset=charset,
         restart=restart,
         jobs=jobs,
         fullscreen=fullscreen,
         banners=banners,
+        keep_going=keep_going,
     )
     return path_to_log, event_handler, exclude_list
 
 
 def watch(path_to_log: Path, event_handler: PigweedBuildWatcher,
           exclude_list: List[Path]):
     """Watches files and runs Ninja commands when they change."""
@@ -927,28 +949,15 @@
     """Watch files for changes and rebuild."""
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter)
     add_parser_arguments(parser)
     args = parser.parse_args()
 
-    path_to_log, event_handler, exclude_list = watch_setup(
-        default_build_targets=args.default_build_targets,
-        build_directories=args.build_directories,
-        patterns=args.patterns,
-        ignore_patterns_string=args.ignore_patterns_string,
-        exclude_list=args.exclude_list,
-        restart=args.restart,
-        jobs=args.jobs,
-        serve_docs=args.serve_docs,
-        serve_docs_port=args.serve_docs_port,
-        serve_docs_path=args.serve_docs_path,
-        fullscreen=args.fullscreen,
-        banners=args.banners,
-    )
+    path_to_log, event_handler, exclude_list = watch_setup(**vars(args))
 
     if args.fullscreen:
         watch_logfile = (pw_console.python_logging.create_temp_log_file(
             prefix=__package__))
         pw_cli.log.install(
             level=logging.DEBUG,
             use_color=True,
```

### Comparing `pigweed-0.0.8/pw_watch/watch_app.py` & `pigweed-0.0.9/pw_watch/watch_app.py`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/pyproject.toml` & `pigweed-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pigweed-0.0.8/setup.cfg` & `pigweed-0.0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [metadata]
 name = pigweed
-version = 0.0.8
+version = 0.0.9
 author = Pigweed Authors
 author_email = pigweed-developers@googlegroups.com
 description = Pigweed Python modules
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pigweed.dev
 project_urls = 
-	Bug Tracker = https://bugs.chromium.org/p/pigweed/issues/list
-	Code Search = https://cs.opensource.google/pigweed/pigweed
-	Gerrit = https://pigweed-review.googlesource.com
+	Documentation = https://pigweed.dev
+	Source Code = https://cs.opensource.google/pigweed/pigweed
+	Code Reviews = https://pigweed-review.googlesource.com
+	Mailing List = https://groups.google.com/g/pigweed
+	Issue Tracker = https://bugs.pigweed.dev
+	Chat = https://discord.gg/M9NSeTA
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Topic :: Software Development :: Embedded Systems
 
 [options]
@@ -26,15 +29,14 @@
 	PyYAML
 	Pygments
 	coloredlogs
 	coverage
 	cryptography
 	google-cloud-storage
 	graphlib-backport;python_version<'3.9'
-	httpwatcher
 	ipython
 	mypy-protobuf==2.9
 	parameterized
 	prompt_toolkit>=3.0.26
 	protobuf
 	ptpython>=3.0.20
 	pyelftools
@@ -90,86 +92,94 @@
 pw_cpu_exception_cortex_m_protos = 
 	py.typed
 	cpu_state_pb2.pyi
 pw_cpu_exception_cortex_m = py.typed
 pw_docgen = py.typed
 pw_doctor = py.typed
 pw_protobuf_codegen_protos = 
-	py.typed
 	options_pb2.pyi
+	py.typed
 pw_protobuf = py.typed
 pw_status = py.typed
-pw_protobuf_protos = 
-	common_pb2.pyi
-	status_pb2.pyi
-	py.typed
 pw_rpc = 
-	benchmark_pb2.pyi
 	echo_pb2.pyi
+	benchmark_pb2.pyi
 	py.typed
 pw_rpc.internal = 
 	packet_pb2.pyi
 	py.typed
 pw_rpc.console_tools = 
 	py.typed
 pw_rpc.callback_client = 
 	py.typed
 pw_protobuf_compiler_protos.nested.more_nesting = 
-	test_pb2.pyi
 	py.typed
-pw_protobuf_compiler_protos = 
 	test_pb2.pyi
+pw_protobuf_compiler_protos = 
 	py.typed
+	test_pb2.pyi
 pw_protobuf_compiler_protos.nested = 
 	py.typed
 pw_tokenizer.proto = 
-	options_pb2.pyi
 	py.typed
+	options_pb2.pyi
 pw_tokenizer = 
 	py.typed
 pw_hdlc = py.typed
+pw_protobuf_protos = 
+	status_pb2.pyi
+	common_pb2.pyi
+	py.typed
 pw_log.proto = 
 	log_pb2.pyi
 	py.typed
 pw_log = 
 	py.typed
+pw_metric = 
+	py.typed
 pw_module = py.typed
 pw_snapshot_metadata_proto = 
 	py.typed
 	snapshot_metadata_pb2.pyi
 pw_snapshot_metadata = 
 	py.typed
 pw_thread_protos = 
-	py.typed
 	thread_pb2.pyi
+	py.typed
 pw_thread = 
 	py.typed
+pw_chrono = 
+	chrono_pb2.pyi
+	py.typed
 pw_snapshot_protos = 
-	snapshot_pb2.pyi
 	py.typed
+	snapshot_pb2.pyi
 pw_snapshot = 
 	py.typed
 pw_software_update = 
+	py.typed
 	update_bundle_pb2.pyi
+	bundled_update_pb2.pyi
 	tuf_pb2.pyi
+pw_metric_proto = 
 	py.typed
-	bundled_update_pb2.pyi
+	metric_service_pb2.pyi
+pw_unit_test_proto = 
+	unit_test_pb2.pyi
+	py.typed
+pw_unit_test = py.typed
 pw_system = 
 	py.typed
 pw_tls_client = py.typed
 pw_toolchain = py.typed
 pw_trace = py.typed
 pw_trace_tokenized = py.typed
 pw_transfer = 
-	transfer_pb2.pyi
 	py.typed
-pw_unit_test_proto = 
-	unit_test_pb2.pyi
-	py.typed
-pw_unit_test = py.typed
+	transfer_pb2.pyi
 pw_watch = py.typed
 
 [options.entry_points]
 console_scripts = 
 	pw = pw_cli.__main__:main
 	arduino_builder = pw_arduino_build.__main__:main
 	teensy_detector = pw_arduino_build.teensy_detector:main
```

